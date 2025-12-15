# awesome-RL-fusion-papers

## [category]

[AuthorYearPub] title, publication, year, vol, no, pp. 



## 平顶层控制

### 磁流体（MHD）平衡、位置与形状控制

> 平顶阶段最基础的任务是维持等离子体的形状（如拉长比、三角变形）和位置稳定。

[Degrave2022]Magnetic control of tokamak plasmas through deep reinforcement learning[J]. Nature, 2022, 602(7897): 414-419.[DOI](https://www.nature.com/articles/s41586-021-04301-9)

> **平顶阶段磁场跟踪与维持控制**。RL 直接驱动 TCV 的控制线圈，实现等离子体位置与形状跟踪/维持，且实现复杂构型（例如双液滴）。RL 控制真实托卡马克的里程碑

[Brendan2024]Towards practical reinforcement learning for tokamak magnetic control[J]. Fusion Engineering and Design, 2024, 200: 114161.[DOI](https://www.sciencedirect.com/science/article/pii/S0920379624000140)

> **长期/稳态跟踪控制**。在Degrave基础上改进 RL 训练与控制精度，增强长期追踪能力（减少 steady-state 偏差）。

[Subbotin2025] Reconstruction-free magnetic control of DIII-D plasma with deep reinforcement learning. arXiv, 2025.

> 深度RL用于实时磁控制，提升鲁棒性并处理放电过程中包括平顶在内的整体控制任务，旨在**维持等离子体目标形状/位置**。“第一个将深度强化学习用于中等大小的DIII-D tokamak等离子体磁控制的工作”，用的SAC算法。

### 核心参数与性能控制

> 平顶阶段的目标是获得高性能输出，涉及对 $\beta$、密度、温度的控制（这些参数是0D参数，关注平均值和总量）

[Seo2021] Feedforward beta control in the KSTAR tokamak by deep reinforcement learning, *Nucl. Fusion*, 2021, 61, p.106010. [DOI](https://iopscience.iop.org/article/10.1088/1741-4326/ac121b)

> 通过深度RL实现KSTAR托卡马克的前馈β控制，提升了聚变前馈控制的灵活性。$\beta$（等离子体压强与磁压强之比）是衡量聚变性能的关键指标，**$\beta$** **控制**是典型的平顶阶段高性能维持任务。

[Zhang2024]Real-time feedback control of β p based on deep reinforcement learning on east[J]. Plasma Physics and Controlled Fusion, 2024, 66(5): 055014.[DOI](https://iopscience.iop.org/article/10.1088/1361-6587/ad3749/meta)

> 在 EAST 上实现极向比压 **β_p** 的实时反馈控制

[Wakatsuki2021] Ion temperature gradient control using reinforcement learning technique, *Nucl. Fusion*, 2021, 61, p.046036. [DOI](https://iopscience.iop.org/article/10.1088/1741-4326/abe68d)

> 用RL实现离子**温度梯度控制**，拓展了RL在聚变参数控制中的应用场景。离子温度梯度（ITG）通过影响湍流输运来决定约束性能，在平顶阶段优化能量约束时间。

[Seo2024]Avoiding fusion plasma tearing instability with deep reinforcement learning[J]. Nature, 2024, 626(8000): 746-751.[DOI](https://www.nature.com/articles/s41586-024-07024-9)

> RL 主动识别并抑制撕裂模。撕裂模是限制托卡马克平顶阶段性能（$\beta$ 极限）和导致破裂的主要原因。该工作通过控制**束功率**等来避免

[Paruchuri2025] Density regulation with disruption avoidance in next-generation tokamaks using a safe reinforcement learning-based controller. Fusion Engineering and Design, 2025, 216, 115064. [DOI](https://doi.org/10.1016/j.fusengdes.2025.115064).

> 主要贡献是引入安全强化学习来进行控制。**密度控制**是平顶阶段的核心问题，特别是在规避密度极限的同时维持高密度。



[Wakatsuki2023]Simultaneous control of safety factor profile and normalized beta for JT-60SA using reinforcement learning[J]. Nuclear Fusion, 2023, 63(7): 076017.[DOI](https://iopscience.iop.org/article/10.1088/1741-4326/acd393/meta)

> 用 RL 同时控制安全因子剖面q-profile 与归一化$\beta_N$，解决多目标**剖面控制**问题。剖面问题的参数是1D参数，关注物理量在空间中的分布。

### 其他

[Seo2022]Development of an operation trajectory design algorithm for control of multiple 0D parameters using deep reinforcement learning in KSTAR[J]. Nuclear Fusion, 2022, 62(8): 086049.[DOI](https://iopscience.iop.org/article/10.1088/1741-4326/ac79be/meta)

> 在 KSTAR 上用 deep RL 同时控制多种电磁参量，自动生成 tokamak 的操作序列，规划整段放电。平顶维持是其中的核心部分。

[Char2023] Offline Model-Based Reinforcement Learning for Tokamak Control, *NeurIPS*, 2023, 211, pp.1357 - 1372. [DOI](https://proceedings.mlr.press/v211/char23a.html)

> 提出离线模型基强化学习算法，解决托卡马克控制中“数据获取成本高”的问题，最终部署到DIII-D装置。算法本身可以用于平顶阶段的控制策略训练，但关注点是离线学习与数据效率，而不是场景阶段本身。

[Wu2025]High-fidelity data-driven dynamics model for reinforcement learning-based control in HL-3 tokamak[J]. Communications Physics, 2025, 8(1): 393.[DOI](https://www.nature.com/articles/s42005-025-02302-y)

> data-driven simulator + RL 控制。用实验数据构建高保真动力学模型，为 RL 提供准确的仿真tokamak模型。用到HL-3上





## 托卡马克等离子体控制（强化学习应用）
[DeGrave2022] Magnetic control of tokamak plasmas through deep reinforcement learning, *Nature*, 2022, 602(7897), pp.414-419. [DOI](https://doi.org/10.1038/s41586-021-04301-9)
>核心内容：用深度强化学习实现托卡马克19个磁线圈的自主控制，精准调控等离子体位置/形状，还实现了双等离子体“液滴”构型，是RL在核聚变领域的里程碑成果。

[Char2023] Offline Model-Based Reinforcement Learning for Tokamak Control, *NeurIPS*, 2023, 211, pp.1357 - 1372. [DOI](https://proceedings.mlr.press/v211/char23a.html)
>核心内容：提出离线模型基强化学习算法，解决托卡马克控制中“数据获取成本高”的问题，提升了RL算法在核聚变场景的实用性。

[Katz2024] Learning plasma dynamics and robust rampdown trajectories with predict-first experiments at TCV, *Nature Communications*, 2024, 15(1), pp.1-11. [DOI](https://www.nature.com/articles/s41467-025-63917-x)
>核心内容：结合“先预测后实验”思路，用强化学习学习等离子体动力学规律，实现了更鲁棒的等离子体放电回落轨迹控制。

[Wakatsuki2019] Safety factor profile control with reduced central solenoid flux consumption during plasma current ramp-up phase using a reinforcement learning technique, *Nucl. Fusion*, 2019, 59, p.066022. [DOI](https://iopscience.iop.org/article/10.1088/1741-4326/ab1571)
>核心内容：将RL用于等离子体电流上升阶段的安全因子剖面控制，是RL在聚变控制中的早期实践。

[Wakatsuki2021] Ion temperature gradient control using reinforcement learning technique, *Nucl. Fusion*, 2021, 61, p.046036. [DOI](https://iopscience.iop.org/article/10.1088/1741-4326/abe68d)
>核心内容：用RL实现离子温度梯度控制，拓展了RL在聚变参数控制中的应用场景。

[Seo2021] Feedforward beta control in the KSTAR tokamak by deep reinforcement learning, *Nucl. Fusion*, 2021, 61, p.106010. [DOI](https://iopscience.iop.org/article/10.1088/1741-4326/ac121b)
>核心内容：通过深度RL实现KSTAR托卡马克的前馈β控制，提升了聚变前馈控制的灵活性。

[Seo2024] Avoiding fusion plasma tearing instability with deep reinforcement learning. Nature, 2024, 626, pp. 746–751. [DOI](https://doi.org/10.1038/s41586-021-04301-9)
> 使用强化学习进行高层控制（控制beam power和triangularity）以防止tearing instability。

[Brendan2024] Towards practical reinforcement learning for tokamak magnetic control.  Fusion Engineering and Design, 2024, 200, 114161. [DOI](https://doi.org/10.1016/j.fusengdes.2024.114161).
> 改进了一下deepmind Nature那篇工作

[Dubbioso2023] A Deep Reinforcement Learning approach for Vertical Stabilization of tokamak plasmas. Fusion Engineering and Design, 2023, 194, 113725. [DOI](https://doi.org/10.1016/j.fusengdes.2023.113725).
> 用DDPG训了一个Vertical Stabilization Agent，环境应该是通过微分方程求解模拟的。动作是线圈中的电压。

[Kerboua-Benlarbi2025] Curriculum Reinforcement Learning for Tokamak Control. [DOI](https://doi.org/10.1007/978-981-97-9536-9_3).
> 用课程学习加速了控制策略的学习。（注：这个官网引用是引用成一本书的一部分，我这里就先只放题目了）

[Kerboua-Benlarbi2024] Artificial intelligence and fusion plasma control : application to the WEST tokamak. HAL, 2024, 2024COAZ5060.
> 同样使用了课程学习，在WEST中使用RL训练控制策略。

[Wang2024] Active Disruption Avoidance and Trajectory Design for Tokamak Ramp-downs with Neural Differential Equations and Reinforcement Learning. arXiv, 2024.
[Wang2025] Active ramp-down control and trajectory design for tokamaks with neural differential equations and reinforcement learning. Commun Phys, 2025, 8, 231. [DOI](https://doi.org/10.1038/s42005-025-02146-6)
> 使用强化学习控制等离子体安全ramp-down。不过好像没提出新RL方法，主要讨论是集中在simulator上。（这两篇应该是同一篇）

[Paruchuri2025] Density regulation with disruption avoidance in next-generation tokamaks using a safe reinforcement learning-based controller. Fusion Engineering and Design, 2025, 216, 115064. [DOI](https://doi.org/10.1016/j.fusengdes.2025.115064).
> 主要贡献是引入安全强化学习来进行控制。

[Seo2022] Development of an operation trajectory design algorithm for control of multiple 0D parameters using deep reinforcement learning in KSTAR. Nuclear Fusion, 2022, 62, 086049. [DOI](https://doi.org/10.1088/1741-4326/ac79be)
> 使用RL控制，使一些参数达到任意预先指定的目标。

[Subbotin2025] Reconstruction-free magnetic control of DIII-D plasma with deep reinforcement learning. arXiv, 2025. 
> “第一个将深度强化学习用于中等大小的DIII-D tokamak等离子体磁控制的工作”，用的SAC算法。

## 可控核聚变中的机器学习/神经网络应用
[Bishop1995] Real time control of a tokamak plasma using neural networks, *Neural Comput.*, 1995, 7, pp.206–217.[DOI](https://direct.mit.edu/neco/article-abstract/7/1/206/5840/Real-Time-Control-of-a-Tokamak-Plasma-Using-Neural?redirectedFrom=fulltext)
>核心内容：早期神经网络用于托卡马克等离子体的实时控制，是智能控制在核聚变领域的早期探索。

[Joung2019] Deep neural network Grad-Shafranov solver constrained with measured magnetic signals, *Nucl. Fusion*, 2019, 60, p.16034. [DOI](https://iopscience.iop.org/article/10.1088/1741-4326/ab555f)
>核心内容：用深度神经网络求解Grad-Shafranov方程，实现等离子体平衡重建，是机器学习在聚变诊断中的典型应用。

[Kates-Harbeck2019] Predicting disruptive instabilities in controlled fusion plasmas through deep learning, *Nature*, 2019, 568(7753), pp.526–531. [DOI](https://doi.org/10.1038/s41586-019-1116-4)
>核心内容：通过深度学习预测等离子体破裂不稳定性，提升了核聚变装置的运行安全性，是AI在聚变安全领域的代表性成果。

[van de Plassche2020] Fast modeling of turbulent transport in fusion plasmas using neural networks, *Phys. Plasmas*, 2020, 27, p.022310. [DOI](https://pubs.aip.org/aip/pop/article-abstract/27/2/022310/1062590/Fast-modeling-of-turbulent-transport-in-fusion?redirectedFrom=fulltext)
>核心内容：用神经网络加速聚变等离子体湍流输运建模，解决了传统物理模型精度不足的问题。

[Abbate2021] Data-driven profile prediction for DIII-D, *Nucl. Fusion*, 2021, 61, p.046027. [DOI](https://iopscience.iop.org/article/10.1088/1741-4326/abe08d)
>核心内容：采用数据驱动方法（机器学习）实现DIII-D托卡马克的剖面预测，是机器学习在聚变参数预测中的应用。

[Wu2025] High-fidelity data-driven dynamics model for reinforcement learning-based control in HL-3 tokamak. Commun Phys, 2025, 8, 393. [DOI](https://doi.org/10.1038/s42005-025-02302-y).
> 一个数据驱动的simulator

## RL基础

[Shakya2023]. Reinforcement learning algorithms: A brief survey[J]. Expert Systems with Applications, 2023, 231: 120495.[DOI](https://journals.aps.org/rmp/abstract/10.1103/RevModPhys.95.025005)

> 综述了强化学习的基本原理、基本方法和实例应用。

[Sutton2018]Reinforcement Learning: An Introduction (Cambridge, MA: MIT press) (available at:[SuttonBartoIPRLBook2ndEd.pdf](https://web.stanford.edu/class/psych209/Readings/SuttonBartoIPRLBook2ndEd.pdf))

> 一本书

[Recht2019]A tour of reinforcement learning: The view from continuous control[J]. Annual Review of Control, Robotics, and Autonomous Systems, 2019, 2(1): 253-279.[DOI](https://www.annualreviews.org/content/journals/10.1146/annurev-control-053018-023825)

> 从优化与控制的角度综述强化学习，重点关注连续控制的应用。

## 可控核聚变背景

[Meschini2023]Review of commercial nuclear fusion projects[J]. Frontiers in Energy Research, 2023, 11: 1157394.[DOI](https://www.frontiersin.org/journals/energy-research/articles/10.3389/fenrg.2023.1157394/full)

> 核聚变项目概述，路线层面

[Ongena2016]Magnetic-confinement fusion[J]. Nature Physics, 2016, 12(5): 398-410.[DOI](https://www.nature.com/articles/nphys3745)

> MCF基础物理、过去成就、现状与未来前景

[Wan2023]Steady-state burning plasma: a new stage in the development of magnetic confinement fusion energy[J]. National Science Review, 2023, 10(12): nwad217.[DOI](https://academic.oup.com/nsr/article/10/12/nwad217/7242561)

> MCF，主要是托克马克，发展阶段、物理问题、工程问题

[Hurricane2023]Physics principles of inertial confinement fusion and US program overview[J]. Reviews of Modern Physics, 2023, 95(2): 025005.[DOI](https://journals.aps.org/rmp/abstract/10.1103/RevModPhys.95.025005)

> ICF美国设施及国际进展，路线、进展、问题

[Hurricane2023]Inertial Confinement Fusion: Status and Challenges[J]. Annual Review of Nuclear and Particle Science, 2025, 75.

> ICF实现方案及最新进展

## 控制问题

> RL 在聚变领域的应用，集中在Tokamak 控制问题上。ICF 的核心瓶颈是物理、过程问题，没有持续可控发反馈阶段。

### 等离子体形状控制

> 等离子体用磁场托着，很容易变形接触到容器壁

[Degrave2022]Magnetic control of tokamak plasmas through deep reinforcement learning[J]. Nature, 2022, 602(7897): 414-419.[DOI](https://www.nature.com/articles/s41586-021-04301-9)

> RL 直接驱动 TCV 的控制线圈，实现复杂形状。RL 控制真实托卡马克的里程碑

[Brendan2024]Towards practical reinforcement learning for tokamak magnetic control[J]. Fusion Engineering and Design, 2024, 200: 114161.[DOI](https://www.sciencedirect.com/science/article/pii/S0920379624000140)

> 在Degrave等人（2022）基础上改进 RL 训练与控制精度

### 内部剖面控制（参数：q-profile、β_p、β_N、压力、电流等）（实时决策）

> 等离子体内部有很多关键剖面参数，剖面的形状指示很多指标（稳定性等等）

[Wakatsuki2023]Simultaneous control of safety factor profile and normalized beta for JT-60SA using reinforcement learning[J]. Nuclear Fusion, 2023, 63(7): 076017.[DOI](https://iopscience.iop.org/article/10.1088/1741-4326/acd393/meta)

> 用 RL 同时控制 q-profile 与归一化，解决多目标剖面控制问题

[Zhang2024]Real-time feedback control of β p based on deep reinforcement learning on east[J]. Plasma Physics and Controlled Fusion, 2024, 66(5): 055014.[DOI](https://iopscience.iop.org/article/10.1088/1361-6587/ad3749/meta)

> 在 EAST 上实现 β_p 的实时反馈控制

### Disruption预测

[Seo2024]Avoiding fusion plasma tearing instability with deep reinforcement learning[J]. Nature, 2024, 626(8000): 746-751.[DOI](https://www.nature.com/articles/s41586-024-07024-9)

> RL 主动识别并抑制撕裂模

[Paruchuri 2025]Density regulation with disruption avoidance in next-generation tokamaks using a safe reinforcement learning-based controller[J]. Fusion Engineering and Design, 2025, 216: 115064.[DOI](https://www.sciencedirect.com/science/article/pii/S0920379625002625)

> 提出 safe RL 控制器，在稳密度调节的同时尽量避免扰动。保持等离子体密度在目标范围，同时避免运行进入危险区导致破裂

### 操作轨迹设计

> 一次完整放电过程有很多阶段，每个阶段需要同时调节电流、密度、温度等参数

[Seo2022]Development of an operation trajectory design algorithm for control of multiple 0D parameters using deep reinforcement learning in KSTAR[J]. Nuclear Fusion, 2022, 62(8): 086049.[DOI](https://iopscience.iop.org/article/10.1088/1741-4326/ac79be/meta)

> 在 KSTAR 上用 deep RL 同时控制多种电磁参量，自动生成 tokamak 的操作序列，规划整段放电

[Wang2025]Active ramp-down control and trajectory design for tokamaks with neural differential equations and reinforcement learning[J]. Communications Physics, 2025, 8(1): 231.[DOI](https://www.nature.com/articles/s42005-025-02146-6)

> 将神经微分方程 (Neural ODE) 与 RL 结合，用于放电尾段 ramp-down 的主动控制与轨迹设计，安全下电 / 减少扰动

### 垂直稳定控制

> 等离子体容易垂直方向不稳定，倾倒撞壁

[Dubbioso2023]A deep reinforcement learning approach for vertical stabilization of tokamak plasmas[J]. Fusion Engineering and Design, 2023, 194: 113725.[DOI](https://www.sciencedirect.com/science/article/pii/S0920379623003083)

> 等离子体磁控问题中垂直稳定控制问题

### 缺乏物理模型的复杂动力学场景

[Wu2025]High-fidelity data-driven dynamics model for reinforcement learning-based control in HL-3 tokamak[J]. Communications Physics, 2025, 8(1): 393.[DOI](https://www.nature.com/articles/s42005-025-02302-y)

> data-driven simulator + RL 控制。用实验数据构建高保真动力学模型，为 RL 提供准确的仿真tokamak模型


## Github Code
### 使用RL训练控制策略
- https://github.com/jaem-seo/AI_tokamak_control
> 可以运行，但这个不是训练，他是基于一个可视化模拟器（ https://github.com/jaem-seo/KSTAR_tokamak_simulator ）提供的实时ai控制可视化（他提供了现成的模型）
- https://github.com/danieleschmidt/tokamak-rl-control-suite
> 据说是一个基于sb3的rl控制套件，实际跑不动，连README里的basic training example都会报错
> 
> 已经给他提issue了（但没有回复）
- https://github.com/ZINZINBIN/Tokamak-Plasma-Operation-Control-based-on-RL
> 首先，这个仓库没有给训练参数，代码里有一组默认的参数，不知道能不能用，我试图去搜了一下论文，根本搜不到，只有一个poster
> 
> 第二，这个仓库没有requirements
> 
> 第三，这个仓库不提供数据集
- https://github.com/LucasCJYSDL/Offline-RL-Kit-for-Nuclear-Fusion
> 一个离线训练的仓库，也跑不动，因为它同时需要数据集和dynamic model

### 环境仿真器
- https://github.com/jaem-seo/KSTAR_tokamak_simulator
> 和前面那个能跑的代码是一起的，应该也能跑
> 
> 但这里提到的论文所里好像没买，看不了
- https://github.com/google-deepmind/torax
> 能跑，但我不太确定这个咋用
- https://github.com/IRFM/METIS
> matlab的代码，先不做尝试了
- https://github.com/ZINZINBIN/KSTAR-data-driven-tokamak-simulator
> 没有readme，也没有demo，但感觉可能可以跑，因为其他东西基本齐全
- https://github.com/yuina822/amaterasu
> 可以跑，似乎是一个基于微分方程的模拟器，没有论文，无法确定其精度如何
- https://github.com/ArvinSKushwaha/Plasma-Simulator
> c++写的，看起来还没完成
- https://github.com/cticenhour/EELS
> 看代码应该也是c++写的，没文档
- https://github.com/nikaslukyanov/Interactive-Tokamak-Simulator
> 一个基于OpenFUSIONToolkit（ https://github.com/OpenFUSIONToolkit/OpenFUSIONToolkit ）的可视化软件，暂时不确定是否可用
