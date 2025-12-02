# awesome-RL-fusion-papers

## [category]

[AuthorYearPub] title, publication, year, vol, no, pp. 



## 托卡马克等离子体控制（强化学习应用）
[DeGrave2022] Magnetic control of tokamak plasmas through deep reinforcement learning, *Nature*, 2022, 602(7897), pp.414-419. [DOI](https://doi.org/10.1038/s41586-021-04301-9)
>核心内容：用深度强化学习实现托卡马克19个磁线圈的自主控制，精准调控等离子体位置/形状，还实现了双等离子体“液滴”构型，是RL在核聚变领域的里程碑成果。

[Chen2023] Offline Model-Based Reinforcement Learning for Tokamak Control, *NeurIPS*, 2023, 211, pp.1357 - 1372. [DOI](https://proceedings.mlr.press/v211/char23a.html)
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

