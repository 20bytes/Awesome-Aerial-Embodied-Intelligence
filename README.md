<p align="center">
  <h1 align="center">🚁 Awesome Aerial Embodied Intelligence</h1>
  <p align="center">
    <a href="https://github.com/sindresorhus/awesome"><img src="https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg" alt="Awesome"></a>
    <img src="https://img.shields.io/badge/Papers-935-0984e3?style=for-the-badge&logo=google-scholar&logoColor=white" alt="Papers">
    <img src="https://img.shields.io/badge/License-MIT-6c5ce7?style=for-the-badge" alt="License">
    <img src="https://img.shields.io/badge/Focus-Aerial%20Embodied%20AI-00b894?style=for-the-badge" alt="Focus">
    <img src="https://img.shields.io/badge/Since-2026.04-fd79a8?style=for-the-badge" alt="Since 2026.04">
  </p>
  <p align="center"><b>面向空中具身智能的中文精读资源库 · 自 2026 年 4 月起持续更新</b></p>
  <p align="center"><i>聚焦无人机视觉语言导航的前沿论文、数据集、仿真器与开源代码，每条目附中文解读与技术标签</i></p>
  <p align="center"><i>VLA 大模型 · Aerial VLN · 零样本导航 · LLM 驱动无人机 · Sim-to-Real</i></p>
</p>

---

## 📋 Table of Contents

| | Section | Description |
|:---:|:---|:---|
| 🤖 | [VLA Models & End-to-End Navigation](#-vla-models--end-to-end-navigation) | 视觉-语言-动作大模型与端到端导航 |
| 🗺️ | [Zero-Shot Navigation & Exploration](#️-zero-shot-navigation--exploration) | 零样本目标导航与自主探索建图 |
| 📊 | [Benchmarks, Datasets & Simulation](#-benchmarks-datasets--simulation) | 评测基准、数据集与仿真平台 |
| 📦 | [Dataset Comparison](#-dataset-comparison) | 数据集结构化对比 |
| 🎮 | [Simulator Comparison](#-simulator-comparison) | 仿真平台结构化对比 |
| 🔄 | [Sim-to-Real](#-sim-to-real) | 模拟到现实迁移 |
| 📝 | [Surveys & Perspectives](#-surveys--perspectives) | 综述与前瞻 |
| 📌 | [Other Foundational Works](#-other-foundational-works) | 其他基础工作 |
| 🔗 | [Related Works](#-related-works) | 相关资源 |

> [!NOTE]
> **论文排序** — 同一年份内按月份降序排列（最新的在前）。特别有影响力或代表性的工作，无论日期均可能被置于顶部。

> [!TIP]
> **欢迎贡献** — 本仓库持续更新！如有尚未收录的论文、项目或资源，或发现错误、失效链接，欢迎提交 **Pull Request** 或开 **Issue**，一起打造空中具身智能社区的综合资源库。
>
> **条目模板：**
> ```markdown
> - **[年份.月][ 会议/来源 年份 - 中文简短描述 ]** 论文英文标题 [[arxiv]](URL) [[hjfy]](URL) [[github]](URL) `Method` `Backbone` `Env`
>   - 概览：一句话中文概述核心贡献。
> ```
> 标签放标题行末尾（链接之后），用 `` `反引号` `` 徽章：`Method`（方法范式）、`Backbone`（主干模型）、`Env`（仿真环境）。
>
> **免责声明** — 本库为个人整理的学术资源索引，论文标题、日期、链接等信息以官方来源（arXiv / 会议官网 / 期刊页面）为准，整理过程中难免存在疏漏或更新不及时。本库内容仅供学习与研究参考，论文版权归原作者及出版方所有。

## 🤖 VLA Models & End-to-End Navigation

### 2026
- **[2026.07][ arXiv 2026 - 快慢双系统空中长时程VLN - FSD-VLN ]** FSD-VLN: Fast-Slow Dual-System Modeling for Aerial Long-Horizon Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2607.08359) [[hjfy]](https://hjfy.top/arxiv/2607.08359) `Hierarchical` `GR00T N1+DiT` `AirVLN-S+OpenFly`
  - 概览：提出快慢双系统空中VLN框架，慢系统用VLM异步提取稳定语义先验、快系统用扩散Transformer高频生成时序连贯飞行动作，未见环境成功率提升近2倍且单步延迟与任务耗时均减半。

- **[2026.07][ arXiv 2026 - 空间感知无人机遮挡追踪VLA - CosFly-VLA ]** CosFly-VLA: A Spatially Aware Vision-Language-Action Model for UAV Tracking [[arxiv]](https://arxiv.org/abs/2607.15004) [[hjfy]](https://hjfy.top/arxiv/2607.15004) `End-to-end` `Qwen3.5` `CARLA`
  - 概览：提出空间感知无人机追踪VLA模型，用元查询解耦多头同步输出目标框、遮挡概率与八步航迹，并以空间预训练、课程微调、CoT推理、闭环强化学习四阶段训练实现遮挡后目标找回。

- **[2026.07][ arXiv 2026 - 语言条件四旋翼动作中心世界动作模型 - AeroAct ]** AeroAct: Action-Centered World-Action Models for Language-Conditioned Quadrotor Flight [[arxiv]](https://arxiv.org/abs/2607.14997) [[hjfy]](https://hjfy.top/arxiv/2607.14997) `World Model` `Wan2.1-1.3B (DiT)` `Isaac Lab+3DGS`
  - 概览：提出动作中心世界动作模型AeroAct，训练时用未来第一视角帧做稠密监督、推理时跳过视频生成直接解码多项式轨迹动作块，首次实现基于WAM的实体四旋翼语言条件闭环飞行。

- **[2026.07][ arXiv 2026 - 纯视觉长时程无人机导航范式与基准 - VoLN ]** VoLN: Vision-Only Long-Horizon Navigation---Paradigm, Benchmark, and Method [[arxiv]](https://arxiv.org/abs/2607.21400) [[hjfy]](https://hjfy.top/arxiv/2607.21400) [[github]](https://github.com/Admire-ljb/VoLN-UAV) [[project]](https://admire-ljb.github.io/VoLN-UAV/) `Benchmark` `Vicuna-7B` `AirSim+UE4`
  - 概览：提出彻底移除GPS、全局地图与文字指令、仅凭终点参考图与机载视觉完成长时程飞行的VoLN范式，构建17场景7210条轨迹的VoLN-UAV仿真基准，并给出DINO-CLIP语义对齐加LoRA微调大模型预测3D航点的VoLN-MLLM基线。

- **[2026.07][ CVPR 2026 - 免训练空中对话导航 - PSC-AVDN ]** Parse, Search, and Confirmation: Training-Free Aerial Vision-and-Dialog Navigation with Chain-of-Thought Reasoning and Structured Spatial Memory [[arxiv]](https://arxiv.org/abs/2607.11529) [[hjfy]](https://hjfy.top/arxiv/2607.11529) [[github]](https://github.com/QY6616/PSC-AVDN) `Zero-Shot` `MLLM+CoT` `ANDH`
  - 概览：提出免训练空中视觉对话导航框架PSC-AVDN，将指令解析、思维链搜索与候选确认三阶段推理同结构化空间记忆耦合，在高空细粒度地标辨识中缓解方向歧义与长期空间一致性问题。

- **[2026.06][ arXiv 2026 - 世界模型驱动的无人机VLA导航 - WorldFly ]** WorldFly: A World-Model-Based Vision-Language-Action Model for UAV Navigation [[arxiv]](https://arxiv.org/abs/2606.06147) [[hjfy]](https://hjfy.top/arxiv/2606.06147) `World Model` `T5+Flow Matching DiT` `OpenFly+AirSim`
  - 概览：提出双分支耦合流匹配的世界模型VLA框架，在预判未来航拍画面的同时同步生成导航动作，用空间想象反哺飞行决策，并构建城市峡谷穿越基准，陌生街区成功率较OpenFly近乎翻倍。

- **[2026.06][ arXiv 2026 - 细粒度长时序无人机导航基准与异步VLA - FLIGHT ]** Think Like a Pilot: Fine-Grained Long-Horizon UAV Navigation [[arxiv]](https://arxiv.org/abs/2606.06836) [[hjfy]](https://hjfy.top/arxiv/2606.06836) [[github]](https://github.com/buaa-colalab/FLIGHT) [[project]](https://buaa-colalab.github.io/FLIGHT/) `Benchmark` `Hierarchical` `VLM+DiT` `UnrealZoo`
  - 概览：构建首个兼顾多阶段长时序指令与稠密6自由度连续轨迹标注的无人机导航基准FLIGHT，并提出低频流式飞行员推理VLM与高频扩散动作模型异步解耦的FLIGHT VLA架构。

- **[2026.06][ arXiv 2026 - 非对称MoE解耦空中操控VLA - AIR-VLA+ ]** AIR-VLA+: Decoupling Movement and Manipulation via Cascaded Dual-Action Decoders with Asymmetric MoE for Aerial Robots [[arxiv]](https://arxiv.org/abs/2606.12859) [[hjfy]](https://hjfy.top/arxiv/2606.12859) `End-to-end` `π0.5 (Flow Matching+MoE)` `AIR-VLA Bench`
  - 概览：为解决无人机宏观运动与机械臂微观操控的表示耦合，提出级联双动作解码器与非对称特征级MoE的流匹配VLA架构，实现认知协同与物理解耦，在AIR-VLA基准上任务完成率较单头π0.5提升80.2%。

- **[2026.06][ arXiv 2026 - 视野内精准抵达空中VLN - 3DG-VLN ]** See-and-Reach: Precise Vision-Language Navigation for UAVs within the Field of View [[arxiv]](https://arxiv.org/abs/2606.20045) [[hjfy]](https://hjfy.top/arxiv/2606.20045) [[github]](https://github.com/xuefanfu/3DG-VLN) `End-to-end` `Qwen2.5-VL-7B` `AirSim+UE4`
  - 概览：首次将“看见-抵达”阶段从整体导航中剥离，提出UAV-VLN-FOV任务与2717条轨迹高分辨率基准，并设计3D方向引导框架3DG-VLN，以双视角观测与在线方向更新将成功率提升13.82%。

- **[2026.06][ arXiv 2026 - 无人机VLN动态感知连续轨迹生成 - DynFly ]** DynFly: Dynamic-Aware Continuous Trajectory Generation for UAV Vision-Language Navigation in Urban Environments [[arxiv]](https://arxiv.org/abs/2606.31654) [[hjfy]](https://hjfy.top/arxiv/2606.31654) `Diffusion` `Spline-DiT (Flow Matching)` `OpenUAV`
  - 概览：提出面向无人机VLN的动态感知连续轨迹生成框架DynFly，在B样条控制点空间用Spline-DiT流匹配生成轨迹，并施加速度、加速度与航向一致性等动态监督，在OpenUAV基准上同步提升导航精度与轨迹平滑度。

- **[2026.06][ arXiv 2026 - 世界-动作模型驱动的空中VLN - ImagineUAV ]** ImagineUAV: Aerial Vision-Language Navigation via World-Action Modeling and Kinodynamic Planning [[arxiv]](https://arxiv.org/abs/2606.01205) [[hjfy]](https://hjfy.top/arxiv/2606.01205) `World Model` `Wan2.1-1.3B` `UAV-Flow`
  - 概览：提出想象驱动的级联世界-动作建模框架，用指令条件视频扩散模型生成未来第一人称观测，再提取6自由度动作并由动力学规划器优化为无碰撞轨迹，仅1.3B参数即取得SOTA。

- **[2026.06][ arXiv 2026 - 双视觉通路启发的无人机-卫星协同空间推理 - SatAgent ]** AeroVerse-SatAgent: UAV-Satellite Collaborative Spatial Reasoning Inspired by the Dual Visual Pathway Theory of Cognitive Neuroscience [[arxiv]](https://arxiv.org/abs/2606.31467) [[hjfy]](https://hjfy.top/arxiv/2606.31467) `End-to-end` `Qwen3.5-9B`
  - 概览：受认知神经科学双视觉通路理论启发提出无人机-卫星协同空间推理模型，用几何感知3D重建编码器与跨视角拓扑-语义对齐在统一BEV下融合双路特征，并发布13万样本的SR130K数据集。

- **[2026.06][ arXiv 2026 - 大模型驱动的无人机自主智能体框架 - AerialClaw ]** AerialClaw: An Open-Source Framework for LLM-Driven Autonomous Aerial Agents [[arxiv]](https://arxiv.org/abs/2606.12142) [[hjfy]](https://hjfy.top/arxiv/2606.12142) [[github]](https://github.com/XDEI-Group/AerialClaw) `Agentic` `AirSim+PX4/Gazebo`
  - 概览：提出开源的大模型无人机自主智能体框架，由认知决策、技能体系、安全约束、硬件适配、设备执行与记忆反思六层架构组成，用户仅用自然语言描述即可完成巡检、避障与报告生成的全流程闭环。

- **[2026.06][ CVPR 2026 - 记忆增强开放世界空中目标导航 - OctMem-Agent ]** Memory-Augmented Scene Understanding and Exploration for Open-World Aerial Object-Goal Navigation [[cvf]](https://openaccess.thecvf.com/content/CVPR2026/papers/Zhou_Memory-Augmented_Scene_Understanding_and_Exploration_for_Open-World_Aerial_Object-Goal_Navigation_CVPR_2026_paper.pdf) `End-to-end` `LLaMA2-7B (OpenVLA)` `UAV-ON`
  - 概览：提出记忆增强空中目标导航框架OctMem-Agent，用距离自适应八叉树构建层级三维场景记忆，以指令调制的场景/探索双分支查询平衡目标定位与未知区域探索，在UAV-ON基准上成功率提升7.5%。

- **[2026.06][ CVPR 2026 Findings - 视觉思维链驱动的无人机导航 - CoTFly ]** CoTFly: Making UAVs Think Where to Fly Next Through Visual Chain-of-Thought Reasoning [[cvf]](https://openaccess.thecvf.com/content/CVPR2026F/papers/Wang_CoTFly_Making_UAVs_Think_Where_to_Fly_Next_Through_Visual_CVPRF_2026_paper.pdf) [[github]](https://github.com/joannahuadu/CoTFly) `End-to-end` `LLaVA-NeXT` `OpenUAV`
  - 概览：提出视觉思维链导航框架CoTFly，让无人机先推理中途子目标地标及包围盒再输出飞行动作，配合自动构建的UAV-CoT数据集与两轮微调，在OpenUAV上成功率提升11.1%、导航误差降低20米。

- **[2026.06][ arXiv 2026 - 无人机细粒度主动感知具身问答 - ScoutVLA ]** ScoutVLA: UAV-Centric Active Perception via a Dual-Expert VLA Model for Open-World Embodied Question Answering [[arxiv]](https://arxiv.org/abs/2606.14772) [[hjfy]](https://hjfy.top/arxiv/2606.14772) [[project]](https://anonymous.4open.science/w/ScoutVLA-B31F/) `End-to-end` `PaliGemma 2 + Flow Matching`
  - 概览：构建首个无人机细粒度主动感知具身问答基准FG-EQA，并提出仿生侦察蜂的双专家VLA模型ScoutVLA，以语义专家与流匹配动作专家解耦训练实现连续视角微调，严格成功率达基线的10.48倍。

- **[2026.05][ arXiv 2026 - 面向空中VLN的自回归世界动作模型 - WorldVLN ]** WorldVLN: Autoregressive World Action Model for Aerial Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2605.15964) [[hjfy]](https://hjfy.top/arxiv/2605.15964) [[github]](https://github.com/EmbodiedCity/WorldVLN.code) [[project]](https://embodiedcity.github.io/WorldVLN/) `World Model` `AR Video Transformer` `UAV-Flow`
  - 概览：提出首个面向空中视觉语言导航的自回归世界动作模型，在隐空间预测短时域世界状态转移并直接解码为可执行航点，配合Action-aware GRPO后训练与闭环观测更新，成功率较VLA基线提升12%以上。

- **[2026.04][ CVPR 2026 - 方向感知空中视觉语言导航 - LookasideVLN ]** LookasideVLN: Direction-Aware Aerial Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2604.17190) [[hjfy]](https://hjfy.top/arxiv/2604.17190) `Hierarchical` `Transformer`
  - 概览：提出了方向感知的无人机视觉语言导航新范式。针对现有方法过度依赖地标而忽视方向线索的问题，通过自我中心的旁视提取图（ELG）和空间地标知识库（SLKB），有效利用语言指令中的方向信息，显著提升了无人机空间推理的准确性与计算效率。

- **[2026.04][ arXiv 2026 - 分层IL-RL城市空中VLN框架 - HTNav ]** HTNav: A Hybrid Navigation Framework with Tiered Structure for Urban Aerial Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2604.08883) [[hjfy]](https://hjfy.top/arxiv/2604.08883) `Hierarchical` `CityNav`
  - 概览：提出模仿学习与强化学习两阶段混合训练的分层导航框架，由宏观规划器生成中间路标、微观执行器输出细粒度动作，并以残差加SCConv地图表征增强空间连续性理解，在CityNav全场景全难度刷新SOTA。

- **[2026.03][ AAAI 2026 - 在线对话引导的无人机导航 - AerialVLA ]** A Vision-Language-Action Model for Aerial Navigation with Online Dialogue [[aaai]](https://ojs.aaai.org/index.php/AAAI/article/view/38878) [[github]](https://colalab.net/) `End-to-end` `VLA`
  - 概览：提出了一种通过在线对话引导的空中导航视觉-语言-动作模型，引入了进度驱动的导航-查询交替机制，允许无人机主动向人类询问指导以克服导航歧义。

- **[2026.03][ arXiv 2026 - 机载零样本视觉语言导航 - OnFly ]** OnFly: Onboard Zero-Shot Aerial Vision-Language Navigation toward Safety and Efficiency [[arxiv]](https://arxiv.org/abs/2603.10682) [[hjfy]](https://hjfy.top/arxiv/2603.10682) [[github]](https://github.com/Robotics-STAR-Lab/OnFly) `Zero-Shot` `Qwen3-VL-4B-AWQ` `AirSim+UE4`
  - 概览：提出了一个全机载的零样本空中视觉-语言导航框架，通过分离目标生成与进度监控，结合语义-几何验证器，在保证安全的前提下大幅提升了导航成功率。

- **[2026.03][ arXiv 2026 - 极简端到端无人机VLA - AerialVLA (Xu) ]** AerialVLA: A Vision-Language-Action Model for UAV Navigation via Minimalist End-to-End Control [[arxiv]](https://arxiv.org/abs/2603.14363) [[hjfy]](https://hjfy.top/arxiv/2603.14363) [[github]](https://github.com/XuPeng23/AerialVLA) `End-to-end` `OpenVLA` `OpenUAV`
  - 概览：提出了基于OpenVLA的极简端到端无人机视觉-语言-动作模型，在OpenUAV平台上验证，通过最小化控制信号设计实现高效的空中导航策略学习。

- **[2026.03][ Neurocomputing 2026 - 统一表征与结构化空间推理的无人机VLN - DroneNav ]** DroneNav: Unified Text-Visual Representation and Structured Spatial Reasoning for Robust UAV Vision-and-Language Navigation [[doi]](https://doi.org/10.1016/j.neucom.2026.133492) `Hierarchical`
  - 概览：提出"先解耦后集成"的两阶段专家模型框架，以层次化特征蒸馏与指令引导多模态交互构建统一文本-视觉表征，结合行为驱动的结构化空间决策提升复杂城市环境下无人机VLN的鲁棒性与泛化性。

- **[2026.03][ arXiv 2026 - 几何引导表征对齐的城市无人机VLN - SpatialFly ]** SpatialFly: Implicit 3D Prior-Guided Visual Reparameterization for Continuous UAV Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2603.21046) [[hjfy]](https://hjfy.top/arxiv/2603.21046) `End-to-end` `Qwen2.5-3B+VGGT` `OpenUAV`
  - 概览：针对无人机VLN中2D视觉感知与3D轨迹决策的表征失配，提出几何先验注入与几何感知重参数化模块，无需显式三维重建即可对齐视觉词元，在OpenUAV未见场景上导航误差降低4.03m。

- **[2026.03][ arXiv 2026 - 物理引导的VLA模型空中操作迁移 - AirVLA ]** $π$, But Make It Fly: Physics-Guided Transfer of VLA Models to Aerial Manipulation [[arxiv]](https://arxiv.org/abs/2603.25038) [[hjfy]](https://hjfy.top/arxiv/2603.25038) [[project]](https://airvla.github.io) `End-to-end` `π0` `3DGS`
  - 概览：探究将操作预训练VLA模型π0迁移至空中平台，提出推理时的有效载荷感知引导在流匹配采样中注入物理约束，并用3DGS管线合成导航数据，460次真机实验中抓放成功率从23%提升至50%。

- **[2026.03][ arXiv 2026 - 空中视觉语言导航 - FreeFly-Thinking ]** FreeFly-Thinking : Aligning Chain-of-Thought Reasoning with Continuous UAV Navigation [[arxiv]](https://arxiv.org/abs/2603.07181) [[hjfy]](https://hjfy.top/arxiv/2603.07181) `End-to-end`
  - 概览：通过将无人机第一视角图像与自然语言指令相结合，构建专用于导航任务的无人机数据集，并采用两阶段训练策略：监督微调与强化微调。

- **[2026.03][ arXiv 2026 - 空中视觉语言导航 - ViSA-Enhanced Aerial VLN ]** ViSA-Enhanced Aerial VLN: A Visual-Spatial Reasoning Enhanced Framework for Aerial Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2603.08007) [[hjfy]](https://hjfy.top/arxiv/2603.08007) `Zero-Shot` `GSM` `VLM`
  - 概览：该框架采用三重协作架构，通过结构化视觉提示技术，使视觉语言模型能够直接在图像平面上进行推理，无需额外训练或复杂的中间表示。

- **[2026.03][ arXiv 2026 - 时序逻辑约束修复的低空无人机语言导航 ]** LLM-Enabled Low-Altitude UAV Natural Language Navigation via Signal Temporal Logic Specification Translation and Repair [[arxiv]](https://arxiv.org/abs/2603.27583) [[hjfy]](https://hjfy.top/arxiv/2603.27583) `Agentic`
  - 概览：提出低空无人机自然语言导航框架，以推理增强LLM将自由文本翻译为信号时序逻辑约束，并结合混合整数规划和语义修复生成安全可行轨迹。

- **[2026.02][ ICLR 2026 - 野外无人机自主导航VLA模型 - AutoFly ]** AutoFly: Vision-Language-Action Model for UAV Autonomous Navigation in the Wild [[arxiv]](https://arxiv.org/abs/2602.09657) [[hjfy]](https://hjfy.top/arxiv/2602.09657) [[project]](https://xiaolousun.github.io/AutoFly) `End-to-end` `LLaMA2-7B`
  - 概览：提出了专为未知野外环境设计的端到端无人机视觉-语言-动作（VLA）模型，引入伪深度编码器增强3D空间推理，并构建了大规模多模态自主导航数据集。

- **[2026.02][ arXiv 2026 - 视频模型做零样本3D导航 - NavDreamer ]** NavDreamer: Video Models as Zero-Shot 3D Navigators [[arxiv]](https://arxiv.org/abs/2602.09765) [[hjfy]](https://hjfy.top/arxiv/2602.09765) `Zero-Shot` `Qwen-VL3 (Wan2.6 + π³)`
  - 概览：提出基于视频生成模型的零样本3D导航框架NavDreamer，将语言指令转化为视频预测再提取航点轨迹，通过采样优化和VLM评分选择最优路径，在未见环境中展现强泛化能力。

- **[2026.02][ arXiv 2026 - 大模型充当室内无人机飞行员 - VLN-Pilot ]** VLN-Pilot: Large Vision-Language Model as an Autonomous Indoor Drone Operator [[arxiv]](https://arxiv.org/abs/2602.05552) [[hjfy]](https://hjfy.top/arxiv/2602.05552) `Agentic` `GPT-4.1/Gemini-2.5-Flash` `Unity`
  - 概览：让大视觉语言模型扮演室内无人机“飞行员”，以VLLM高层语义推理加有限状态机低层执行的混合架构，在Unity高真实感室内仿真基准上实现自由形式自然语言指令的全自主飞行。

- **[2026.01][ arXiv 2026 - 大规模真实世界UAV VLN数据集 - AirNav ]** AirNav: A Large-Scale UAV Vision-and-Language Navigation Dataset with Natural and Diverse Instructions [[arxiv]](https://arxiv.org/abs/2601.03707) [[hjfy]](https://hjfy.top/arxiv/2601.03707) `End-to-end` `VLM+RL`
  - 概览：提出基于真实城市航拍数据构建的大规模UAV VLN基准AirNav，包含自然多样的导航指令，并引入AirVLN-R1结合监督微调与强化微调提升泛化性能。

- **[2026.01][ TechRxiv 2026 - 无人机室内外统一视觉语言导航 - AirUniNav ]** AirUniNav: Unified Vision-Language Navigation for UAVs in Indoor and Outdoor Scenes [[techrxiv]](https://www.techrxiv.org/doi/full/10.36227/techrxiv.176834454.46554529) [[project]](https://forhumble.github.io/AirUni/) `End-to-end` `VideoChat-Flash` `Habitat+AirSim`
  - 概览：基于视频多模态大模型构建室内外统一的无人机视觉语言导航框架，以视觉-文本令牌交互联合建模历史与当前观测，并用时间衰减权重动态采样压缩长航程视觉流，在240万联合样本上实现跨场景泛化。

### 2025

- **[2025.12][ AAAI 2026 - 历史增强两阶段空中VLN - HETT ]** History-Enhanced Two-Stage Transformer for Aerial Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2512.14222) [[hjfy]](https://hjfy.top/arxiv/2512.14222) `End-to-end` `Transformer (Two-Stage)`
  - 概览：提出两阶段Transformer框架（HETT），首先结合地标和历史上下文预测粗粒度的全局目标方位，然后再通过历史栅格地图聚合视觉特征，执行局部的细粒度动作调整（Coarse-to-fine）。

- **[2025.12][ AAAI 2026 - 室内无人机视觉语言导航基准 - IndoorUAV ]** IndoorUAV: Benchmarking Vision-Language UAV Navigation in Continuous Indoor Environments [[arxiv]](https://arxiv.org/abs/2512.19024) [[hjfy]](https://hjfy.top/arxiv/2512.19024) `End-to-end`
  - 概览：提出首个面向室内无人机的视觉语言导航基准IndoorUAV，包含IndoorUAV-VLN（长时导航）和IndoorUAV-VLA（短时规划）两个子集，并提出IndoorUAV-Agent利用LLM分段指令再由VLA执行飞行控制。

- **[2025.12][ arXiv 2025 - 长距离UAV视觉语言导航 - LongFly ]** LongFly: Long-Horizon UAV Vision-and-Language Navigation with Spatiotemporal Context Integration [[arxiv]](https://arxiv.org/abs/2512.22010) [[hjfy]](https://hjfy.top/arxiv/2512.22010) `End-to-end` `Attention/GRU`
  - 概览：提出面向长距离UAV VLN的时空上下文建模框架LongFly，将碎片化冗余的历史数据转化为结构化紧凑的表征，有效提升长时程导航中的语义对齐和路径规划稳定性。

- **[2025.12][ arXiv 2025 - 复杂环境下的机载VLA导航框架 - VLA-AN ]** VLA-AN: An Efficient and Onboard Vision-Language-Action Framework for Aerial Navigation in Complex Environments [[arxiv]](https://arxiv.org/abs/2512.15258) [[hjfy]](https://hjfy.top/arxiv/2512.15258) `End-to-end` `3D-GS`
  - 概览：提出了一种渐进式训练的高效机载视觉-语言-动作（VLA）飞行框架，采用基于3D高斯喷溅（3D-GS）的高保真仿真来弥合 Sim-to-Real 差异，并能以极低延迟部署在受限机载硬件上。

- **[2025.12][ arXiv 2025 - 空中导航世界模型 - ANWM ]** Aerial World Model for Long-horizon Visual Generation and Navigation in 3D Space [[arxiv]](https://arxiv.org/abs/2512.21887) [[hjfy]](https://hjfy.top/arxiv/2512.21887) `World Model`
  - 概览：提出一种空中导航世界模型（ANWM），利用"未来帧投影（FFP）"模块将过去帧映射到未来视角以提供几何先验。智能体能以此对未来画面进行长距离预测并依据语义合理性去评估规划路线。

- **[2025.12][ arXiv 2025 - 单目RGB空中VLN时空具身统一框架 - AeroAct ]** Aerial Vision-Language Navigation with a Unified Framework for Spatial, Temporal and Embodied Reasoning [[arxiv]](https://arxiv.org/abs/2512.08639) [[hjfy]](https://hjfy.top/arxiv/2512.08639) [[github]](https://github.com/return-sleep/AeroAct) `End-to-end` `NVILA-8B` `AerialVLN+OpenFly`
  - 概览：仅凭单目RGB观测与语言指令，将空中VLN统一建模为下一Token预测并联合优化空间感知、轨迹推理与动作预测，配合关键帧选择、动作合并与标签重加权，在AerialVLN与OpenFly上取得单目设定SOTA。

- **[2025.11][ arXiv 2025 - 开放世界空中视觉语言导航 - OpenVLN ]** OpenVLN: Open-world Aerial Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2511.06182) [[hjfy]](https://hjfy.top/arxiv/2511.06182) `End-to-end`
  - 概览：提出面向开放世界的空中视觉语言导航框架OpenVLN，利用强化学习和值模型应对数据稀缺和长视域规划的双重挑战，在复杂空中环境中实现语言引导飞行。

- **[2025.11][ arXiv 2025 - 无人机导航空间智能基准与感知模型 - SpatialSky ]** Is your VLM Sky-Ready? A Comprehensive Spatial Intelligence Benchmark for UAV Navigation [[arxiv]](https://arxiv.org/abs/2511.13269) [[hjfy]](https://hjfy.top/arxiv/2511.13269) [[github]](https://github.com/linglingxiansen/SpatialSKy) `Benchmark` `Qwen2.5-VL-7B`
  - 概览：构建覆盖环境感知与场景理解两大类13项子能力的无人机空间智能基准与百万级数据集，并以SFT+GRPO两阶段训练出Sky-VLM，在全部任务上超越现有开源与闭源VLM。

- **[2025.09][ CoRL 2025 - 免训练VLM无人机导航框架 ]** See, Point, Fly: A Learning-Free VLM Framework for Universal Unmanned Aerial Navigation [[arxiv]](https://arxiv.org/abs/2509.22653) [[hjfy]](https://hjfy.top/arxiv/2509.22653) [[github]](https://github.com/Hu-chih-yao/see-point-fly) `Zero-Shot` `VLM (GPT-4V)`
  - 概览：提出免训练的空中VLN框架SPF，将导航决策重新定义为2D空间定位任务，VLM直接在图像上标注下一步航点，无需任何任务特定训练即可实现视觉-语言对齐导航，在主要基准上超越现有方法63%。

- **[2025.09][ ICIP 2025 - 结构化指令解析与场景对齐无人机VLN ]** Structured Instruction Parsing and Scene Alignment For UAV Vision-Language Navigation [[doi]](https://doi.org/10.1109/ICIP55913.2025.11084696) `Hierarchical`
  - 概览：提出结构化指令解析与场景对齐框架，利用大语言模型从导航指令中提取关键要素并构建粒度适宜的子任务，实现指令语言与无人机视觉线索的精确对齐，提升空中VLN导航性能。

- **[2025.08][ ACM MM 2025 - 双无人机协同VLN - AeroDuo ]** AeroDuo: Aerial Duo for UAV-based Vision and Language Navigation [[arxiv]](https://arxiv.org/abs/2508.15232) [[hjfy]](https://hjfy.top/arxiv/2508.15232) `End-to-end`
  - 概览：提出了一种双无人机协同的视觉-语言导航（VLN）框架。高空无人机利用多模态大模型进行目标推理，低空无人机利用轻量级多阶段策略进行精细导航与目标定位，两者仅交换最小坐标信息即可实现高效协同。

- **[2025.08][ arXiv 2025 - 语义感知高斯课程调度的无人机VLN - SA-GCS ]** SA-GCS: Semantic-Aware Gaussian Curriculum Scheduling for UAV Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2508.00390) [[hjfy]](https://hjfy.top/arxiv/2508.00390) `RL` `Qwen2.5-VL` `CityNav`
  - 概览：提出语义感知高斯课程调度框架，用VLM跨模态注意力与Soft-IoU量化训练样本难度，再以高斯调度器动态调整GRPO强化学习的采样分布实现由易到难训练，在CityNav上加速收敛并全面超越基线。

- **[2025.07][ arXiv 2025 - 流式视觉语言导航 - StreamVLN ]** StreamVLN: Streaming Vision-and-Language Navigation via SlowFast Context Modeling [[arxiv]](https://arxiv.org/abs/2507.05240) [[hjfy]](https://hjfy.top/arxiv/2507.05240) [[project]](https://streamvln.github.io/) `End-to-end` `SlowFast`
  - 概览：为应对真实环境的长视频流处理，提出混合的SlowFast上下文建模策略。Fast支路通过滑动窗口实现低延迟流式响应，Slow支路通过Token剪枝实现历史状态的记忆更新，极大提升了流式VLN效率。

- **[2025.07][ ACM MM demo 2025 - 无人机多模态交互与智能助手 ]** "Hi AirStar, Guide Me to the Badminton Court." [[arxiv]](https://arxiv.org/abs/2507.04430) [[hjfy]](https://hjfy.top/arxiv/2507.04430) `End-to-end` `LLM`
  - 概览：推出了一款名为 AirStar 的无人机具身智能助理系统。该系统将大语言模型作为认知核心，支持用户通过自然语音和手势直接与无人机交互，内置长程地理知识导航与短程精细控制等功能，摆脱了传统遥控器。

- **[2025.07][ IROS 2025 - 城市无人机VLN与NMPC控制 - SkyVLN ]** SkyVLN: Vision-and-Language Navigation and NMPC Control for UAVs in Urban Environments [[arxiv]](https://arxiv.org/abs/2507.06564) [[hjfy]](https://hjfy.top/arxiv/2507.06564) `Hierarchical` `GPT-4` `AirSim+UE4`
  - 概览：提出融合细粒度空间描述器与轨迹回溯记忆阵列的城市无人机视觉语言导航框架，结合非线性模型预测控制实现动态避障与轨迹跟踪，显著提升未见城市场景下的导航成功率与效率。

- **[2025.05][ ACL 2025 - 分层语义规划空中VLN - CityNavAgent ]** CityNavAgent: Aerial Vision-and-Language Navigation with Hierarchical Semantic Planning and Global Memory [[arxiv]](https://arxiv.org/abs/2505.05622) [[hjfy]](https://hjfy.top/arxiv/2505.05622) `GSM` `LLM (Hierarchical)`
  - 概览：提出分层语义规划与全局记忆结合的空中VLN智能体CityNavAgent，通过LLM进行高层语义规划并维护全局地标记忆，在CityNav基准上取得SOTA性能。

- **[2025.05][ arXiv 2025 - 低空终端配送无人机VLN系统 - LogisticsVLN ]** LogisticsVLN: Vision-Language Navigation For Low-Altitude Terminal Delivery Based on Agentic UAVs [[arxiv]](https://arxiv.org/abs/2505.03460) [[hjfy]](https://hjfy.top/arxiv/2505.03460) `Agentic` `Qwen2-VL-7B` `CARLA`
  - 概览：提出首个面向窗口级低空终端配送的无人机视觉语言导航系统，以轻量级LLM/VLM模块化完成请求理解、楼层定位与目标探索，并在CARLA中构建了VLD配送数据集。

- **[2025.05][ arXiv 2025 - 可泛化可解释的无人机VLN - FlightGPT ]** FlightGPT: Towards Generalizable and Interpretable UAV Vision-and-Language Navigation with Vision-Language Models [[arxiv]](https://arxiv.org/abs/2505.12835) [[hjfy]](https://hjfy.top/arxiv/2505.12835) [[github]](https://github.com/Uavln/FlightGPT) `RL` `Qwen2.5-VL-7B` `CityNav`
  - 概览：提出基于视觉语言模型的无人机VLN框架FlightGPT，采用监督微调加GRPO强化学习的两阶段训练并引入思维链推理机制，在CityNav未见环境上成功率较最强基线提升9.22%。

- **[2025.05][ arXiv 2025 - 多智能体ReAct无人机任务规划 - UAV-CodeAgents ]** UAV-CodeAgents: Scalable UAV Mission Planning via Multi-Agent ReAct and Vision-Language Reasoning [[arxiv]](https://arxiv.org/abs/2505.07236) [[hjfy]](https://hjfy.top/arxiv/2505.07236) `Agentic` `Qwen2.5-VL-7B`
  - 概览：提出基于ReAct范式的多智能体无人机任务规划框架，由空域管理智能体解析卫星影像与自然语言指令并协同生成航迹，微调Qwen2.5-VL-7B实现像素级语义定位，任务成功率达93%。

- **[2025.04][ AAAI 2025 - 细粒度对齐的空中视觉对话导航 ]** Learning Fine-Grained Alignment for Aerial Vision-Dialog Navigation [[aaai]](https://ojs.aaai.org/index.php/AAAI/article/view/32758) `End-to-end`
  - 概览：针对空中视觉对话导航（AVDN）中细粒度跨模态对齐问题，构建了实体-地标级标注数据集FG-AVDN，并提出FELA方法通过定位、描述和对比学习三种辅助任务显式学习实体-地标对齐，SR提升3.2%。

- **[2025.04][ ECMR 2025 - 端到端无人机视觉语言导航 - UAV-VLN ]** UAV-VLN: End-to-End Vision Language guided Navigation for UAVs [[arxiv]](https://arxiv.org/abs/2504.21432) [[hjfy]](https://hjfy.top/arxiv/2504.21432) `Hierarchical` `TinyLlama-1.1B` `Gazebo+ROS2`
  - 概览：提出无人机端到端视觉语言导航框架UAV-VLN，微调TinyLlama-1.1B解析自由指令生成子目标，结合Grounding DINO开放词汇定位与ROS2规划执行，并构建1000+条空中指令数据集实现室内外零样本导航。

- **[2025.04][ Pattern Recognition 2026 - 双尺度地理空间推理空中导航 - GeoNav ]** GeoNav: Empowering MLLMs with dual-scale geospatial reasoning for language-goal aerial navigation [[arxiv]](https://arxiv.org/abs/2504.09587) [[hjfy]](https://hjfy.top/arxiv/2504.09587) [[doi]](https://doi.org/10.1016/j.patcog.2026.113365) `Agentic` `GPT-4o` `CityNav`
  - 概览：提出面向语言目标空中导航的多模态智能体GeoNav，构建图解式认知地图与层次化场景图双尺度空间表征，以空间思维链驱动MLLM分阶段完成地标导航、目标搜索与精确定位。

- **[2025.04][ IEEE SMC 2025 - 无人机动态场景语义理解智能体 - AirVista-II ]** AirVista-II: An Agentic System for Embodied UAVs Toward Dynamic Scene Semantic Understanding [[arxiv]](https://arxiv.org/abs/2504.09583) [[hjfy]](https://hjfy.top/arxiv/2504.09583) `Agentic` `GPT-4o/LLaVA-1.6`
  - 概览：提出面向无人机动态场景语义理解的端到端智能体系统AirVista-II，通过智能体任务识别调度与针对即时图像/短视频/长视频的差异化关键帧提取策略，在零样本设置下实现高质量场景问答与推理。

- **[2025.03][ arXiv 2025 - 竞速无人机VLA导航 - RaceVLA ]** RaceVLA: VLA-based Racing Drone Navigation with Human-like Behaviour [[arxiv]](https://arxiv.org/abs/2503.02572) [[hjfy]](https://hjfy.top/arxiv/2503.02572) `End-to-end`
  - 概览：首个专为竞速无人机设计的VLA大模型，模型输入FPV视频和自然语言，直接输出4D连续控制信号（三轴线速度+偏航角速度），使无人机在动态场景中表现出类人的自主避障和穿梭能力。

- **[2025.03][ arXiv 2025 - 网格视图选择与地图构建的空中VLN ]** Aerial Vision-and-Language Navigation with Grid-based View Selection and Map Construction [[arxiv]](https://arxiv.org/abs/2503.11091) [[hjfy]](https://hjfy.top/arxiv/2503.11091) `End-to-end` `Cross-modal Transformer` `AirSim+UE4`
  - 概览：将空中VLN动作预测建模为网格化视图选择任务，显式耦合垂直与水平动作，并构建鸟瞰网格地图融合导航历史，用跨模态Transformer对齐长程历史与指令。

- **[2025.03][ arXiv 2025 - 无人机认知任务VLA模型与基准 - CognitiveDrone ]** CognitiveDrone: A VLA Model and Evaluation Benchmark for Real-Time Cognitive Task Solving and Reasoning in UAVs [[arxiv]](https://arxiv.org/abs/2503.01378) [[hjfy]](https://hjfy.top/arxiv/2503.01378) [[project]](https://cognitivedrone.github.io/) `End-to-end` `OpenVLA-7B` `Gazebo`
  - 概览：提出面向无人机认知任务的VLA模型CognitiveDrone及其VLM推理增强版R1，并基于Gazebo构建首个无人机认知能力开源评测基准CognitiveDroneBench，涵盖人类识别、符号理解与推理三类任务。

- **[2025.02][ ICLR 2026 - 监督到强化自适应空中VLN - Openfly ]** Openfly: A comprehensive platform for aerial vision-language navigation [[arxiv]](https://arxiv.org/abs/2502.18041) [[hjfy]](https://hjfy.top/arxiv/2502.18041) [[project]](https://shailab-ipec.github.io/openfly/) `End-to-end` `LLaMA` `OpenFly`
  - 概览：提出从监督学习到强化学习的自适应训练框架，结合大规模空中 VLN 数据集与仿真工具链，显著提升无人机在复杂真实环境中的导航成功率。
  - 个人评价：目前最好用的 benchmark 和数据生成工具链，算力要求较高 8 张 A100（每张 80 G）

- **[2025.01][ IEEE HRI 2025 - 大规模空中任务生成 - UAV-VLA ]** UAV-VLA: Vision-Language-Action System for Large Scale Aerial Mission Generation [[arxiv]](https://arxiv.org/abs/2501.05014) [[hjfy]](https://hjfy.top/arxiv/2501.05014) `End-to-end` `VLM+GPT`
  - 概览：提出一种将卫星图像处理、VLM与基于GPT的规划相结合的系统，仅需简单的文本指令即可全局生成无人机的航路点与动作序列，在大规模任务生成上比人类操作快6.5倍。

### 2024

- **[2024.11][ arXiv 2024 - 多尺度城市街景融合无人机VLN - NavAgent ]** NavAgent: Multi-scale Urban Street View Fusion For UAV Embodied Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2411.08579) [[hjfy]](https://hjfy.top/arxiv/2411.08579) `End-to-end` `VLM`
  - 概览：提出多尺度城市街景融合的无人机VLN框架NavAgent，通过融合不同粒度的城市街景信息增强空间推理，提升城市级复杂环境下的导航能力。

- **[2024.10][ ICLR 2025 - 真实感UAV导航基准与大模型方法 ]** Towards Realistic UAV Vision-Language Navigation: Platform, Benchmark, and Methodology [[arxiv]](https://arxiv.org/abs/2410.07087) [[hjfy]](https://hjfy.top/arxiv/2410.07087) [[github]](https://github.com/prince687028/Travel) `End-to-end` `LLaMA` `AirSim+UE4`
  - 概览：构建了基于虚幻引擎的连续飞行导航基准，并提出了基于多模态大模型的层次化轨迹生成方法。

- **[2024.10][ arXiv 2024 - 语义拓扑度量表示引导LLM推理空中VLN - STMR ]** Exploring Spatial Representation to Enhance LLM Reasoning in Aerial Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2410.08500) [[hjfy]](https://hjfy.top/arxiv/2410.08500) `Zero-Shot` `LLM (CoT)` `AirSim+UE4`
  - 概览：提出免训练的LLM空中VLN端到端框架，设计融合语义、拓扑与度量信息的矩阵表示STMR增强LLM户外空间推理能力，在AerialVLN-S仿真与真机实验中显著提升导航成功率。

### 2023

- **[2023.12][ arXiv 2023 - LLM驱动无人机飞行控制 - TypeFly ]** TypeFly: Flying Drones with Large Language Model [[arxiv]](https://arxiv.org/abs/2312.14950) [[hjfy]](https://hjfy.top/arxiv/2312.14950) [[github]](https://github.com/typefly/TypeFly) `Zero-Shot` `LLM (MiniSpec)`
  - 概览：提出ChatFly系统，利用自定义的MiniSpec语言大幅降低LLM在无人机控制中的响应延迟（减少62%），使大语言模型能够高效、实时地驱动无人机完成复杂飞行任务。

- **[2023.08][ ICCV 2023 - 开篇之作 - AerialVLN ]** AerialVLN: Vision-and-Language Navigation for UAVs [[arxiv]](https://arxiv.org/abs/2308.06735) [[hjfy]](https://hjfy.top/arxiv/2308.06735) [[github]](https://github.com/AirVLN/AirVLN) `End-to-end` `CMA` `AirSim+UE4`
  - 概览：提出首个面向无人机连续环境的视觉语言导航任务、AirVLN仿真平台与基准模型，系统刻画空中视角、三维动作空间和长距离飞行给指令跟随带来的挑战。
  - 个人评价：benchmark 不好用，复现结果不一致，算力要求一般

### 2022

- **[2022.05][ ACL 2023 Findings - 空中视觉对话导航 - AVDN ]** Aerial Vision-and-Dialog Navigation [[arxiv]](https://arxiv.org/abs/2205.12219) [[hjfy]](https://hjfy.top/arxiv/2205.12219) [[project]](https://sites.google.com/view/aerial-vision-and-dialog/home) `End-to-end` `Transformer`
  - 概览：提出了空中视觉与对话导航（AVDN）任务和数据集，无人机通过多轮自然语言对话与人类协作完成目标定位，是对话引导式空中导航的早期基础工作（ACL 2023 Findings）。

## 🗺️ Zero-Shot Navigation & Exploration

### 2026
- **[2026.07][ arXiv 2026 - 扩散精炼的无人机最后十米视觉伺服 - DreamNav ]** Last-Meter Precision Navigation for UAVs: A Diffusion-Refined Aerial Visual Servoing Approach [[arxiv]](https://arxiv.org/abs/2607.04352) [[hjfy]](https://hjfy.top/arxiv/2607.04352) [[github]](https://github.com/YaxuanLi-cn/PairUAV) `Diffusion` `World Model` `PairUAV`
  - 概览：提出粗到精的扩散精炼空中视觉伺服框架，先用三角参数化回归稳定旋转估计，再借预训练世界模型想象候选动作的未来视觉以筛选轨迹，并发布481万图像对的PairUAV基准。

- **[2026.07][ arXiv 2026 - 野外无人机主动目标检测数据集与世界模型方法 - ATRNet-LUDO ]** Toward Active Object Detection for UAVs in the Wild: A Large-Scale Dataset, Benchmark and Method [[arxiv]](https://arxiv.org/abs/2607.09078) [[hjfy]](https://hjfy.top/arxiv/2607.09078) [[github]](https://github.com/Leo000ooo/ATRNet-LUDO) `World Model` `JEPA+Dueling DQN`
  - 概览：发布首个野外无人机-地面主动目标检测实景数据集ATRNet-LUDO与统一评测基准，含12.1万全景航拍图和121万目标切片，并提出结合JEPA世界模型与场景净化的AOD-JEPA策略提升跨场景泛化。

- **[2026.07][ arXiv 2026 - 波浪平台无人机自主着舰分层RL - WaveLander ]** WaveLander: A Generalizable Hierarchical Control Framework for UAV Landing on Wave-Disturbed Platforms via Reinforcement Learning [[arxiv]](https://arxiv.org/abs/2607.01281) [[hjfy]](https://hjfy.top/arxiv/2607.01281) `Hierarchical` `GRU+PPO` `MuJoCo+Isaac Sim`
  - 概览：提出分层无人机着舰框架，高层强化学习仅凭四维甲板相对观测输出连续垂向速度指令决策下降时机，底层沿用PID飞控，经仿真、软件在环与真实海试验证显著提升风浪环境着陆成功率。

- **[2026.06][ arXiv 2026 - 双视图扩散规划室内无人机寻物导航 - AgenticDiffusion ]** AgenticDiffusion: Agentic Diffusion-based Path Planning for Vision-Based UAV Navigation [[arxiv]](https://arxiv.org/abs/2606.04111) [[hjfy]](https://hjfy.top/arxiv/2606.04111) `Agentic` `Grounding DINO+Diffusion` `ProcTHOR`
  - 概览：把LLM智能体推理、开放词汇目标定位、FPV与顶视双视角扩散轨迹生成及NMPC控制串成统一的室内无人机导航流水线，仿真训练零微调上机，40次真机试飞任务成功率80%。

- **[2026.06][ arXiv 2026 - 世界模型驱动的通用无人机导航 - AirDreamer ]** AirDreamer: Generalist Drone Navigation with World Models [[arxiv]](https://arxiv.org/abs/2606.03252) [[hjfy]](https://hjfy.top/arxiv/2606.03252) `World Model` `DreamerV3-RSSM` `OmniDrones`
  - 概览：用DreamerV3的RSSM世界模型把深度图与机身状态编码进隐空间，仅靠稀疏奖励训练强化学习策略，无人机自发涌现转头扫视与绕障脱困行为，域随机化后零微调迁移真机。

- **[2026.06][ ICRA 2026 - 微型无人机光流极简导航 - MinNav ]** MinNav: Minimalist Navigation Using Optical Flow For Active Tiny Aerial Robots [[arxiv]](https://arxiv.org/abs/2606.07813) [[hjfy]](https://hjfy.top/arxiv/2606.07813) [[project]](https://pear.wpi.edu/research/minnav.html) `Zero-Shot` `Optical Flow (2.8M)` `Blender+Real`
  - 概览：提出仅依赖单目光流及其不确定性的极简导航栈，配合仿蜜蜂对角线主动探索消除FOE死区，在零场景先验下统一实现静态避障、动态闪避与未知形状间隙穿越，算力仅为深度方法的1/118。

- **[2026.06][ arXiv 2026 - 世界模型环境随机性泛化研究 ]** Generalization of World Models under Environmental Variability for Vision-based Quadrotor Navigation [[arxiv]](https://arxiv.org/abs/2606.05015) [[hjfy]](https://hjfy.top/arxiv/2606.05015) [[github]](https://github.com/ntnu-arl/world-model-nav-generalization) `World Model` `DreamerV3` `Aerial Gym`
  - 概览：以视觉四旋翼导航为平台研究DreamerV3世界模型在四级环境随机性下的泛化性，发现自监督预训练的跨环境重构质量比仿真RL胜率更能预测真机部署效果，并实现2.5秒输入后纯想象飞行12米。

- **[2026.06][ arXiv 2026 - 全链路不确定性纯视觉导航 - UNSEEN ]** UNSEEN: Uncertainty-aware Navigation via Sparse Estimation in Unknown Environments [[arxiv]](https://arxiv.org/abs/2606.20755) [[hjfy]](https://hjfy.top/arxiv/2606.20755) `Hierarchical` `Uncertainty-aware V-SLAM`
  - 概览：提出仅用单目前视相机的全链路不确定性感知导航框架，将SLAM位姿与地标协方差贯通传递至概率占据建图、滚动时域规划与SE(3)轨迹优化，实机飞行零碰撞、任务成功率100%。

- **[2026.06][ arXiv 2026 - 四旋翼零样本Sim2Real控制世界模型 - SkyJEPA ]** SkyJEPA: Learning Long-Horizon World Models for Zero-Shot Sim-to-Real Control of Quadrotors [[arxiv]](https://arxiv.org/abs/2606.23444) [[hjfy]](https://hjfy.top/arxiv/2606.23444) `World Model` `JEPA (TCN+GRU)` `Sim2Real`
  - 概览：提出面向四旋翼实时控制的JEPA式潜空间动力学世界模型，配合物理启发的状态探测头与MPPI采样最优控制，仅用域随机化仿真数据训练即可实现长时域精确预测与零样本Sim2Real机载实时飞行控制。

- **[2026.06][ ICRA 2026 - 平面扇区制导升力翼四旋翼拦截 - PS-LOS ]** Planar-Sector LOS Guidance for Interception of Agile Targets with Lifting-Wing Quadcopters [[arxiv]](https://arxiv.org/abs/2606.10639) [[hjfy]](https://hjfy.top/arxiv/2606.10639) `Hierarchical` `PS-LOS Guidance` `Lifting-Wing Quadcopter`
  - 概览：提出平面扇区视线（PS-LOS）制导律，以收紧横向、放宽纵向的非对称视场约束在保持目标可见性的同时释放机动能力，配合升力翼四旋翼双层控制器与延迟补偿状态估计，户外实现138米超远距敏捷目标自主拦截。

- **[2026.06][ arXiv 2026 - 共享暴露信念的多无人机护航信息规划 ]** UGV-Conditioned Multi-UAV Informative Planning on a Shared Exposure Belief [[arxiv]](https://arxiv.org/abs/2606.12306) [[hjfy]](https://hjfy.top/arxiv/2606.12306) `Hierarchical` `Voronoi + IPP`
  - 概览：提出以共享暴露信念为核心的空地协同框架，把多无人机信息规划与无人车暴露感知重规划连成在线闭环，并用Voronoi区域分配消除感知冗余，累积暴露风险降低38%。

- **[2026.06][ IROS 2026 - 时序失配下鲁棒的连续时间无人机避障 - LNN-Fly ]** LNN-Fly: Continuous-Time UAV Navigation for Robust Obstacle Avoidance under Timing Mismatch [[arxiv]](https://arxiv.org/abs/2606.28827) [[hjfy]](https://hjfy.top/arxiv/2606.28827) `End-to-end` `Liquid NN (CfC)` `Gazebo+PX4`
  - 概览：提出将真实控制间隔Δt显式输入网络、并引入输入驱动自适应遗忘门的连续时间液态网络导航策略，经可微物理训练后零微调迁移真机，在控制周期抖动与稀疏观测下仍稳健避障。

- **[2026.06][ IEEE RA-L 2026 - 大模型赋能空地两栖机器人导航 - DS-LABRNav ]** DS-LABRNav: Land-Air Bimodal Robot Navigation with Traversable Obstacles Base On Vision-Language Model [[ieee]](https://ieeexplore.ieee.org/abstract/document/11539000) `GSM` `Align-DS-V (DeepSeek-R1)`
  - 概览：首个把视觉语言大模型引入空地两栖机器人路径规划的框架，通过OITT事件触发按需调用VLM区分门帘、缓坡等可穿越障碍与刚性障碍并据此更新栅格地图，室内外实测最高节省70%能耗。

- **[2026.06][ EAAI 2026 - 纯稀疏奖励空中对抗双层强化学习 - R2SP ]** Trajectory-level reward relabelling and progressive sub-task flight control for engineering-grade simulation of adversarial aerial engagements [[doi]](https://www.sciencedirect.com/science/article/pii/S0952197626015897) `Hierarchical` `Sparse-Reward RL` `6-DoF Sim`
  - 概览：提出双层强化学习框架R2SP，仅用纯物理事件稀疏奖励，以轨迹级奖励重标记无偏解决时间信用分配、渐进式子任务飞控化解6自由度耦合，工程级仿真中总胜率73.5%并击败人类操作员。

- **[2026.06][ CVPR 2026 - 无建图统一主动搜索与跟踪 - UAST ]** UAST: Unified Active Search and Tracking for Arbitrary Targets with UAVs [[cvf]](https://openaccess.thecvf.com/content/CVPR2026/papers/Qin_UAST_Unified_Active_Search_and_Tracking_for_Arbitrary_Targets_with_CVPR_2026_paper.pdf) [[github]](https://github.com/qinliangql/UAST) `End-to-end`
  - 概览：提出仅用RGB-D、无需显式建图的端到端主动搜索与跟踪统一框架，通过双分支感知、规则化引导点策略与跟踪感知可见性损失实现搜索-跟踪-重捕获无缝切换，并完成真机验证。

- **[2026.05][ arXiv 2026 - 生成模型驱动BEV可通行掩码的无GPS长距导航 - PathPainter ]** PathPainter: Transferring the Generalization Ability of Image Generation Models to Embodied Navigation [[arxiv]](https://arxiv.org/abs/2605.07496) [[hjfy]](https://hjfy.top/arxiv/2605.07496) [[github]](https://github.com/E-hash-42/PathPainter) `Zero-Shot` `Gemini`
  - 概览：把图像生成大模型的泛化能力迁移到BEV具身导航，由语言指令推理目标并生成可通行掩码后执行带边界惩罚的A*搜索，配合BEV-Patch-PF跨视角定位修正里程计漂移，实现无GPS的160米室外长距无人机自主飞行。

- **[2026.05][ arXiv 2026 - 碰撞感知与记忆增强的多尺度避障 - CaMeRL ]** CaMeRL: Collision-Aware and Memory-Enhanced Reinforcement Learning for UAV Navigation in Multi-Scale Obstacle Environments [[arxiv]](https://arxiv.org/abs/2605.14810) [[hjfy]](https://hjfy.top/arxiv/2605.14810) [[project]](https://honghongdev.github.io/camerl/) `RL` `VAE+LSTM` `Flightmare`
  - 概览：用碰撞感知深度隐表征保留超小障碍细粒度结构、用LSTM时序记忆补全超大障碍遮挡信息，在七档尺度仿真场景与室外真机飞行中全面超越现有强化学习避障方案。

- **[2026.05][ RSS 2026 - 潜扩散驱动的人群中微型飞行器导航 - HumanFlow ]** HumanFlow -- Diffusion-Driven MAV Navigation Among Humans via Tightly-Coupled Motion Tracking, Forecasting, and Control [[arxiv]](https://arxiv.org/abs/2605.25685) [[hjfy]](https://hjfy.top/arxiv/2605.25685) `Diffusion` `Latent Diffusion + Flow Matching`
  - 概览：提出以3D场景为条件的潜扩散模型HumanFlow，统一人体运动跟踪与未来轨迹预测，并将冻结潜表征与流匹配MPC控制策略紧耦合，使微型飞行器在强遮挡人群中实现100%无碰撞的社交导航。

- **[2026.05][ RA-L 2026 - 强化学习赋能的无人机户外立体视觉避障 ]** Vision-Guided Outdoor Flight and Obstacle Evasion via Reinforcement Learning [[arxiv]](https://arxiv.org/abs/2605.24449) [[hjfy]](https://hjfy.top/arxiv/2605.24449) [[doi]](https://ieeexplore.ieee.org/document/11282444) `RL` `Autoencoder+LSTM` `Flightmare`
  - 概览：提出融合立体深度与视觉惯性里程计、直接输出速度指令的感觉运动策略，以特权学习加课程学习两阶段训练配合域随机化与奖励重塑，零样本迁移到重量8倍于仿真机的DJI M300商用无人机完成户外避障飞行。

- **[2026.03][ CVPR 2026 - 非对齐空天视角纯视觉无人机导航 - Bearing-UAV ]** Beyond Matching to Tiles: Bridging Unaligned Aerial and Satellite Views for Vision-Only UAV Navigation [[arxiv]](https://arxiv.org/abs/2603.22153) [[hjfy]](https://hjfy.top/arxiv/2603.22153) [[github]](https://github.com/liukejia121/bearinguav) `End-to-end` `VGG-16`
  - 概览：突破跨视角地理定位的瓦片匹配范式，提出单阶段联合回归无人机绝对位置与航向的轻量模型，并构建考虑任意旋转与非对齐的多城市数据集Bearing-UAV-90K，支撑GNSS拒止下的纯视觉点对点导航。

- **[2026.03][ arXiv 2026 - 意图-上下文协同的无人机空战决策 - ICS-RL ]** Intent-Context Synergy Reinforcement Learning for Autonomous UAV Decision-Making in Air Combat [[arxiv]](https://arxiv.org/abs/2603.00974) [[hjfy]](https://hjfy.top/arxiv/2603.00974) `RL` `LSTM+Dueling DQN`
  - 概览：提出意图-上下文协同强化学习框架，用LSTM预测敌机未来轨迹做状态增强，并按最大优势值动态切换安全巡航、隐身规划、突破突防三类Dueling DQN专家，渗透任务成功率达88%。

- **[2026.03][ arXiv 2026 - 连通性感知的多无人机协同探索 - C²-Explorer ]** C²-Explorer: Contiguity-Driven Task Allocation with Connectivity-Aware Task Representation for Decentralized Multi-UAV Exploration [[arxiv]](https://arxiv.org/abs/2603.07699) [[hjfy]](https://hjfy.top/arxiv/2603.07699) [[github]](https://github.com/Robotics-STAR-Lab/C2-Explorer) `Hierarchical` `Connectivity Graph`
  - 概览：面向通信受限的去中心化多无人机探索，构建连通图把空间不连通的未知区域拆分为独立任务单元，并以图邻接惩罚约束任务分配的时空连续性，探索时间减少43.1%。

- **[2026.03][ arXiv 2026 - 恶劣视觉环境毫瓦级超声无人机导航 - Saranga ]** Saranga: MilliWatt Ultrasound for Navigation in Visually Degraded Environments on Palm-Sized Aerial Robots [[arxiv]](https://arxiv.org/abs/2603.24699) [[hjfy]](https://hjfy.top/arxiv/2603.24699) `Ultrasound`
  - 概览：提出Saranga毫瓦级双声纳感知栈，结合物理降噪与学习式回波去噪，使掌上无人机仅凭机载感知和计算在浓雾、黑暗及积雪环境中避障导航。

- **[2026.02][ arXiv 2026 - 解耦语义与几何的零样本空中导航 - Fly0 ]** Fly0: Persistent Metric Anchoring for Zero-Shot Aerial Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2602.15875) [[hjfy]](https://hjfy.top/arxiv/2602.15875) [[github]](https://github.com/xuzhenxing1/Fly0) `GSM` `MLLM + Ego-Planner`
  - 概览：提出将语义推理与几何规划解耦的零样本空中导航框架Fly0，MLLM仅负责将指令定位到2D像素坐标，再通过深度投影获取3D目标并由Ego-Planner生成无碰撞轨迹，SR提升超20%。

- **[2026.02][ arXiv 2026 - 轻量级UAV零样本目标导航 - USS-Nav ]** USS-Nav: Unified Spatio-Semantic Scene Graph for Lightweight UAV Zero-Shot Object Navigation [[arxiv]](https://arxiv.org/abs/2602.00708) [[hjfy]](https://hjfy.top/arxiv/2602.00708) [[github]](https://github.com/ZJU-FAST-Lab) `Zero-Shot` `LLM (Scene Graph)`
  - 概览：构建了轻量级的统一时空语义场景图，结合大语言模型（LLM）的推理能力，实现了轻型无人机在未知环境中的实时（15Hz）零样本开放词汇目标导航。

- **[2026.02][ CVPR 2026 - 解耦记忆异步空中目标导航 - APEX ]** APEX: A Decoupled Memory-based Explorer for Asynchronous Aerial Object Goal Navigation [[arxiv]](https://arxiv.org/abs/2602.00551) [[hjfy]](https://hjfy.top/arxiv/2602.00551) [[github]](https://github.com/4amGodvzx/apex) `GSM+RL` `Spatio-Semantic Map`
  - 概览：提出分层异步并行框架APEX，通过动态时空语义建图记忆、强化学习动作决策和开放词汇目标定位三个模块并行运行，有效绕过VLM推理延迟，在UAV-ON基准上显著超越现有方法。

- **[2026.02][ arXiv 2026 - 可重光照3DGS零样本森林高速飞行 ]** Zero-Shot UAV Navigation in Forests via Relightable 3D Gaussian Splatting [[arxiv]](https://arxiv.org/abs/2602.07101) [[hjfy]](https://hjfy.top/arxiv/2602.07101) `RL` `CNN+GRU` `3DGS`
  - 概览：提出可重光照3D高斯泼溅表征，将场景几何、材质反照率与环境光照物理解耦，通过光照随机化训练端到端强化学习策略，使轻量四旋翼仅凭单目RGB在真实森林零样本实现10m/s高速无碰撞飞行。

- **[2026.01][ arXiv 2026 - 室内空中双策略目标导航 - AION ]** AION: Aerial Indoor Object-Goal Navigation Using Dual-Policy Reinforcement Learning [[arxiv]](https://arxiv.org/abs/2601.15614) [[hjfy]](https://hjfy.top/arxiv/2601.15614) `RL` `Dual-Policy`
  - 概览：提出端到端双策略强化学习框架AION，将探索行为和目标趋近行为解耦为两个专用策略，无需外部定位或全局地图即可实现室内空中目标导航。

- **[2026.01][ arXiv 2026 - VLM语义与连续规划结合的导航 - AirHunt ]** AirHunt: Bridging VLM Semantics and Continuous Planning for Efficient Aerial Object Navigation [[arxiv]](https://arxiv.org/abs/2601.12742) [[hjfy]](https://hjfy.top/arxiv/2601.12742) `GSM` `VLM (3D Value Map)`
  - 概览：采用双路径异步架构，桥接了低频的VLM语义推理与高频的连续飞行规划，实现了高效且安全的空中目标导航。

- **[2026.01][ arXiv 2026 - 大模型赋能无人机开放世界扫描 - FlyCo ]** FlyCo: Foundation Model-Empowered Drones for Autonomous 3D Structure Scanning in Open-World Environments [[arxiv]](https://arxiv.org/abs/2601.07558) [[hjfy]](https://hjfy.top/arxiv/2601.07558) [[github]](https://github.com/FC-Family/FlyCo) `VLM-driven` `VLM`
  - 概览：结合视觉语言大模型（VLM）赋能无人机，仅需简单的人类提示即可在开放世界中自主跟踪、预测并扫描复杂的 3D 目标结构。

- **[2026.01][ IEEE RA-L 2026 - 惯性感知空中操作 - FlyAware ]** FlyAware: Inertia-Aware Aerial Manipulation via Vision-Based Estimation and Post-Grasp Adaptation [[arxiv]](https://arxiv.org/abs/2601.22686) [[hjfy]](https://hjfy.top/arxiv/2601.22686) [[project]](https://flyaware.github.io/) `End-to-end`
  - 概览：提出一种面向空中操作的惯性感知框架，集成基于视觉的抓前惯性估计模块与抓后自适应机制，实现对未知负载的实时惯性动力学估计与自适应控制，真实世界实验验证了其有效性。

- **[2026.01][ arXiv 2026 - 复杂环境微型飞行器在线时间最优飞行 - LOONG ]** LOONG: Online Time-Optimal Autonomous Flight for MAVs in Cluttered Environments [[arxiv]](https://arxiv.org/abs/2601.07434) [[hjfy]](https://hjfy.top/arxiv/2601.07434) `Hierarchical` `IL+MPCC`
  - 概览：提出规划与控制一体化的在线时间最优飞行框架，以模仿学习加速多项式轨迹的时间分配，并把安全飞行走廊约束嵌入变步长时间最优MPCC，实机在复杂环境中达到18m/s峰值速度。

- **[2026.01][ RA-L 2026 - 绝对黑暗中的无人机单目结构光自主导航 - AsterNav ]** AsterNav: Autonomous Aerial Robot Navigation In Darkness Using Passive Computation [[arxiv]](https://arxiv.org/abs/2601.17550) [[hjfy]](https://hjfy.top/arxiv/2601.17550) [[doi]](https://ieeexplore.ieee.org/document/11346995) `Zero-Shot` `U-Net/DenseNet121`
  - 概览：将编码孔径大光圈镜头的被动计算与低功耗结构光相结合，纯仿真训练的AsterNet单目深度网络零样本迁移真机，在照度低于1毫勒克斯的绝对黑暗中实现20Hz机载实时避障飞行，成功率达95.5%。

### 2025
- **[2025.12][ IEEE RA-L 2026 - 单目RGB杂乱环境飞行与3D辐射场 ]** Flying in Clutter on Monocular RGB by Learning in 3D Radiance Fields with Domain Adaptation [[arxiv]](https://arxiv.org/abs/2512.17349) [[hjfy]](https://hjfy.top/arxiv/2512.17349) `RL` `Domain Adaptation` `3DGS`
  - 概览：利用3D高斯喷溅（3DGS）渲染生成高保真仿真环境，结合对抗性域自适应（Domain Adaptation），实现了仅依赖单目RGB相机的强化学习策略在真实复杂杂乱环境中的零样本泛化飞行。

- **[2025.11][ IEEE RA-L 2026 - 单目SLAM大规模无人机自主探索 - MonoSpheres ]** MonoSpheres: Large-Scale Monocular SLAM-Based UAV Exploration through Perception-Coupled Mapping and Planning [[arxiv]](https://arxiv.org/abs/2511.17299) [[hjfy]](https://hjfy.top/arxiv/2511.17299) [[github]](https://github.com/ctu-mrs/monospheres) `Autonomous Exploration` `OpenVINS` `Gazebo`
  - 概览：针对单目SLAM深度稀疏且不可靠的问题，提出以相交球体表示自由空间、显式跟踪障碍位置不确定性的建图方法与感知耦合的快速重规划策略，首次实现真实户外大规模三维单目自主探索。

- **[2025.11][ IEEE RA-L 2026 - 仿蚂蚁窄视场微型无人机视觉示教-重复 - Antflie ]** Antflie: Frugal Visual Teach and Repeat on Narrow FoV Micro-Drones [[ieee]](https://ieeexplore.ieee.org/document/11408827) [[hal]](https://hal.science/hal-05347280) `End-to-end` `Mushroom Body Net` `Gazebo`
  - 概览：受沙漠蚂蚁启发提出路线侧化(R-Lat)视觉示教-重复框架，在33克微型无人机上仅用24×24像素窄视场图像与不到4KB的蘑菇体视觉记忆，实现无地图、无SLAM、无里程计的纯视觉自主返航与精准降落。

- **[2025.10][ arXiv 2025 - 基于世界模型RL的端到端视觉无人机竞速 - SkyDreamer ]** SkyDreamer: Interpretable End-to-End Vision-Based Drone Racing with Model-Based Reinforcement Learning [[arxiv]](https://arxiv.org/abs/2510.14783) [[hjfy]](https://hjfy.top/arxiv/2510.14783) `World Model` `Informed Dreamer` `Sim-to-Real`
  - 概览：基于informed Dreamer世界模型提出首个由像素级分割掩码直接映射到电机指令的端到端视觉自主竞速策略，世界模型兼作隐式状态与参数估计器，全机载真机飞行达21m/s与6g加速度。

- **[2025.09][ ICRA 2026 - 零样本远距离户外导航 - EzReal ]** EZREAL: Enhancing Zero-Shot Outdoor Robot Navigation toward Distant Targets under Varying Visibility [[arxiv]](https://arxiv.org/abs/2509.13720) [[hjfy]](https://hjfy.top/arxiv/2509.13720) `Zero-Shot`
  - 概览：针对大规模户外环境中远距离目标的零样本导航，提出利用目标轮廓记忆和方向推理的方法，在目标间歇性可见的条件下实现鲁棒导航。

- **[2025.09][ arXiv 2025 - 开放集语义记忆与行为自适应空中导航 - RAVEN ]** RAVEN: Resilient Aerial Navigation via Open-Set Semantic Memory and Behavior Adaptation [[arxiv]](https://arxiv.org/abs/2509.23563) [[hjfy]](https://hjfy.top/arxiv/2509.23563) [[github]](https://github.com/castacks/RAVEN) [[project]](https://raven-semantic.github.io/) `GSM` `RayFronts+SigLIP+InternVL3-2B` `Isaac Sim`
  - 概览：提出以开放集语义体素-射线地图为内部记忆、用行为树在边界探索与语义体素/射线搜索间自适应切换的空中语义导航框架，在10个户外仿真环境与真机上实现稀疏语义线索下的长距离目标搜索。

- **[2025.08][ arXiv 2025 - 模仿学习的果园无人机视觉导航 ]** Vision-based Navigation of Unmanned Aerial Vehicles in Orchards: An Imitation Learning Approach [[arxiv]](https://arxiv.org/abs/2508.02617) [[hjfy]](https://hjfy.top/arxiv/2508.02617) `End-to-end` `VAE`
  - 概览：提出基于变分自编码器的端到端视觉运动控制器，通过人类干预式模仿学习仅需数轮迭代即可让无人机在GPS失效的果园行间自主避障飞行，并在真实果园验证跨树种与速度的泛化能力。

- **[2025.06][ IEEE RA-L 2025 - VLM+3DGS机载无人机导航 - GRaD-Nav++ ]** GRaD-Nav++: Vision-Language Model Enabled Visual Drone Navigation with Gaussian Radiance Fields and Differentiable Dynamics [[arxiv]](https://arxiv.org/abs/2506.14009) [[hjfy]](https://hjfy.top/arxiv/2506.14009) `RL` `VLM+3DGS (MoE)`
  - 概览：提出轻量级全机载VLA框架GRaD-Nav++，在3DGS仿真器中通过可微强化学习训练，结合混合专家（MoE）动作头实现多任务泛化，真实硬件上达到67%成功率。

- **[2025.06][ IEEE RA-L 2025 - 跨模态无人机视觉运动策略 ]** Learning Cross-Modal Visuomotor Policies for Autonomous Drone Navigation [[doi]](https://doi.org/10.1109/LRA.2025.3559824) [[github]](https://github.com/zzzzzyh111/CL4Nav) `RL` `Cross-Modal Contrastive Learning`
  - 概览：提出跨模态视觉运动策略学习方法，利用对比强化学习将不同传感器模态（RGB、深度、事件相机）的表征对齐，使无人机在单一模态缺失时仍能鲁棒自主导航。

- **[2025.06][ arXiv 2025 - 开放词汇目标理解无人机VLN - VLFly ]** Grounded Vision-Language Navigation for UAVs with Open-Vocabulary Goal Understanding [[arxiv]](https://arxiv.org/abs/2506.10756) [[hjfy]](https://hjfy.top/arxiv/2506.10756) [[github]](https://github.com/zzzzzyh111/Vision-Language-Fly) [[project]](https://zzzzzyh111.github.io/VLFly/) `Zero-Shot` `LLaMA+CLIP` `Unity`
  - 概览：提出面向无人机的模块化VLN框架VLFly，级联LLaMA指令编码、CLIP目标图像检索与航点规划三个模块，仅凭机载单目RGB将自然语言指令转化为连续控制命令，实现无需任务微调的零样本室内外导航。

- **[2025.05][ AAAI 2026 - 城市空间UAV视觉目标搜索 ]** Towards Autonomous UAV Visual Object Search in City Space: Benchmark and Agentic Methodology [[arxiv]](https://arxiv.org/abs/2505.08765) [[hjfy]](https://hjfy.top/arxiv/2505.08765) `Agentic` `VLM+LLM`
  - 概览：提出首个城市空间无人机视觉目标搜索基准CityAVOS及智能体方法PRPSearcher，通过感知-推理-规划三层认知架构和3D语义吸引力地图，在复杂城市环境中实现高效自主搜索，SR提升37.69%。

- **[2025.05][ IEEE RA-L 2025 - Sim-to-Real深度迁移无人机导航 ]** Depth Transfer: Learning to See Like a Simulator for Real-World Drone Navigation [[arxiv]](https://arxiv.org/abs/2505.12428) [[hjfy]](https://hjfy.top/arxiv/2505.12428) `RL` `VAE` `Sim-to-Real`
  - 概览：提出基于域自适应的深度迁移方法，通过VAE将仿真深度图编码为潜在空间供RL策略使用，部署时对齐真实立体深度输入，无需微调即可实现Sim-to-Real无人机避障导航。

- **[2025.05][ arXiv 2025 - 低空城市多无人机任务分配协调场 - CoordField ]** CoordField: Coordination Field for Agentic UAV Task Allocation In Low-altitude Urban Scenarios [[arxiv]](https://arxiv.org/abs/2505.00091) [[hjfy]](https://hjfy.top/arxiv/2505.00091) `Agentic` `DeepSeek`
  - 概览：提出基于协调场的异构无人机集群任务分配智能体系统，用大模型解析自然语言指令，并以动态演化的势场、流场与局部涡旋机制实现低空城市场景下去中心化的实时任务分配与协同。

- **[2025.05][ IEEE RA-L 2025 - 主动触碰透明玻璃的无人机自主导航 ]** Active Contact Engagement for Aerial Navigation in Unknown Environments with Glass [[arxiv]](https://arxiv.org/abs/2505.00332) [[hjfy]](https://hjfy.top/arxiv/2505.00332) [[doi]](https://doi.org/10.1109/LRA.2025.3569120) `Active Perception` `Visual-Contact Fusion`
  - 概览：融合视觉候选玻璃检测与轻量接触传感器，让无人机主动触碰验证透明障碍、增量更新体素地图并在线重规划安全轨迹，从而在未知真实环境中实现可靠的玻璃感知与自主绕障。

- **[2025.04][ IEEE RA-L 2025 - 零样本目标导航自适应探索 - ApexNav ]** ApexNav: An Adaptive Exploration Strategy for Zero-Shot Object Navigation with Target-centric Semantic Fusion [[arxiv]](https://arxiv.org/abs/2504.14478) [[hjfy]](https://hjfy.top/arxiv/2504.14478) [[github]](https://github.com/Robotics-STAR-Lab/ApexNav) `Zero-Shot` `VLM`
  - 概览：针对零样本目标导航，提出了在语义推理和几何探索之间动态切换的自适应策略，并结合以目标为中心的语义融合来过滤错误检测。

- **[2025.04][ arXiv 2025 - 数字孪生物体级建图的空地机器人导航 - MorphoNavi ]** MorphoNavi: Aerial-Ground Robot Navigation with Object Oriented Mapping in Digital Twin [[arxiv]](https://arxiv.org/abs/2504.16914) [[hjfy]](https://hjfy.top/arxiv/2504.16914) `Zero-Shot` `OWLv2+Depth Anything` `Unity`
  - 概览：提出仅依赖单目相机的物体级语义建图方法，用开放词汇检测与单目深度估计把物体语义与位置映射进Unity数字孪生，无需环境微调即可支撑空地变形机器人MorphoGear完成搜救定位任务。

- **[2025.04][ SSRN 2025 - 单目视觉+VLM驱动的无地图无人机导航 - VLM-Nav ]** VLM-Nav: Mapless UAV-Navigation Using Monocular Vision Driven by Vision-Language Model [[ssrn]](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5231854) [[github]](https://github.com/gcsarker/vlm_nav) [[project]](https://gcsarker.github.io/vlmnav/) `Zero-Shot` `GPT-4o/Gemini-1.5-Flash` `AirSim+UE4`
  - 概览：仅用单目RGB图像经深度估计模型生成深度图，再由视觉语言模型给出避障方向并结合近物检测与轻量导航网络输出离散动作，实现无需地图和人工指令的无人机自主飞行。

- **[2025.03][ ICRA 2025 - 微型无人机免地图单目视觉导航 ]** A Map-free Deep Learning-based Framework for Gate-to-Gate Monocular Visual Navigation aboard Miniaturized Aerial Vehicles [[arxiv]](https://arxiv.org/abs/2503.05251) [[hjfy]](https://hjfy.top/arxiv/2503.05251) `End-to-end`
  - 概览：提出面向掌上级微型无人机（<50g）的免地图视觉导航框架，结合轻量级深度学习门检测前端与经典视觉伺服控制后端，仅用单目相机在极受限机载算力上实现30Hz闭环穿门飞行。

- **[2025.03][ arXiv 2025 - 无人机搜救快速响应 - UAV-VLRR ]** UAV-VLRR: Vision-Language Informed NMPC for Rapid Response in UAV Search and Rescue [[arxiv]](https://arxiv.org/abs/2503.02465) [[hjfy]](https://hjfy.top/arxiv/2503.02465) `NMPC` `VLM+Control`
  - 概览：为无人机搜救提出视觉-语言-快速响应（VLRR）框架，将多模态大模型（解析场景与目标坐标）与非线性模型预测控制（NMPC）结合，在保证避障的同时大幅缩短急救场景的响应与飞行时间。

- **[2025.03][ arXiv 2025 - 大模型驱动的通用空中智能体 ]** General-Purpose Aerial Intelligent Agents Empowered by Large Language Models [[arxiv]](https://arxiv.org/abs/2503.08302) [[hjfy]](https://hjfy.top/arxiv/2503.08302) `Hierarchical` `DeepSeek-R1-14B`
  - 概览：提出软硬件协同设计的通用空中智能体，在220W机载边缘平台上以5-6 tokens/s运行14B大模型，并用双向认知架构将LLM慢速任务规划与状态估计、建图、避障等快速反应控制耦合。

- **[2025.02][ RSS 2025 - 逆强化学习的敏捷视觉飞行规划器 - RAPID ]** RAPID: Robust and Agile Planner Using Inverse Reinforcement Learning for Vision-Based Drone Navigation [[arxiv]](https://arxiv.org/abs/2502.02054) [[hjfy]](https://hjfy.top/arxiv/2502.02054) `RL` `Inverse Soft-Q+AE` `AirSim`
  - 概览：提出基于逆软Q学习的敏捷视觉规划器，免去人工奖励设计并用辅助自编码器压缩高维深度输入，毫秒级生成无碰撞航点，纯仿真训练策略零微调迁移到真实森林与城市环境实现平均7m/s高速飞行。

- **[2025.02][ RA-L 2025 - 柔顺机器人手指驱动的空中触觉导航 ]** Embodying Compliant Touch on Drones for Aerial Tactile Navigation [[ieee]](https://ieeexplore.ieee.org/document/10806756) [[github]](https://github.com/BioMorphic-Intelligence-Lab/tactile-drone) `Hierarchical`
  - 概览：为四旋翼装配腱驱动的柔顺机器人手指，直接由关节形变推断三维接触力的大小与方向，无需环境先验即可生成沿表面法向对齐的接触式航点，36次真实飞行实现厘米级未知墙面跟随。

- **[2025.01][ IEEE IoT-J 2025 - 语义地图与认知逃逸强化学习的大规模户外视觉导航 - SM-CERL ]** UAV Visual Navigation in the Large-Scale Outdoor Environment: A Semantic Map-Based Cognitive Escape Reinforcement Learning Method [[ieee]](https://ieeexplore.ieee.org/document/10847926) `RL` `ResNet-18+D3QN`
  - 概览：针对大规模户外视觉导航的部分可观测与局部最优难题，用孪生网络构建探索图与相似度图双通道语义地图充当记忆，并设计认知逃逸模块主动识别局部最优并依规则知识跳出。

### 2024

- **[2024.12][ arXiv 2024 - 零样本Sim-to-Real飞行策略 - SOUS VIDE ]** SOUS VIDE: Cooking Visual Drone Navigation Policies in a Gaussian Splatting Vacuum [[arxiv]](https://arxiv.org/abs/2412.16346) [[hjfy]](https://hjfy.top/arxiv/2412.16346) [[github]](https://github.com/stanfordmsl/SousVide) `RL` `3DGS`
  - 概览：提出在高保真3D高斯喷溅（3DGS）轻量级仿真器中端到端训练纯视觉导航策略，实现了向真实物理世界复杂环境的零样本平滑迁移与鲁棒飞行。

- **[2024.11][ CJA 2026 - 噪声驱动探索增强的无人机深度强化学习导航 - NDE-PMTD3 ]** Noise-driven enhancement for exploration: Deep reinforcement learning for UAV autonomous navigation in complex environments [[doi]](https://doi.org/10.1016/j.cja.2025.103769) `RL` `TD3+LSTM`
  - 概览：在TD3基础上引入LSTM时序建模与优先经验回放，并设计全局/局部双模型噪声控制和噪声-确定性双经验回放缓冲区，加速训练收敛并提升复杂动态环境中无人机自主导航的泛化能力。

- **[2024.09][ IROS 2024 - 异构无人机协同探索建图 - SOAR ]** SOAR: Simultaneous Exploration and Photographing with Heterogeneous UAVs for Fast Autonomous Reconstruction [[arxiv]](https://arxiv.org/abs/2409.02738) [[hjfy]](https://hjfy.top/arxiv/2409.02738) [[github]](https://github.com/Robotics-STAR-Lab/SOAR) `Autonomous Exploration`
  - 概览：设计了异构无人机协同系统，探索机负责快速未知空间建图，摄影机负责高分辨率图像采集，实现了针对未知环境的快速自主 3D 重建。

- **[2024.09][ RA-L 2025 - 动态环境安全飞行的强化学习导航 - NavRL ]** NavRL: Learning Safe Flight in Dynamic Environments [[arxiv]](https://arxiv.org/abs/2409.15634) [[hjfy]](https://hjfy.top/arxiv/2409.15634) [[github]](https://github.com/Zhefan-Xu/NavRL) [[ieee]](https://ieeexplore.ieee.org/document/10904341) `RL` `PPO` `Isaac Sim`
  - 概览：基于PPO设计静态与动态障碍统一的状态动作表示，在Isaac Sim中用大规模并行与课程学习训练策略，并叠加速度障碍安全防护盾，实现零样本sim-to-real的动态环境安全飞行。

- **[2024.09][ RA-L 2025 - 场景感知控制障碍函数的无人机VLN安全裕度 - ASMA ]** ASMA: An Adaptive Safety Margin Algorithm for Vision-Language Drone Navigation via Scene-Aware Control Barrier Functions [[arxiv]](https://arxiv.org/abs/2409.10283) [[hjfy]](https://hjfy.top/arxiv/2409.10283) [[github]](https://github.com/souravsanyal06/ASMA) [[ieee]](https://ieeexplore.ieee.org/abstract/document/11091440/) `Hierarchical` `CLIP+YOLOv5` `Gazebo`
  - 概览：为视觉语言导航无人机提出基于RGB-D观测的场景感知控制障碍函数与自适应安全裕度算法，并嵌入MPC实时求解，在轨迹仅增长1.4%-5.8%的前提下将导航成功率提升64%-67%。

- **[2024.07][ IEEE T-RO 2024 - 快速自主空中探索导航 - Falcon ]** FALCON: Fast Autonomous Aerial Exploration using Coverage Path Guidance [[arxiv]](https://arxiv.org/abs/2407.00577) [[hjfy]](https://hjfy.top/arxiv/2407.00577) [[github]](https://github.com/HKUST-Aerial-Robotics/FALCON) `Coverage Path Guidance`
  - 概览：提出了基于覆盖路径引导的快速自主空中探索框架，通过连通性空间分解和分层规划，有效减少了重复探索，提升了完全未知环境中的探索效率。

- **[2024.01][ Remote Sensing 2024 - GNSS拒止与视觉退化环境下的无人机自主导航与目标检测 ]** Framework for Autonomous UAV Navigation and Target Detection in Global-Navigation-Satellite-System-Denied and Visually Degraded Environments [[mdpi]](https://www.mdpi.com/2072-4292/16/3/471) `RL` `YOLOv5` `Gazebo+PX4`
  - 概览：将GNSS拒止与低能见度下的无人机搜救建模为POMDP并用ABT算法在线求解，融合热成像相机与YOLOv5检测，在Gazebo仿真与真实飞行中实现无碰撞自主探索与目标发现。

## 📊 Benchmarks, Datasets & Simulation

### 2026

- **[2026.07][ arXiv 2026 - 扩散精炼的无人机最后十米视觉伺服 - DreamNav ]** Last-Meter Precision Navigation for UAVs: A Diffusion-Refined Aerial Visual Servoing Approach [[arxiv]](https://arxiv.org/abs/2607.04352) [[hjfy]](https://hjfy.top/arxiv/2607.04352) [[github]](https://github.com/YaxuanLi-cn/PairUAV) `Diffusion` `World Model` `PairUAV`
  - 概览：提出粗到精的扩散精炼空中视觉伺服框架，先用三角参数化回归稳定旋转估计，再借预训练世界模型想象候选动作的未来视觉以筛选轨迹，并发布481万图像对的PairUAV基准。

- **[2026.07][ arXiv 2026 - 野外无人机主动目标检测数据集与世界模型方法 - ATRNet-LUDO ]** Toward Active Object Detection for UAVs in the Wild: A Large-Scale Dataset, Benchmark and Method [[arxiv]](https://arxiv.org/abs/2607.09078) [[hjfy]](https://hjfy.top/arxiv/2607.09078) [[github]](https://github.com/Leo000ooo/ATRNet-LUDO) `World Model` `JEPA+Dueling DQN`
  - 概览：发布首个野外无人机-地面主动目标检测实景数据集ATRNet-LUDO与统一评测基准，含12.1万全景航拍图和121万目标切片，并提出结合JEPA世界模型与场景净化的AOD-JEPA策略提升跨场景泛化。

- **[2026.07][ arXiv 2026 - 无人机双认知时空推理基准 - UAV-DualCog ]** Knowing the Self, Understanding the World: A Dual-Cognition Benchmark for UAV Spatio-temporal Reasoning with MLLMs [[arxiv]](https://arxiv.org/abs/2607.16193) [[hjfy]](https://hjfy.top/arxiv/2607.16193) [[github]](https://github.com/SmartDianLab/UAV-DualCog) [[project]](https://uav-dualcog.lozumi.com) `Benchmark` `MLLM` `AerialVLN`
  - 概览：提出首个同时考核无人机自状态认知与环境认知的时空推理基准，基于语义点云仿真流水线自动生成图像与视频双模态样本并强制输出时空定位证据，揭示主流多模态大模型的视角转换与时序定位瓶颈。

- **[2026.07][ arXiv 2026 - 纯视觉长时程无人机导航范式与基准 - VoLN ]** VoLN: Vision-Only Long-Horizon Navigation---Paradigm, Benchmark, and Method [[arxiv]](https://arxiv.org/abs/2607.21400) [[hjfy]](https://hjfy.top/arxiv/2607.21400) [[github]](https://github.com/Admire-ljb/VoLN-UAV) [[project]](https://admire-ljb.github.io/VoLN-UAV/) `Benchmark` `Vicuna-7B` `AirSim+UE4`
  - 概览：提出彻底移除GPS、全局地图与文字指令、仅凭终点参考图与机载视觉完成长时程飞行的VoLN范式，构建17场景7210条轨迹的VoLN-UAV仿真基准，并给出DINO-CLIP语义对齐加LoRA微调大模型预测3D航点的VoLN-MLLM基线。

- **[2026.07][ ACM MM 2026 - 无人机自我认知与空间认知评测基准 - SIS-Bench ]** Self in Space: Benchmarking Self-Awareness and Spatial Cognition in UAV Embodied Intelligence [[arxiv]](https://arxiv.org/abs/2607.12477) [[hjfy]](https://hjfy.top/arxiv/2607.12477) [[github]](https://github.com/IntelliSensing/Self-in-Space) [[project]](https://choucisan.github.io/publications/self-in-space) `Benchmark` `Qwen2.5-VL`
  - 概览：提出从空间认知与自我认知双维度、按感知/记忆/推理三层组织13项任务的SIS-Bench基准（1646段真实无人机视频、4856道问答），揭示主流多模态大模型自我运动理解的明显短板，并用光流双分支的SIS-Motion验证显式运动建模的增益。

- **[2026.06][ arXiv 2026 - 细粒度长时序无人机导航基准与异步VLA - FLIGHT ]** Think Like a Pilot: Fine-Grained Long-Horizon UAV Navigation [[arxiv]](https://arxiv.org/abs/2606.06836) [[hjfy]](https://hjfy.top/arxiv/2606.06836) [[github]](https://github.com/buaa-colalab/FLIGHT) [[project]](https://buaa-colalab.github.io/FLIGHT/) `Benchmark` `Hierarchical` `VLM+DiT` `UnrealZoo`
  - 概览：构建首个兼顾多阶段长时序指令与稠密6自由度连续轨迹标注的无人机导航基准FLIGHT，并提出低频流式飞行员推理VLM与高频扩散动作模型异步解耦的FLIGHT VLA架构。

- **[2026.06][ arXiv 2026 - 视野内精准抵达空中VLN - 3DG-VLN ]** See-and-Reach: Precise Vision-Language Navigation for UAVs within the Field of View [[arxiv]](https://arxiv.org/abs/2606.20045) [[hjfy]](https://hjfy.top/arxiv/2606.20045) [[github]](https://github.com/xuefanfu/3DG-VLN) `End-to-end` `Qwen2.5-VL-7B` `AirSim+UE4`
  - 概览：首次将“看见-抵达”阶段从整体导航中剥离，提出UAV-VLN-FOV任务与2717条轨迹高分辨率基准，并设计3D方向引导框架3DG-VLN，以双视角观测与在线方向更新将成功率提升13.82%。

- **[2026.06][ arXiv 2026 - 低空无人机空间智能评测基准 - SpatialUAV ]** SpatialUAV: Benchmarking Spatial Intelligence for Low-Altitude UAV Perception, Collaboration, and Motion [[arxiv]](https://arxiv.org/abs/2606.27876) [[hjfy]](https://hjfy.top/arxiv/2606.27876) [[github]](https://github.com/Hyu-Zhang/SpatialUAV) `Benchmark`
  - 概览：构建真实低空无人机空间智能基准SpatialUAV，含4331条样本与14类精细任务，覆盖语义判别、空间关系、空空与空地协作及运动理解，横评18个视觉语言模型揭示跨视角关联与几何推理短板。

- **[2026.06][ arXiv 2026 - RGB+辐射热成像野火VQA基准 - FlameVQA ]** FlameVQA: A Physically-Grounded UAV Wildfire VQA Benchmark with Radiometric Thermal Supervision [[arxiv]](https://arxiv.org/abs/2606.27128) [[hjfy]](https://hjfy.top/arxiv/2606.27128) [[github]](https://github.com/mobiiin/WildFire_VQA) `Benchmark`
  - 概览：基于FLAME 3配对RGB与辐射热成像数据构建首个无人机野火VQA基准FlameVQA，单图34题覆盖检测、分布估算、跨模态推理与飞行规划六类能力，揭示现有多模态大模型在浓烟火情判读上的短板。

- **[2026.06][ arXiv 2026 - 无人机细粒度主动感知具身问答 - ScoutVLA ]** ScoutVLA: UAV-Centric Active Perception via a Dual-Expert VLA Model for Open-World Embodied Question Answering [[arxiv]](https://arxiv.org/abs/2606.14772) [[hjfy]](https://hjfy.top/arxiv/2606.14772) [[project]](https://anonymous.4open.science/w/ScoutVLA-B31F/) `End-to-end` `PaliGemma 2 + Flow Matching`
  - 概览：构建首个无人机细粒度主动感知具身问答基准FG-EQA，并提出仿生侦察蜂的双专家VLA模型ScoutVLA，以语义专家与流匹配动作专家解耦训练实现连续视角微调，严格成功率达基线的10.48倍。

- **[2026.05][ arXiv 2026 - GPS拒止与退化视觉下的无人机V-SLAM多范式评测 ]** Robust Visual SLAM for UAV Navigation in GPS-Denied and Degraded Environments: A Multi-Paradigm Evaluation and Deployment Study [[arxiv]](https://arxiv.org/abs/2605.03678) [[hjfy]](https://hjfy.top/arxiv/2605.03678) `Benchmark`
  - 概览：在低光、沙尘雾霾、运动模糊等五类可控退化条件下统一评测ORB-SLAM3、DPVO、DROID-SLAM、DUSt3R、MASt3R五种范式的单目V-SLAM，并结合Jetson实测给出SWaP受限无人机的选型部署指南。

- **[2026.05][ arXiv 2026 - 无人机具身搜救高保真基准 - ESARBench ]** ESARBench: A Benchmark for Agentic UAV Embodied Search and Rescue [[arxiv]](https://arxiv.org/abs/2605.01371) [[hjfy]](https://hjfy.top/arxiv/2605.01371) [[github]](https://github.com/4amGodvzx/ESAR) [[project]](https://4amgodvzx.github.io/ESAR.github.io/) `Benchmark` `UE5+AirSim`
  - 概览：定义具身搜救(ESAR)新任务，基于UE5与AirSim-Colosseum及真实GIS/DEM复刻鳌太线、罗布泊等四类野外环境，构建12事件/60快照/600任务的高保真基准与SR、TSR、CDS、RS指标体系评估MLLM驱动的空中智能体。

- **[2026.05][ arXiv 2026 - 生成式世界模型自动构建航拍VLN数据 - FlyMirage ]** FlyMirage: A Fully Automated Generation Pipeline for Diverse and Scalable UAV Flight Data via Generative World Model [[arxiv]](https://arxiv.org/abs/2605.19600) [[hjfy]](https://hjfy.top/arxiv/2605.19600) `Benchmark` `3DGS`
  - 概览：用大模型充当场景设计师、生成式世界模型合成可漫游3DGS实景，再自动完成语义标注与动力学可行轨迹规划，全自动产出500个场景、5万条6自由度航拍VLN飞行数据。

- **[2026.05][ arXiv 2026 - 大规模多模态无人机视觉跟踪数据集 - CosFly-Track ]** CosFly-Track: A Large-Scale Multi-Modal Dataset for UAV Visual Tracking via Multi-Constraint Trajectory Optimization [[arxiv]](https://arxiv.org/abs/2605.17776) [[hjfy]](https://hjfy.top/arxiv/2605.17776) [[project]](https://huggingface.co/datasets/AutelRobotics/CosFly) `Benchmark` `MuCO`
  - 概览：面向动态目标持续跟拍任务，用MuCO多约束连续空间轨迹优化器生成约1.2万条专家/扰动轨迹、240万时间步的七通道对齐数据，并在7个视觉语言模型上完成微调基准评测。

- **[2026.04][ arXiv 2026 - 城市空域目标导向具身导航基准 ]** How Far Are Large Multimodal Models from Human-Level Spatial Action? A Benchmark for Goal-Oriented Embodied Navigation in Urban Airspace [[arxiv]](https://arxiv.org/abs/2604.07973) [[hjfy]](https://hjfy.top/arxiv/2604.07973) [[github]](https://github.com/serenditipy-AC/Embodied-Navigation-Bench) `Benchmark` `AirSim+UE`
  - 概览：耗时500余小时构建5037条城市低空目标导向导航轨迹基准，评测17款多模态大模型并揭示导航误差在“关键决策分叉”处非线性发散的现象，同时验证了几何感知、跨视角理解等四个改进方向。

- **[2026.04][ arXiv 2026 - 无人机-卫星动态跨视图空间智能基准 - LinkS²Bench ]** Are VLMs Lost Between Sky and Space? LinkS²Bench for UAV-Satellite Dynamic Cross-View Spatial Intelligence [[arxiv]](https://arxiv.org/abs/2604.02020) [[hjfy]](https://hjfy.top/arxiv/2604.02020) `Benchmark`
  - 概览：构建首个关联1022分钟无人机动态视频与200km²卫星影像的跨视图空间智能基准，含17.9k问答对与感知/定位/关系/推理四维12项任务，实测18个VLM并提出跨视图对齐适配器CVAA缓解动态对齐瓶颈。

- **[2026.03][ arXiv 2026 - 高层次无人机VLA基准 - HUGE-Bench ]** HUGE-Bench: A Benchmark for High-Level UAV Vision-Language-Action Tasks [[arxiv]](https://arxiv.org/abs/2603.19822) [[hjfy]](https://hjfy.top/arxiv/2603.19822) `Benchmark`
  - 概览：针对传统导航基准"指令过于细碎"的缺陷，提出了一个面向高层次、粗粒度指令理解的基准。基于3DGS+网格（Mesh）双表征构建数字孪生场景，创新性引入了兼顾流程保真度与物理碰撞安全性的严苛评价指标。

- **[2026.03][ CVPR 2026 - 非对齐空天视角纯视觉无人机导航 - Bearing-UAV ]** Beyond Matching to Tiles: Bridging Unaligned Aerial and Satellite Views for Vision-Only UAV Navigation [[arxiv]](https://arxiv.org/abs/2603.22153) [[hjfy]](https://hjfy.top/arxiv/2603.22153) [[github]](https://github.com/liukejia121/bearinguav) `End-to-end` `VGG-16`
  - 概览：突破跨视角地理定位的瓦片匹配范式，提出单阶段联合回归无人机绝对位置与航向的轻量模型，并构建考虑任意旋转与非对齐的多城市数据集Bearing-UAV-90K，支撑GNSS拒止下的纯视觉点对点导航。

- **[2026.03][ arXiv 2026 - 空地统一仿真基础设施 - CARLA-Air ]** CARLA-Air: Fly Drones Inside a CARLA World -- A Unified Infrastructure for Air-Ground Embodied Intelligence [[arxiv]](https://arxiv.org/abs/2603.28032) [[hjfy]](https://hjfy.top/arxiv/2603.28032) [[github]](https://github.com/louiszengCN/CarlaAir) `Benchmark` `CARLA+AirSim+UE4`
  - 概览：在单个UE4进程内深度融合CARLA与AirSim，共享物理帧与渲染管线实现空地严格时空同步，零改动兼容两者原生Python/ROS 2接口并每帧同步采集18种传感器模态，为空地协同与具身导航提供开源统一仿真基座。

- **[2026.03][ AAAI 2026 - 超低空无人机全景定位基准 - RflyPano ]** RflyPano: A Panoramic Benchmark for Ultra-low Altitude UAV Localization Powered by RflySim [[aaai]](https://ojs.aaai.org/index.php/AAAI/article/view/38884) [[github]](https://github.com/DUNDAI1998/RflyPano) `Benchmark` `RflySim+UE5`
  - 概览：基于RflySim与UE5构建首个超低空无人机全景定位基准，用四鱼眼拼接的360°全景相机采集13个场景117条轨迹共14万余张图像并配套真机数据，评测图像检索与位姿回归两类定位任务。

- **[2026.01][ arXiv 2026 - 大规模真实世界UAV VLN数据集 - AirNav ]** AirNav: A Large-Scale UAV Vision-and-Language Navigation Dataset with Natural and Diverse Instructions [[arxiv]](https://arxiv.org/abs/2601.03707) [[hjfy]](https://hjfy.top/arxiv/2601.03707) `End-to-end` `VLM+RL`
  - 概览：提出基于真实城市航拍数据构建的大规模UAV VLN基准AirNav，包含自然多样的导航指令，并引入AirVLN-R1结合监督微调与强化微调提升泛化性能。

- **[2026.01][ arXiv 2026 - 空中操纵VLA基准与数据集 - AIR-VLA ]** AIR-VLA: Vision-Language-Action Systems for Aerial Manipulation [[arxiv]](https://arxiv.org/abs/2601.21602) [[hjfy]](https://hjfy.top/arxiv/2601.21602) [[github]](https://github.com/SpencerSon2001/AIR-VLA) `Benchmark` `π0/π0.5` `Isaac Sim`
  - 概览：基于Isaac Sim构建首个面向空中操纵系统的VLA基准，发布3000条人工遥操作演示数据，覆盖基础操纵、物体与空间理解、语义推理和长时程规划四类任务，并系统评测主流VLA与VLM模型。

- **[2026.01][ arXiv 2026 - 6G下大模型无人机智能体安全评测 - α³-SecBench ]** $α^3$-SecBench: A Large-Scale Evaluation Suite of Security, Resilience, and Trust for LLM-based UAV Agents over 6G Networks [[arxiv]](https://arxiv.org/abs/2601.18754) [[hjfy]](https://hjfy.top/arxiv/2601.18754) [[github]](https://github.com/maferrag/AlphaSecBench) `Benchmark` `LLM`
  - 概览：面向6G网络下基于大模型的无人机智能体，构建首个覆盖七层自主栈、175种威胁与2万条攻击场景的安全-韧性-可信评测套件，实测23个主流大模型总分仅12.9%~57.1%。

### 2025

- **[2025.12][ NeurIPS 2025 - 动态城市机器人导航协作 - SimWorld-Robotics ]** SimWorld-Robotics: Synthesizing Photorealistic and Dynamic Urban Environments for Multimodal Robot Navigation and Collaboration [[arxiv]](https://arxiv.org/abs/2512.10046) [[hjfy]](https://hjfy.top/arxiv/2512.10046) [[github]](https://github.com/SimWorld-AI/SimWorld) `Benchmark`
  - 概览：SimWorld 的机器人专题拓展，生成带有人群和交通系统的动态逼真城市场景。提供了"多模态指令导航"与"多智能体搜寻汇合"两个极具挑战的基准，全面测试机器人复杂感知与协作。

- **[2025.12][ arXiv 2025 - 多模态LLM低空无人机基准 - MM-UAVBench ]** MM-UAVBench: How Well Do Multimodal Large Language Models See, Think, and Plan in Low-Altitude UAV Scenarios? [[arxiv]](https://arxiv.org/abs/2512.23219) [[hjfy]](https://hjfy.top/arxiv/2512.23219) [[github]](https://github.com/AI9Stars/MM-UAVBench) [[dataset]](https://huggingface.co/datasets/daisq/MM-UAVBench) [[project]](https://mm-uavbench.github.io/) `Benchmark`
  - 概览：提出面向低空无人机场景的多模态大模型综合评测基准MM-UAVBench，系统评估MLLM在感知、认知和规划三个维度的能力。

- **[2025.12][ NeurIPS 2025 - 开放式真实世界模拟器 - SimWorld ]** SimWorld: An Open-ended Realistic Simulator for Autonomous Agents in Physical and Social Worlds [[arxiv]](https://arxiv.org/abs/2512.01078) [[hjfy]](https://hjfy.top/arxiv/2512.01078) [[project]](https://github.com/SimWorld-AI/SimWorld) `Benchmark`
  - 概览：基于虚幻引擎5（UE5）构建的开放式沙盒模拟器。支持语言驱动的程序化场景生成、多模态智能体交互和高度拟真的物理及社会规则，专为评测前沿大模型代理（如GPT-4o）的长程推理能力而生。

- **[2025.11][ AAAI 2026 - 多无人机协同感知推理基准 - AirCopBench ]** AirCopBench: A Benchmark for Multi-drone Collaborative Embodied Perception and Reasoning [[arxiv]](https://arxiv.org/abs/2511.11025) [[hjfy]](https://hjfy.top/arxiv/2511.11025) `Benchmark`
  - 概览：提出首个多无人机协同的具身感知与推理基准，包含超过1.4万个VQA问答对。着重考察多模态大模型在遮挡、信号丢失等真实"感知退化"场景下的多视角融合与决策推理能力。

- **[2025.11][ arXiv 2025 - 无人机导航空间智能基准与感知模型 - SpatialSky ]** Is your VLM Sky-Ready? A Comprehensive Spatial Intelligence Benchmark for UAV Navigation [[arxiv]](https://arxiv.org/abs/2511.13269) [[hjfy]](https://hjfy.top/arxiv/2511.13269) [[github]](https://github.com/linglingxiansen/SpatialSKy) `Benchmark` `Qwen2.5-VL-7B`
  - 概览：构建覆盖环境感知与场景理解两大类13项子能力的无人机空间智能基准与百万级数据集，并以SFT+GRPO两阶段训练出Sky-VLM，在全部任务上超越现有开源与闭源VLM。

- **[2025.11][ arXiv 2025 - LLM生成飞行场景的无人机自主智能基准 - UAVBench ]** UAVBench: An Open Benchmark Dataset for Autonomous and Agentic AI UAV Systems via LLM-Generated Flight Scenarios [[arxiv]](https://arxiv.org/abs/2511.11252) [[hjfy]](https://hjfy.top/arxiv/2511.11252) [[github]](https://github.com/maferrag/UAVBench) `Benchmark` `LLM`
  - 概览：提出统一的无人机场景模式与分类法引导的LLM生成框架，构建5万条经几何/物理/安全校验并带风险标注的飞行场景及UAVBench_MCQ推理基准，系统评测32个前沿大模型。

- **[2025.09][ AAAI 2026 - 多无人机集群自主飞行数据集 - U2UData+ ]** U2UData+: A Scalable Swarm UAVs Autonomous Flight Dataset for Embodied Long-horizon Tasks [[arxiv]](https://arxiv.org/abs/2509.00055) [[hjfy]](https://hjfy.top/arxiv/2509.00055) `Benchmark`
  - 概览：提出首个面向具身长时程任务的大规模多无人机集群自主飞行数据集，由15架无人机协同采集，涵盖12个场景、720条轨迹、120小时飞行数据，并提供可扩展的在线数据采集与闭环验证平台。

- **[2025.08][ ACM MM 2025 - 开放世界空中目标导航基准 - UAV-ON ]** UAV-ON: A Benchmark for Open-World Object Goal Navigation with Aerial Agents [[arxiv]](https://arxiv.org/abs/2508.00288) [[hjfy]](https://hjfy.top/arxiv/2508.00288) `Benchmark`
  - 概览：提出首个面向开放世界的无人机目标导航基准UAV-ON，包含14个高保真虚幻引擎环境和1270个标注目标，定义了基于语义目标描述的大规模空中ObjectNav任务。

- **[2025.06][ NeurIPS 2025 D&B - VLM开放世界探索能力基准 - FlySearch ]** FlySearch: Exploring how vision-language models explore [[arxiv]](https://arxiv.org/abs/2506.02896) [[hjfy]](https://hjfy.top/arxiv/2506.02896) [[github]](https://github.com/gmum/FlySearch) `Benchmark` `UE5`
  - 概览：基于UE5构建高保真程序化生成户外环境的无人机目标搜索基准，系统评测主流VLM的零样本具身探索能力，揭示其在视觉幻觉、上下文理解与任务规划上与人类基线的显著差距。

- **[2025.06][ ICLR 2026 Workshop - RAG增强无人机数学推理与基准 - RAG-UAV ]** Mathematical Reasoning for Unmanned Aerial Vehicles: A RAG-Based Approach for Complex Arithmetic Reasoning [[arxiv]](https://arxiv.org/abs/2506.04998) [[hjfy]](https://hjfy.top/arxiv/2506.04998) [[github]](https://github.com/Mehdiazarafza/UAV-RAG) `Benchmark` `LLM+RAG`
  - 概览：提出检索增强生成框架RAG-UAV，为通用大模型注入无人机领域文献中的公式知识，并构建四难度等级的UAV-Math-Bench，显著提升多步复杂算术与物理推理的公式选择准确率并降低数值误差。

- **[2025.05][ arXiv 2025 - 无人机具身智能评测基准 - BEDI ]** BEDI: A Comprehensive Benchmark for Evaluating Embodied Agents on UAVs [[arxiv]](https://arxiv.org/abs/2505.18229) [[hjfy]](https://hjfy.top/arxiv/2505.18229) [[github]](https://github.com/lostwolves/BEDI) `Benchmark`
  - 概览：提出了一个用于评估无人机具身智能体（Embodied Agents）的全面基准，包含基于感知-决策-动作循环的标准化子任务，并提供了混合测试平台。

- **[2025.05][ arXiv 2025 - 大规模真实世界模仿学习基准 ]** UAV-Flow Colosseo: A Real-World Benchmark for Flying-on-a-Word UAV Imitation Learning [[arxiv]](https://arxiv.org/abs/2505.15725) [[hjfy]](https://hjfy.top/arxiv/2505.15725) [[project]](https://prince687028.github.io/UAV-Flow) `Benchmark`
  - 概览：收集了大量真实世界飞行数据，侧重于细粒度语言指令控制下的无人机模仿学习，直面Sim-to-Real难题。

- **[2025.04][ ICCV 2025 - 空中视觉定位基准 - AerialVG ]** AerialVG: A Challenging Benchmark for Aerial Visual Grounding by Exploring Positional Relations [[arxiv]](https://arxiv.org/abs/2504.07836) [[hjfy]](https://hjfy.top/arxiv/2504.07836) `Benchmark`
  - 概览：提出首个面向空中视角的视觉定位（Visual Grounding）基准AerialVG，包含5K真实航拍图像和50K人工标注描述，强调空间位置关系推理，并设计层次交叉注意力与关系感知定位模块。

- **[2025.03][ arXiv 2025 - 无人机认知任务VLA模型与基准 - CognitiveDrone ]** CognitiveDrone: A VLA Model and Evaluation Benchmark for Real-Time Cognitive Task Solving and Reasoning in UAVs [[arxiv]](https://arxiv.org/abs/2503.01378) [[hjfy]](https://hjfy.top/arxiv/2503.01378) [[project]](https://cognitivedrone.github.io/) `End-to-end` `OpenVLA-7B` `Gazebo`
  - 概览：提出面向无人机认知任务的VLA模型CognitiveDrone及其VLM推理增强版R1，并基于Gazebo构建首个无人机认知能力开源评测基准CognitiveDroneBench，涵盖人类识别、符号理解与推理三类任务。

- **[2025.02][ ICLR 2026 - 监督到强化自适应空中VLN - Openfly ]** Openfly: A comprehensive platform for aerial vision-language navigation [[arxiv]](https://arxiv.org/abs/2502.18041) [[hjfy]](https://hjfy.top/arxiv/2502.18041) [[project]](https://shailab-ipec.github.io/openfly/) `End-to-end` `LLaMA` `OpenFly`
  - 概览：构建覆盖数据生成、仿真训练与统一评测的空中视觉语言导航平台OpenFly，并提出从监督微调到强化学习的自适应方法以提升复杂连续场景中的导航成功率。
  - 个人评价：目前最好用的 benchmark 和数据生成工具链，算力要求较高 8 张 A100（每张 80 G）

### 2024

- **[2024.11][ ICCV 2025 - 无人机视频转BEV地理定位 - Video2BEV ]** Video2BEV: Transforming Drone Videos to BEVs for Video-based Geo-localization [[arxiv]](https://arxiv.org/abs/2411.13610) [[hjfy]](https://hjfy.top/arxiv/2411.13610) `Benchmark`
  - 概览：针对单张无人机图像地理定位易受遮挡和视角局限的问题，提出 Video2BEV 范式。利用 3D 高斯喷溅（3DGS）将连续的无人机视频流三维重建并投影为无畸变的鸟瞰图（BEV），大幅提高跨视角匹配准确率，并发布了首个基于视频的无人机地理定位数据集 UniV。

- **[2024.10][ ICLR 2025 - 真实感UAV导航基准与大模型方法 ]** Towards Realistic UAV Vision-Language Navigation: Platform, Benchmark, and Methodology [[arxiv]](https://arxiv.org/abs/2410.07087) [[hjfy]](https://hjfy.top/arxiv/2410.07087) [[github]](https://github.com/prince687028/Travel) `End-to-end` `LLaMA` `AirSim+UE4`
  - 概览：构建了基于虚幻引擎的连续飞行导航基准，并提出了基于多模态大模型的层次化轨迹生成方法。

- **[2024.10][ Sensors 2024 - 跨视角无人机地理定位数据集与方法 - VDUAV ]** UAV Geo-Localization Dataset and Method Based on Cross-View Matching [[mdpi]](https://www.mdpi.com/1424-8220/24/21/6905) `Benchmark`
  - 概览：提出了一个由数字孪生技术（结合真实环境3D建模与虚拟投影）生成的跨视角定位数据集 VDUAV，并建立了一个多尺度特征自适应加权融合的基线模型 VRLM，有效匹配无人机视角与卫星视角进行定位。

- **[2024.08][ arXiv 2024 - 空中具身世界模型基准套件 - AeroVerse ]** AeroVerse: UAV-Agent Benchmark Suite for Simulating, Pre-training, Finetuning, and Evaluating Aerospace Embodied World Models [[arxiv]](https://arxiv.org/abs/2408.15511) [[hjfy]](https://hjfy.top/arxiv/2408.15511) `Benchmark` `VLM/3D-VLM` `AeroVerse`
  - 概览：构建AerialAgent-Ego10k、CyberAgent-Ego500k及五类下游指令数据集，集成多种2D/3D视觉语言模型、模拟器与SkyAgentEval，形成面向空中具身世界模型预训练、微调和评测的一体化基准套件。

- **[2024.06][ ICCV 2025 - 大规模真实世界空中导航数据集 - CityNav ]** CityNav: A Large-Scale Dataset for Real-World Aerial Navigation [[arxiv]](https://arxiv.org/abs/2406.14240) [[hjfy]](https://hjfy.top/arxiv/2406.14240) `Benchmark` `CityFlight`
  - 概览：提出首个大规模真实世界空中VLN数据集CityNav，包含32637条人类示范轨迹覆盖剑桥和伯明翰两座城市4.65km²，并提供地理语义地图辅助导航。

### 2023

- **[2023.11][ ECCV 2024 - 自然语言引导无人机地理定位基准 - GeoText-1652 ]** Towards Natural Language-Guided Drones: GeoText-1652 Benchmark with Spatial Relation Matching [[arxiv]](https://arxiv.org/abs/2311.12751) [[hjfy]](https://hjfy.top/arxiv/2311.12751) [[github]](https://github.com/MultimodalGeo/GeoText-1652) [[project]](https://multimodalgeo.github.io/GeoText/) `Benchmark`
  - 概览：在University-1652基础上扩展空间感知文本标注，构建含27.6万文本-边界框对的自然语言引导无人机地理定位基准，并提出混合空间匹配目标实现区域级空间关系对齐。

- **[2023.08][ ICCV 2023 - 开篇之作 - AerialVLN ]** AerialVLN: Vision-and-Language Navigation for UAVs [[arxiv]](https://arxiv.org/abs/2308.06735) [[hjfy]](https://hjfy.top/arxiv/2308.06735) [[github]](https://github.com/AirVLN/AirVLN) `End-to-end` `CMA` `AirSim+UE4`
  - 概览：提出首个面向无人机连续环境的视觉语言导航任务、AirVLN仿真平台与基准模型，系统刻画空中视角、三维动作空间和长距离飞行给指令跟随带来的挑战。
  - 个人评价：benchmark 不好用，复现结果不一致，算力要求一般

### 📦 Dataset Comparison

| 数据集 | 环境 | 规模 | 指令粒度 | 传感器 | 类型 | 备注 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **[AerialVLN](https://www.kaggle.com/datasets/shuboliu/aerialvln)/[S](https://www.kaggle.com/datasets/shuboliu/aerialvln-s)** | 25 城市场景 | 8,446/3,916 | 分步 | RGB-D | Virtual | 早期 3D，飞手轨迹 |
| **[CityNav](https://github.com/water-cookie/citynav)** | 剑桥+伯明翰 | 32,637 | 分步 | RGB-D | Real | 真人演示轨迹 |
| **[OpenFly](https://huggingface.co/datasets/IPEC-COMMUNITY/OpenFly)** | 18 场景，150+ km² | 100k | 高层 | RGB-D, LiDAR, PC | Real→Virtual | 多引擎，跨场景 |
| **[AVDN](https://sites.google.com/view/aerial-vision-and-dialog/home)** | 全球卫星 | 3,064 | 对话/混合 | RGB | Real | xView 卫星图 |
| **[OpenUAV](https://huggingface.co/datasets/wangxiangyu0814/TravelUAV)** | 22 多样场景 | 12k | 混合 | RGB-D(5), LiDAR, IMU, GPS | Virtual | 城/乡/林/沙漠 |
| **[IndoorUAV](https://www.modelscope.cn/datasets/valyentine/Indoor_UAV)** | 室内连续环境 | 大规模 | 长/短程混合 | RGB-D | Virtual | 首个室内 UAV-VLN |
| **[EmbodiedCity](https://github.com/tsinghua-fib-lab/EmbodiedCity)** | 北京 CBD | 大规模 | 具身任务 | RGB-D, Seg, IMU, GPS | Real(重建) | 动态行人/车辆 |
| **[AirNav](https://arxiv.org/abs/2601.03707)** | 真实城市航拍 | 大规模 | 自然多样 | RGB | Real | 自然语言指令 |

> [!NOTE]
> - **规模**：轨迹数量 · **指令粒度**：指令的描述层级
> - **类型**：Virtual（仅模拟） / Real（真实采集） / Real→Virtual（真实数据重建为仿真）

### 🎮 Simulator Comparison

| 模拟器 | 引擎 | 环境 | 类型 | 传感器 | 核心特性 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **[AerialVLN](https://www.kaggle.com/datasets/shuboliu/aerialvln-simulators)** | UE4 + AirSim | 25 城市场景 | Virtual | RGB-D | 首个 UAV-VLN 仿真器，870+ 物体，4-DoF |
| **[OpenUAV](https://huggingface.co/datasets/wangxiangyu0814/TravelUAV_env)** | UE4 + AirSim | 22 郊区/自然场景 | Virtual | RGB-D, IMU, GPS | 6-DoF，天气/光照变化，复杂动力学 |
| **[OpenFly](https://github.com/SHAILAB-IPEC/OpenFly-Platform)** | UE4/5, GTA-V, GE, 3DGS | 18 场景，150+ km² | Real→Virtual | RGB, D | 统一 API，多渲染引擎，跨场景泛化 |
| **[CityNav](https://github.com/water-cookie/citynav)** | WebGL (Potree) | 剑桥+伯明翰 (8.7 km²) | Real(重建) | RGB, D (PC) | 真实 3D 重建，地理语义图 |
| **[EmbodiedCity](https://huggingface.co/datasets/EmbodiedCity/EmbodiedCity-Simulator)** | UE5 + AirSim | 北京 CBD | Real(重建) | RGB-D, Seg, IMU, GPS | 动态行人/车辆，高精度还原 |
| **[SimWorld](https://github.com/SimWorld-AI/SimWorld)** | UE5 | 程序生成场景 | Virtual | 多模态 | 沙盒式，语言驱动场景生成 |

> [!NOTE]
> - **类型**：Virtual（仅软件） / Real（涉及硬件） / Real→Virtual（真实数据重建为仿真）

### 🔄 Sim-to-Real

| 论文 | 方法 | 核心贡献 |
| :--- | :--- | :--- |
| **AutoFly** (ICLR 2026) | 伪深度编码器 + 端到端 VLA | 引入伪深度增强 RGB-only 空间推理, 在真实野外环境中验证 |
| **SOUS VIDE** (arXiv 2024) | 3D Gaussian Splatting | 在 3DGS 重建环境中训练策略, 直接迁移到真实无人机 |
| **Fly-DA** (arXiv 2025) | 域适应 + RL | 通过域随机化与自适应在 3DGS 仿真与真实环境间迁移 |
| **OnFly** (arXiv 2026) | 零样本 + 语义-几何验证 | 全机载零样本框架, 无需仿真训练直接在真机部署 |
| **See, Point, Fly** (CoRL 2025) | VLM 零样本 + 针孔模型 | 2D 像素 → 3D 位移, 零训练在真实无人机上飞行 |

> [!IMPORTANT]
> **Sim-to-Real 是落地关键环节，本板块持续征集。** 如有相关论文、域随机化/系统辨识技术、或真机演示视频，欢迎通过 PR / Issue 补充！

## 📝 Surveys & Perspectives
- **[2026.07][ Drones 2026 - 无人机与双臂操作的VLA大模型综述 ]** Vision Language Action (VLA) Models for Unmanned Aerial Robotics and Bimanual Manipulation: A Review [[arxiv]](https://arxiv.org/abs/2607.06706) [[hjfy]](https://hjfy.top/arxiv/2607.06706) [[doi]](https://doi.org/10.3390/drones10060412) `Survey`
  - 概览：横跨2017-2026年的183篇文献，将无人机导航控制与双臂机器人操作放在统一VLA框架下比较，系统总结架构、训练配方、动作表征、记忆与世界模型，并归纳十四项跨具身研究方向。

- **[2026.04][ arXiv 2026 - 迈向大模型时代的空中VLN综述 ]** Vision-Language Navigation for Aerial Robots: Towards the Era of Large Language Models [[arxiv]](https://arxiv.org/abs/2604.07705) [[hjfy]](https://hjfy.top/arxiv/2604.07705) `Survey`
  - 概览：深度聚焦于大语言模型（LLM）和视觉语言模型（VLM）在空中导航中的整合。将领域方法划分为端到端大模型、分层架构、多智能体及对话驱动导航等类别，并深刻剖析了离散/连续动作空间与虚实迁移（Sim-to-Real）等七大开放性难题。

- **[2026.04][ arXiv 2026 - UAV-VLN进展、挑战与路线图 ]** Vision-and-Language Navigation for UAVs: Progress, Challenges, and a Research Roadmap [[arxiv]](https://arxiv.org/abs/2604.13654) [[hjfy]](https://hjfy.top/arxiv/2604.13654) `Survey`
  - 概览：从正式的任务定义（POMDP与连续环境）出发，梳理了从早期深度学习到当今基于多模态大模型（VLM）、视觉-语言-动作（VLA）模型以及"生成式世界模型（World Models）"结合的技术演进路线图。

- **[2026.03][ Remote Sensing 2026 - 无人机具身智能九维对比综述 ]** Embodied AI in the Sky: A Comparative Review of UAV Embodied AI, from Autonomous Remote Sensing to Task Execution [[mdpi]](https://www.mdpi.com/2072-4292/18/10/1509) `Survey`
  - 概览：首篇用九维框架把无人机具身智能与室内机器人、自动驾驶具身智能系统对标的综述，梳理其核心任务、模拟器与数据集基建、建模范式，并剖析大模型迁移失效与Sim-to-Real鸿沟等瓶颈。

- **[2026.02][ arXiv 2026 - 大模型赋能无人机作业与通信综述 ]** Large Language Model-Assisted UAV Operations and Communications: A Multifaceted Survey and Tutorial [[arxiv]](https://arxiv.org/abs/2602.19534) [[hjfy]](https://hjfy.top/arxiv/2602.19534) `Survey` `LLM/MLLM`
  - 概览：系统综述大语言模型与无人机的融合路径，提出认知决策-感知-控制通信三层统一架构，梳理预训练/微调/RAG/提示工程四类适配范式及其在导航、任务规划、集群协同与通信管理中的应用与伦理风险。

- **[2026.01][ 航空学报 2026 - 空中操作机器人运动规划综述 ]** Research progress and prospect of motion planning technology for aerial manipulators [[doi]](https://hkxb.buaa.edu.cn/CN/10.7527/S1000-6893.2026.33402) `Survey`
  - 概览：系统梳理空中操作机器人的平台构型与面向规划的建模约束体系，横向对比基于采样、优化与学习的三类运动规划算法，并展望仿生、多机协同、人机协同与跨介质四大方向。

- **[2025.10][ arXiv 2025 - 自然语言驱动多尺度无人机飞行的前瞻 - NeLV ]** Next-Generation LLM for UAV: From Natural Language to Autonomous Flight [[arxiv]](https://arxiv.org/abs/2510.21739) [[hjfy]](https://hjfy.top/arxiv/2510.21739) [[github]](https://github.com/liangqiyuan/NeLV) [[project]](https://liangqiyuan.github.io/NeLV/) `Survey` `Phi-4-mini`
  - 概览：立场论文提出由LLM解析、航线规划、路径规划、控制平台与实时监控组成的五阶段NeLV系统，将自然语言指令转为短中远程可执行飞行轨迹，并给出迈向LLM自动驾驶仪的五级自动化路线图。

- **[2025.09][ IEEE IoT Magazine 2026 - 多模态大模型赋能无人机意图识别 ]** Enhancing Low-Altitude Airspace Security: MLLM-Enabled UAV Intent Recognition [[arxiv]](https://arxiv.org/abs/2509.06312) [[hjfy]](https://hjfy.top/arxiv/2509.06312) [[ieee]](https://ieeexplore.ieee.org/document/11373864) `Survey` `Qwen-VL-Plus` `AirSim`
  - 概览：面向低空空域安全，提出首个多模态大模型赋能的非合作无人机意图识别架构，融合RGB/红外/雷达决策级感知与思维链推理，并在AirSim低空对抗场景中验证可行性与五大落地挑战。

- **[2025.09][ The Innovation Informatics 2025 - 空中具身视觉语言导航综述 - AeroVerse-Review ]** AeroVerse-Review: Comprehensive survey on aerial embodied vision-and-language navigation [[doi]](https://doi.org/10.59717/j.xinn-inform.2025.100015) `Survey`
  - 概览：系统综述空中具身视觉语言导航的仿真平台、数据集与核心算法，分析语言、三维感知和飞行动力学耦合带来的独特挑战，并总结低空真实部署方向。

- **[2025.06][ arXiv 2025 - Agentic UAV多领域综述 ]** UAVs Meet Agentic AI: A Multidomain Survey of Autonomous Aerial Intelligence and Agentic UAVs [[arxiv]](https://arxiv.org/abs/2506.08045) [[hjfy]](https://hjfy.top/arxiv/2506.08045) `Survey`
  - 概览：系统定义具备自主推理、多模态感知与反思控制的Agentic UAV概念与分层架构，综述其在精准农业、灾难救援、基础设施巡检等七大领域的应用、挑战与未来路线图。

- **[2025.04][ 导航定位与授时 2025 - 飞行器视觉导航演进综述 ]** New era of aircraft visual navigation: from terrain matching to spatial intelligence [[doi]](https://doi.org/10.19306/j.cnki.2095-8110.2025.03.001) `Survey`
  - 概览：将飞行器视觉导航梳理为地形匹配、景象匹配、空间计算与空间智能认知四个阶段，比较各阶段的信息输入、导航输出和应用特征，并展望空间大模型驱动的自主认知导航。

- **[2025.02][ 机器人 2025 - 自主飞行器技术及其低空经济应用综述 ]** Overview on Autonomous Aircraft Technology and Its Application to Low-altitude Economy [[doi]](https://robot.sia.cn/article/doi/10.13973/j.cnki.robot.250073) `Survey`
  - 概览：系统梳理低空经济的概念、政策与典型应用场景，提出“感-通-算-控”一体化技术框架，剖析自主飞行器构形、能源管理、感知定位、高效通信、任务规划与协同控制等关键技术及发展趋势。

- **[2025.01][ Information Fusion 2025 - 无人机与LLM综述 ]** UAVs Meet LLMs: Overviews and Perspectives Toward Agentic Low-Altitude Mobility [[arxiv]](https://arxiv.org/abs/2501.02341) [[hjfy]](https://hjfy.top/arxiv/2501.02341) `Survey`
  - 概览：系统综述了LLM与无人机系统的融合，涵盖自主决策、人机交互、实时适应等方面，提出面向智能低空机动的代理化框架愿景。

- **[2024.07][ 电子学报 2025 - 基于视觉的无人机定位与导航方法综述 ]** A Review of Vision-Based UAV Localization and Navigation Methods [[doi]](https://www.ejournal.org.cn/CN/10.12263/DZXB.20240699) `Survey`
  - 概览：系统梳理基于视觉的无人机定位（图像检索与图像匹配）与导航（障碍物检测规避与路径规划）四大类方法，重点覆盖深度学习最新进展，并展望数据集多样性、实时性、能耗与虚实迁移等挑战。

## 📌 Other Foundational Works

### 1. VLA Foundation Models

涵盖语义与三维空间的对齐、自然语言到物理坐标或控制信号的映射基础。

- **[2026/07][ arXiv 2026 - 统一五类具身导航任务 - ABot-N1 ]** ABot-N1: Toward a General Visual Language Navigation Foundation Model [[arxiv]](https://arxiv.org/abs/2607.10383) [[hjfy]](https://hjfy.top/arxiv/2607.10383) `End-to-end`
  - 概览：提出ABot-N1快慢架构：慢速视觉语言推理器生成显式思维链与像素目标，像素锚点作为点目标、物体目标、兴趣点、指令跟随和人员跟随任务的统一接口；快速动作专家再结合文本线索与像素引导输出连续航点。

- **[2026/06][ arXiv 2026 - 统一跨任务具身模型 - OneVLA ]** OneVLA: A Unified Framework for Embodied Tasks [[arxiv]](https://arxiv.org/abs/2606.01241) [[hjfy]](https://hjfy.top/arxiv/2606.01241) `End-to-end`
  - 概览：提出OneVLA统一具身任务框架，以共享视觉语言动作表征支持跨导航与操作任务学习，并增强跨任务和跨本体泛化。

- **[2026/06][ arXiv 2026 - 统一数据生成、评测与策略学习 - GN0 ]** GN0: Toward a Unified Paradigm for Generation, Evaluation, and Policy Learning in Visual-Language Navigation [[arxiv]](https://arxiv.org/abs/2606.03682) [[hjfy]](https://hjfy.top/arxiv/2606.03682) `Benchmark`
  - 概览：提出GN0统一VLN体系，联合GN-Matrix大规模数据、支持动态3DGS人物的GN-Bench仿真基准和经监督学习、DAgger及强化学习训练的BAE导航基础模型。

- **[2026/06][ arXiv 2026 - 面向五类任务的可扩展导航模型 - Qwen-RobotNav ]** Qwen-RobotNav Technical Report: A Scalable Navigation Model Designed for an Agentic Navigation System [[arxiv]](https://arxiv.org/abs/2606.18112) [[hjfy]](https://hjfy.top/arxiv/2606.18112) `Zero-Shot`
  - 概览：提出Qwen-RobotNav可参数化导航模型，以任务模式、视觉令牌预算和多相机权重在推理时动态调整观察策略，使同一骨干支持指令跟随、目标搜索、跟踪和自主驾驶。

- **[2026/06][ arXiv 2026 - 几何轨迹监督的野外视频导航VLA - VEGA ]** VEGA: Learning Navigation VLAs from In-the-Wild Egocentric Video with Geometric Trajectory Supervision [[arxiv]](https://arxiv.org/abs/2606.18426) [[hjfy]](https://hjfy.top/arxiv/2606.18426) `End-to-end`
  - 概览：提出几何监督的导航VLA训练范式，无需人工动作标注与机器人示教，仅靠无标签野外第一人称视频即可提炼避障导航行为。

- **[2026/05][ ICML 2026 - VLA因果理解与泛化的具身可解释性 ]** Embodied Interpretability: Linking Causal Understanding to Generalization in Vision-Language-Action Models [[arxiv]](https://arxiv.org/abs/2605.00321) [[hjfy]](https://hjfy.top/arxiv/2605.00321) `Benchmark`
  - 概览：提出干预显著性得分ISS与干扰质量比NMR两项因果可解释性指标，揭示VLA策略依赖虚假视觉相关性的缺陷并证明NMR可预测分布偏移下的泛化性能。

- **[2026/05][ arXiv 2026 - 动作翻译驱动的跨任务跨本体导航 - Uni-LaViRA ]** Uni-LaViRA: Language-Vision-Robot Actions Translation for Unified Embodied Navigation [[arxiv]](https://arxiv.org/abs/2605.27582) [[hjfy]](https://hjfy.top/arxiv/2605.27582) `Zero-Shot`
  - 概览：提出Uni-LaViRA语言-视觉-机器人动作翻译框架，以统一中间决策接口在无需任务专用训练的情况下连接不同视觉语言输入和机器人动作空间，覆盖四类导航任务。

- **[2026/05][ arXiv 2026 - 跨任务、跨环境、跨形态的统一具身大模型 - Qwen-VLA ]** Qwen-VLA: Unifying Vision-Language-Action Modeling across Tasks, Environments, and Robot Embodiments [[arxiv]](https://arxiv.org/abs/2605.30280) [[hjfy]](https://hjfy.top/arxiv/2605.30280) `Zero-Shot`
  - 概览：提出Qwen-VLA统一视觉语言动作模型，以共享动作与轨迹表示及流匹配动作解码器联合建模操作、视觉语言导航、第一人称动作和轨迹预测，并支持多类机器人本体。

- **[2026/04][ arXiv 2026 - 实时技能切换机器狗 - OpenGo ]** OpenGo: An OpenClaw-Based Robotic Dog with Real-Time Skill Switching [[arxiv]](https://arxiv.org/abs/2604.01708) [[hjfy]](https://hjfy.top/arxiv/2604.01708) `End-to-end`
  - 概览：提出OpenGo四足机器人框架，以经验证的结构化技能库约束底层执行，并由大语言模型完成自然语言任务分解、技能选择与实时切换。

- **[2026/04][ arXiv 2026 - 面向机器人的快速、安全、通用零样本目标导航 - FSUNav ]** FSUNav: A Cerebrum-Cerebellum Architecture for Fast, Safe, and Universal Zero-Shot Goal-Oriented Navigation [[arxiv]](https://arxiv.org/abs/2604.03139) [[hjfy]](https://hjfy.top/arxiv/2604.03139) `Zero-Shot`
  - 概览：提出FSUNav大小脑协同的零样本目标导航架构，由强化学习小脑执行跨本体安全局部规划，并由VLM大脑完成开放词汇目标检测、验证与高层推理。

- **[2026/04][ arXiv 2026 - 分层语义-物理异构多机器人协作 - ROSClaw ]** ROSClaw: A Hierarchical Semantic-Physical Framework for Heterogeneous Multi-Agent Collaboration [[arxiv]](https://arxiv.org/abs/2604.04664) [[hjfy]](https://hjfy.top/arxiv/2604.04664) `RL`
  - 概览：提出ROSClaw分层语义-物理多机器人协作框架，以信息空间、软件系统和物理执行三层异步解耦低频任务规划与高频控制，统一异构智能体的长时序协同。

- **[2026/04][ arXiv 2026 - 预算感知高效开源VLA - A1 ]** A1: A Fully Transparent Open-Source, Adaptive and Efficient Truncated Vision-Language-Action Model [[arxiv]](https://arxiv.org/abs/2604.05672) [[hjfy]](https://hjfy.top/arxiv/2604.05672) `Diffusion`
  - 概览：提出完全开源透明的A1视觉语言动作模型，通过预算感知的自适应推理与截断动作生成降低部署延迟和计算成本。

- **[2026/04][ arXiv 2026 - 持续协作自进化机器人智能体 - ABot-Claw ]** ABot-Claw: A Foundation for Persistent, Cooperative, and Self-Evolving Robotic Agents [[arxiv]](https://arxiv.org/abs/2604.10096) [[hjfy]](https://hjfy.top/arxiv/2604.10096) `Agentic`
  - 概览：在OpenClaw之上加入异构机器人能力调度、跨本体多模态长期记忆和通用评论器闭环反馈，使自然语言意图能够持续执行、纠错、重规划并跨机器人协作。

- **[2026/04][ arXiv 2026 - 自主在轨服务智能体框架 - SpaceMind ]** SpaceMind: A Modular and Self-Evolving Embodied Vision-Language Agent Framework for Autonomous On-orbit Servicing [[arxiv]](https://arxiv.org/abs/2604.14399) [[hjfy]](https://hjfy.top/arxiv/2604.14399) `End-to-end`
  - 概览：提出SpaceMind模块化在轨服务智能体，将知识、工具与推理解耦并通过MCP-Redis接口编排，使同一视觉语言导航系统可在UE5仿真与物理机器人间迁移。

- **[2026/03][ arXiv 2026 - 通用具身VLA基础模型 - OmniVLN ]** OmniVLN: Omnidirectional 3D Perception and Token-Efficient LLM Reasoning for Visual-Language Navigation across Air and Ground Platforms [[arxiv]](https://arxiv.org/abs/2603.17351) [[hjfy]](https://hjfy.top/arxiv/2603.17351) `Zero-Shot` `GSM` `Hierarchical`
  - 概览：该系统采用基于持续同调的房间分区技术，结合多分辨率空间注意力提示，将全局场景转化为以智能体为中心的八分树表示，使大语言模型能逐步筛选候选房间、推断自身方位并生成可执行导航指令。

- **[2026/03][ arXiv 2026 - 博弈驱动多智能体VLA跟踪 - CoMaTrack ]** CoMaTrack: Competitive Multi-Agent Game-Theoretic Tracking with Vision-Language-Action Models [[arxiv]](https://arxiv.org/abs/2603.22846) [[hjfy]](https://hjfy.top/arxiv/2603.22846) `RL`
  - 概览：提出CoMaTrack竞争式多智能体强化学习框架，让语言条件跟踪者在动态对手参与的博弈子任务中学习适应性规划与抗干扰策略；同时发布Habitat上的CoMaTrack-Bench，标准化评测主动对抗条件下的具身视觉跟踪。

- **[2026/03][ arXiv 2026 - 导航与预抓取统一扩散策略 - DiffusionAnything ]** DiffusionAnything: End-to-End In-context Diffusion Learning for Unified Navigation and Pre-Grasp Motion [[arxiv]](https://arxiv.org/abs/2603.26322) [[hjfy]](https://hjfy.top/arxiv/2603.26322) `Zero-Shot`
  - 概览：提出DiffusionAnything图像空间扩散策略，以任务模式、深度尺度和空间注意力的多尺度FiLM调制统一导航与预抓取运动，并加入轨迹对齐深度预测和AnyTraverse自监督注意力，仅用RGB生成目标导向路径。

- **[2026/03][ AAAI 2026 - 视听语言动作导航模型 - NaVLA² ]** NaVLA²: A Vision-Language-Audio-Action Model for Multimodal Instruction Navigation [[doi]](https://doi.org/10.1609/aaai.v40i22.38886) [[github]](https://github.com/felixfjg/NaVLA) `VLA`
  - 概览：提出融合视觉、语言、空间音频与动作的NaVLA²，并构建43.9K规模MINav多模态指令数据集，使智能体能消解目标歧义并生成可解释导航决策。

- **[2026/02][ arXiv 2026 - 多本体机器人操作VLA基础模型 - ABot-M0 ]** ABot-M0: VLA Foundation Model for Robotic Manipulation with Action Manifold Learning [[arxiv]](https://arxiv.org/abs/2602.11236) [[hjfy]](https://hjfy.top/arxiv/2602.11236) `End-to-end`
  - 概览：提出ABot-M0通用机器人操作VLA基础模型，以统一数据整理和动作流形学习整合多本体轨迹，并用DiT直接预测连续可行动作序列。

- **[2026/02][ arXiv 2026 - 具身导航VLA基础模型与真机部署 - ABot-N0 ]** ABot-N0: Technical Report on the VLA Foundation Model for Versatile Embodied Navigation [[arxiv]](https://arxiv.org/abs/2602.11598) [[hjfy]](https://hjfy.top/arxiv/2602.11598) `Diffusion`
  - 概览：提出ABot-N0统一导航VLA基础模型，以LLM认知模块和流匹配动作专家覆盖点目标、物体目标、指令跟随、兴趣点与跟人导航，并结合拓扑记忆执行长程任务。

- **[2026/01][ EAAI 2026 - 大规模多模态具身机器人综述 ]** Large-scale multimodal model based embodied intelligent robots: A survey [[doi]](https://doi.org/10.1016/j.engappai.2025.112991) `Survey`
  - 概览：构建大规模多模态模型驱动具身机器人的感知、推理、执行与协作框架，综述工业和医疗应用，并分析安全、伦理及仿真到现实迁移挑战。

- **[2025/12][ arXiv 2025 - 模块构建、发展历程与核心挑战 ]** An Anatomy of Vision-Language-Action Models: From Modules to Milestones and Challenges [[arxiv]](https://arxiv.org/abs/2512.11362) [[hjfy]](https://hjfy.top/arxiv/2512.11362) `Survey`
  - 概览：综述视觉语言动作模型的模块组成与技术演进，并围绕表征、执行、泛化、安全及数据与评测五类挑战组织代表方法和研究方向。

- **[2025/11][ arXiv 2025 - 四足移动机器人推理增强VLA - MobileVLA-R1 ]** MobileVLA-R1: Reinforcing Vision-Language-Action for Mobile Robots [[arxiv]](https://arxiv.org/abs/2511.17889) [[hjfy]](https://hjfy.top/arxiv/2511.17889) [[github]](https://github.com/AIGeeksGroup/MobileVLA-R1) [[project]](https://aigeeksgroup.github.io/MobileVLA-R1/) `RL`
  - 概览：构建多粒度思维链数据集MobileVLA-CoT，采用监督CoT对齐与GRPO强化学习两阶段训练，统一四足机器人的显式推理与连续控制并在真机上验证泛化能力。

- **[2025/10][ arXiv 2025 - 能力调制分层导航VLA - VAMOS ]** VAMOS: A Hierarchical Vision-Language-Action Model for Capability-Modulated and Steerable Navigation [[arxiv]](https://arxiv.org/abs/2510.20818) [[hjfy]](https://hjfy.top/arxiv/2510.20818) `Hierarchical`
  - 概览：提出分层VLA导航模型VAMOS，将开放世界数据训练的通用语义规划器与仿真习得的具身可供性模型解耦，在轮式与四足机器人上实现能力调制、语言可引导且高可靠的室内外导航。

- **[2025/10][ arXiv 2025 - 通用具身VLA基础模型 - MM-Nav ]** MM-Nav: Multi-View VLA Model for Robust Visual Navigation via Multi-Expert Learning [[arxiv]](https://arxiv.org/abs/2510.03142) [[hjfy]](https://hjfy.top/arxiv/2510.03142) [[project]](https://pku-epic.github.io/MM-Nav-Web/) `RL` `VLA` `Pretraining`
  - 概览：设计包含两个阶段的训练过程：首先利用从RL专家那里收集的大规模离线数据集对VLA模型进行初始微调；然后通过在线教师-学生训练迭代，以能力平衡的方式对VLA模型进行进一步的精细化调整。

- **[2025/10][ arXiv 2025 - 空间推理与记忆增强视觉跟踪 - TrackVLA++ ]** TrackVLA++: Unleashing Reasoning and Memory Capabilities in VLA Models for Embodied Visual Tracking [[arxiv]](https://arxiv.org/abs/2510.07134) [[hjfy]](https://hjfy.top/arxiv/2510.07134) `Zero-Shot`
  - 概览：提出TrackVLA++，以Polar-CoT将目标相对位置编码为紧凑极坐标推理令牌，并用Target Identification Memory按空间先验门控更新长期目标表征，以在遮挡和相似干扰物下保持时空一致跟踪。

- **[2025/09][ ICLR 2026 - 跨具身导航基础模型 - NavFoM ]** Embodied Navigation Foundation Model [[arxiv]](https://arxiv.org/abs/2509.12129) [[hjfy]](https://hjfy.top/arxiv/2509.12129) [[project]](https://pku-epic.github.io/NavFoM-Web/) `End-to-end`
  - 概览：提出了一个跨智能体（四足、无人机、轮式、汽车）和跨任务的具身导航基础模型，在800万导航数据上训练，通过创新性的时空视角指示Token（TVI），无需微调即可统一处理零样本泛化导航。

- **[2025/09][ arXiv 2025 - 全模态机器人导航VLA - OmniVLA ]** OmniVLA: An Omni-Modal Vision-Language-Action Model for Robot Navigation [[arxiv]](https://arxiv.org/abs/2509.19480) [[hjfy]](https://hjfy.top/arxiv/2509.19480) `VLA`
  - 概览：提出OmniVLA，以统一模型接收二维位姿、第一人称目标图像、自然语言及其组合，学习跨目标模态的机器人导航策略并支持真实平台迁移。

- **[2025/08][ arXiv 2025 - 通用具身VLA基础模型 - NaviMaster ]** NaviMaster: Learning a Unified Policy for GUI and Embodied Navigation Tasks [[arxiv]](https://arxiv.org/abs/2508.02046) [[hjfy]](https://hjfy.top/arxiv/2508.02046) `RL`
  - 概览：提出NaviMaster，将GUI导航与具身导航统一建模为MDP，使用同一视觉目标轨迹采集流程生成两类数据，并通过混合强化学习和距离感知奖励训练共享策略。

- **[2025/08][ arXiv 2025 - 通用具身VLA基础模型 - $\mathcal{P}^3$ ]** $\mathcal{P}^3$: Toward Versatile Embodied Agents [[arxiv]](https://arxiv.org/abs/2508.07033) [[hjfy]](https://hjfy.top/arxiv/2508.07033) `Multi-task` `Transformer`
  - 概览：提出P3统一具身智能体框架，使智能体主动感知任务相关环境变化、即插即用地调用无需反馈的工具，并依据任务优先级与依赖关系动态安排多任务执行顺序。

- **[2025/08][ arXiv 2025 - 通用具身VLA基础模型 - ODYSSEY ]** ODYSSEY: Open-World Quadrupeds Exploration and Manipulation for Long-Horizon Tasks [[arxiv]](https://arxiv.org/abs/2508.08240) [[hjfy]](https://hjfy.top/arxiv/2508.08240) [[project]](https://kaijwang.github.io/odyssey.github.io/) `Hierarchical` `Sim-to-Real` `Planning`
  - 概览：提出面向带机械臂四足机器人的ODYSSEY移动操作框架，以视觉语言模型分层分解长时指令、全身控制策略协调机身与末端执行器，并配套室内外长期移动操作基准。

- **[2025/08][ arXiv 2025 - 通用具身VLA基础模型 - AI ]** Large Model Empowered Embodied AI: A Survey on Decision-Making and Embodied Learning [[arxiv]](https://arxiv.org/abs/2508.10399) [[hjfy]](https://hjfy.top/arxiv/2508.10399) `Survey` `World Model` `RL`
  - 概览：综述大模型赋能的具身决策与学习：分别比较分层和端到端决策范式、模仿学习与强化学习方法，并梳理世界模型在规划、反馈和具身学习中的作用。

- **[2025/08][ arXiv 2025 - 通用具身VLA基础模型 - CAST ]** CAST: Counterfactual Labels Improve Instruction Following in Vision-Language-Action Models [[arxiv]](https://arxiv.org/abs/2508.13446) [[hjfy]](https://hjfy.top/arxiv/2508.13446) [[project]](https://cast-vla.github.io/) [[github]](https://github.com/catglossop/CAST) `Zero-Shot` `VLA` `VLM`
  - 概览：提出CAST数据增强方法，通过利用视觉语言模型（VLM）生成反事实的语言和行动标签，以增加机器人数据集中语言的多样性和粒度。

- **[2025/08][ arXiv 2025 - 具身操作VLA模型综述 ]** Survey of Vision-Language-Action Models for Embodied Manipulation [[arxiv]](https://arxiv.org/abs/2508.15201) [[hjfy]](https://hjfy.top/arxiv/2508.15201) `Survey`
  - 概览：从发展历程、模型结构、训练数据、预训练、后训练和评估五个维度系统综述具身操作VLA，并分析通用控制模型落地开放物理环境的关键挑战。

- **[2025/07][ arXiv 2025 - 通用具身VLA基础模型 - Foundation Model Driven Robotics ]** Foundation Model Driven Robotics: A Comprehensive Review [[arxiv]](https://arxiv.org/abs/2507.10087) [[hjfy]](https://hjfy.top/arxiv/2507.10087) `Survey` `Sim-to-Real` `VLM`
  - 概览：系统综述基础模型驱动机器人研究，按仿真驱动设计、开放世界执行、仿真到现实迁移与自适应机器人四类组织方法，并比较系统集成、落地约束与安全问题。

- **[2025/07][ arXiv 2025 - 跨具身导航基础模型 - S2E ]** From Seeing to Experiencing: Scaling Navigation Foundation Models with Reinforcement Learning [[arxiv]](https://arxiv.org/abs/2507.22028) [[hjfy]](https://hjfy.top/arxiv/2507.22028) [[project]](https://vail-ucla.github.io/S2E) [[github]](https://github.com/metadriverse/S2E) `Foundation Model` `RL` `Pretraining`
  - 概览：提出S2E导航基础模型扩展框架：离线阶段用锚点引导分布匹配从真实视频学习多样运动，在线阶段以残差注意力模块在仿真中强化学习反应式行为并保持预训练知识；同时构建NavBench-GS评测跨环境与跨具身泛化及安全性。

- **[2025/06][ CVPR 2026 - 通用具身导航大模型 - OctoNav ]** OctoNav: Towards Generalist Embodied Navigation [[arxiv]](https://arxiv.org/abs/2506.09839) [[hjfy]](https://hjfy.top/arxiv/2506.09839) `End-to-end`
  - 概览：探索通用具身导航的统一框架，旨在构建一个跨任务、跨智能体（包含无人机、轮式机器人等）的导航基础模型底座，大幅提升智能体在复杂物理环境中的零样本泛化导航能力。

- **[2025/06][ arXiv 2025 - VLA测试时缩放定律 - RoboMonkey ]** RoboMonkey: Scaling Test-Time Sampling and Verification for Vision-Language-Action Models [[arxiv]](https://arxiv.org/abs/2506.17811) [[hjfy]](https://hjfy.top/arxiv/2506.17811) [[project]](https://robomonkey-vla.github.io/) `End-to-end`
  - 概览：探索了VLA的"测试时计算缩放定律（Test-time Scaling）"，提出RoboMonkey框架，在部署时通过动作的高斯扰动多次采样、投票并配合VLM验证器选择最优动作，大幅提升机器人OOD泛化性。

- **[2025/06][ arXiv 2025 - 自回归动作世界模型 - WorldVLA ]** WorldVLA: Towards Autoregressive Action World Model [[arxiv]](https://arxiv.org/abs/2506.21539) [[hjfy]](https://hjfy.top/arxiv/2506.21539) `World Model`
  - 概览：朝着自回归动作世界模型的方向探索，将状态转移预测与视觉-语言-动作策略统一在一个自回归生成框架下，提升机器人在复杂场景下的闭环动作生成能力。

- **[2025/06][ arXiv 2025 - 通用具身VLA基础模型 - FindingDory ]** FindingDory: A Benchmark to Evaluate Memory in Embodied Agents [[arxiv]](https://arxiv.org/abs/2506.15635) [[hjfy]](https://hjfy.top/arxiv/2506.15635) [[project]](https://FindingDory-benchmark.github.io/) `Benchmark` `Memory` `VLM`
  - 概览：构建FindingDory长期具身记忆基准，在Habitat中设置60项可程序化延长的导航与操作任务，联合检验智能体从多日视觉历史中召回相关信息并据此执行动作的能力。

- **[2025/05][ arXiv 2025 - Sim-to-Real导航扩散策略 - NavDP ]** NavDP: Learning Sim-to-Real Navigation Diffusion Policy with Privileged Information Guidance [[arxiv]](https://arxiv.org/abs/2505.08712) [[hjfy]](https://hjfy.top/arxiv/2505.08712) [[github]](https://github.com/InternRobotics/NavDP) [[project]](https://wzcai99.github.io/navigation-diffusion-policy.github.io/) `Diffusion` `Transformer`
  - 概览：提出端到端导航扩散策略NavDP，基于RGB-D观测联合学习轨迹生成与批评值评估，利用仿真特权信息监督与3000余场景超百万米导航数据，实现跨具身零样本Sim-to-Real迁移。

- **[2025/05][ arXiv 2025 - 通用具身VLA基础模型 - Vision-Language-Action ]** Vision-Language-Action (VLA) Models: Concepts, Progress, Applications and Challenges [[arxiv]](https://arxiv.org/abs/2505.04769) [[hjfy]](https://hjfy.top/arxiv/2505.04769) `Agentic` `Hierarchical` `VLA`
  - 概览：架构设计总结：详细分析了VLA模型的架构设计，包括早期融合模型、双系统架构和自校正框架等，并探讨了这些架构如何平衡效率、模块化和鲁棒性。

- **[2025/05][ arXiv 2025 - 通用具身VLA基础模型 - Toward Embodied AGI ]** Toward Embodied AGI: A Review of Embodied AI and the Road Ahead [[arxiv]](https://arxiv.org/abs/2505.14235) [[hjfy]](https://hjfy.top/arxiv/2505.14235) `Survey`
  - 概览：提出L3+机器人大脑的概念框架：包括模型架构和训练范式，旨在满足全模态处理、类人认知能力、实时响应和泛化能力等核心要求，为未来的研究和开发提供了技术展望。

- **[2025/05][ arXiv 2025 - 通用具身VLA基础模型 - TrackVLA ]** TrackVLA: Embodied Visual Tracking in the Wild [[arxiv]](https://arxiv.org/abs/2505.23189) [[hjfy]](https://hjfy.top/arxiv/2505.23189) [[project]](https://pku-epic.github.io/TrackVLA-web/) [[github]](https://github.com/wsakobe/TrackVLA) `Diffusion` `Zero-Shot` `VLA`
  - 概览：构建一个大规模数据集，包含855K具身视觉跟踪样本和855K开放世界识别样本，用于训练TrackVLA，使其学习视觉跟踪和目标识别之间的协同作用。

- **[2025/04][ arXiv 2025 - 通用具身VLA基础模型 - Embodied-R ]** Embodied-R: Collaborative Framework for Activating Embodied Spatial Reasoning in Foundation Models via Reinforcement Learning [[arxiv]](https://arxiv.org/abs/2504.12680) [[hjfy]](https://hjfy.top/arxiv/2504.12680) [[project]](https://embodiedcity.github.io/Embodied-R/) [[github]](https://github.com/EmbodiedCity/Embodied-R.code) `RL` `Pretraining` `VLM`
  - 概览：提出Embodied-R协同框架，以大型视觉语言模型负责视频感知、小型语言模型负责推理，并用兼顾思考—答案逻辑一致性的奖励进行强化学习，学习具身空间慢思考能力。

- **[2025/03][ CVPR 2025 - 通用零样本目标导航 - UniGoal ]** UniGoal: Towards Universal Zero-shot Goal-oriented Navigation [[arxiv]](https://arxiv.org/abs/2503.10630) [[hjfy]](https://hjfy.top/arxiv/2503.10630) `Zero-Shot`
  - 概览：提出通用零样本目标导航统一框架，利用统一图表示将物体类别、实例图像和文本描述三类目标统一建模，结合在线场景图维护与LLM图匹配推理，单一模型在三种导航任务上均达到SOTA零样本性能。

- **[2025/03][ arXiv 2025 - 通用具身VLA基础模型 - Embodied-Reasoner ]** Embodied-Reasoner: Synergizing Visual Search, Reasoning, and Action for Embodied Interactive Tasks [[arxiv]](https://arxiv.org/abs/2503.21696) [[hjfy]](https://hjfy.top/arxiv/2503.21696) [[project]](https://embodied-reasoner.github.io/) [[github]](https://github.com/zwq2018/embodied_reasoner) `Agentic` `IL`
  - 概览：提出Embodied Reasoner，以9.3K条观察—思考—动作轨迹训练具身搜索模型，并依次采用模仿学习、拒绝采样自探索和反思调优，使模型在交互过程中联合执行空间推理、规划、验证与自我纠错。

- **[2025/02][ arXiv 2025 - 通用具身VLA基础模型 - EmbodiedBench ]** EmbodiedBench: Comprehensive Benchmarking Multi-modal Large Language Models for Vision-Driven Embodied Agents [[arxiv]](https://arxiv.org/abs/2502.09560) [[hjfy]](https://hjfy.top/arxiv/2502.09560) [[project]](https://EmbodiedBench.github.io/) [[github]](https://github.com/EmbodiedBench/EmbodiedBench) `Benchmark` `Transformer`
  - 概览：提出全面的基准测试套件EmbodiedBench，用于评估基于多模态大语言模型（MLLM）的具身智能体在不同动作级别和细粒度能力导向子集上的表现。

- **[2025/02][ arXiv 2025 - 通用具身VLA基础模型 - Magma ]** Magma: A Foundation Model for Multimodal AI Agents [[arxiv]](https://arxiv.org/abs/2502.13130) [[hjfy]](https://hjfy.top/arxiv/2502.13130) [[project]](https://microsoft.github.io/Magma/) [[github]](https://github.com/microsoft/Magma) `Agentic` `Pretraining` `Planning`
  - 概览：提出Set-of-Mark（SoM）和Trace-of-Mark（ToM）来增强模型的时空智能，以便进行动作对齐和规划，使得Magma能够在大量异构数据集上进行有效预训练。

- **[2025/02][ arXiv 2025 - 通用具身VLA基础模型 - AI ]** Towards Robust and Secure Embodied AI: A Survey on Vulnerabilities and Attacks [[arxiv]](https://arxiv.org/abs/2502.13175) [[hjfy]](https://hjfy.top/arxiv/2502.13175) `Survey` `VLM`
  - 概览：系统综述具身AI的鲁棒性与安全问题，按外源攻击和内源故障分类漏洞，并梳理传感欺骗、对抗攻击、越狱与指令误解对感知、决策、任务规划和具身交互的影响及对应防护。

- **[2025/02][ arXiv 2025 - 通用具身VLA基础模型 ]** Exploring Embodied Multimodal Large Models: Development, Datasets, and Future Directions [[arxiv]](https://arxiv.org/abs/2502.15336) [[hjfy]](https://hjfy.top/arxiv/2502.15336) `Navigation` `Transformer`
  - 概览：综述具身多模态大模型的发展脉络，按具身感知、导航、交互和仿真组织模型与训练数据，并归纳可扩展性、泛化和实时决策等共性挑战。

- **[2025/X][ CVPR 2025 - 因果引导扩散具身对话定位 - CGD ]** Towards Precise Embodied Dialogue Localization via Causality Guided Diffusion [[cvf]](https://openaccess.thecvf.com/content/CVPR2025/papers/Wang_Towards_Precise_Embodied_Dialogue_Localization_via_Causality_Guided_Diffusion_CVPR_2025_paper.pdf) `Diffusion`
  - 概览：摒弃传统将坐标定位视为受限于分辨率的"热力图生成"思路，利用因果引导的扩散模型（CGD）直接预测连续坐标分布，并通过前门和后门干预机制有效消除了数据集本身隐藏的混杂偏见。

- **[2024/12][ arXiv 2024 - 通用具身VLA基础模型 - InfiniteWorld ]** InfiniteWorld: A Unified Scalable Simulation Framework for General Visual-Language Robot Interaction [[arxiv]](https://arxiv.org/abs/2412.05789) [[hjfy]](https://hjfy.top/arxiv/2412.05789) [[github]](https://github.com/pzhren/InfiniteWorld) `GSM`
  - 概览：发布基于Isaac Sim的统一仿真框架InfiniteWorld，整合生成式三维资产构建、Real2Sim、自动标注和统一资产处理，并提供场景图协作探索等四类机器人交互基准。

- **[2024/10][ arXiv 2024 - 真实城市环境具身Agent基准 - EmbodiedCity ]** EmbodiedCity: A Benchmark Platform for Embodied Agent in Real-world City Environment [[arxiv]](https://arxiv.org/abs/2410.09604) [[hjfy]](https://hjfy.top/arxiv/2410.09604) [[github]](https://github.com/tsinghua-fib-lab/EmbodiedCity) `Benchmark`
  - 概览：提出真实世界城市级具身智能基准平台EmbodiedCity，覆盖街景导航、交互和长距离目标搜索等任务，为跨具身（包括无人机）的城市级Agent评测提供统一框架。

- **[2024/09][ arXiv 2024 - 通用具身VLA基础模型 - Embodied-RAG ]** Embodied-RAG: General Non-parametric Embodied Memory for Retrieval and Generation [[arxiv]](https://arxiv.org/abs/2409.18313) [[hjfy]](https://hjfy.top/arxiv/2409.18313) [[project]](https://quanting-xie.github.io/Embodied-RAG-web/) `Hierarchical` `Memory` `Retrieval`
  - 概览：将检索增强生成（RAG）技术扩展到具身设置中，通过引入非参数记忆系统，展示了如何在具身智能体中实现更高级别的语义记忆和检索能力。

- **[2024/08][ arXiv 2024 - 通用具身VLA基础模型 - EARBench ]** EARBench: Towards Evaluating Physical Risk Awareness for Task Planning of Foundation Model-based Embodied AI Agents [[arxiv]](https://arxiv.org/abs/2408.04449) [[hjfy]](https://hjfy.top/arxiv/2408.04449) [[github]](https://github.com/zihao-ai/EARBench) `Agentic`
  - 概览：提出自动化物理风险评估框架EARBench，用于评估基于基础模型的具身人工智能（EAI）智能体在任务规划中的物理风险意识，包括安全指南生成、风险场景创建、任务规划和系统评估等步骤。

- **[2024/08][ arXiv 2024 - 通用具身VLA基础模型 - All Robots in One ]** All Robots in One: A New Standard and Unified Dataset for Versatile, General-Purpose Embodied Agents [[arxiv]](https://arxiv.org/abs/2408.10899) [[hjfy]](https://hjfy.top/arxiv/2408.10899) [[project]](https://imaei.github.io/project_pages/ario/) `Benchmark`
  - 概览：提出统一具身数据标准ARIO，将真实与仿真数据、不同传感模态和机器人任务映射为一致格式；据此汇集约300万回合、258个数据系列和321,064项任务，形成可联合训练的ARIO数据集。

- **[2024/07][ arXiv 2024 - 通用具身VLA基础模型 - GRUtopia ]** GRUtopia: Dream General Robots in a City at Scale [[arxiv]](https://arxiv.org/abs/2407.10943) [[hjfy]](https://hjfy.top/arxiv/2407.10943) [[github]](https://github.com/OpenRobotLab/GRUtopia) `Sim-to-Real`
  - 概览：发布城市规模具身仿真平台GRUtopia：GRScenes提供10万套可组合的交互场景，GRResidents以大语言模型驱动NPC完成社交、任务生成与分派，GRBench则统一评测目标导航、社交导航和移动操作。

- **[2024/02][ arXiv 2024 - 迭代视觉提示激发VLM可执行知识 - PIVOT ]** PIVOT: Iterative Visual Prompting Elicits Actionable Knowledge for VLMs [[arxiv]](https://arxiv.org/abs/2402.07872) [[hjfy]](https://hjfy.top/arxiv/2402.07872) [[project]](https://pivot-prompt.github.io/) `Zero-Shot`
  - 概览：提出迭代视觉提示框架PIVOT，通过在图像上叠加候选动作的可视化标注让VLM直接选择具身动作，无需微调即可将预训练VLM转化为零样本机器人策略，在导航和操作任务上效果显著。

- **[2024/02][ ICML 2024 - VLM偏好反馈自动奖励生成 - RL-VLM-F ]** RL-VLM-F: Reinforcement Learning from Vision Language Foundation Model Feedback [[arxiv]](https://arxiv.org/abs/2402.03681) [[hjfy]](https://hjfy.top/arxiv/2402.03681) [[github]](https://github.com/yufeiwang63/RL-VLM-F) [[project]](https://rlvlmf2024.github.io/) `RL` `GPT-4V`
  - 概览：提出仅凭任务目标文本与视觉观测自动生成奖励函数的方法，让VLM对成对图像观测给出偏好标签并从中学习奖励，避免直接输出噪声奖励分数，为强化学习免去人工奖励工程。

- **[2023/11][ arXiv 2023 - 通用具身VLA基础模型 - See and Think ]** See and Think: Embodied Agent in Virtual Environment [[arxiv]](https://arxiv.org/abs/2311.15209) [[hjfy]](https://hjfy.top/arxiv/2311.15209) `Benchmark` `Retrieval`
  - 概览：提出虚拟环境中的具身智能体框架STEVE，结合了视觉感知、语言指令和代码动作三个关键组件，能够在开放世界环境中实现智能行为和适应性。

### 2. World Models

涵盖结合物理控制动作的未来场景生成与环境预测。

- **[2026/06][ arXiv 2026 - 稀疏关键帧插值具身世界模型 - SKIP ]** SKIP: Sparse Keyframe Interpolation Paradigm for Efficient Embodied World Models [[arxiv]](https://arxiv.org/abs/2606.00664) [[hjfy]](https://hjfy.top/arxiv/2606.00664) `World Model`
  - 概览：提出SKIP稀疏关键帧插值世界模型，先识别并生成接近、接触、抓取和释放等任务关键帧，再由动作条件插值器补全区间，以降低长时域机器人视频推演成本。

- **[2026/06][ arXiv 2026 - 非对称潜在世界动作统一视觉导航 - WAM-Nav ]** WAM-Nav: Asymmetric Latent World-Action Modeling for Unified Visual Navigation [[arxiv]](https://arxiv.org/abs/2606.04907) [[hjfy]](https://hjfy.top/arxiv/2606.04907) `World Model`
  - 概览：提出WAM-Nav非对称潜在世界动作模型，通过共享视觉表征联合学习未来预测与动作生成，实现统一的目标条件视觉导航。

- **[2026/06][ arXiv 2026 - 端到端动作生成导航世界模型 - NavWAM ]** NavWAM: A Navigation World Action Model for Goal-Conditioned Visual Navigation [[arxiv]](https://arxiv.org/abs/2606.13494) [[hjfy]](https://hjfy.top/arxiv/2606.13494) `World Model`
  - 概览：提出NavWAM扩散Transformer策略，将未来观测、目标进度价值和动作块表示在共享潜在序列中联合学习，使视觉未来预测直接参与闭环动作输出；模型通过仿真预训练后适配真实机器人。

- **[2026/06][ arXiv 2026 - 统一世界模型、凭视觉前瞻实现远见规划 - NavWM ]** NavWM: A Unified Navigation World Model for Foresight-Driven Planning [[arxiv]](https://arxiv.org/abs/2606.24101) [[hjfy]](https://hjfy.top/arxiv/2606.24101) `World Model`
  - 概览：提出NavWM统一导航世界模型，以潜在世界词元压缩几何与语义先验，通过锚点式多模态轨迹预测生成多样候选动作，再让可控视觉生成提供未来观测并在闭环中评估、选择路径。

- **[2026/06][ arXiv 2026 - 统一世界-动作建模与未来预测 - FutureNav ]** FutureNav: Unified World-Action Modeling for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2606.30367) [[hjfy]](https://hjfy.top/arxiv/2606.30367) `World Model`
  - 概览：提出FutureNav统一世界—动作建模框架，将文本、视觉和空间特征共同输入VLM，并联合优化动作策略、前向动力学、逆动力学和未来空间状态生成四项目标，在预测导航动作的同时显式学习状态转移。

- **[2026/06][ ECCV 2026 - 时序经验MoE端到端驾驶 - TEX-Drive ]** TEX-Drive: Temporal Perception Meets Experience-Guided Mixture-of-Experts for End-to-End Autonomous Driving [[project]](https://gr.xjtu.edu.cn/hsun/zh_CN/article/280386/content/37612.htm) `MoE`
  - 概览：提出关键帧引导的时序感知单元和经验驱动MoE规划器，使历史帧筛选与专家路由双向耦合，在端到端自动驾驶中兼顾长时决策稳定性和可解释性。

- **[2026/05][ arXiv 2026 - 策略・模拟器・视频生成全覆盖 ]** World Model for Robot Learning: A Comprehensive Survey [[arxiv]](https://arxiv.org/abs/2605.00080) [[hjfy]](https://hjfy.top/arxiv/2605.00080) `Survey`
  - 概览：从机器人学习视角综述世界模型，系统分析其与策略学习、规划、仿真、评估和数据生成的耦合方式，并整理导航、自动驾驶相关数据集与评测协议。

- **[2026/05][ arXiv 2026 - 世界动作模型框架与研究前沿 - World Action Models ]** World Action Models: The Next Frontier in Embodied AI [[arxiv]](https://arxiv.org/abs/2605.12090) [[hjfy]](https://hjfy.top/arxiv/2605.12090) `World Model`
  - 概览：系统定义世界动作模型，将其概括为联合预测未来状态与动作的具身基础模型，并按级联式与联合式架构、生成模态、条件机制和动作解码方式梳理现有方法。

- **[2026/04][ arXiv 2026 - 生成式世界模型引导VLN轨迹预测 - WorldMAP ]** WorldMAP: Bootstrapping Vision-Language Navigation Trajectory Prediction with Generative World Models [[arxiv]](https://arxiv.org/abs/2604.07957) [[hjfy]](https://hjfy.top/arxiv/2604.07957) `World Model`
  - 概览：提出师生框架WorldMAP，教师利用世界模型生成的未来视图构建持久语义-空间记忆并产生规划派生监督信号，引导学生仅凭单帧第一视角观测预测可靠的导航轨迹。

- **[2026/04][ arXiv 2026 - 几何感知统一生成与规划世界动作模型 - DriveDreamer-Policy ]** DriveDreamer-Policy: A Geometry-Grounded World-Action Model for Unified Generation and Planning [[arxiv]](https://arxiv.org/abs/2604.01765) [[hjfy]](https://hjfy.top/arxiv/2604.01765) [[github]](https://github.com/youngzhou1999/DriveDreamer-Policy) [[project]](https://drivedreamer-policy.github.io/) `World Model`
  - 概览：DriveDreamer系列新作，将深度生成、未来视频生成与运动规划统一于单一模块化架构，借助几何感知表征同时提升生成质量与驾驶规划性能。

- **[2026/03][ arXiv 2026 - 流式VLN语义空间融合潜在预测 - PROSPECT ]** PROSPECT: Unified Streaming Vision-Language Navigation via Semantic--Spatial Fusion and Latent Predictive Representation [[arxiv]](https://arxiv.org/abs/2603.03739) [[hjfy]](https://hjfy.top/arxiv/2603.03739) `End-to-end` `CUT3R+SigLIP`
  - 概览：提出统一流式VLN智能体PROSPECT，将CUT3R流式3D空间特征与SigLIP语义特征交叉注意力融合，并用可学习流查询token预测下一步2D/3D潜在特征作为自监督，强化对环境动态与空间结构的预测建模。

- **[2026/03][ arXiv 2026 - 免测试时未来想象的世界动作模型 - Fast-WAM ]** Fast-WAM: Do World Action Models Need Test-time Future Imagination? [[arxiv]](https://arxiv.org/abs/2603.16666) [[hjfy]](https://hjfy.top/arxiv/2603.16666) [[project]](https://yuantianyuan01.github.io/FastWAM/) `World Model`
  - 概览：发现世界动作模型的增益主要源于训练期视频协同建模而非测试时未来想象，据此提出推理时省去未来生成的Fast-WAM，以约4倍加速在LIBERO与RoboTwin上保持相当性能。

- **[2026/03][ arXiv 2026 - 以动作为中心的高效世界动作模型 - GigaWorld-Policy ]** GigaWorld-Policy: An Efficient Action-Centered World--Action Model [[arxiv]](https://arxiv.org/abs/2603.17240) [[hjfy]](https://hjfy.top/arxiv/2603.17240) `World Model`
  - 概览：提出以动作为中心的世界动作模型，将未来动作序列预测置于核心并可选生成对应视频，较"想象再执行"范式推理提速约9倍、任务成功率提升7%。

- **[2026/03][ arXiv 2026 - 隐空间世界动作建模端到端自动驾驶 - Latent-WAM ]** Latent-WAM: Latent World Action Modeling for End-to-End Autonomous Driving [[arxiv]](https://arxiv.org/abs/2603.24581) [[hjfy]](https://hjfy.top/arxiv/2603.24581) `World Model`
  - 概览：提出空间感知压缩世界编码器与动态隐世界模型，在紧凑隐空间自回归预测未来世界状态并指导轨迹规划，以104M参数小模型在NAVSIM v2等基准取得SOTA。

- **[2026/03][ arXiv 2026 - 导航世界模型 - DreamToNav ]** DreamToNav: Generalizable Navigation for Robots via Generative Video Planning [[arxiv]](https://arxiv.org/abs/2603.06190) [[hjfy]](https://hjfy.top/arxiv/2603.06190) `World Model`
  - 概览：提出DreamToNav，先用Qwen2.5-VL把自然语言指令细化为视觉描述，再由Cosmos 2.5生成机器人执行视频，并以姿态估计、机器人检测和轨迹恢复从视频中提取可执行路径。

- **[2026/03][ arXiv 2026 - 导航世界模型 - RAE-NWM ]** RAE-NWM: Navigation World Model in Dense Visual Representation Space [[arxiv]](https://arxiv.org/abs/2603.09241) [[hjfy]](https://hjfy.top/arxiv/2603.09241) `World Model` `Diffusion` `Transformer`
  - 概览：提出导航世界模型RAE-NWM，在稠密DINOv2视觉表示空间中用条件扩散Transformer建模动作条件状态转移，并以时间门控模块调节生成过程中的动作注入强度。

- **[2026/03][ arXiv 2026 - 利用人类第一视角视频扩展开放世界具身导航 - ImagiNav ]** ImagiNav: Scalable Embodied Navigation via Generative Visual Prediction and Inverse Dynamics [[arxiv]](https://arxiv.org/abs/2603.13833) [[hjfy]](https://hjfy.top/arxiv/2603.13833) `World Model`
  - 概览：提出ImagiNav模块化导航框架：VLM先把指令分解为文本子目标，微调视频生成模型想象到达子目标的未来轨迹，再由逆动力学模型从生成视频提取轨迹交给低层控制器；训练数据由网络导航视频自动标注。

- **[2026/03][ arXiv 2026 - 基于动作条件世界模型的社交导航耦合预测与规划 - NavThinker ]** NavThinker: Action-Conditioned World Models for Coupled Prediction and Planning in Social Navigation [[arxiv]](https://arxiv.org/abs/2603.15359) [[hjfy]](https://hjfy.top/arxiv/2603.15359) `World Model`
  - 概览：提出NavThinker，在Depth Anything V2块特征空间自回归预测动作条件下的未来场景几何与行人运动，并把未来特征融合进当前观测表示、把预测行人轨迹用于社会奖励塑形，再以DD-PPO训练导航策略。

- **[2026/03][ arXiv 2026 - 策略引导世界模型语言导航规划 ]** Policy-Guided World Model Planning for Language-Conditioned Visual Navigation [[arxiv]](https://arxiv.org/abs/2603.25981) [[hjfy]](https://hjfy.top/arxiv/2603.25981) `World Model`
  - 概览：提出PiJEPA两阶段导航框架，先微调带冻结视觉编码器的Octo策略生成语言条件动作分布，再用该分布热启动MPPI，在独立JEPA世界模型的潜在空间中预测未来状态并优化动作序列。

- **[2026/02][ arXiv 2026 - 自由空间手势驱动第一视角交互世界模型 - Hand2World ]** Hand2World: Autoregressive Egocentric Interaction Generation via Free-Space Hand Gestures [[arxiv]](https://arxiv.org/abs/2602.09600) [[hjfy]](https://hjfy.top/arxiv/2602.09600) [[github]](https://github.com/NTUYWANG103/Hand2World) [[project]](https://hand2world.github.io/) `World Model` `Diffusion`
  - 概览：提出由单张场景图与自由空间手势驱动的自回归第一视角交互世界模型，以投影3D手网格实现遮挡不变控制、以逐像素Plücker射线解耦头部与手部运动，并将双向扩散模型蒸馏为支持任意长度生成的因果模型。

- **[2026/02][ arXiv 2026 - 世界动作模型即零样本策略 - DreamZero ]** World Action Models are Zero-shot Policies [[arxiv]](https://arxiv.org/abs/2602.15922) [[hjfy]](https://hjfy.top/arxiv/2602.15922) [[project]](https://dreamzero0.github.io/) `World Model` `Video Diffusion 14B`
  - 概览：提出基于预训练视频扩散骨干的世界动作模型DreamZero，联合建模视频与动作以从异构机器人数据学习物理动态，真机新任务泛化较SOTA VLA提升逾2倍，并使14B模型实现7Hz实时闭环控制。

- **[2026/02][ arXiv 2026 - 空间AI智能体与世界模型综述 ]** From Perception to Action: Spatial AI Agents and World Models [[arxiv]](https://arxiv.org/abs/2602.01644) [[hjfy]](https://hjfy.top/arxiv/2602.01644) `World Model`
  - 概览：综述两千余篇空间智能研究，以智能体能力、空间任务和空间尺度构建三轴分类法，并区分几何与物理约束的空间落地和图文关联的符号落地；进一步归纳层次记忆、GNN—LLM融合及世界模型在长时空间任务中的作用。

- **[2026/02][ arXiv 2026 - 稀疏视频超视野视觉语言导航 - SparseVideoNav ]** Sparse Video Generation Propels Real-World Beyond-the-View Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2602.05827) [[hjfy]](https://hjfy.top/arxiv/2602.05827) `World Model`
  - 概览：提出SparseVideoNav超视野视觉语言导航方法，以视频生成模型预测20秒稀疏未来观测并从中解码轨迹，在保持长时域视觉规划的同时实现亚秒级推理。

- **[2026/01][ arXiv 2026 - 机器人视频生成与具身世界模型综述 ]** Video Generation Models in Robotics -- Applications, Research Challenges, Future Directions [[arxiv]](https://arxiv.org/abs/2601.07823) [[hjfy]](https://hjfy.top/arxiv/2601.07823) `Survey` `World Model`
  - 概览：系统梳理视频生成模型作为具身世界模型在机器人数据生成、模仿学习、动力学与奖励建模、视觉规划及策略评估中的应用，并总结物理幻觉、指令跟随、安全性与计算成本等可信部署挑战。

- **[2026/01][ arXiv 2026 - 具身世界模型的综合性评估图灵测试 ]** Wow, wo, val! A Comprehensive Embodied World Model Evaluation Turing Test [[arxiv]](https://arxiv.org/abs/2601.04137) [[hjfy]](https://hjfy.top/arxiv/2601.04137) `Benchmark`
  - 概览：提出WoW-World-Eval具身世界模型评测，基于609条机器人操作数据覆盖感知、规划、预测、泛化和执行五种能力，以22项指标并结合人类偏好相关性评价生成质量，同时用逆动力学模型检验生成视频在真实执行中的可用性。

- **[2026/01][ TechRxiv 2026 - 专家到通才世界模型综述 ]** From Specialist to Generalist: A Comprehensive Survey on World Models [[doi]](https://doi.org/10.36227/techrxiv.176800434.49068726/v1) `World Model`
  - 概览：从专家模型与通才模型的视角梳理世界模型由显式物理建模到数据驱动学习的谱系，分析精度、泛化和长时预测之间的权衡及未来融合方向。

- **[2026/01][ TechRxiv 2026 - VLA智能体世界模型综述 ]** Towards Generalist Embodied AI: A Survey on World Models for VLA Agents [[doi]](https://doi.org/10.36227/techrxiv.176948355.54623875/v1) `World Model`
  - 概览：将VLA世界模型归纳为世界规划器、世界动作模型、世界合成器和世界模拟器四类，系统比较基础模型、数据与评估生态，并讨论物理一致性和泛化问题。

- **[2026/X][ ICLR 2026 - DroneDreamer ]** Multi-View Low-Altitude World Model with Adaptive Control [[openreview]](https://openreview.net/forum?id=eDyMFksVCl) [[github]](https://github.com/Myd-tech/dronedreamer) `World Model`
  - 概览：首个聚焦于"低空飞行"的生成式世界模型（LAWM）。引入自适应视角控制机制与图像风格域适应技术，仅通过单一前视条件输入即可生成高度一致的无人机环视飞行预测视频。

- **[2025/12][ arXiv 2025 - 视觉语言世界模型导航预测 - NavForesee ]** NavForesee: A Unified Vision-Language World Model for Hierarchical Planning and Dual-Horizon Navigation Prediction [[arxiv]](https://arxiv.org/abs/2512.01550) [[hjfy]](https://hjfy.top/arxiv/2512.01550) `World Model`
  - 概览：提出了一种统一的视觉语言世界模型，将大语言模型的高级分层规划与世界模型的"双层视野预测（短期动态与长期里程碑想象）"相结合，解决了智能体在未见环境长时程导航时容易迷失的问题。

- **[2025/12][ arXiv 2025 - 导航前瞻控制世界模型 - AstraNav-World ]** AstraNav-World: World Model for Foresight Control and Consistency [[arxiv]](https://arxiv.org/abs/2512.21714) [[hjfy]](https://hjfy.top/arxiv/2512.21714) `World Model`
  - 概览：提出统一导航世界模型AstraNav-World，将扩散视频生成与视觉语言策略通过双向约束耦合，同步预测未来视觉状态与动作序列，提升轨迹精度并实现免微调的零样本真机迁移。

- **[2025/12][ TechRxiv 2025 - 世界模型与VLA/VLN融合综述 ]** Integrating World Models into Vision Language Action and Navigation: A Comprehensive Survey [[doi]](https://doi.org/10.36227/techrxiv.176531987.77979037/v1) `World Model`
  - 概览：以世界模型与策略的耦合强度为主线，将其融入VLA/VLN的方式归纳为模块化、序列式和统一式三类架构，并比较其可解释性、规划能力与泛化取舍。

- **[2025/11][ arXiv 2025 - 多模态世界模型协同推理导航 - UNeMo ]** UNeMo: Collaborative Visual-Language Reasoning and Navigation via a Multimodal World Model [[arxiv]](https://arxiv.org/abs/2511.18845) [[hjfy]](https://hjfy.top/arxiv/2511.18845) `World Model`
  - 概览：提出视觉状态推理与导航决策协同优化框架UNeMo，其多模态世界模型以视觉、指令与动作为输入预测后续视觉状态，经分层预测-反馈机制与导航策略双向促进，在R2R与REVERIE未见场景上超越SOTA。

- **[2025/11][ arXiv 2025 - 导航世界模型 - Target-Bench ]** Target-Bench: Can Video World Models Achieve Mapless Path Planning with Semantic Targets? [[arxiv]](https://arxiv.org/abs/2511.17792) [[hjfy]](https://hjfy.top/arxiv/2511.17792) `World Model` `Planning`
  - 概览：构建Target-Bench，以450个机器人采集场景和47类语义目标评测视频世界模型；基准从生成视频中恢复度量尺度运动，并用五项指标衡量目标接近能力与方向一致性。

- **[2025/10][ ICLR 2026 - 世界模型放大数据缩放定律 - DriveVLA-W0 ]** DriveVLA-W0: World Models Amplify Data Scaling Law in Autonomous Driving [[arxiv]](https://arxiv.org/abs/2510.12796) [[hjfy]](https://hjfy.top/arxiv/2510.12796) `World Model`
  - 概览：揭示了仅靠低维动作监督训练VLA会导致"监督匮乏"，创新性引入世界模型预测未来画面作为密集自监督信号，证明了世界模型能像催化剂一样放大端到端自动驾驶模型的数据Scaling Law。

- **[2025/10][ arXiv 2025 - 导航世界模型 - Memory-Augmented ]** Towards Unified World Models for Visual Navigation via Memory-Augmented Planning and Foresight [[arxiv]](https://arxiv.org/abs/2510.08713) [[hjfy]](https://hjfy.top/arxiv/2510.08713) [[github]](https://github.com/F1y1113/UniWM) `World Model` `Zero-Shot` `Hierarchical`
  - 概览：提出端到端的交错训练策略，将规划器和世界模型的实例统一在一个自回归骨干网络中，联合优化离散化动作预测和视觉重建，紧密对齐想象与控制。

- **[2025/10][ arXiv 2025 - 导航世界模型 - AI ]** A Comprehensive Survey on World Models for Embodied AI [[arxiv]](https://arxiv.org/abs/2510.16732) [[hjfy]](https://hjfy.top/arxiv/2510.16732) `Survey` `World Model`
  - 概览：提出基于三个核心维度的分类体系，包括功能性（Functionality）、时间建模（Temporal Modeling）和空间表示（Spatial Representation），将现有的世界模型方法进行了系统分类，为后续研究提供了清晰的结构和方向。

- **[2025/09][ arXiv 2025 - 导航世界模型 - 3D and 4D World Modeling ]** 3D and 4D World Modeling: A Survey [[arxiv]](https://arxiv.org/abs/2509.07996) [[hjfy]](https://hjfy.top/arxiv/2509.07996) [[github]](https://github.com/worldbench/survey) `Survey` `World Model`
  - 概览：系统界定3D与4D世界模型，并按视频生成、占用生成和激光雷达生成三类表示梳理方法，同时汇总相应数据集、评测指标、应用与开放问题。

- **[2025/09][ arXiv 2025 - 导航世界模型 - Embodied AI ]** Embodied AI: From LLMs to World Models [[arxiv]](https://arxiv.org/abs/2509.20021) [[hjfy]](https://hjfy.top/arxiv/2509.20021) `World Model` `End-to-end` `Transformer`
  - 概览：综述具身AI从单模态到多模态的发展，分别梳理LLM通过语义推理与任务分解驱动具身认知、世界模型通过状态表征与未来预测支持物理交互的路径，并讨论二者联合架构。

- **[2025/07][ ACM MM 2025 - AirScape ]** AirScape: An Aerial Generative World Model with Motion Controllability [[arxiv]](https://arxiv.org/abs/2507.08885) [[hjfy]](https://hjfy.top/arxiv/2507.08885) `World Model`
  - 概览：赋予无人机"空间想象力"的世界模型基础工作。使用两阶段训练计划（动作意图注入+时空物理约束博弈对抗），输入当前视觉和飞行指令即可生成高度真实的未来视角切换视频。

- **[2025/07][ arXiv 2025 - 导航世界模型 - A Survey ]** A Survey: Learning Embodied Intelligence from Physical Simulators and World Models [[arxiv]](https://arxiv.org/abs/2507.00917) [[hjfy]](https://hjfy.top/arxiv/2507.00917) [[github]](https://github.com/NJU3DV-LoongGroup/Embodied-World-Models-Survey) `Survey` `World Model` `Sim-to-Real`
  - 概览：系统综述物理模拟器与世界模型在具身智能中的互补作用：前者提供可控训练和评测环境，后者学习环境内部表征以支持预测规划，并分析两者协同缩小仿真到现实差距的路径。

- **[2025/07][ arXiv 2025 - 导航世界模型 - DIVER ]** DIVER: Reinforced Diffusion Breaks Imitation Bottlenecks in End-to-End Autonomous Driving [[arxiv]](https://arxiv.org/abs/2507.04049) [[hjfy]](https://hjfy.top/arxiv/2507.04049) `World Model` `Diffusion` `RL`
  - 概览：引入了策略感知扩散生成器（PADG），通过条件扩散生成器结合地图元素和周围智能体信息，生成多种模式的轨迹，捕捉不同的驾驶风格。

- **[2025/06][ ICCV 2025 - VLN自进化世界模型 - NavMorph ]** NavMorph: A Self-Evolving World Model for Vision-and-Language Navigation in Continuous Environments [[arxiv]](https://arxiv.org/abs/2506.23468) [[hjfy]](https://hjfy.top/arxiv/2506.23468) `World Model`
  - 概览：提出自进化世界模型NavMorph，利用紧凑潜在表示建模环境动态，结合上下文进化记忆（Contextual Evolution Memory）实现在线自适应，在VLN-CE基准上显著提升导航性能。

- **[2025/03][ arXiv 2025 - 导航世界模型 - WMNav ]** WMNav: Integrating Vision-Language Models into World Models for Object Goal Navigation [[arxiv]](https://arxiv.org/abs/2503.02247) [[hjfy]](https://hjfy.top/arxiv/2503.02247) `World Model` `Zero-Shot` `Memory`
  - 概览：提出WMNav，以视觉语言世界模型预测候选动作的未来状态，并用在线Curiosity Value Map保存预测记忆；策略根据计划状态与真实观测的差异反馈决策，再以先广域探索、后精确定位的两阶段动作提议完成目标导航。

- **[2025/02][ arXiv 2025 - 导航世界模型 - EvolvingAgent ]** EvolvingAgent: Curriculum Self-evolving Agent with Continual World Model for Long-Horizon Tasks [[arxiv]](https://arxiv.org/abs/2502.05907) [[hjfy]](https://hjfy.top/arxiv/2502.05907) `World Model` `Agentic` `Memory`
  - 概览：提出自进化智能体EvolvingAgent，由经验驱动任务规划器、世界模型动作控制器和课程学习反思器组成闭环，自动选择多模态经验并持续更新世界知识。

- **[2024/12][ CVPR 2025 - 可控视频生成导航世界模型 - NWM ]** Navigation World Models [[arxiv]](https://arxiv.org/abs/2412.03572) [[hjfy]](https://hjfy.top/arxiv/2412.03572) [[github]](https://github.com/facebookresearch/nwm) [[project]](https://www.amirbar.net/nwm/) `World Model` `CDiT`
  - 概览：提出基于10亿参数条件扩散Transformer(CDiT)的可控视频生成导航世界模型NWM，通过模拟未来观测来规划并评估导航轨迹，还可凭单张图像想象未知环境中的可行轨迹。

- **[2024/11][ arXiv 2024 - 理解与预测世界模型综述 ]** Understanding World or Predicting Future? A Comprehensive Survey of World Models [[arxiv]](https://arxiv.org/abs/2411.14499) [[hjfy]](https://hjfy.top/arxiv/2411.14499) [[github]](https://github.com/tsinghua-fib-lab/World-Model) `World Model`
  - 概览：将世界模型归纳为理解世界的隐式表征与预测未来的动力学模型两类，比较其在机器人、自动驾驶和社会仿真中的目标、技术路线与发展趋势。

- **[2024/06][ ICLR 2025 - 潜在世界模型增强端到端驾驶 - LAW ]** Enhancing End-to-End Autonomous Driving with Latent World Model [[arxiv]](https://arxiv.org/abs/2406.08481) [[hjfy]](https://hjfy.top/arxiv/2406.08481) `World Model`
  - 概览：通过引入潜在空间的世界模型（Latent World Model）增强端到端自动驾驶能力，利用环境预测能力解决轨迹规划中的长时程推理与安全性问题。

- **[2023/11][ arXiv 2023 - 导航世界模型 - RoboGen ]** RoboGen: Towards Unleashing Infinite Data for Automated Robot Learning via Generative Simulation [[arxiv]](https://arxiv.org/abs/2311.01455) [[hjfy]](https://hjfy.top/arxiv/2311.01455) [[project]](https://robogen-ai.github.io/) [[github]](https://github.com/Genesis-Embodied-AI/RoboGen) `World Model` `RL`
  - 概览：介绍了生成式机器人智能体RoboGen，能够通过生成模拟环境自动学习多样化的机器人技能，利用现有的基础模型和生成模型的进展，通过生成多样化的任务、场景和训练监督来扩展机器人技能的学习规模。

- **[2022/12][ CVPR 2023 Best Paper - 规划导向端到端自动驾驶 - UniAD ]** Planning-oriented Autonomous Driving [[arxiv]](https://arxiv.org/abs/2212.10156) [[hjfy]](https://hjfy.top/arxiv/2212.10156) [[github]](https://github.com/opendrivelab/uniad) `End-to-end`
  - 概览：自动驾驶领域的里程碑工作（CVPR最佳论文），提出了首个以规划为导向的端到端自动驾驶统一框架UniAD，利用统一的Query设计将感知、预测和规划节点相连，显著提升安全性。

### 3. Multimodal Foundation Models

涵盖大语言模型定律、视觉特征提取底座及图文理解基座模型。

- **[2025/11][ arXiv 2025 - 视觉语言基础模型 - Qwen3-VL ]** Qwen3-VL Technical Report [[arxiv]](https://arxiv.org/abs/2511.21631) [[hjfy]](https://hjfy.top/arxiv/2511.21631) `MLLM`
  - 概览：视觉语言基座模型，在保持纯文本推理能力的同时原生支持最高256K Token的多模态上下文，可处理长视频信息抽取与多页复杂文档分析。

- **[2025/10][ arXiv 2025 - 多模态空间智能 - SpatialLadder ]** SpatialLadder: Progressive Training for Spatial Reasoning in Vision-Language Models [[arxiv]](https://arxiv.org/abs/2510.08531) [[hjfy]](https://hjfy.top/arxiv/2510.08531) `RL` `Hierarchical` `VLM`
  - 概览：构建包含26,610个样本的SpatialLadder-26k，并设计从目标定位、空间理解到可验证奖励强化学习的三阶段渐进训练，使3B模型逐层获得多图与视频空间推理能力。

- **[2025/08][ arXiv 2025 - 多模态空间智能 - AI ]** Multimodal Data Storage and Retrieval for Embodied AI: A Survey [[arxiv]](https://arxiv.org/abs/2508.13901) [[hjfy]](https://hjfy.top/arxiv/2508.13901) `Survey` `Retrieval`
  - 概览：综述具身AI多模态数据管理，比较图数据库、多模型数据库、数据湖、向量数据库和时序数据库五类存储架构，并归纳融合、表示对齐、图结构、生成式及效率优化五类检索范式。

- **[2025/06][ arXiv 2025 - 多模态空间智能 - AI ]** A Survey of Multi-sensor Fusion Perception for Embodied AI: Background, Methods, Challenges and Prospects [[arxiv]](https://arxiv.org/abs/2506.19769) [[hjfy]](https://hjfy.top/arxiv/2506.19769) `Survey` `Agentic`
  - 概览：从任务无关视角综述具身智能中的多传感器融合感知，分别梳理多模态、多智能体、时序与多模态大模型融合方法，并总结其数据、模型和应用层挑战。

- **[2025/05][ arXiv 2025 - 多模态空间智能 - USTBench ]** USTBench: Benchmarking and Dissecting Spatiotemporal Reasoning of LLMs as Urban Agents [[arxiv]](https://arxiv.org/abs/2505.17572) [[hjfy]](https://hjfy.top/arxiv/2505.17572) [[github]](https://github.com/usail-hkust/USTBench) `Benchmark` `Agentic` `End-to-end`
  - 概览：构建USTBench，在交互式城市环境UAgentEnv中设置5类城市决策、4类时空预测任务和62,466个结构化问答，从理解、预测、规划和反馈反思四个维度诊断城市智能体。

- **[2025/05][ arXiv 2025 - 多模态空间智能 - ReasonMap ]** ReasonMap: Towards Fine-Grained Visual Reasoning from Transit Maps [[arxiv]](https://arxiv.org/abs/2505.18675) [[hjfy]](https://hjfy.top/arxiv/2505.18675) [[project]](https://fscdc.github.io/Reason-Map/) [[github]](https://github.com/fscdc/ReasonMap) `Multimodal Reasoning` `VLM`
  - 概览：开发可扩展的半自动化数据集构建流程，创建了REASONMAP基准数据集，包含来自13个国家30个城市的高分辨率交通地图以及1008个人类验证的问题-答案对，涵盖了两种问题类型和三种模板。

- **[2025/05][ arXiv 2025 - 多模态空间智能 - ViewSpatial-Bench ]** ViewSpatial-Bench: Evaluating Multi-perspective Spatial Localization in Vision-Language Models [[arxiv]](https://arxiv.org/abs/2505.21500) [[hjfy]](https://hjfy.top/arxiv/2505.21500) `Multimodal Reasoning` `VLM`
  - 概览：构建ViewSpatial-Bench，通过自动化3D标注生成五类多视角空间定位任务，区分相机自我中心与人物分配中心视角，用于检验视觉语言模型的跨视点空间推理能力。

- **[2025/05][ arXiv 2025 - 多模态空间智能 - Spatial-MLLM ]** Spatial-MLLM: Boosting MLLM Capabilities in Visual-based Spatial Intelligence [[arxiv]](https://arxiv.org/abs/2505.23747) [[hjfy]](https://hjfy.top/arxiv/2505.23747) [[project]](https://diankun-wu.github.io/Spatial-MLLM/) [[github]](https://github.com/diankun-wu/Spatial-MLLM) `Pretraining` `VLM`
  - 概览：提出Spatial-MLLM，以二维视觉编码器提取语义、由几何基础模型初始化的三维编码器提取结构，再通过连接器融合为统一视觉令牌，并以空间感知帧采样保留视频中的关键几何信息。

- **[2025/04][ arXiv 2025 - 多模态空间智能 - Vision-Language ]** Multimodal Fusion and Vision-Language Models: A Survey for Robot Vision [[arxiv]](https://arxiv.org/abs/2504.02477) [[hjfy]](https://hjfy.top/arxiv/2504.02477) [[github]](https://github.com/Xiaofeng-Han-Res/MF-RV) `Survey` `Memory` `Human Preference`
  - 概览：系统整合了传统的多模态融合策略与新兴的视觉语言模型（VLMs），并从架构设计、功能特性及适用任务等方面进行了比较分析，揭示了它们之间的联系、互补优势及融合潜力。

- **[2025/04][ arXiv 2025 - 多模态空间智能 - Model-Powered ]** A Survey of Large Language Model-Powered Spatial Intelligence Across Scales: Advances in Embodied Agents, Smart Cities, and Earth Science [[arxiv]](https://arxiv.org/abs/2504.09848) [[hjfy]](https://hjfy.top/arxiv/2504.09848) `Survey` `Memory` `Transformer`
  - 概览：综述大语言模型空间智能，先梳理空间记忆、知识表示和抽象推理，再按具身、城市与全球尺度比较导航、城市规划、遥感和地球科学中的空间理解与推理。

- **[2025/03][ arXiv 2025 - 多模态空间智能 - UrbanVideo-Bench ]** UrbanVideo-Bench: Benchmarking Vision-Language Models on Embodied Intelligence with Video Data in Urban Spaces [[arxiv]](https://arxiv.org/abs/2503.06157) [[hjfy]](https://hjfy.top/arxiv/2503.06157) [[project]](https://embodiedcity.github.io/UrbanVideo-Bench/) [[github]](https://github.com/EmbodiedCity/UrbanVideo-Bench.code) `Benchmark` `Sim-to-Real` `VLM`
  - 概览：构建UrbanVideo-Bench，收集真实城市与仿真环境中的1.5K段无人机第一人称运动视频，并生成5.2K道题，评测视频语言模型的回忆、感知、推理和导航能力。

- **[2025/03][ arXiv 2025 - 多模态空间智能 - Open3D-VQA ]** Open3D-VQA: A Benchmark for Comprehensive Spatial Reasoning with Multimodal Large Language Model in Open Space [[arxiv]](https://arxiv.org/abs/2503.11094) [[hjfy]](https://hjfy.top/arxiv/2503.11094) [[github]](https://github.com/WeichenZh/Open3DVQA) `Benchmark` `VLM`
  - 概览：提出用于户外环境的综合空间推理基准Open3DVQA，涵盖了39种基本的空间问答任务，包括以自我为中心的、以他人为中心的和以目标为中心的空间推理。

- **[2025/01][ arXiv 2025 - 多模态空间智能 ]** Lifelong Learning of Large Language Model based Agents: A Roadmap [[arxiv]](https://arxiv.org/abs/2501.07278) [[hjfy]](https://hjfy.top/arxiv/2501.07278) [[github]](https://github.com/qianlima-lab/awesome-lifelong-llm-agent) `Survey` `Agentic` `Memory`
  - 概览：详细分析了感知、记忆和动作等关键模块，这些模块使LLM智能体能够实现自适应行为，并展示了它们如何共同支持智能体的持续学习和适应能力。

- **[2025/01][ arXiv 2025 - 多模态空间智能 - LLaVA-ST ]** LLaVA-ST: A Multimodal Large Language Model for Fine-Grained Spatial-Temporal Understanding [[arxiv]](https://arxiv.org/abs/2501.08282) [[hjfy]](https://hjfy.top/arxiv/2501.08282) [[github]](https://github.com/appletea233/LLaVA-ST) `Hierarchical` `Transformer` `VLM`
  - 概览：为了支持模型的训练，构建一个包含430万个样本的ST-Align数据集，并提出一个渐进的训练策略，使模型能够逐步学习内容对齐、坐标对齐和多任务能力。

- **[2025/01][ arXiv 2025 - 多模态空间智能 - SpatialCoT ]** SpatialCoT: Advancing Spatial Reasoning through Coordinate Alignment and Chain-of-Thought for Embodied Task Planning [[arxiv]](https://arxiv.org/abs/2501.10074) [[hjfy]](https://hjfy.top/arxiv/2501.10074) [[project]](https://spatialcot.github.io/) `Navigation` `VLM`
  - 概览：提出SpatialCoT两阶段训练：先将视觉语言输入与空间坐标双向对齐，再以空间思维链把语言推理落到可执行坐标，用于导航与操作任务中的细粒度空间规划。

- **[2025/01][ arXiv 2025 - 多模态空间智能 - EmbodiedEval ]** EmbodiedEval: Evaluate Multimodal LLMs as Embodied Agents [[arxiv]](https://arxiv.org/abs/2501.11858) [[hjfy]](https://hjfy.top/arxiv/2501.11858) [[project]](https://embodiedeval.github.io/) [[github]](https://github.com/thunlp/EmbodiedEval) `Navigation` `VLM`
  - 概览：构建交互式评测基准EmbodiedEval，在125个3D场景中设置328项任务，并按导航、物体交互、社会交互、属性问答和空间问答五类统一检验多模态大模型的具身能力。

- **[2024/12][ arXiv 2024 - 多模态空间智能 - MageBench ]** MageBench: Bridging Large Multimodal Models to Agents [[arxiv]](https://arxiv.org/abs/2412.04531) [[hjfy]](https://hjfy.top/arxiv/2412.04531) [[github]](https://github.com/microsoft/MageBench) `Multimodal Reasoning`
  - 概览：提出面向多模态智能体的推理能力基准测试MageBench，旨在评估多模态大模型在复杂视觉任务中的表现，特别是那些需要持续视觉反馈的任务。

- **[2024/12][ 中国图象图形学报 2025 - 多模态大模型三维视觉理解综述 ]** Advancements in 3D Vision Understanding Using Multimodal Large Language Models [[doi]](https://doi.org/10.11834/jig.240588) `Survey`
  - 概览：系统梳理多模态大模型驱动的三维表示学习、空间推理任务与三维多模态数据集，并讨论面向机器人边端部署的模型轻量化和云边协同方向。

- **[2024/11][ arXiv 2024 - 多模态空间智能 - RoboSpatial ]** RoboSpatial: Teaching Spatial Understanding to 2D and 3D Vision-Language Models for Robotics [[arxiv]](https://arxiv.org/abs/2411.16537) [[hjfy]](https://hjfy.top/arxiv/2411.16537) `Multimodal Reasoning` `VLM`
  - 概览：构建机器人空间理解数据集RoboSpatial，配对第一人称图像与三维扫描，标注自我、世界和物体参考系下的空间关系，用于训练二维与三维视觉语言模型。

- **[2024/10][ arXiv 2024 - 多模态空间智能 - Embodied Agent Interface ]** Embodied Agent Interface: Benchmarking LLMs for Embodied Decision Making [[arxiv]](https://arxiv.org/abs/2410.07166) [[hjfy]](https://hjfy.top/arxiv/2410.07166) [[project]](https://embodied-agent-interface.github.io/) [[github]](https://github.com/embodied-agent-interface/embodied-agent-interface) `Benchmark`
  - 概览：定义了四个用于决策制定的能力模块（目标解释、子目标分解、动作序列生成和转换建模），并为其制定了标准化的输入输出规范，使得LLM可以更有效地与其他环境模块集成。

- **[2024/10][ arXiv 2024 - 多模态空间智能 - ET-Plan-Bench ]** ET-Plan-Bench: Embodied Task-level Planning Benchmark Towards Spatial-Temporal Cognition with Foundation Models [[arxiv]](https://arxiv.org/abs/2410.14682) [[hjfy]](https://hjfy.top/arxiv/2410.14682) `Benchmark`
  - 概览：构建ET-Plan-Bench，通过可控难度任务检验基础模型对空间关系、目标遮挡以及动作序列时序与因果关系的理解，并借助多源模拟器反馈支持智能体交互和重规划。

- **[2024/08][ arXiv 2024 - 多模态空间智能 - UrBench ]** UrBench: A Comprehensive Benchmark for Evaluating Large Multimodal Models in Multi-View Urban Scenarios [[arxiv]](https://arxiv.org/abs/2408.17267) [[hjfy]](https://hjfy.top/arxiv/2408.17267) [[project]](https://opendatalab.github.io/UrBench/) [[github]](https://github.com/opendatalab/UrBench) `Benchmark`
  - 概览：构建UrBench城市多视角基准，汇集11.6K个区域级与角色级问题，覆盖地理定位、场景推理、场景理解和物体理解四个维度、14类任务，并以跨视角检测匹配生成标注。

- **[2024/06][ arXiv 2024 - 具根空间推理VLM - SpatialRGPT ]** SpatialRGPT: Grounded Spatial Reasoning in Vision-Language Models [[arxiv]](https://arxiv.org/abs/2406.01584) [[hjfy]](https://hjfy.top/arxiv/2406.01584) `Spatial Reasoning`
  - 概览：提出SpatialRGPT，通过区域表示模块和可插拔深度信息增强VLM的局部区域与三维几何推理，并配套OSD训练数据和SpatialRGPT-Bench进行评测。

- **[2024/06][ arXiv 2024 - 具身空间理解评测 - EmbSpatial-Bench ]** EmbSpatial-Bench: Benchmarking Spatial Understanding for Embodied Tasks with Large Vision-Language Models [[arxiv]](https://arxiv.org/abs/2406.05756) [[hjfy]](https://hjfy.top/arxiv/2406.05756) `Benchmark`
  - 概览：构建从自我中心视角评测六类空间关系的EmbSpatial-Bench，并发布EmbSpatial-SFT指令微调数据，用于诊断和增强大视觉语言模型的具身空间理解能力。

- **[2024/01][ CVPR 2024 - 赋予VLM空间推理能力 - SpatialVLM ]** SpatialVLM: Endowing Vision-Language Models with Spatial Reasoning Capabilities [[arxiv]](https://arxiv.org/abs/2401.12168) [[hjfy]](https://hjfy.top/arxiv/2401.12168) [[project]](https://spatial-vlm.github.io/) `End-to-end` `PaLM 2-E`
  - 概览：构建互联网规模的三维空间VQA数据生成管线（20亿样本）训练视觉语言模型，赋予VLM定量空间估计与推理能力，为机器人操作与导航等下游具身任务提供空间感知基座。

- **[2023/11][ arXiv 2023 - 第一人称视觉推理评测 - EgoThink ]** EgoThink: Evaluating First-Person Perspective Thinking Capability of Vision-Language Models [[arxiv]](https://arxiv.org/abs/2311.15596) [[hjfy]](https://hjfy.top/arxiv/2311.15596) `Benchmark`
  - 概览：构建基于第一人称视频的EgoThink视觉问答基准，覆盖六项核心能力和十二个细分维度，并系统评估多种视觉语言模型的自我中心推理表现。

- **[2023/04][ arXiv 2023 - 自监督视觉基础模型 - DINOv2 ]** DINOv2: Learning Robust Visual Features without Supervision [[arxiv]](https://arxiv.org/abs/2304.07193) [[hjfy]](https://hjfy.top/arxiv/2304.07193) [[github]](https://github.com/facebookresearch/dinov2) `Self-Supervised`
  - 概览：视觉基础模型代表作。利用1.42亿高质量清洗数据进行自监督学习，训练出具有极强泛化特征的ViT基座模型，其特征不仅直接支持分类，还能无需微调广泛用于像素级密集预测与深度估计。

- **[2021/07][ arXiv 2021 - 多模态空间智能 - CLIP ]** How Much Can CLIP Benefit Vision-and-Language Tasks? [[arxiv]](https://arxiv.org/abs/2107.06383) [[hjfy]](https://hjfy.top/arxiv/2107.06383) `Zero-Shot` `Pretraining`
  - 概览：系统评估CLIP作为视觉编码器对视觉语言任务的作用，分别研究任务微调和视觉语言预训练两种接入方式，并在问答、蕴含和导航任务中验证其可迁移表征。

- **[2021/03][ arXiv 2021 - 多模态空间智能 ]** Learning Transferable Visual Models From Natural Language Supervision [[arxiv]](https://arxiv.org/abs/2103.00020) [[hjfy]](https://hjfy.top/arxiv/2103.00020) `Zero-Shot` `Pretraining`
  - 概览：提出CLIP，以4亿组互联网图文对进行对比式预训练，并把自然语言作为开放类别接口，使视觉模型无需下游任务专用标注即可执行零样本迁移。

- **[2020/01][ arXiv 2020 - 神经语言模型缩放定律 ]** Scaling Laws for Neural Language Models [[arxiv]](https://arxiv.org/abs/2001.08361) [[hjfy]](https://hjfy.top/arxiv/2001.08361) `Scaling Law`
  - 概览：大语言模型（LLM）算力与数据扩展的基石论文。揭示了模型性能与算力、模型参数量和数据集规模之间呈幂律缩放关系，启发了后续大模型（包括具身VLA模型）的一系列参数缩放革命。

### 4. 3D Scene & Reconstruction

涵盖无人机对物理环境的三维建模、几何表达与渲染技术。

- **[2026/05][ arXiv 2026 - 多尺度高斯-语言地图攻克具身导航几何语义失衡难题 ]** Multi-Scale Gaussian-Language Map for Zero-shot Embodied Navigation and Reasoning [[arxiv]](https://arxiv.org/abs/2605.01736) [[hjfy]](https://hjfy.top/arxiv/2605.01736) `Zero-Shot`
  - 概览：提出GLMap多尺度高斯语言地图，将区域与实例级语义、二维索引网格和三维高斯场统一表示，为零样本导航提供可定位、可渲染且可由大模型查询的空间记忆。

- **[2026/05][ arXiv 2026 - 多模态交互场解决人形机器人导航动态环境适配难题 - Learning to Evolve ]** Learning to Evolve: Multi-modal Interactive Fields for Robust Humanoid Navigation in Dynamic Environments [[arxiv]](https://arxiv.org/abs/2605.21935) [[hjfy]](https://hjfy.top/arxiv/2605.21935) `GSM`
  - 概览：提出用于动态环境人形导航的多模态交互场，将视觉、语义与运动线索统一为可在线更新的空间表示，以支持规划和安全避障。

- **[2026/05][ arXiv 2026 - 相对三维地图中的WayPixel导航 - MASt3R-Nav ]** MASt3R-Nav: WayPixel Navigation in Relative 3D Maps [[arxiv]](https://arxiv.org/abs/2605.24111) [[hjfy]](https://hjfy.top/arxiv/2605.24111) `GSM`
  - 概览：提出MASt3R-Nav，依据图像对各自相对三维坐标系中的像素对应关系构建像素级连通图，再近似并稀疏化图内连接得到WayPixel代价图，最后以该代价图为条件训练控制器预测轨迹展开。

- **[2026/04][ arXiv 2026 - 深度先验玻璃表面重建与机器人导航 ]** Enhancing Glass Surface Reconstruction via Depth Prior for Robot Navigation [[arxiv]](https://arxiv.org/abs/2604.18336) [[hjfy]](https://hjfy.top/arxiv/2604.18336) `GSM`
  - 概览：提出无训练的玻璃表面重建框架，以深度基础模型提供结构先验并通过局部RANSAC对齐恢复度量尺度，从受玻璃干扰的RGB-D观测中重建可靠几何，同时发布GlassRecon数据集。

- **[2025/12][ arXiv 2025 - 机器人三维场景表示综述 ]** What Is The Best 3D Scene Representation for Robotics? From Geometric to Foundation Models [[arxiv]](https://arxiv.org/abs/2512.03422) [[hjfy]](https://hjfy.top/arxiv/2512.03422) `Survey`
  - 概览：系统综述点云、体素、符号距离场、场景图、NeRF、三维高斯和基础模型等三维场景表示，并按感知、建图、定位、导航、操作五个机器人模块比较其优缺点，讨论稠密语义表示与三维基础模型的潜力及待解挑战。

- **[2025/10][ arXiv 2025 - 物理可执行3D高斯具身导航环境 - SAGE-3D ]** Towards Physically Executable 3D Gaussian for Embodied Navigation [[arxiv]](https://arxiv.org/abs/2510.21307) [[hjfy]](https://hjfy.top/arxiv/2510.21307) [[project]](https://sage-3d.github.io/) `Benchmark` `3DGS`
  - 概览：提出SAGE-3D范式为3DGS场景注入物体级语义标注与物理碰撞执行能力，构建InteriorGS数据集与SAGE-Bench具身导航基准，使高保真3D高斯场景成为物理可执行的导航训练环境。

- **[2025/08][ arXiv 2025 - 三维场景理解 - Co-Adaptation ]** Quantifying and Alleviating Co-Adaptation in Sparse-View 3D Gaussian Splatting [[arxiv]](https://arxiv.org/abs/2508.12720) [[hjfy]](https://hjfy.top/arxiv/2508.12720) [[project]](https://chenkangjie1123.github.io/Co-Adaptation-3DGS/) [[github]](https://github.com/chenkangjie1123/Co-Adaptation-of-3DGS/) `3D Representation`
  - 概览：提出共适应分数度量稀疏视图3DGS中高斯之间的纠缠程度，并设计随机高斯丢弃与不透明度乘性噪声两种即插即用策略，抑制训练视图过拟合造成的新视角伪影。

- **[2025/03][ arXiv 2025 - 三维场景理解 ]** Controllable 3D Outdoor Scene Generation via Scene Graphs [[arxiv]](https://arxiv.org/abs/2503.07152) [[hjfy]](https://hjfy.top/arxiv/2503.07152) [[project]](https://yuheng.ink/project-page/control-3d-scene/) [[github]](https://github.com/yuhengliu02/control-3d-scene) `Diffusion` `GSM`
  - 概览：提出可控室外3D场景生成方法，将稀疏场景图经图神经网络与空间分配模块变换为稠密BEV嵌入图，再以其为条件驱动3D扩散模型；同时构建场景图—三维语义场景配对数据集。

- **[2025/02][ arXiv 2025 - 三维场景理解 ]** Embodied Intelligence for 3D Understanding: A Survey on 3D Scene Question Answering [[arxiv]](https://arxiv.org/abs/2502.00342) [[hjfy]](https://hjfy.top/arxiv/2502.00342) `Survey` `Zero-Shot`
  - 概览：系统综述3D场景问答，从数据集、方法和评测指标三条主线组织工作，并比较指令调优、跨模态对齐与零样本方法的共用架构和泛化局限。

- **[2025/01][ arXiv 2025 - 视频生成可交互城市仿真 - Vid2Sim ]** Vid2Sim: Realistic and Interactive Simulation from Video for Urban Navigation [[arxiv]](https://arxiv.org/abs/2501.06693) [[hjfy]](https://hjfy.top/arxiv/2501.06693) `Simulation`
  - 概览：提出Vid2Sim，将单目城市视频转换为具有可交互几何和物理属性的三维仿真环境，为城市导航策略提供可扩展的逼真训练与评测场景。

- **[2024/12][ arXiv 2024 - 航拍视角生成地面漫游城市重建 - AerialGo ]** AerialGo: Walking-through City View Generation from Aerial Perspectives [[arxiv]](https://arxiv.org/abs/2412.00157) [[hjfy]](https://hjfy.top/arxiv/2412.00157) `Diffusion`
  - 概览：提出多视图扩散框架AerialGo，仅以易获取的航拍图像为条件生成逼真的地面漫游视角，规避地面采集的隐私风险，并发布覆盖134平方公里、345万张空地配对图像的AerialGo数据集。

- **[2024/12][ arXiv 2024 - 三维场景理解 - UnrealZoo ]** UnrealZoo: Enriching Photo-realistic Virtual Worlds for Embodied AI [[arxiv]](https://arxiv.org/abs/2412.20977) [[hjfy]](https://hjfy.top/arxiv/2412.20977) [[project]](http://unrealzoo.site/) [[github]](https://github.com/UnrealZoo/unrealzoo-gym) `RL` `Agentic` `Sim-to-Real`
  - 概览：发布UnrealZoo，提供基于Unreal Engine构建的百余个照片级3D开放世界与多类可控实体，并扩展UnrealCV的数据采集、环境增强、分布式训练和基准接口。

- **[2024/10][ arXiv 2024 - 三维场景理解 - EmbodiedRAG ]** EmbodiedRAG: Dynamic 3D Scene Graph Retrieval for Efficient and Scalable Robot Task Planning [[arxiv]](https://arxiv.org/abs/2410.23968) [[hjfy]](https://hjfy.top/arxiv/2410.23968) `GSM` `Planning` `Retrieval`
  - 概览：提出3D场景子图检索框架EmbodiedRAG，旨在增强基于大模型（LLM）的机器人规划器，通过提取与任务相关的3D场景图的子图来提高效率和可扩展性。

- **[2024/09][ AAAI 2025 - 大规模平面3D高斯场景重建 - GigaGS ]** GigaGS: Scaling up Planar-Based 3D Gaussians for Large Scene Surface Reconstruction [[arxiv]](https://arxiv.org/abs/2409.06685) [[hjfy]](https://hjfy.top/arxiv/2409.06685) `3DGS`
  - 概览：针对大规模场景的 3DGS 重建面临的显存爆炸与几何不一致痛点，提出一种基于区域可见性的分块训练策略，并融合细节层次(LoD)的多视角光度一致性约束，实现了极高精度的城市场景表面重建。

- **[2024/09][ arXiv 2024 - 三维场景理解 - Point2Graph ]** Point2Graph: An End-to-end Point Cloud-based 3D Open-Vocabulary Scene Graph for Robot Navigation [[arxiv]](https://arxiv.org/abs/2409.10350) [[hjfy]](https://hjfy.top/arxiv/2409.10350) [[project]](https://point2graph.github.io/) [[github]](https://github.com/zimingluo/Point2Graph) `Zero-Shot` `GSM` `Hierarchical`
  - 概览：提出基于点云的端到端三维开放词汇场景图生成框架Point2Graph，无需依赖于对齐的RGB-D图像序列，解决了现有开放词汇场景图生成算法在RGB-D图像或相机姿态信息不可用场景下应用受限的问题。

- **[2023/08][ SIGGRAPH 2023 - 实时辐射场渲染 - 3DGS ]** 3D Gaussian Splatting for Real-Time Radiance Field Rendering [[arxiv]](https://arxiv.org/abs/2308.04079) [[hjfy]](https://hjfy.top/arxiv/2308.04079) `3DGS`
  - 概览：3DGS开山之作。摒弃了NeRF庞大的MLP隐式体渲染计算，直接将场景表示为无数可微分的带向三维高斯椭球，利用光栅化实现了照片级的高速（100+ FPS）实时三维渲染。

### 5. UAV Visual Perception

涵盖传统空中视角的2D/3D目标检测、多机协同感知等基础视觉任务。

- **[2026/07][ arXiv 2026 - 航拍通用多模态指代基准 - UniRef-UAV ]** UniRef-UAV: A Multimodal Benchmark for Universal Referring in UAV Imagery [[arxiv]](https://arxiv.org/abs/2607.08267) [[hjfy]](https://hjfy.top/arxiv/2607.08267) `Benchmark` `GroundingDINO`
  - 概览：提出“通用指代”新任务并构建首个航拍多模态指代基准UniRef-UAV，覆盖纯文本、纯图像与图文混合查询及无、单、多目标输出，配套集合预测式轻量基线UAV-URNet。

- **[2026/07][ arXiv 2026 - 无人机开放词汇视频实例分割 - AeroTrack ]** UAV-OVVIS: Unmanned Aerial Vehicles Also Need Open-Vocabulary Video Instance Segmentation [[arxiv]](https://arxiv.org/abs/2607.08075) [[hjfy]](https://hjfy.top/arxiv/2607.08075) [[github]](https://github.com/Dmygithub/AeroTrack) `Zero-Shot` `Grounding DINO+SAM3`
  - 概览：首创无人机开放词汇视频实例分割任务UAV-OVVIS，提出免训练模块化框架AeroTrack以周期关键帧检测、分段掩码传播与生命周期ID关联维持全局轨迹，并构建航拍专用基准AeroVIS。

- **[2026/07][ arXiv 2026 - 公开地图先验锚定的无人机单目6DoF定位 - AeroMap3D ]** AeroMap3D: Anchoring Monocular UAV 6-DoF Localization to Visual-Geometric-Semantic Map Priors [[arxiv]](https://arxiv.org/abs/2607.14009) [[hjfy]](https://hjfy.top/arxiv/2607.14009) `GSM` `RoMav2+EKF`
  - 概览：提出仅依托公开卫星影像、裸地DEM与OSM语义地图的无人机单目6自由度定位框架，用轻量尺度-航向适配器修正跨视角偏差、OSM掩码剔除建筑高程失真，55km航线平均三维误差5.88米。

- **[2026/07][ CVPR Findings 2026 - 大倾角无人机-卫星跨视角定位基准与框架 - OffNadirLoc ]** OffNadirLoc: Benchmark and Framework for Challenging UAV-to-Satellite Geo-Localization under Large Off-Nadir Views [[arxiv]](https://arxiv.org/abs/2607.19951) [[hjfy]](https://hjfy.top/arxiv/2607.19951) [[project]](https://montalario.github.io/offnadirloc/) `Benchmark` `DINOv2`
  - 概览：构建首个覆盖70°~85°大倾角侧视的无人机-卫星跨视角定位基准OffNadirLoc，并提出ONLoc框架，以结构感知上下文加权与视角协同学习实现强零样本泛化。

- **[2026/06][ ECCV 2026 - 几何感知单阶段跨视角目标地理定位 - GAGeo ]** Beyond 2D Matching: A Unified Single-Stage Framework for Geometry-Aware Cross-View Object Geo-Localization [[arxiv]](https://arxiv.org/abs/2606.30576) [[hjfy]](https://hjfy.top/arxiv/2606.30576) [[project]](https://cipual.github.io/GAGeo-project-page/) `End-to-end` `π³+DINOv2`
  - 概览：提出单阶段几何感知跨视角目标地理定位框架GAGeo，基于排列等变3D基础模型一次前向同步输出检测框、分割掩码与相机位姿，并配套发布22万实例对的大规模基准CMA-Loc。

- **[2026/06][ ECCV 2026 - 语义3D城市模型驱动的无人机6DoF定位 - SemCityLoc ]** SemCityLoc: Aerial 6DoF Localization Using Semantic 3D City Models [[arxiv]](https://arxiv.org/abs/2606.27444) [[hjfy]](https://hjfy.top/arxiv/2606.27444) [[project]](https://albertchen98.github.io/SemCityLoc) `GSM` `DINOv3+MoGe-2`
  - 概览：将无人机6DoF定位重构为大模型语义深度先验与LoD语义3D城市模型的曲面配准，无需稠密重建即把城市峡谷平均定位误差从9.89米降至2.62米，并发布厘米级基准SemCityLockeD。

- **[2026/06][ arXiv 2026 - 正射地图像素对齐的无人机地理定位 - PiLoT v2 ]** PiLoT v2: Pixel-to-Orthogonal Map Alignment for Free-view UAV Geo-localization [[arxiv]](https://arxiv.org/abs/2606.31098) [[hjfy]](https://hjfy.top/arxiv/2606.31098) `End-to-end` `MobileOne+UNet`
  - 概览：以TDOM正射影像加DSM的2.5D地图替代三维网格并在CPU上完成裁剪，结合跨视角配准网络与IMU重力、单点激光约束做多假设LM位姿优化，地图体积压缩97%且长序列零定位失效。

- **[2026/06][ ECCV 2026 - 公开正射影像锚定的无人机6DoF轨迹估计 - OrthoTrack ]** OrthoTrack: Continuous 6-DoF UAV Trajectory Estimation Anchored in Public Orthophotos [[arxiv]](https://arxiv.org/abs/2606.25245) [[hjfy]](https://hjfy.top/arxiv/2606.25245) [[project]](https://orthotrack.ethz.ch) `Zero-Shot` `RoMa-v2`
  - 概览：提出免训练实时跟踪框架，仅用公开正射影像与地表模型，关键帧全局稠密匹配锚定、中间帧光流轻量传播，逐帧输出无漂移的度量级6DoF位姿，并发布时序多模态仿真数据集MovingDrone。

- **[2026/06][ arXiv 2026 - 低空无人机前视单目语义占据基准 - SkyShield ]** SkyShield: Occupancy as a Safety Interface for Low-Altitude UAV Autonomy [[arxiv]](https://arxiv.org/abs/2606.00747) [[hjfy]](https://hjfy.top/arxiv/2606.00747) `Benchmark` `ResNet50+FPN` `CARLA`
  - 概览：基于CARLA构建首个面向20米以下低空飞行的前视单目语义占据基准SkyShield，配套风险加权指标KAR-mIoU与姿态补偿基线模型SkyOcc，显著提升细线、行人等稀疏致命障碍物的感知精度。

- **[2026/06][ ECCV 2026 - 航拍单目度量深度基准与适配 - AerialMetric ]** AerialMetric: Benchmarking and Adapting UAV Monocular Metric Depth Estimation in the Real World [[arxiv]](https://arxiv.org/abs/2606.29716) [[hjfy]](https://hjfy.top/arxiv/2606.29716) [[github]](https://github.com/kuieless/AerialMetric-ECCV2026) [[project]](https://kuieless.github.io/AerialMetric-ECCV2026-page/) `Benchmark` `MoGe2 (LoRA)`
  - 概览：构建含52K真实与16K仿真图像-深度对、解耦俯仰角/高度/视场三大成像变量的航拍单目度量深度基准，并以LoRA微调得到MoGe2-Aerial，大幅提升航拍测距精度且不损失地面场景能力。

- **[2026/06][ CVPR 2026 - 低成本高效时序学习无人机跟踪 - LETrack ]** Toward Low-Cost yet Effective Temporal Learning for UAV Tracking [[cvf]](https://openaccess.thecvf.com/content/CVPR2026/papers/Xue_Toward_Low-Cost_yet_Effective_Temporal_Learning_for_UAV_Tracking_CVPR_2026_paper.pdf) [[github]](https://github.com/GXNU-ZhongLab/LETrack) `End-to-end` `DeiT-Tiny`
  - 概览：提出精度每浮点运算数(PPF)指标公平评估时序模块效率，并设计细粒度外观token流的低成本时序学习方法LETL，仅增加0.09G FLOPs即在6大无人机跟踪基准上全面登顶。

- **[2026/06][ CVPR 2026 - 空频双域选择航拍小目标检测 - SFS-DETR ]** SFS-DETR: Spatial-Frequency Selection for UAV Object Detection [[cvf]](https://openaccess.thecvf.com/content/CVPR2026F/papers/Jia_SFS-DETR_Spatial-Frequency_Selection_for_UAV_Object_Detection_CVPRF_2026_paper.pdf) `End-to-end` `RT-DETR`
  - 概览：提出空间-频域自适应选择骨干SSFNet，配合语义对齐融合、多分支特征增强与Inner-MPDIoU损失，在5个航拍检测数据集上以更低算力超越SOTA并达到96FPS实时推理。

- **[2026/06][ CVPR 2026 - 卫星-无人机-地面三视角地理定位基准 - UniGeoRS ]** UniGeoRS: A Unified Benchmark for Tri-view Geo-Localization [[cvf]](https://openaccess.thecvf.com/content/CVPR2026/papers/Liang_UniGeoRS_A_Unified_Benchmark_for_Tri-view_Geo-Localization_CVPR_2026_paper.pdf) [[github]](https://github.com/BIT-MSense/UniGeoRS) `Benchmark`
  - 概览：构建首个融合真实与合成数据的卫星-无人机-地面三视角地理定位基准，覆盖1154个地点、14万余张图像，并提出即插即用的交叉注意力匹配增强模块CAME稳定提升主流模型精度。

- **[2026/05][ ICML 2026 - 信息瓶颈物体中心跨视角无人机定位 - InfoGeo ]** InfoGeo: Information-Theoretic Object-Centric Learning for Cross-View Generalizable UAV Geo-Localization [[arxiv]](https://arxiv.org/abs/2605.07099) [[hjfy]](https://hjfy.top/arxiv/2605.07099) `End-to-end` `DINOv2+Slot Attention`
  - 概览：首次将物体中心学习与信息瓶颈理论引入跨视角无人机地理定位，最大化跨视角物体结构共识并压缩视角特有噪声，在跨区域迁移与雨雪雾极端天气下刷新SOTA。

- **[2026/05][ CVPR 2026 - 双分支蒸馏高效无人机跟踪 - EATrack ]** Dual-branch Distilled Transformer for Efficient Asymmetric UAV Tracking [[arxiv]](https://arxiv.org/abs/2605.28018) [[hjfy]](https://hjfy.top/arxiv/2605.28018) [[github]](https://github.com/GXNU-ZhongLab/EATrack) `End-to-end` `Transformer (Distillation)`
  - 概览：提出高效非对称无人机跟踪框架EATrack，用教师引导的特征级与预测级双分支目标感知蒸馏补强轻量学生模型的表征与定位能力，推理端零额外开销，在五大无人机基准上兼顾精度与速度。

- **[2026/04][ ECCV 2026 - 百万级几何标注航拍3D视觉数据集 - AirZoo ]** AirZoo: A Unified Large-Scale Dataset for Grounding Aerial Geometric 3D Vision [[arxiv]](https://arxiv.org/abs/2604.26567) [[hjfy]](https://hjfy.top/arxiv/2604.26567) [[project]](https://nudt-sawlab.github.io/AirZoo/) `Benchmark` `AirSim+UE5+Cesium`
  - 概览：依托全球实景3D瓦片与AirSim-Cesium-UE5仿真管线，构建覆盖22国、120万帧、带像素级度量深度与6自由度地理位姿标注的航拍几何3D视觉统一基准，大幅提升检索/匹配/重建模型的真实泛化能力。

- **[2026/04][ TPAMI 2026 - 百万级无人机指代表达理解基准 - SkyFind ]** SkyFind: A Large-Scale Benchmark Unveiling Referring Expression Comprehension for UAV [[doi]](https://ieeexplore.ieee.org/document/11475181) [[github]](https://github.com/wangkunyu241/SkyFind) `Benchmark` `SeqTR/PolyFormer`
  - 概览：首次把指代表达理解任务拓展到无人机航拍视角，构建含3.5万张航拍图、35万标注目标与百万级目标-描述对的SkyFind基准，并提出先粗搜候选区域再精修边界框的两阶段序列回归框架AerialREC。

- **[2026/04][ CVPR 2026 - RGB+热成像+事件三模态无人机检测 ]** Tri-Modal Fusion Transformers for UAV-based Object Detection [[arxiv]](https://arxiv.org/abs/2604.16630) [[hjfy]](https://hjfy.top/arxiv/2604.16630) [[github]](https://github.com/radlab-sketch/trimodal-uav-det) [[cvf]](https://openaccess.thecvf.com/content/CVPR2026/papers/Iaboni_Tri-Modal_Fusion_Transformers_for_UAV-based_Object_Detection_CVPR_2026_paper.pdf) `End-to-end` `MixTransformer (MiT)`
  - 概览：提出首个统一RGB-热成像-事件三模态的无人机检测框架，用MAGE门控交换与BiTE双向Token交换在双分支MixTransformer任意层级融合，并开源1万余帧同步标注数据集与61组消融基准。

- **[2026/04][ CVPR 2026 - 视觉原型条件聚焦区域生成的检测数据增强 - UAVGen ]** Visual Prototype Conditioned Focal Region Generation for UAV-Based Object Detection [[arxiv]](https://arxiv.org/abs/2604.02966) [[hjfy]](https://hjfy.top/arxiv/2604.02966) [[github]](https://github.com/Sirius-Li/UAVGen) [[cvf]](https://openaccess.thecvf.com/content/CVPR2026/papers/Li_Visual_Prototype_Conditioned_Focal_Region_Generation_for_UAV-Based_Object_Detection_CVPR_2026_paper.pdf) `Diffusion` `FLUX + ControlNet`
  - 概览：提出首个无人机专用扩散数据增强框架UAVGen，用视觉原型条件扩散模型提升密集小目标的布局条件质量，并以聚焦区域增强管道集中生成并细化标签，仅用11%合成数据即超越现有方法。

- **[2026/04][ arXiv 2026 - 跨本体主动视觉跟踪 - AdaTracker ]** AdaTracker: Learning Adaptive In-Context Policy for Cross-Embodiment Active Visual Tracking [[arxiv]](https://arxiv.org/abs/2604.20305) [[hjfy]](https://hjfy.top/arxiv/2604.20305) `Zero-Shot`
  - 概览：提出AdaTracker跨本体主动视觉跟踪框架，通过本体上下文编码器从历史交互中推断平台约束，并动态调制跟踪策略以零样本适配未见机器人。

- **[2026/03][ CVPR 2026 Highlight - 单目无人机自定位与目标地理定位 - PiLoT ]** PiLoT: Neural Pixel-to-3D Registration for UAV-based Ego and Target Geo-localization [[arxiv]](https://arxiv.org/abs/2603.20778) [[hjfy]](https://hjfy.top/arxiv/2603.20778) [[github]](https://github.com/nudt-sawlab/PiLoT) [[project]](https://nudt-sawlab.github.io/PiLoT/) `Zero-Shot` `MobileOne-UNet` `AirSim+Cesium+UE`
  - 概览：将无人机自定位与目标定位统一为像素到三维地图的配准问题，通过渲染-定位双线程引擎、百万级全球尺度合成数据与神经引导随机梯度优化器，在Jetson Orin上以25FPS实现10km无漂移定位。

- **[2026/03][ CVPR 2026 - 实例轮廓对齐的密集城市航拍定位 - LoD-Loc v3 ]** LoD-Loc v3: Generalized Aerial Localization in Dense Cities using Instance Silhouette Alignment [[arxiv]](https://arxiv.org/abs/2603.19609) [[hjfy]](https://hjfy.top/arxiv/2603.19609) [[github]](https://github.com/nudt-sawlab/LoD-Loc-v3) [[project]](https://nudt-sawlab.github.io/LoD-Locv3/) `Zero-Shot` `SAM` `UE5+AirSim`
  - 概览：将定位范式从语义轮廓对齐升级为建筑实例轮廓对齐，并构建10万张图像的InsLoD-Loc航拍实例分割合成数据集，在密集城区与跨场景零样本定位上大幅超越SOTA。

- **[2026/03][ CVPR 2026 - 车-无人机协同感知实景数据集 - V2U4Real ]** V2U4Real: A Real-world Large-scale Dataset for Vehicle-to-UAV Cooperative Perception [[arxiv]](https://arxiv.org/abs/2603.25275) [[hjfy]](https://hjfy.top/arxiv/2603.25275) [[github]](https://github.com/VjiaLi/V2U4Real) `Benchmark`
  - 概览：发布全球首个真实场景大规模车-无人机协同感知数据集，含5.6万帧同步激光雷达与相机数据、70万个3D标注框，并建立单体/协同3D检测与跟踪的完整评测基准。

- **[2026/03][ CVPR 2026 - 跨模态模糊对齐的文本-航拍行人检索 - CFAN ]** Cross-modal Fuzzy Alignment Network for Text-Aerial Person Retrieval and A Large-scale Benchmark [[arxiv]](https://arxiv.org/abs/2603.20721) [[hjfy]](https://hjfy.top/arxiv/2603.20721) [[github]](https://github.com/Yifei-AHU/AERI-PEDES) `End-to-end` `CLIP`
  - 概览：提出跨模态模糊对齐网络CFAN，以地面图像为语义桥梁动态调节全局对齐强度，并用模糊隶属度筛选可靠语义单元，同时构建最大规模文本-航拍行人检索基准AERI-PEDES。

- **[2026/03][ CVPR 2026 - 高动态工况无人机多目标跟踪基准 - DynUAV ]** Breaking Smooth-Motion Assumptions: A UAV Benchmark for Multi-Object Tracking in Complex and Adverse Conditions [[arxiv]](https://arxiv.org/abs/2603.05970) [[hjfy]](https://hjfy.top/arxiv/2603.05970) [[github]](https://github.com/kxzhang-lab/DynUAV) `Benchmark`
  - 概览：构建面向无人机剧烈自运动的多目标跟踪基准DynUAV，包含42段长序列、超170万标注框与工程特种车辆类别，评测11种SOTA跟踪器揭示其检测与关联性能的显著下滑。

- **[2026/01][ IEEE TGRS 2025 - 遥感三维空间理解与空中智能体 - AirSpatialBot ]** AirSpatialBot: A Spatially-Aware Aerial Agent for Fine-Grained Vehicle Attribute Recognization and Retrieval [[arxiv]](https://arxiv.org/abs/2601.01416) [[hjfy]](https://hjfy.top/arxiv/2601.01416) [[github]](https://github.com/VisionXLab/AirSpatialBot) `Agentic`
  - 概览：构建首个带3D边界框的遥感空间定位与问答数据集AirSpatial(20万+指令)，用两阶段训练与辅助监督、几何映射学习赋予遥感VLM空间感知能力，并搭建细粒度车辆属性识别与检索的空中智能体。

- **[2026/01][ ISPRS JPRS 2026 - 无人机影像隐式视觉定位基准与模型 - DVGBench ]** DVGBench: Implicit-to-Explicit Visual Grounding Benchmark in UAV Imagery with Large Vision-Language Models [[arxiv]](https://arxiv.org/abs/2601.00998) [[hjfy]](https://hjfy.top/arxiv/2601.00998) [[github]](https://github.com/zytx121/DVGBench) [[doi]](https://doi.org/10.1016/j.isprsjprs.2026.01.005) `Benchmark` `Qwen2.5-VL+SAM2`
  - 概览：构建首个无人机影像隐式视觉定位基准DVGBench，含2863条人工标注的显隐配对样本，并提出隐转显思维链I2E-CoT与GRPO训练的DroneVG-R1模型，区域级与像素级定位均达SOTA。

- **[2026/X][ AAAI 2026 - 多模态提示无人机跨视角目标定位基准 - MoP-UAV ]** Learning Better UAV-Based Cross-View Object Geo-Localization from Multi-Modal Prompts: MoP-UAV Benchmark and MoPT Framework [[aaai]](https://ojs.aaai.org/index.php/AAAI/article/view/38282) `Benchmark` `CLIP+DINOv2`
  - 概览：构建首个支持自然语言、包围框与点击点三类提示的无人机跨视角目标地理定位基准MoP-UAV，并提出MoPT框架，验证多模态联合训练能反哺单模态提示推理。

- **[2026/X][ CVPR 2026 - 聚类遮挡建模的高帧率无人机跟踪 - OCTrack ]** Rethinking Occlusion Modeling for UAV Tracking [[cvf]](https://openaccess.thecvf.com/content/CVPR2026/papers/Zhang_Rethinking_Occlusion_Modeling_for_UAV_Tracking_CVPR_2026_paper.pdf) `End-to-end` `ViT-Tiny`
  - 概览：将航拍遮挡重新建模为空间结构化的聚类过程（COM），并以代价感知深度偏置（CADB）自适应选择ViT推理层数，在四大无人机跟踪基准上以265FPS取得SOTA。

- **[2025/12][ CVPR 2026 - 空中视角3D语义场景补全基准 - OccuFly ]** OccuFly: A 3D Vision Benchmark for Semantic Scene Completion from the Aerial Perspective [[arxiv]](https://arxiv.org/abs/2512.20770) [[hjfy]](https://hjfy.top/arxiv/2512.20770) [[github]](https://github.com/markus-42/occufly) [[project]](https://markus-42.github.io/publications/2026/occufly/) `Benchmark` `Depth-Anything-V2`
  - 概览：构建首个真实世界纯相机空中语义场景补全基准，用三维重建把不足10%的二维标注自动迁移到点云，覆盖城市、工业、乡村三类场景与四季共2万余样本及21类语义，并发布配套深度估计器。

- **[2025/12][ CVPR 2026 - 语义锚定多视图地理定位基础模型 - GeoBridge ]** GeoBridge: A Semantic-Anchored Multi-View Foundation Model Bridging Images and Text for Geo-Localization [[arxiv]](https://arxiv.org/abs/2512.02697) [[hjfy]](https://hjfy.top/arxiv/2512.02697) [[github]](https://github.com/MiliLab/GeoBridge) `End-to-end` `CLIP-L/14`
  - 概览：以大模型生成的视角无关文本描述作为语义锚，把无人机、街景全景与卫星三视图对齐到统一嵌入空间，支持任意视角双向匹配与文本检索，并构建覆盖36国5.2万组三视图的GeoLoc数据集。

- **[2025/11][ AAAI 2026 - UAV场景指代多目标跟踪 - AerialMind ]** AerialMind: Towards Referring Multi-Object Tracking in UAV Scenarios [[arxiv]](https://arxiv.org/abs/2511.21053) [[hjfy]](https://hjfy.top/arxiv/2511.21053) `End-to-end`
  - 概览：提出首个面向无人机场景的大规模指代多目标跟踪（RMOT）基准AerialMind，开发半自动协作标注框架COALA降低标注成本，并提出HawkEyeTrack方法协同增强视觉-语言表征学习，提升UAV场景感知能力。

- **[2025/11][ IEEE IoT-J 2026 - 视觉提示扩散跨视角无人机定位 - DiffusionUavLoc ]** DiffusionUavLoc: Visually Prompted Diffusion for Cross-View UAV Localization [[arxiv]](https://arxiv.org/abs/2511.06422) [[hjfy]](https://hjfy.top/arxiv/2511.06422) `Diffusion` `ControlNet + LoRA`
  - 概览：提出跨视角无人机定位框架DiffusionUavLoc，用免训练几何渲染生成伪卫星图充当视觉提示替代文本条件，结合ControlNet结构约束与自适应小波细节损失，单次前向隐空间检索提速约18倍。

- **[2025/10][ arXiv 2025 - 低空经济无人机识别定位与反制综述 ]** Intelligent Multimodal Multi-Sensor Fusion-Based UAV Identification, Localization, and Countermeasures for Safeguarding Low-Altitude Economy [[arxiv]](https://arxiv.org/abs/2510.22947) [[hjfy]](https://hjfy.top/arxiv/2510.22947) `Survey`
  - 概览：面向低空经济空域安全系统综述无人机管控技术，涵盖射频、雷达、光电与声学的分层融合识别、空天地一体化网络实时定位以及软硬杀伤协同反制的闭环处置框架。

- **[2025/04][ arXiv 2025 - 低空空地协同任务导向通信定位 - O-VIB ]** Task-Oriented Semantic Compression for Localization at the Network Edge [[arxiv]](https://arxiv.org/abs/2504.18317) [[hjfy]](https://hjfy.top/arxiv/2504.18317) [[github]](https://github.com/fangzr/TOC-Edge-Aerial) `End-to-end` `CLIP-ViT` `CARLA`
  - 概览：提出空地协同的任务导向通信视觉定位框架，设计正交约束与ARD自动剪枝的O-VIB压缩编码器并发布35.7万帧五视角无人机数据集，在极低带宽下实现高精度低时延的无GPS定位。

- **[2025/04][ AAAI 2025 - 自提示类比推理的无人机目标检测 - SPAR ]** Self-Prompting Analogical Reasoning for UAV Object Detection [[aaai]](https://ojs.aaai.org/index.php/AAAI/article/view/34026) `End-to-end` `CLIP+YOLO`
  - 概览：提出自提示类比推理框架SPAR，用可学习描述与CLIP文本编码器生成上下文感知提示及目标性分数图，并以类别级与像素级图节点的图卷积推理增强难检小目标的特征表达。

- **[2025/04][ CVPRW 2025 - 反无人机方法、基准与未来方向综述 ]** Securing the Skies: A Comprehensive Survey on Anti-UAV Methods, Benchmarking, and Future Directions [[arxiv]](https://arxiv.org/abs/2504.11967) [[hjfy]](https://hjfy.top/arxiv/2504.11967) [[cvf]](https://openaccess.thecvf.com/content/CVPR2025W/Anti-UAV/papers/Dong_Securing_the_Skies_A_Comprehensive_Survey_on_Anti-UAV_Methods_Benchmarking_CVPRW_2025_paper.pdf) `Survey`
  - 概览：系统综述反无人机领域的分类、检测与跟踪三大目标，横向评测RGB/红外/雷达/射频/音频单模态与多传感器融合方案，梳理扩散生成、视觉-语言建模与强化学习等新兴方向，并指出实时性、隐身目标与集群场景的缺口。

- **[2025/03][ CVPR Findings 2026 - 低空多视角无人机视觉定位基准 - AnyVisLoc ]** Exploring the best way for UAV visual localization under Low-altitude Multi-view Observation Condition: a Benchmark [[arxiv]](https://arxiv.org/abs/2503.10692) [[hjfy]](https://hjfy.top/arxiv/2503.10692) [[github]](https://github.com/UAV-AVL/Benchmark) `Benchmark`
  - 概览：构建覆盖30~300米飞行高度、20°~90°俯仰角的1.8万张实景影像定位数据集AnyVisLoc，统一评测主流检索与匹配算法组合，并提出更贴合定位任务的PDM@K指标。

- **[2025/02][ arXiv 2025 - 无人机场景指代表达理解基准 - RefDrone ]** RefDrone: A Challenging Benchmark for Referring Expression Comprehension in Drone Scenes [[arxiv]](https://arxiv.org/abs/2502.00392) [[hjfy]](https://hjfy.top/arxiv/2502.00392) [[github]](https://github.com/sunzc-sunny/refdrone) `Benchmark` `GroundingDINO`
  - 概览：构建首个无人机视角指代表达理解基准RefDrone（8536张图像、17900条表达），配套多智能体半自动标注框架RDAgent，并提出显式建模目标数量的NGDINO方法应对多目标与无目标样本。

- **[2024/11][ arXiv 2024 - 无人机视角主动目标检测数据集 - UEVAVD ]** UEVAVD: A Dataset for Developing UAV's Eye View Active Object Detection [[arxiv]](https://arxiv.org/abs/2411.04348) [[hjfy]](https://hjfy.top/arxiv/2411.04348) [[github]](https://github.com/Leo000ooo/UEVAVD_dataset) `RL` `SAM+GRU` `AirSim+UE`
  - 概览：发布首个无人机视角主动目标检测数据集UEVAVD，并用GRU序列状态表征与SAM场景预分解引入归纳偏置，提升深度强化学习主动观测策略的零样本泛化能力。

- **[2024/09][ AAAI 2025 - 游戏数据无人机地理定位基准 - Game4Loc ]** Game4Loc: A UAV Geo-Localization Benchmark from Game Data [[arxiv]](https://arxiv.org/abs/2409.16925) [[hjfy]](https://hjfy.top/arxiv/2409.16925) [[github]](https://github.com/Yux1angJi/GTA-UAV) [[project]](https://yux1angji.github.io/game4loc/) `Benchmark`
  - 概览：基于GTAV游戏构建覆盖80~650米多高度多场景的大规模无人机地理定位数据集GTA-UAV，将任务从完美匹配检索扩展到部分匹配与米级定位，并提出加权对比学习Weighted-InfoNCE。

- **[2024/06][ IEEE TGRS 2024 - UCDNet ]** UCDNet: Multi-UAV Collaborative 3D Object Detection Network by Reliable Feature Mapping [[arxiv]](https://arxiv.org/abs/2406.04648) [[hjfy]](https://hjfy.top/arxiv/2406.04648) `End-to-end`
  - 概览：面向多无人机协同的3D目标检测基础工作，创新性引入"对地深度先验"与"同源点几何一致性损失"，解决了远距离空中观测导致跨视图特征对齐困难的问题。

### 6. General VLN & Embodied Navigation

> 本分类共 **561** 篇，因 GitHub Markdown 512KB 渲染限制，已完整移至 [GENERAL_VLN.md](GENERAL_VLN.md)。

## 🔗 Related Works

- [lvkailin0118/Awesome-VLN-Evolution](https://github.com/lvkailin0118/Awesome-VLN-Evolution) — 视觉语言导航发展脉络、论文分类与资源汇总
- [jonyzhang2023/awesome-embodied-vla-va-vln](https://github.com/jonyzhang2023/awesome-embodied-vla-va-vln) — 具身 AI 前沿研究汇总（VLA / VLN / 多模态学习）
- [Hub-Tian/UAVs_Meet_LLMs](https://github.com/Hub-Tian/UAVs_Meet_LLMs) — 无人机 × 大语言模型相关工作
- [Jiaaqiliu/Awesome-VLA-Robotics](https://github.com/Jiaaqiliu/Awesome-VLA-Robotics) — 机器人领域 VLA 论文与资源
- [TheBrainLab/Awesome-VLA-UAVs](https://github.com/TheBrainLab/Awesome-VLA-UAVs) — 面向无人机的 VLA/VLN 资源
- [Sautenich/Awesome-Aerial-Vision-Language-Navigation](https://github.com/Sautenich/Awesome-Aerial-Vision-Language-Navigation) — 空中视觉语言导航资源
- [earth-insights/awesome-uav-vln](https://github.com/earth-insights/awesome-uav-vln) — UAV-VLN 精选集
- [20bytes/Aerial-VLN-Arxiv-Daily](https://github.com/20bytes/Aerial-VLN-Arxiv-Daily) — 每日 arXiv 自动追踪

> **参考来源** — 条目格式与分类体系参考自 [jonyzhang2023/awesome-embodied-vla-va-vln](https://github.com/jonyzhang2023/awesome-embodied-vla-va-vln)；对比表与技术标签徽章排版参考自 [earth-insights/awesome-uav-vln](https://github.com/earth-insights/awesome-uav-vln)。特此致谢。

> [!NOTE]
> **版本说明** — 本仓库为公开维护版本，与内部目录同步更新。

---

<sub>本仓库内容以 [MIT License](./LICENSE) 发布 © 2026 20bytes；论文版权归原作者及出版方所有，本库仅作学习与研究索引。</sub>
