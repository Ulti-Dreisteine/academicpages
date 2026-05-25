---
title: "Box-Jenkins模型辨识"
date: 2026-05-25
mathjax: true
---


# **一、基本介绍**

辨识的目的是从动态数据中识别输入对输出的**真实**影响。这里的真实，指的是**不受测量误差、未建模动态、环境漂移等因素干扰**的影响。接下来，我将通过Box-Jenkins（BJ）模型辨识来阐述这一观点。

BJ模型的形式为：

$$
\begin{align*}
y_k &= G(z)u_k + H(z)e_k \\
    &= \frac{B(z)}{F(z)}u_k + \frac{C(z)}{D(z)}e_k, \\
\end{align*}
$$

其中，噪声通道 $H(z) = C(z)/D(z)$ 描述了系统的噪声特性，负责**吸收所有与输入 $u_k$ 无关的波动**（测量误差、未建模动态、环境漂移等）。

由于系统假设“物理过程的惯性”和“环境干扰的扩散规律”相互独立，因此BJ模型可以实现比ARMAX等模型更好的信噪分离效果。但是，**有色噪声 $H(z)e_k$ 的存在导致我们无法直接使用常规的线性最小二乘法（OLS）求出解析解**，必须通过非线性优化迭代算法（如 Gauss-Newton 或 Levenberg-Marquardt）来求解参数。

---
# **二、参数估计**

采用预测误差法（Prediction Error Method, PEM）对BJ模型进行参数估计。首先，分离出当前时刻的白噪声项：

$$
e_k = \frac{D(z)}{C(z)}\left[y_k - \frac{B(z)}{F(z)}u_k\right]
$$

注意，$y_k$ 表示当前时刻输出观测值，$u_k$ 是当前时刻输入值。上式表示，如果我们知道了 $B(z)$、$F(z)$、$C(z)$ 和 $D(z)$ 的参数，以及当前时刻的输入和输出观测数据，就可以计算出当前时刻的预测误差 $e_k$，进而知道当前时刻输出的估计值：

$$
\begin{align*}
\hat{y}_k &= y_k - e_k \\
&= y_k - \frac{D(z)}{C(z)}\left[y_k - \frac{B(z)}{F(z)}u_k\right] \\
&= \left[1 - \frac{D(z)}{C(z)}\right]y_k + \frac{D(z)}{C(z)}\frac{B(z)}{F(z)}u_k \\
\end{align*}
$$

这里的 $\hat y_k$ 是排除了噪声影响后的输出估计值，是 $u_k$ 对 $y_k$ 的**真实**影响。

PEM 的目标就是通过最小化所有时刻的预测误差平方和来求解参数：

$$
\begin{align*}
\hat{\theta} &= \argmin_{\boldsymbol{\theta}} \sum_{k=1}^{N} e_k^2 \\
    &= \argmin_{\boldsymbol{\theta}} \sum_{k=1}^{N} \left[y_k - \hat{y}_k\right]^2 \\
    &= \argmin_{\boldsymbol{\theta}} \sum_{k=1}^{N} \left[\frac{D(z)}{C(z)}\left[y_k - \frac{B(z)}{F(z)}u_k\right]\right]^2 \\
\end{align*}
$$

对应的损失函数为：

$$
J(\boldsymbol{\theta}) = \sum_{k=1}^{N} e_k^2 = \sum_{k=1}^{N} \left[y_k - \hat{y}_k\right]^2.
$$

当 $J(\boldsymbol{\theta})$ 收敛到局部最小值时，留下来的残差将退化为完美的白噪声。这代表数据中的所有有用信息（物理规律、时序相关性）已被 BJ 模型完全榨干，实现**信噪分离**，从而得到了输入对输出的**真实**影响。
