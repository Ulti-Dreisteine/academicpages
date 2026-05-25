---
layout: archive
name: "罗磊"
tagline: "工学博士 | 工业过程分析、数据建模和预测控制"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
meta: "1992.05 | 四川成都"
---


<div style="background:#f2f2f2;padding:6px 12px;font-weight:bold;font-size:2em;">
个人信息
</div>

- **姓名:** 罗磊
- **Email:** [dreisteine262@163.com](mailto:dreisteine262@163.com)
- **地址:** 四川省成都市
- **生日:** 1992 年 05 月 03 日
- **个人博客:** [ulti-dreisteine.github.io](https://ulti-dreisteine.github.io/academicpages/)



<div style="background:#f2f2f2;padding:6px 12px;font-weight:bold;font-size:2em;">
教育背景
</div>



### 四川大学 | 化学工程学院
**工学博士 (全日制) · 化学工程与技术 · 过程系统工程方向** | *2020.09 - 2023.06*
- **荣誉与排名:** 申请考核笔试面试成绩均第一，博士年级排名 **1 / 74**导师：吉旭 教授
- **研究方向:** 复杂系统、过程优化、因果挖掘、预测控制、贝叶斯优化
- **亮点:** 仅用 **3 年** 即获得四川大学化学工程与技术专业（过程系统工程方向）全日制科学博士学位

### 美国威斯康星大学麦迪逊分校 | 化学工程学院
**全奖攻博 · 化学工程** | *2017.08 - 2018.12*
- **研究方向:** 过程系统工程、机器学习、模拟优化
- **备注:** 中途因研究方向分配不合理且导师身患重病，无奈放弃攻读博士学位，退学回国

### 清华大学 | 化学工程系
**工学硕士 (全日制) · 化学工程与技术 · 过程系统工程方向** | *2014.09 - 2017.06*
- **荣誉与排名:** 平均学分绩 **90**，年级排名 **5 / 37**导师：邱彤 教授
- **研究方向:** 系统工程、过程建模、因果挖掘、鲁棒优化
- **获奖:** 2014-2015 年及 2015-2016 年连续获得**清华大学综合优秀奖学金**
- **亮点:** 曾获得美国康奈尔大学、威斯康星大学麦迪逊分校等提供全额奖学金攻读系统工程博士的机会

### 清华大学 | 化学工程系
**工学学士 · 化学工程与工业生物工程** | *2010.09 - 2014.06*
- **排名:** 平均学分绩 **88**，年级排名 **15 / 82**
- **获奖:** 2010-2011 年清华大学学业优秀奖学金、2011-2012 年清华大学综合优秀奖学金、2013-2014 年清华大学化工系优秀学生干部



<div style="background:#f2f2f2;padding:6px 12px;font-weight:bold;font-size:2em;">
研究经历
</div>



### 基于数据信息和概率图理论的因果挖掘和过程优化
**四川大学 · 互联化工研究中心** | *2021.01 - 2023.06*
- 针对高维的工业过程和设备数据，提出因果挖掘算法自动识别过程变量和参数间的因果作用网络在某个实际工业催化裂化过程应用中，**模型特征复杂度降低 90%，变量间关联复杂度降低 97%**
- 基于上述因果网络，利用机器学习与深度学习构建输入、操作与关键输出之间的低维紧凑数据驱动预测模型，在不损失模型预测准确性的同时提升其泛化能力
- 在数据预测与 Python + ASPEN 模型基础上，通过模拟优化手段获得在不同输入下，使过程未来一段时期内关键输出满足排放达标、安全性与经济性最优的操作方案分别使用遗传算法(GA)和粒子群优化(PSO)对类别型和连续型操作变量的最优值进行**分层求解**，显著提高计算效率
- 基于所得变量和参数因果网络和贝叶斯理论，提出一种适用于复杂过程的参数估计方法，实现过程机理知识与观测数据的融合建模；并提出**案例推理优化算法**，针对特定输入自动通过案例样本库和后验分布估计求解对应的最优操作方案

### 故障预测与健康管理 (PHM)
**四川大学 · 互联化工研究中心 & 华西医院器械监管研究与评价中心** | *2022.01 - 2022.12*
- **工业设备维护:** 基于卡尔曼滤波和蒙特卡洛模拟实现对工业过程中循环泵等设备的可靠性评价、剩余寿命预计和维护基于过程先验机理和观测数据构建变量后验因果关系图，并成功在田纳西伊士曼（Tennessee Eastman）等著名工业过程中对异常扰动和故障信号的传播路径进行识别与故障根源准确定位
- **医疗设备诊断:** 基于物联网技术，对华西医院内 CT 球管传感器和故障日志数据进行收集、清洗、治理与相关性分析考虑到故障识别中的样本不平衡问题，设计重采样算法并构建故障诊断（**F1 分数准确率为 90%**）和可靠性评价机器学习模型（**未来失效时间预测 R² > 95%**，平均误差小于 1 天）基于 SHAP、PDP 等模型解释算法，对设备故障和可靠性变化的根因进行挖掘与可视化评价

### 非线性过程动态模拟、安全边界分析和鲁棒优化
**清华大学 · 过程系统工程研究所** | *2014.07 - 2017.05*
- 基于非线性动力系统理论，对丙烯聚合反应器设备进行数学机理和 ASPEN 建模、开闭环操作稳定性和 Hopf 分岔行为分析，确定该设备的安全运行边界约束条件
- 基于鲁棒优化 and 蒙特卡洛模拟，求解过程在存在操作和参数不确定条件下，满足设备安全和产品质量等约束的最优操作方案，**降低过程操作成本、提升过程生产效率约 5%**

### 基于 GREET 软件的生物燃料全生命周期分析 (LCA)
**清华大学 · 过程系统工程研究所** | *2014.01 - 2014.06*
- 基于系统论的观点并考虑种植、运输等环节的损失和不确定影响，对小桐子等生物燃料在整个寿命周期内所有投入产出阶段的环境影响进行量化计算和能量流分析



<div style="background:#f2f2f2;padding:6px 12px;font-weight:bold;font-size:2em;">
工作经历
</div>



### 民航成都物流技术有限公司 (国企)

**运筹算法工程师 (算法组工作管理)** | *2023.09 - 2024.04*
- 负责运筹算法组工作管理，主导研发基于**混合整数规划 (MIP)**、**路径优化**等算法的机场行李分拣系统（独立高速运载、智能搬运机器人等）实时调度算法软件平台，并在实际项目中落地实施
- 负责算法数学原理推导、方案撰写、代码编写、工作组沟通协调等

### 成都佳华物链云科技有限公司 (已上市)

**技术顾问** | *2020.03 - 2023.08*
- 为项目和产品研发提供理论指导；为双碳、脱硫、污染管控等工业大数据项目的工程化部署难点攻坚提供建议和协助
- 负责算法人员招聘、机器学习和深度学习相关理论算法培训，协助技术管理工作

**算法工程师** | *2019.01 - 2023.08*
- **时序预测平台:** 主导研发基于 LSTM 等深度学习技术的时序数据预测平台，对全国地级市的气象和空气质量进行长时高精度预测，产品性能处于国内领先地位，**每年取得千万级盈利**，相关成果已申请专利
- **智慧脱硫与双碳管理:** 主导研发基于工业大数据、深度学习和模拟优化算法的智慧脱硫和双碳管理模型平台，通过 **Seq2Seq + GCN** 神经网络对 FGD 脱硫、SCR 脱硝等过程关键指标未来数十分钟内的连续变化进行预测
- **工业节能效益:** 进一步地，基于模拟优化自动计算对于当前过程的最优操作方案，辅助现场决策该产品实现了对某 600 MW 火力发电过程的实时预测，并在数秒内实现对优化问题的求解，**将过程操作的耗电量降低 3%，每年节省约 200 万元成本**（相关成果已申请专利）



<div style="background:#f2f2f2;padding:6px 12px;font-weight:bold;font-size:2em;">
参与项目
</div>


- **2022.01 - 2022.12** | 国自然青年基金项目: 基于机器学习的直肠癌术后低位前切综合征发展轨迹及预测建模 (No. 72104157)
- **2021.01 - 2023.06** | 国家重点研发计划: 十万吨级可再生能源电解水制氢合成氨示范工程 (No. 2021YFB4000500)
- **2013 - 2017** | 国家自然科学基金重点项目: 炼油过程分子管理的基础理论研究 (No. U1462206)
- **2012 - 2016** | 国家重点基础研发计划: 化工过程物质与能量高效利用的集成优化基础研究 (No. 2012CB720500)



<div style="background:#f2f2f2;padding:6px 12px;font-weight:bold;font-size:2em;">
研究成果
</div>



### 已发表论文

1. **[SCI] L. Luo**, Y. Zhou, Z. Zhou, et al. Online Optimization of Petrochemical Process via Case-based Reasoning and Conditional Mutual Information. *Chemical Engineering Research and Design*, 2024.
2. **[SCI] L. Luo**, G. He, C. Chen, et al. Adaptive Data Dimensionality Reduction for Chemical Process Modeling Based on the Information Criterion Related to Data Association and Redundancy. *Ind. Eng. Chem. Res.*, 2022.
3. **[SCI] L. Luo**, G. He, Y. Zhang, X. Ji, et al. Association Measure and Compact Prediction for Chemical Process Data from An Information-Theoretic Perspective. *Processes*, 2022.
4. **[SCI] L. Luo**, F. Cheng, T. Qiu, et al. Refined Convergent Cross-Mapping for Disturbance Propagation Analysis of Chemical Processes. *Comp. & Chem. Eng.*, 2017.
5. **[SCI] L. Luo**, N. Zhang, Z. Xia, et al. Dynamics and Stability Analysis of Gas-Phase Bulk Polymerization of Propylene. *Chem. Eng. Sci.*, 2016.
6. **[EI] 罗磊**, 程非凡, 邱彤等. 改进 CCM 算法检测外部扰动下系统变量间的时滞和因果关系. *化工学报*, 2016.
7. **[国际会议] L. Luo**, T. Qiu. Process Optimization of the Polymerization of Propylene under Parametric Disturbances. *The 7th International Symposium on Design, Operation and Control of Chemical Processes (PSE ASIA 2016)*, Tokyo, 2017.
8. **[国内会议] 罗磊**, 吉旭. 一种基于相关性分析和深度学习的多元非线性时间序列通用预测方法及其在化工过程中的应用. *2020 年中国过程系统工程年会*, 重庆, 2020.
9. **[SCI]** G. He, **L. Luo**, L. Zhou, et al. Deep learning prediction of yields of fluid catalytic cracking via differential evolutionary dual-stage attention-based LSTM. *Fuel*, 2024.
10. **[SCI]** Y. Zhang, **L. Luo**, X. Ji, et al. Improved Random Forest Algorithm Based on Decision Paths for Fault Diagnosis of Chemical Process with Incomplete Data. *Sensors*, 2021.
11. **[SCI]** L. He, **L. Luo**, X. Hou, et al. Predicting Venous Thromboembolism in Hospitalized Trauma Patients: A Combination of the Caprini Score and Data-Driven Machine Learning Model. *BMC Emergency Medicine*, 2021.
12. **[SCI]** S. Wang, M. Cheng, **L. Luo**, et al. High-throughput screening of metal–organic frameworks for hydrogen purification. *Chem. Eng. J.*, 2022.
13. **[SCI]** M. Cheng, S. Wang, **L. Luo**, et al. Large-Scale Computational Screening of Metal-Organic Framework Membranes for Ethane/Ethylene Separation. *Acta Chimica Sinica*, 2022.
14. **[SCI]** Wei Jiang, Z. Li, X. Kang, **L. Luo** et al. Hybrid modeling approach for natural gas desulfurization process: Coupling mechanism and data modeling via compact variable identification. *Gas Science and Engineering*, 2024.

### 专利申请

- **[已授权]** **罗磊**, 李辰等. 一种污染物浓度的预测模型训练方法、预测方法及装置, 2020.
- **[已授权]** 张承武, **罗磊**等. 一种复合脱硫装置石膏浆液密度测量方法及测量系统, 2020.
- **[已授权]** 廖强, **罗磊**, 王晓健等. 一种脱硫优化方法、装置、电子设备及存储介质, 2020.
- **[已授权]** 廖强, 王向勇, 陈俊, 李辰, **罗磊**, 段斌. 一种工艺参数的预测方法、装置、电子设备及存储介质, 2021.
- **[审中]** **罗磊**, 李玮, 廖强等. 基于高斯回归的大气污染物浓度的预测方法及装置, 2020.
- **[审中]** 廖强, 陈俊, 王向勇, 李辰, 刘正一, **罗磊**. 机器负荷预测方法、装置、电子设备及可读存储介质, 2021.

### 参与比赛与获奖

- **2021 年** | 百度天池国家电网调控 AI 创新大赛：新能源发电预测，技术顾问
- **2020 年** | 中国环境保护产业协会“环境技术进步二等奖”，第五完成人
- **2019 年** | 阿里天池比赛：面料裁剪利用率优化，主要参与人



<div style="background:#f2f2f2;padding:6px 12px;font-weight:bold;font-size:2em;">
能力擅长
</div>



- **方法技术:**
  - **化工模拟:** 精通 **ASPEN** (5年)、精通 **HYSYS** (3年) 等
  - **数据挖掘:** 相关分析、统计因果推断、显著性检验、数据降维等
  - **统计模型:** 广义线性模型、贝叶斯网络、因果结构学习、参数估计、时间序列等
  - **机器学习:** 决策树、集成学习树、支持向量机、K 近邻等
  - **深度学习:** MLP、**LSTM**、CNN、**GCN** 等适用于时空域的神经网络模型
  - **优化算法:** 线性规划、**混合整数规划 (MIP)**、鲁棒优化、模拟退火、遗传算法、粒子群算法等
  - **过程控制:** 强化学习、自适应控制等
- **工程能力:**
  - **编程语言:** 精通 **Python** (5年)、熟悉 **Matlab** (3年)、**R** (2年) 等
  - **工具与求解器:** 熟悉 **PyTorch** (深度学习)、PyCaret (机器学习)、PyMC (贝叶斯统计)、**Gurobi** (运筹优化)、GAMS (运筹优化)、COPT (运筹学) 等求解器和软件
  - **数据库与接口:** 熟悉 MySQL、Redis、Flask 等数据库和接口使用方法
- **外语能力:**
  - 通过 **CET-4、CET-6** 考试，具有优秀的英文读写能力
  - 通过 **TOEFL、GRE** 考试



<div style="background:#f2f2f2;padding:6px 12px;font-weight:bold;font-size:2em;">
自我评价
</div>



1. **顶尖大学工科专业出身 (清华、川大)**，数理能力扎实，富有进取心，乐于挑战高难度问题
2. 善于利用**系统工程思维**对任务进行统筹规划和分解，思路清晰严谨，做事高效干练
3. **兼具较强的科研和工作经历**，能够将理论研究和工程应用很好地结合，实现研究成果的快速工程化落地
4. 在**工业物联网、大数据**等领域取得了一定的学术积累和成果，有丰富的数据分析、模型研发和项目落地经验
5. 具有较强的组织和沟通协调能力，带领技术团队完成了多个关键产品的研发落地并实现千万级盈利
6. 为人真诚善良，做事踏实，乐于分享，兴趣广泛，爱好机器学习、历史、足球等
