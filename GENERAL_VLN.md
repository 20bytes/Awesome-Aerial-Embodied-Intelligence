# 📌 6. General VLN & Embodied Navigation

[← 返回主目录](README.md)

> 收录室内/地面 VLN、ObjectNav、ImageNav、具身问答与非空中主场景导航基准；条目格式与主目录一致。

- **[2026/07][ arXiv 2026 - 通信辅助社交导航 - Robots Ask the Way ]** Robots Ask the Way: Communication-Enabled Social Navigation [[arxiv]](https://arxiv.org/abs/2607.01044) [[hjfy]](https://hjfy.top/arxiv/2607.01044) `Agentic`
  - 概览：提出通信赋能社交导航CommNav，使机器人主动向居民询问目标人物的近期位置与移动线索；同时扩展Habitat 3.0为支持多人物信息交换的Habitat 3.0c，并以COMM模块把结构化或自然语言回答接入导航策略。

- **[2026/07][ arXiv 2026 - 扇区流场解耦高层推理与底层执行 - CoFL-S ]** CoFL-S: Spatially Queryable Sector Flow Fields for Local Language-Conditioned Navigation [[arxiv]](https://arxiv.org/abs/2607.02222) [[hjfy]](https://hjfy.top/arxiv/2607.02222) `Zero-Shot`
  - 概览：提出CoFL-S，从第一人称RGB-D和局部子指令预测可空间查询的扇区流场，并通过场积分生成连续轨迹；训练时把VLN-CE回合转换为逐帧子指令、动作、轨迹和稠密流场监督，评测则以连续时间Habitat控制接口隔离高层分解与底层控制。

- **[2026/07][ arXiv 2026 - 从区域抵达走向实例级目标落地 ]** From Region Arrival to Instance-Level Grounding in Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2607.03792) [[hjfy]](https://hjfy.top/arxiv/2607.03792) `End-to-end`
  - 概览：形式化VLN的“最后3米实例落地鸿沟”，以距离精度、目标可见性和终止视图落地三项指标评测；进一步提出REALM可见性感知停止模块，并构建含18万条短时域样本的REVERIE-AIM用于精细目标接近。

- **[2026/07][ arXiv 2026 - 统一 MLLM 框架实现移动操作精准位姿推理 - UniLM-Nav ]** UniLM-Nav: A Unified Framework for Zero-Shot Last-Mile Navigation [[arxiv]](https://arxiv.org/abs/2607.06537) [[hjfy]](https://hjfy.top/arxiv/2607.06537) `Zero-Shot`
  - 概览：提出UniLM-Nav零样本最后一米导航框架，以共享MLLM依次选择最能观察目标的参考视图、落地任务相关可供性点并转换到机器人坐标系，再结合任务上下文与机器人几何推断可执行操作的基座位姿。

- **[2026/07][ arXiv 2026 - 四足机器人行为基础模型 - ABot-C0 ]** Behavior Foundations for Quadruped Robots: ABot-C0 Technical Report [[arxiv]](https://arxiv.org/abs/2607.07370) [[hjfy]](https://hjfy.top/arxiv/2607.07370) `Flow Matching`
  - 概览：提出ABot-C0四足机器人通用运动控制系统，以多源运动数据金字塔、流匹配通用策略和感知式全地形训练统一动作跟踪、移动与场景交互，并通过部署栈实现多策略平滑切换和安全实机运行。

- **[2026/07][ arXiv 2026 - 方向感知与自动纠错城市导航 - DA-Nav ]** DA-Nav: Direction-Aware City-Scale Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2607.11638) [[hjfy]](https://hjfy.top/arxiv/2607.11638) `End-to-end`
  - 概览：提出DA-Nav方向感知城市VLN框架，将粗粒度道路方向指令转化为自中心图像网格目标，并通过链式推理依次判断路线偏差、选择修正动作和定位目标区域。

- **[2026/07][ arXiv 2026 - 反思推理缓解长时序视觉导航漂移 - ReflectVLN ]** ReflectVLN: Training Vision-Language Navigation Agents with Reflective Reasoning [[arxiv]](https://arxiv.org/abs/2607.12680) [[hjfy]](https://hjfy.top/arxiv/2607.12680) `Agentic`
  - 概览：提出ReflectVLN双智能体闭环：意图智能体分解子任务并生成纠正计划，执行智能体依据当前观测输出短时动作、监测进度与偏航，再用进度和偏差信号按需触发高层反思；Action-CoT以路径条件双查询训练动作生成。

- **[2026/07][ arXiv 2026 - 将3D场景Token注入VLM，消除文本带来的空间信息损耗 - SoftNav ]** SoftNav: Injecting 3D Scene Tokens into VLMs for Embodied Navigation [[arxiv]](https://arxiv.org/abs/2607.14586) [[hjfy]](https://hjfy.top/arxiv/2607.14586) `Zero-Shot`
  - 概览：提出SoftNav，将每个检测物体或探索边界的连续3D表示经轻量投影器变为软令牌，直接注入冻结VLM的隐藏空间，以嵌入级传输替代有损的场景文本序列化。

- **[2026/07][ arXiv 2026 - 室内外连续导航仿真基准 - NavVerse ]** NavVerse: Benchmarking Indoor-to-Outdoor Embodied Navigation in Continuous Robot Simulation [[arxiv]](https://arxiv.org/abs/2607.19695) [[hjfy]](https://hjfy.top/arxiv/2607.19695) `Benchmark`
  - 概览：构建NavVerse统一机器人导航仿真基准，在同一物理、感知与控制框架中连接室内、城市户外及室内外互通场景，并支持多种轮式和四足机器人。

- **[2026/07][ Preprints 2026 - 从指令跟随到认知导航综述 ]** From Instruction Following to Cognitive Navigation: A Survey on the Evolution of Vision-and-Language Navigation [[doi]](https://doi.org/10.20944/preprints202606.2231.v1) [[github]](https://github.com/lvkailin0118/Awesome-VLN-Evolution) `Survey`
  - 概览：以感知、认知、学习和泛化四层能力演进框架重构VLN研究脉络，覆盖空间理解、世界模型、强化学习、持续学习及可信开放世界部署。

- **[2026/07][ RSS 2026 - 时空语义SLAM视觉语言导航 - SuperMap ]** SuperMap: A Spatio-Temporal SLAM System for Visual-Language Navigation [[rss]](https://www.roboticsproceedings.org/rss22/p052.pdf) `SLAM`
  - 概览：提出面向动态环境的实时开放词汇时空语义SLAM，通过跨帧实例关联、变化感知更新和四维场景图，为语言查询、历史关系推理及零样本导航提供地图记忆。

- **[2026/06][ NeurIPS 2025 - 层级语义图最优传输VLN - HSAN ]** Hierarchical Semantic-Augmented Navigation: Optimal Transport and Graph-Driven Reasoning for Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2606.01565) [[hjfy]](https://hjfy.top/arxiv/2606.01565) [[openreview]](https://openreview.net/forum?id=ypVW5jvguX) `GSM+RL`
  - 概览：提出HSAN框架，动态构建物体-区域-分区三级语义场景图，采用基于Kantorovich对偶的最优传输拓扑规划器选择长期目标，并以图感知强化学习策略实现连续环境VLN的鲁棒控制。

- **[2026/06][ arXiv 2026 - 层次语义几何地图 - HSGM ]** Bridging the 2D-3D Gap: A Hierarchical Semantic-Geometric Map for Vision Language Navigation [[arxiv]](https://arxiv.org/abs/2606.00095) [[hjfy]](https://hjfy.top/arxiv/2606.00095) `Semantic-Geometric Map`
  - 概览：构建几何、语义和决策三层地图并栅格化为VLM可读的二维鸟瞰图，将高层航点选择与A*低层无碰撞控制解耦，实现免训练连续VLN。

- **[2026/06][ arXiv 2026 - 概率场景图多世界决策 - PSG-Nav ]** PSG-Nav: Probabilistic Scene Graph Navigation via Multiverse Decision Making [[arxiv]](https://arxiv.org/abs/2606.01313) [[hjfy]](https://hjfy.top/arxiv/2606.01313) `GSM`
  - 概览：提出PSG-Nav，以完整类别概率分布构建三维概率场景图，再从联合分布采样多个高概率世界设定并按跨世界兼容性选择导航地标；同时用证据式经验校准器依据历史成败记忆在线抑制开放词汇误检。

- **[2026/06][ arXiv 2026 - 像素目标落地与关键帧记忆 - Goal2Pixel ]** Goal2Pixel: Grounding Goals to Pixels for Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2606.01621) [[hjfy]](https://hjfy.top/arxiv/2606.01621) `End-to-end`
  - 概览：提出Goal2Pixel像素级VLN接口和ViKeyMem可见性感知关键帧记忆，将导航动作统一为图像像素目标预测，并以少量历史帧支撑长程决策。

- **[2026/06][ arXiv 2026 - 自演化细粒度记忆零样本导航 - EvoMemNav ]** EvoMemNav: Efficient Self-Evolving Fine-Grained Memory for Zero-Shot Embodied Navigation [[arxiv]](https://arxiv.org/abs/2606.03509) [[hjfy]](https://hjfy.top/arxiv/2606.03509) `Zero-Shot`
  - 概览：提出EvoMemNav自演化细粒度记忆框架，持续提炼和更新导航经历中的空间语义证据，以提升零样本具身导航的长期决策能力。

- **[2026/06][ arXiv 2026 - 轨迹中心航点视觉语言导航 - Beyond Waypoints ]** Beyond Waypoints: A Trajectory-Centric Waypointing Paradigm for Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2606.07244) [[hjfy]](https://hjfy.top/arxiv/2606.07244) `Diffusion`
  - 概览：提出Trajectory Waypoint范式，以TSDF引导的扩散策略直接生成无碰撞候选轨迹及其终点，并由轨迹增强导航器把整段可执行路径纳入高层选择，使语义决策与低层控制保持一致。

- **[2026/06][ arXiv 2026 - 在线空间认知记忆零样本导航 - SpaceVLN ]** SpaceVLN: A Zero-Shot Vision-and-Language Navigation Agent with Online Spatial Cognitive Memory and Reasoning [[arxiv]](https://arxiv.org/abs/2606.08992) [[hjfy]](https://hjfy.top/arxiv/2606.08992) `Zero-Shot`
  - 概览：提出SpaceVLN，以空间航点和子任务地标证据逐步构建层次空间认知记忆，再由Spatial-CoT结合任务进度、空间感知、分析与预测组织可验证的“空间—地标”规划执行阶段。

- **[2026/06][ arXiv 2026 - 面向机器人导航的度量感知视觉几何框架 - VGP-Nav ]** VGP-Nav: Metric-Aware Visual Geometric Perception for Robot Navigation [[arxiv]](https://arxiv.org/abs/2606.09268) [[hjfy]](https://hjfy.top/arxiv/2606.09268) `End-to-end`
  - 概览：提出VGP-Nav单目度量几何感知框架，以地平面几何提供物理尺度锚点，在线消除单目尺度歧义，并联合输出全局度量定位与可供规划使用的稠密障碍表示。

- **[2026/06][ arXiv 2026 - 双关系归纳偏置零样本具身导航 ]** Rethinking Embodied Navigation via Relational Inductive Bias [[arxiv]](https://arxiv.org/abs/2606.10348) [[hjfy]](https://hjfy.top/arxiv/2606.10348) `End-to-end`
  - 概览：提出DB-Nav，把目标关系分解为传播上下文证据的激活偏置和抑制误检、过时先验及失败区域的抑制偏置，并在关系激活—抑制探索图中用在线观测和失败访问共同调制前沿价值。

- **[2026/06][ arXiv 2026 - 把视觉语言导航变成VLM的工具调用任务 - AgenticNav ]** AgenticNav: Zero-Shot Vision-and-Language Navigation as a Tool-Calling Harness [[arxiv]](https://arxiv.org/abs/2606.10577) [[hjfy]](https://hjfy.top/arxiv/2606.10577) `Zero-Shot`
  - 概览：提出AgenticNav工具调用式零样本VLN框架：VLM以像素目标工具生成可执行运动、按需查询目标像素的度量深度，并通过轨迹地图与视觉回忆工具选择性访问历史观测，无需训练航点预测器。

- **[2026/06][ arXiv 2026 - 仅输入一次目标，零样本穿越复杂迷宫死局 - GUIDE ]** GUIDE: Goal-Initialized Directional Understanding for End-to-End Visual Navigation [[arxiv]](https://arxiv.org/abs/2606.10832) [[hjfy]](https://hjfy.top/arxiv/2606.10832) `RL`
  - 概览：提出GUIDE目标初始化视觉导航任务与端到端方向理解策略，使智能体只在起始时接收目标提示，随后依靠观测历史维持目标方向并完成长程导航。

- **[2026/06][ arXiv 2026 - 单目跨本体自适应导航 - AgniNav ]** AgniNav: Configuration-Driven Cross-Embodiment Local Planning for Robot Navigation [[arxiv]](https://arxiv.org/abs/2606.10903) [[hjfy]](https://hjfy.top/arxiv/2606.10903) `End-to-end`
  - 概览：提出AgniNav跨本体局部导航框架，用高度、前后长度和半宽四项碰撞包络参数共同配置感知与规划：高度条件网络从单目RGB预测碰撞相关伪激光，其余尺寸参数驱动局部碰撞检查。

- **[2026/06][ arXiv 2026 - 全天候在线强化学习与终身导航 - AllDayNav ]** AllDayNav: Lifelong Navigation via Real-World Reinforcement Learning [[arxiv]](https://arxiv.org/abs/2606.10927) [[hjfy]](https://hjfy.top/arxiv/2606.10927) `RL`
  - 概览：提出AllDayNav真实世界终身导航方案，通过持续强化学习适应昼夜、天气与场景变化，并在长期部署中更新导航策略。

- **[2026/06][ arXiv 2026 - VLM自主关键线索发现 - Foresight ]** Foresight: Iterative Reasoning About Clues that Matter for Navigation [[arxiv]](https://arxiv.org/abs/2606.12550) [[hjfy]](https://hjfy.top/arxiv/2606.12550) `RL`
  - 概览：提出Foresight测试时计划-批判循环，让VLM交替生成图像空间运动计划并依据语言目标和视觉线索批判修正，再以人类反馈奖励模型和强化学习对齐开放集导航行为。

- **[2026/06][ arXiv 2026 - 平面图引导多模态导航 - FloVerse ]** FloVerse: Floor Plan-Guided Multi-Modal Navigation [[arxiv]](https://arxiv.org/abs/2606.14267) [[hjfy]](https://hjfy.top/arxiv/2606.14267) `Benchmark`
  - 概览：提出同时覆盖点目标、物体目标与图像目标的平面图引导导航任务和FloVerse-1.6K数据集，并以双阶段ThreeDiff结合全局平面图与局部RGB-D几何。

- **[2026/06][ arXiv 2026 - 自进记忆与主动预判零样本导航 - EvolveNav ]** EvolveNav: Proactive Preflection and Self-Evolving Memory for Zero-Shot Object Goal Navigation [[arxiv]](https://arxiv.org/abs/2606.18235) [[hjfy]](https://hjfy.top/arxiv/2606.18235) `Zero-Shot`
  - 概览：提出EvolveNav零样本目标导航框架，从历史成功与失败轨迹提取可执行规则，并以置信上界兼顾语义相关性与历史成功率进行检索，再由记忆引导的预反思模块在行动前预测结果。

- **[2026/06][ arXiv 2026 - 空间碰撞感知规划器赋能长距离自主导航 - SCAN-Planner ]** SCAN-Planner: Spatial Collision-Aware Local Planning for Route-Guided Long-Range Quadruped Navigation [[arxiv]](https://arxiv.org/abs/2606.19555) [[hjfy]](https://hjfy.top/arxiv/2606.19555) `End-to-end`
  - 概览：提出SCAN-Planner，以偏航感知双圆柱足迹在膨胀3D占据图中检查全身碰撞，以投影A*在地形表面生成引导路径，并用机器人中心滑动地图和边界回退支持长程四足导航与局部死路恢复。

- **[2026/06][ arXiv 2026 - 抗延迟VLM增强城市导航 - Slow Brain, Fast Planner ]** Slow Brain, Fast Planner: Latency-Resilient VLM-Augmented Urban Navigation [[arxiv]](https://arxiv.org/abs/2606.20458) [[hjfy]](https://hjfy.top/arxiv/2606.20458) `End-to-end`
  - 概览：提出免训练的VLM增强城市导航方法，通过Score Fusion与Probability Fusion把延迟返回的VLM轨迹选择融合进实时规划器评分，在不微调模型的情况下提升长延迟场景中的规划鲁棒性。

- **[2026/06][ arXiv 2026 - 时序条件流视觉复原 - FlowDec ]** FlowDec: Temporal Conditional Flow Decorruptor for Robust Continuous Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2606.22424) [[hjfy]](https://hjfy.top/arxiv/2606.22424) `End-to-end`
  - 概览：提出FlowDec导航图像复原框架，以混合时序条件把生成流路径与历史观测对齐，再用动作质心引导过滤动态评估并融合复原结果，为受视觉损坏的连续VLN提供实时输入修复。

- **[2026/06][ arXiv 2026 - 跨视角空间推理与想象基准 - CVSBench ]** CVSBench: A Comprehensive Benchmark for Cross-view Spatial Reasoning and Dreaming [[arxiv]](https://arxiv.org/abs/2606.22476) [[hjfy]](https://hjfy.top/arxiv/2606.22476) `Benchmark`
  - 概览：构建CVSBench卫星-街景跨视角空间推理基准，覆盖问答、目标定位和视角识别，并验证显式三维场景想象对VLM保持物体与布局一致性的作用。

- **[2026/06][ arXiv 2026 - 人形机器人有限感知导航避障一体化框架 - LP-NavOA ]** LP-NavOA: Integrated Local Navigation and Obstacle Avoidance for Humanoid Robots under Limited Perception [[arxiv]](https://arxiv.org/abs/2606.23249) [[hjfy]](https://hjfy.top/arxiv/2606.23249) `RL`
  - 概览：提出LP-NavOA有限感知人形导航框架，先训练带共享安全过滤器的PPO全身运动策略，再用A*与航点教师轨迹蒸馏循环局部规划器；部署时仅凭本体感、短距测距和机体坐标系目标方向改写航向指令。

- **[2026/06][ arXiv 2026 - 机器人与监控系统协同目标导航 - SurveilNav ]** SurveilNav: Collaborative Object Goal Navigation with Robot and Surveillance System [[arxiv]](https://arxiv.org/abs/2606.25119) [[hjfy]](https://hjfy.top/arxiv/2606.25119) `GSM`
  - 概览：构建含206个监控点、74个楼层和1,000个回合的机器人—监控协同导航数据集，并提出SurveilNav，以主动相机调度、联合2D/3D建图、VLM价值估计和协同目标验证融合机器人局部视角与监控全局视角。

- **[2026/06][ arXiv 2026 - 视觉时空记忆长程导航 - RAVEN ]** RAVEN: Long-Horizon Reasoning & Navigation with a Visuo-Spatio-Temporal Memory [[arxiv]](https://arxiv.org/abs/2606.25206) [[hjfy]](https://hjfy.top/arxiv/2606.25206) `Agentic`
  - 概览：提出RAVEN视—时—空记忆系统，把视觉嵌入、位姿和时间戳存入向量数据库，并以空间地图约束检索，用于长时域问答与自然语言目标导航，避免图像转字幕造成的信息损失。

- **[2026/06][ arXiv 2026 - LLM分层规划与场景图对齐 - SAGE-Nav ]** SAGE-Nav: Leveraging LLM Planning and Alignment Fusion for Hierarchical Scene Graph-Guided Navigation [[arxiv]](https://arxiv.org/abs/2606.25497) [[hjfy]](https://hjfy.top/arxiv/2606.25497) `Zero-Shot`
  - 概览：提出SAGE-Nav分层框架，由LLM把目标指令拆为语义航点并异步进行全局规划，HSGE以关系图卷积编码场景图的语义与空间拓扑，GAFN再通过自适应门控把结构先验与实时感知融合给低层策略。

- **[2026/06][ arXiv 2026 - 文本驱动的社交机器人仿真框架 - GROVE ]** GROVE: Grounded Pedestrian Simulation via Natural Language for Interactive Social Robot Navigation [[arxiv]](https://arxiv.org/abs/2606.25504) [[hjfy]](https://hjfy.top/arxiv/2606.25504) `End-to-end`
  - 概览：提出GROVE自然语言驱动的行人仿真生成框架，联合语义推理、行为规划与几何运动规划，将文本场景描述转换为可在Isaac Sim、Gazebo和ROS2中执行的行人行为。

- **[2026/06][ arXiv 2026 - 意图感知人群视觉导航 ]** Learning Robot Visual Navigation in Crowds via Intention-Aware Scene Representations [[arxiv]](https://arxiv.org/abs/2606.26047) [[hjfy]](https://hjfy.top/arxiv/2606.26047) `RL`
  - 概览：提出iCrowdNav视觉人群导航方法，以时空编码器提取场景占据结构，并用Intent-Interact Former从人体姿态推断行人运动意图；两类特征融合为紧凑状态后训练深度强化学习策略。

- **[2026/06][ arXiv 2026 - 真实人群导航场景生成与Sim-to-Real - NavIsaacLab ]** NavIsaacLab: Generating Realistic Crowd via Parallel Robot Learning for Benchmarking Human-aware Navigation [[arxiv]](https://arxiv.org/abs/2606.26265) [[hjfy]](https://hjfy.top/arxiv/2606.26265) `Benchmark`
  - 概览：提出基于Isaac Lab的NavIsaacLab仿真平台，支持GPU并行的照片级渲染与物理动力学仿真，提供关节级可控的高保真行人仿真能力。

- **[2026/06][ arXiv 2026 - 序数神经坍缩先验视觉导航 ]** Ordinal Neural Collapse as a Representation Prior for Visual Navigation [[arxiv]](https://arxiv.org/abs/2606.26839) [[hjfy]](https://hjfy.top/arxiv/2606.26839) `Diffusion`
  - 概览：提出ORION序数神经坍缩先验，将从“远左”到“远右”的导航动作类沿单一判别轴按顺序排列并抑制类内离轴方差，再把预训练编码器接入扩散式导航策略联合微调。

- **[2026/06][ arXiv 2026 - 端侧小模型物体目标导航 - LocalNav ]** LocalNav: Distilling Frontier VLMs and Embodied RL for On-Device Object Goal Navigation [[arxiv]](https://arxiv.org/abs/2606.27871) [[hjfy]](https://hjfy.top/arxiv/2606.27871) `GSM`
  - 概览：提出LocalNav端侧物体目标导航方法，将前沿视觉语言模型的语义能力蒸馏到轻量VLM，并结合具身强化学习，使本地模型在受限算力上完成开放词汇导航。

- **[2026/06][ arXiv 2026 - 上下文记忆强化学习规划 - CORE ]** CORE Planner: Contextual-memory Oriented Reinforcement-learning in Unknown Environments for Robot Navigation [[arxiv]](https://arxiv.org/abs/2606.29222) [[hjfy]](https://hjfy.top/arxiv/2606.29222) `RL`
  - 概览：将可视图与上下文历史记忆结合，并以动态图稀疏化保持大场景实时性；强化学习策略可缓解未知环境中的死锁震荡并实现零样本仿真到现实迁移。

- **[2026/06][ arXiv 2026 - 人类活动规律预测具身导航 - HUMEMBR ]** HUMEMBR: Learning Human Routines for Predictive Embodied Navigation [[arxiv]](https://arxiv.org/abs/2606.30404) [[hjfy]](https://hjfy.top/arxiv/2606.30404) `End-to-end`
  - 概览：提出HUMEMBR人类规律记忆系统，以持续记忆构建并行配合检索和查询，把长期观测整理为结构化人物日常规律，用于回答人物位置、时间习惯等问题并执行规律条件导航。

- **[2026/06][ TPAMI 2026 - 多目标导航动态权重优化 - GDWO ]** Goal-Oriented Dynamic Weight Optimization for Multi-Object Navigation [[doi]](https://doi.org/10.1109/TPAMI.2026.3657778) `Multi-Object Nav`
  - 概览：提出GDWO，将连续多目标的价值损失置于统一优化空间，并按梯度与各目标成功率动态调整权重，使策略优先改善困难子目标并缓解稀疏奖励下的局部最优。

- **[2026/06][ ACM ICMR 2026 - 偏好引导语义推理目标导航 - PRISM ]** PRISM: Preference-Guided Semantic Reasoning with Vision-Language Models for Object Goal Navigation [[doi]](https://doi.org/10.1145/3805622.3810883) `Zero-shot`
  - 概览：以偏好引导语义地图统一连续信念场和层次拓扑记忆，并用自适应探索策略按不确定性选择性调用VLM，在无需端到端训练的条件下提升目标导航。

- **[2026/06][ CVPR 2026 - 无地图自动驾驶视觉语言导航 - DriveVLN ]** DriveVLN: Towards Mapless Vision-and-Language Navigation in Autonomous Driving [[cvf]](https://openaccess.thecvf.com/content/CVPR2026/html/Guo_DriveVLN_Towards_Mapless_Vision-and-Language_Navigation_in_Autonomous_Driving_CVPR_2026_paper.html) `Autonomous Driving`
  - 概览：定义无高精地图的自动驾驶视觉语言导航任务，在CARLA构建200个数字孪生场景，并以候选轨迹规划器和多模态路线选择器结合监督与强化学习完成导航。

- **[2026/06][ CVPR 2026 - 想象引导生成式图像目标导航 - GeniNav ]** GeniNav: Generative Model Driven Image-Goal Navigation via Imagination-Guided Consistency Flow Matching [[cvf]](https://openaccess.thecvf.com/content/CVPR2026/html/Chen_GeniNav_Generative_Model_Driven_Image-Goal_Navigation_via_Imagination-Guided_Consistency_Flow_CVPR_2026_paper.html) [[project]](https://cyq638.github.io/geninav/) `Flow Matching`
  - 概览：以VLM生成隐式语义子目标，以一致性流匹配产生候选轨迹，再联合语义、几何安全和可见性排序；同时提供大规模闭环图像目标导航基准。

- **[2026/05][ ICLR 2026 - 不确定性感知高斯地图VLN ]** Uncertainty-Aware Gaussian Map for Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2605.26503) [[hjfy]](https://hjfy.top/arxiv/2605.26503) [[openreview]](https://openreview.net/forum?id=LPv59noPAy) [[github]](https://github.com/Gaozzzz/Uncertainty-Aware-VLN) `GSM` `3DGS`
  - 概览：提出不确定性感知的语义高斯地图导航框架，用可微3D高斯基元显式建模几何、语义与外观三类感知不确定性并纳入智能体观测空间，实现部分可观测环境下更可靠的导航决策。

- **[2026/05][ ICCV 2025 - 开放集语义分组3D高斯地图导航 ]** 3D Gaussian Map with Open-Set Semantic Grouping for Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2605.26500) [[hjfy]](https://hjfy.top/arxiv/2605.26500) [[github]](https://github.com/Gaozzzz/3D-Gaussian-Map-VLN) `GSM`
  - 概览：将环境表示为可微3D高斯并在线构建自中心场景地图，通过开放集语义分组将高斯基元聚合为物体实例与场景类别，结合多层级动作预测提升VLN在未见环境中的泛化能力。

- **[2026/05][ arXiv 2026 - 用几何-语义经验检索，实现智能体终身导航学习 - TrajRAG ]** TrajRAG: Retrieving Geometric-Semantic Experience for Zero-Shot Object Navigation [[arxiv]](https://arxiv.org/abs/2605.01700) [[hjfy]](https://hjfy.top/arxiv/2605.01700) `Zero-Shot`
  - 概览：提出TrajRAG，将历史回合压缩为同时编码空间布局与语义的拓扑—极坐标轨迹，并以层次分块汇总相似经验；导航时由候选前沿生成轨迹假设，粗到细检索相似经历辅助大模型选择航点。

- **[2026/05][ arXiv 2026 - 比较式消歧框架，解决机器人模糊导航难题 - ProCompNav ]** ProCompNav: Proactive Instance Navigation with Comparative Judgment for Ambiguous User Queries [[arxiv]](https://arxiv.org/abs/2605.06223) [[hjfy]](https://hjfy.top/arxiv/2605.06223) `End-to-end`
  - 概览：提出ProCompNav两阶段实例导航框架，先探索并建立候选实例池，再在每轮抽取可划分当前候选池的属性—值对，向用户提出是非问题并一次删除所有不一致候选，直至消除目标歧义。

- **[2026/05][ arXiv 2026 - 顶视图单步全局VLN规划 - NavOne ]** NavOne: One-Step Global Planning for Vision-Language Navigation on Top-Down Maps [[arxiv]](https://arxiv.org/abs/2605.06317) [[hjfy]](https://hjfy.top/arxiv/2605.06317) `End-to-end`
  - 概览：提出Top-Down VLN，把导航改写为预建顶视地图上的单步全局路径规划，并构建R2R-TopDown；NavOne以多模态顶视图融合器和空间感知深度混合模块一次前向预测整张地图的稠密路径概率。

- **[2026/05][ arXiv 2026 - 候选感知几何增强拓扑规划 - LCGNav ]** LCGNav: Local Candidate-Aware Geometric Enhancement for General Topological Planning in Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2605.09053) [[hjfy]](https://hjfy.top/arxiv/2605.09053) `End-to-end`
  - 概览：提出LCGNav局部候选感知的几何增强模块，在不改变既有拓扑规划器主体的情况下补充候选航点关系，可直接接入ETPNav、BEVBert和DGNav等VLN方法。

- **[2026/05][ arXiv 2026 - 通用机器人导航统一基准 - OmniNavBench ]** Beyond Isolation: A Unified Benchmark for General-Purpose Navigation [[arxiv]](https://arxiv.org/abs/2605.09441) [[hjfy]](https://hjfy.top/arxiv/2605.09441) `Benchmark`
  - 概览：构建OmniNavBench通用导航基准，以复合指令联合评测多种导航技能及其时序协同能力，并提供专家轨迹、指令、统一仿真接口和跨任务模型分析。

- **[2026/05][ arXiv 2026 - 语义执行控制一招补齐动作一致性缺口 - ConsistNav ]** ConsistNav: Closing the Action Consistency Gap in Zero-Shot Object Navigation with Semantic Executive Control [[arxiv]](https://arxiv.org/abs/2605.09869) [[hjfy]](https://hjfy.top/arxiv/2605.09869) `Zero-Shot`
  - 概览：提出ConsistNav免训练目标导航框架，以有限状态执行器控制语义阶段、持久候选记忆跨帧累积目标证据，并用稳定性感知动作控制抑制旋转停滞、无效追逐和未经验证的提前停止。

- **[2026/05][ arXiv 2026 - TinyML地形分割微型机器人导航 - Nano-U ]** Nano-U: Efficient Terrain Segmentation for Tiny Robot Navigation [[arxiv]](https://arxiv.org/abs/2605.10210) [[hjfy]](https://hjfy.top/arxiv/2605.10210) `End-to-end`
  - 概览：提出Nano-U微型地形分割网络，以量化感知蒸馏补偿极小模型容量，并通过MicroFlow部署到ESP32-S3，为资源受限机器人提供低内存、低延迟的可通行区域感知。

- **[2026/05][ arXiv 2026 - 在线模仿学习跨域导航 - NavOL ]** NavOL: Navigation Policy with Online Imitation Learning [[arxiv]](https://arxiv.org/abs/2605.11762) [[hjfy]](https://hjfy.top/arxiv/2605.11762) `Zero-Shot`
  - 概览：提出NavOL在线模仿学习框架，以预训练扩散策略根据局部观测预测未来航点；滚动时策略在模拟器中行动并向拥有全局信息的规划器查询最优路径片段，随后用在线收集的观测—轨迹对持续更新。

- **[2026/05][ arXiv 2026 - 人本语义几何推理VLN - HCSG ]** HCSG: Human-Centric Semantic-Geometric Reasoning for Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2605.13321) [[hjfy]](https://hjfy.top/arxiv/2605.13321) `GSM`
  - 概览：提出HCSG人本VLN框架，以几何分支预测人体姿态与轨迹、VLM分支描述人的动作和意图，再把语义—几何表示融合进拓扑图进行指令条件规划，并用社交距离损失约束交互距离。

- **[2026/05][ arXiv 2026 - 立体视觉具身导航Sim-to-Real研究 ]** What Limits Vision-and-Language Navigation ? [[arxiv]](https://arxiv.org/abs/2605.13328) [[hjfy]](https://hjfy.top/arxiv/2605.13328) `Benchmark`
  - 概览：提出StereoNav视觉语言动作框架，用目标位置先验在仿真与现实间提供稳定视觉锚点以处理欠明确指令，并以立体视觉联合编码语义与几何，缓解光照变化和运动模糊下的空间落地不稳定。

- **[2026/05][ arXiv 2026 - 深挖VLM-LLM零样本视觉导航的核心性能瓶颈 ]** Exploring Bottlenecks in VLM-LLM Navigation: How 3D Scene Understanding Capability Impacts Zero-Shot VLN [[arxiv]](https://arxiv.org/abs/2605.14801) [[hjfy]](https://hjfy.top/arxiv/2605.14801) `Zero-Shot`
  - 概览：量化三维场景理解对零样本VLN的影响，分别为依赖拓扑地图语义的慢速LLM规划器和依赖坐标、包围框执行决策的快速反应导航器推导成功率上界，并观察到感知精度超过阈值后导航收益递减。

- **[2026/05][ arXiv 2026 - 系统级强化学习导航Sim-to-Real框架 - NavRL++ ]** NavRL++: A System-Level Framework for Improving Sim-to-Real Transfer in Reinforcement Learning-Based Robot Navigation [[arxiv]](https://arxiv.org/abs/2605.15559) [[hjfy]](https://hjfy.top/arxiv/2605.15559) `Zero-Shot`
  - 概览：提出NavRL++强化学习导航训练—部署管线，系统分离传感噪声、感知故障、系统时延和控制响应等迁移因素，并以扰动感知后训练和基于短时观测的Transformer策略增强实机控制鲁棒性。

- **[2026/05][ arXiv 2026 - 快慢双系统长程VLN - SEDualVLN ]** SEDualVLN: A Spatially-Enhanced Dual-System for Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2605.17249) [[hjfy]](https://hjfy.top/arxiv/2605.17249) `Zero-Shot`
  - 概览：提出SEDualVLN双系统框架：系统一以兼具全局和局部空间感知的VLM生成动作，系统二让通用MLLM结合实时三维地图的俯视图和渲染路径图像规划航点，再以快慢协同完成导航。

- **[2026/05][ arXiv 2026 - 全景-俯视双级零样本视觉语言导航 - P2DNav ]** P2DNav: Panorama-to-Downview Reasoning for Zero-shot Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2605.19634) [[hjfy]](https://hjfy.top/arxiv/2605.19634) `Zero-Shot`
  - 概览：提出P2DNav，先在360°全景中选择指令相关方向，再于对应下视RGB图像上预测像素级局部目标；滑窗对话记忆保存近期历史，反思重定向模块在局部落地不可靠时返回全景方向选择。

- **[2026/05][ arXiv 2026 - 基于可通行感知3D规划的跨楼层零样本目标搜索 - TravExplorer ]** TravExplorer: Cross-Floor Embodied Exploration via Traversability-Aware 3-D Planning [[arxiv]](https://arxiv.org/abs/2605.19958) [[hjfy]](https://hjfy.top/arxiv/2605.19958) `Zero-Shot`
  - 概览：提出TravExplorer跨楼层探索框架，以统一体素地图表示地面、楼梯与平台等可通行支撑面，并结合语义目标引导、视场感知主动观测和足点约束三维规划执行开放词汇目标搜索。

- **[2026/05][ arXiv 2026 - 几何感知BEV高效VLN - GA-VLN ]** GA-VLN: Geometry-Aware BEV Representation for Efficient Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2605.22036) [[hjfy]](https://hjfy.top/arxiv/2605.22036) `BEV`
  - 概览：构建融合显式深度几何与三维大模型先验的GA-BEV表征，在显著压缩视觉Token的同时保留可通行结构，并支持高效连续视觉语言导航。

- **[2026/05][ arXiv 2026 - 自感知推理视觉语言导航 - AwareVLN ]** AwareVLN: Reasoning with Self-awareness for Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2605.22816) [[hjfy]](https://hjfy.top/arxiv/2605.22816) `End-to-end`
  - 概览：提出AwareVLN端到端自感知导航框架，以结构化推理模块显式建模智能体状态、空间关系和任务进度，并通过带进度分段的自动数据引擎生成训练监督，无需显式三维地图。

- **[2026/05][ arXiv 2026 - 检索增强户外地理推理与动态规划 - G-DRAGON ]** G-DRAGON: Geospatial Reasoning and Dynamic Planning for Retrieval-Augmented Outdoor Navigation [[arxiv]](https://arxiv.org/abs/2605.25646) [[hjfy]](https://hjfy.top/arxiv/2605.25646) `Agentic`
  - 概览：提出G-DRAGON户外导航框架，以受约束生成式检索把自然语言映射到本地版本化OSM实体和坐标，由高层规划器把全局拓扑路线投影到SLAM可行空间，最后切换到前沿探索与开放集语义体素图定位目标。

- **[2026/05][ arXiv 2026 - 真实商圈POI末段导航 - POINav ]** POINav: Benchmarking and Enhancing Final-Meters Arrival in Real-World Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2605.28237) [[hjfy]](https://hjfy.top/arxiv/2605.28237) `Benchmark`
  - 概览：构建POINav-Bench，以11个3DGS重建商业区、163个POI和可通行参考轨迹评测真实POI最后数米到达；同时提出Brain-Action框架，以POI落地推理指导连续航点预测，并整理70K组标牌—入口配对数据。

- **[2026/05][ arXiv 2026 - 记忆增强的可通行感知户外VLN框架 - TARIC ]** TARIC: Memory-Augmented Traversability-Aware Outdoor VLN under Interrupted Semantic Cues [[arxiv]](https://arxiv.org/abs/2605.31121) [[hjfy]](https://hjfy.top/arxiv/2605.31121) `End-to-end`
  - 概览：提出统一的户外VLN框架TARIC，首次将可通行性从局部安全约束升级为导航稳定性条件，可在长时间语义线索中断阶段维持连续、可执行的目标一致导航指引。

- **[2026/05][ arXiv 2026 - 具身推理与地理定位基准 - ERGeoBench ]** ERGeoBench:A Comprehensive Benchmark for Embodied Reasoning and Geo-localization in Multimodal Large Language Models [[arxiv]](https://arxiv.org/abs/2605.31251) [[hjfy]](https://hjfy.top/arxiv/2605.31251) `Benchmark`
  - 概览：构建ERGeoBench真实街景具身地理定位基准，允许智能体通过旋转、俯仰和缩放主动观察全景，并评测多模态模型的交互式视觉推理与定位能力。

- **[2026/05][ RA-L 2026 - 人形机器人跨模态导航 - TNavRL ]** TNavRL: Cross-Modal Transformer for Humanoid Visual Navigation [[doi]](https://doi.org/10.1109/LRA.2026.3669788) `Transformer`
  - 概览：提出TNavRL，以跨模态Transformer融合抖动视觉流与本体感状态，并结合动作硬约束和强化学习，在仿真训练后零样本迁移到人形机器人完成安全避障导航。

- **[2026/05][ TCSVT 2026 - 动态物体过滤空间增强 - SPENav ]** SPENav: Dynamic Object Filtering With Spatial Perception Enhancement for Vision-Language Navigation [[doi]](https://doi.org/10.1109/TCSVT.2026.3651320) `Spatial Perception`
  - 概览：提出SPENav，将开放词汇目标检测与分割接入动态地图更新，过滤移动物体造成的不稳定记忆，并通过空间感知增强选择与任务相关的导航线索。

- **[2026/05][ ACM Manuscript 2026 - 有限感知端到端VLN综述 ]** End-to-End Visual Language Navigation with Limited Sensing: A Survey [[pdf]](https://github.com/waynechu1021/Awesome_Visual_Language_Navigation/blob/main/assets/VLN_surwey.pdf) [[github]](https://github.com/waynechu1021/Awesome_Visual_Language_Navigation) `Survey`
  - 概览：聚焦单目RGB和连续空间下的有限感知端到端VLN，以上下文建模、想象预测、决策与错误反思四个维度整理LLM/VLM导航方法及真实部署挑战。

- **[2026/04][ 对话增强长程多机协同VLN - DeCoNav ]** DeCoNav: Dialog enhanced Long-Horizon Collaborative Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2604.12486) [[hjfy]](https://hjfy.top/arxiv/2604.12486) `Agentic` `Habitat`
  - 概览：面向长程多机器人协同VLN提出去中心化对话框架，通过事件触发对话动态重分配子目标并同步重规划，并构建含1213个任务的DeCoNavBench基准，将双机成功率提升69.2%。

- **[2026/04][ arXiv 2026 - 元认知推理高效导航 - MetaNav ]** Stop Wandering: Efficient Vision-Language Navigation via Metacognitive Reasoning [[arxiv]](https://arxiv.org/abs/2604.02318) [[hjfy]](https://hjfy.top/arxiv/2604.02318) `Zero-Shot`
  - 概览：提出元认知导航智能体MetaNav，整合持久3D语义地图、惩罚重复访问的历史感知规划与由LLM生成纠正规则的反思修正机制，在GOAT-Bench等基准上达到SOTA并减少20.7%的VLM查询。

- **[2026/04][ ECCV 2026 - VLN状态漂移双锚定框架 - Dual-Anchoring ]** Dual-Anchoring: Addressing State Drift in Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2604.17473) [[hjfy]](https://hjfy.top/arxiv/2604.17473) `End-to-end` `Video-LLM`
  - 概览：针对Video-LLM导航智能体长程任务中的状态漂移问题，提出指令进度锚定与记忆地标锚定的双锚定框架，并构建360万进度描述与93.7万地标验证数据，长程轨迹成功率提升24.7%。

- **[2026/04][ arXiv 2026 - 空间激活转移学习与课程自适应VLN - SpaAct ]** SpaAct: Spatially-Activated Transition Learning with Curriculum Adaptation for Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2604.27620) [[hjfy]](https://hjfy.top/arxiv/2604.27620) `End-to-end`
  - 概览：提出SpaAct框架，通过动作回溯与未来帧选择两项空间感知任务将视觉变化与动作显式对齐，并结合TriPA课程学习由易到难渐进训练，在VLN-CE基准上取得SOTA表现。

- **[2026/04][ arXiv 2026 - 开放词汇记忆终身物体目标导航 - OVAL ]** OVAL: Open-Vocabulary Augmented Memory Model for Lifelong Object Goal Navigation [[arxiv]](https://arxiv.org/abs/2604.12872) [[hjfy]](https://hjfy.top/arxiv/2604.12872) `GSM`
  - 概览：提出开放词汇增强记忆模型OVAL，结合记忆描述子与多值边界评分的概率探索策略，提升机器人长期部署中终身物体目标导航的效率与鲁棒性。

- **[2026/04][ ACL 2026 - 虚假前提指令可行性感知VLN - VLN-NF ]** VLN-NF: Feasibility-Aware Vision-and-Language Navigation with False-Premise Instructions [[arxiv]](https://arxiv.org/abs/2604.10533) [[hjfy]](https://hjfy.top/arxiv/2604.10533) `Benchmark`
  - 概览：构建允许指令目标不存在的可行性感知导航基准VLN-NF，提出融合房间级导航与LLM/VLM引导探索的两阶段方法ROAM及REV-SPL评测指标。

- **[2026/04][ IEEE RA-L 2026 - 低成本空地协同导航 - LAGCN ]** LAGCN: Low-Cost Aerial-Ground Collaborative Navigation in Unknown Environments [[ieee]](https://ieeexplore.ieee.org/document/11393907) `Diffusion` `YOLOv8+SAM2` `Gazebo`
  - 概览：提出低成本空地协同导航系统LAGCN，用无人机单目RGB相机生成融合几何障碍与语义风险的BEV栅格地图，再以目标引导扩散模型为无车载感知的无人车规划安全路径，通信开销比点云方案降低95%。

- **[2026/04][ IEEE RA-L 2026 - 动态开放世界物体导航具身记忆知识图谱 - EMKG ]** EMKG: Embodied Memory Knowledge Graphs for Object-Goal Navigation in Dynamic Open Worlds [[doi]](https://doi.org/10.1109/LRA.2026.3655297) `GSM+RL` `CLIP` `Habitat`
  - 概览：提出具身多模态记忆知识图谱框架EMKG，以融合视觉、3D坐标与目标描述的动态记忆知识图谱持续更新开放世界知识，并结合检索增强评估与PPO-CLIP规划实现四足机器人端到端物体目标导航。

- **[2026/04][ arXiv 2026 - 混合现实手绘路径导航交互 - MRReP ]** MRReP: Mixed Reality-based Hand-drawn Reference Path Editing Interface for Mobile Robot Navigation [[arxiv]](https://arxiv.org/abs/2604.00059) [[hjfy]](https://hjfy.top/arxiv/2604.00059) `End-to-end`
  - 概览：提出MRReP混合现实交互界面，允许用户用手势在物理地面绘制参考路径，再由定制规划器把手绘点序列转换为机器人可执行的全局路径；受试实验将其与传统二维界面比较路径精度、可用性和工作负荷。

- **[2026/04][ arXiv 2026 - 可复现协同实例目标导航基准 - Light-CoNav ]** Benchmarking Interaction, Beyond Policy: a Reproducible Benchmark for Collaborative Instance Object Navigation [[arxiv]](https://arxiv.org/abs/2604.00265) [[hjfy]](https://hjfy.top/arxiv/2604.00265) `Benchmark`
  - 概览：构建QAsk-Nav协作实例目标导航基准，以独立问答协议和增强导航协议分离评估交互与移动，并提供28,000条推理和提问轨迹；同时提出轻量统一模型Light-CoNav作为协作导航基线。

- **[2026/04][ arXiv 2026 - 人形机器人全场景导航 ]** Learning Humanoid Navigation from Human Data [[arxiv]](https://arxiv.org/abs/2604.00416) [[hjfy]](https://hjfy.top/arxiv/2604.00416) `Zero-Shot`
  - 概览：提出EgoNav，以扩散模型根据历史轨迹、融合颜色深度语义的360°视觉记忆和DINOv3视频特征预测未来轨迹分布，再由混合采样和滚动时域控制器实时选择可执行路径。

- **[2026/04][ arXiv 2026 - 实现复杂城市环境下机器人多模态共享自主导航 - AURA ]** AURA: Multimodal Shared Autonomy for Real-World Urban Navigation [[arxiv]](https://arxiv.org/abs/2604.01659) [[hjfy]](https://hjfy.top/arxiv/2604.01659) `End-to-end`
  - 概览：提出AURA城市共享自主框架，将人类高层多模态指令与AI低层移动控制分解，并以空间感知指令编码器对齐指令、视觉和空间上下文；同时构建含遥操作与视觉语言描述的MM-CoS数据集，并支持在线适应。

- **[2026/04][ arXiv 2026 - 通用视觉语言导航 - Spatially-Guided ]** Audio Spatially-Guided Fusion for Audio-Visual Navigation [[arxiv]](https://arxiv.org/abs/2604.02389) [[hjfy]](https://hjfy.top/arxiv/2604.02389) `Planning` `Transformer` `Audio-Visual`
  - 概览：通过设计音频空间特征编码器，结合声强注意力机制自适应提取目标相关空间状态，并利用ASGF模块实现多模态特征的动态对齐与自适应融合，有效缓解感知不确定性带来的噪声干扰。

- **[2026/04][ arXiv 2026 - 通用视觉语言导航 - Spatial-Aware ]** Spatial-Aware Conditioned Fusion for Audio-Visual Navigation [[arxiv]](https://arxiv.org/abs/2604.02390) [[hjfy]](https://hjfy.top/arxiv/2604.02390) `Navigation` `Audio-Visual`
  - 概览：提出空间感知条件融合方法，通过离散化目标相对方向与距离、预测其分布并编码为紧凑描述符，进而利用条件线性变换调制视觉特征，生成目标导向的融合表征。

- **[2026/04][ arXiv 2026 - 通用视觉语言导航 - Reliability-Aware ]** Reliability-Aware Geometric Fusion for Robust Audio-Visual Navigation [[arxiv]](https://arxiv.org/abs/2604.02391) [[hjfy]](https://hjfy.top/arxiv/2604.02391) `Navigation` `Audio-Visual`
  - 概览：提出RAVN，以声学几何推理器在几何代理监督下估计观测相关的不确定度，再由可靠性感知几何调制把该置信线索变为软门控，动态调节视觉特征与双耳音频的融合。

- **[2026/04][ arXiv 2026 - 实现机器人高精度视觉导航 - STRNet ]** STRNet: Visual Navigation with Spatio-Temporal Representation through Dynamic Graph Aggregation [[arxiv]](https://arxiv.org/abs/2604.02829) [[hjfy]](https://hjfy.top/arxiv/2604.02829) `End-to-end`
  - 概览：提出STRNet时空视觉表示框架，将观测序列与目标图像特征送入融合模块，以帧内空间图推理建模结构，再结合混合时序移位和多分辨率差分感知卷积编码动态关系。

- **[2026/04][ arXiv 2026 - 通用视觉语言导航 - Hypothesis Graph Refinement ]** Hypothesis Graph Refinement: Hypothesis-Driven Exploration with Cascade Error Correction for Embodied Navigation [[arxiv]](https://arxiv.org/abs/2604.04108) [[hjfy]](https://hjfy.top/arxiv/2604.04108) `Memory` `VLM`
  - 概览：提出HGR，把前沿语义预测保存为依赖图中的可修订假设节点，并按目标相关性、路程和不确定性排序探索；到达后以真实观测验证假设，若不一致则级联删除该节点及下游依赖。

- **[2026/04][ arXiv 2026 - 通用视觉语言导航 - Audio-Visual ]** Generalizable Audio-Visual Navigation via Binaural Difference Attention and Action Transition Prediction [[arxiv]](https://arxiv.org/abs/2604.05007) [[hjfy]](https://hjfy.top/arxiv/2604.05007) `Navigation` `Transformer` `Audio-Visual`
  - 概览：提出BDATP框架，通过双耳差异注意力模块增强空间方位感知，减少对语义特征的依赖；同时引入动作转移预测任务作为正则化项，有效抑制环境过拟合。

- **[2026/04][ arXiv 2026 - 图像目标导航最后一米精准定位 - AnyImageNav ]** AnyImageNav: Any-View Geometry for Precise Last-Meter Image-Goal Navigation [[arxiv]](https://arxiv.org/abs/2604.05351) [[hjfy]](https://hjfy.top/arxiv/2604.05351) `End-to-end`
  - 概览：提出AnyImageNav免训练图像目标导航系统，把任意目标图像作为几何查询：语义相关性先引导探索并触发近距门控，随后多视图3D基础模型以稠密像素对应恢复并自校验目标相机的6自由度位姿。

- **[2026/04][ arXiv 2026 - 通用视觉语言导航 - Few-Step ]** Rectified Schr\"odinger Bridge Matching for Few-Step Visual Navigation [[arxiv]](https://arxiv.org/abs/2604.05673) [[hjfy]](https://hjfy.top/arxiv/2604.05673) `Diffusion`
  - 概览：提出Rectified Schrödinger Bridge Matching (RSBM)框架，通过理论证明速度场结构在熵正则化参数ε变化时保持不变，单个网络即可适配不同正则化强度。

- **[2026/04][ arXiv 2026 - 通用视觉语言导航 - Privacy-Preserving ]** Designing Privacy-Preserving Visual Perception for Robot Navigation Based on User Privacy Preferences [[arxiv]](https://arxiv.org/abs/2604.06382) [[hjfy]](https://hjfy.top/arxiv/2604.06382) `Navigation`
  - 概览：从两项用户研究提取机器人视觉导航中的隐私偏好，并据此设计可配置的距离—分辨率策略，在拍摄时按机器人与人的距离降低图像分辨率以保护敏感信息。

- **[2026/04][ arXiv 2026 - 通用视觉语言导航 - Real-World ]** Incremental Residual Reinforcement Learning Toward Real-World Learning for Social Navigation [[arxiv]](https://arxiv.org/abs/2604.07945) [[hjfy]](https://hjfy.top/arxiv/2604.07945) `RL`
  - 概览：提出增量残差强化学习（IRRL），融合无需经验回放缓冲区的轻量增量学习与基于残差策略的高效学习机制。

- **[2026/04][ arXiv 2026 - 混合推理赋能具身智能导航 - HiRO-Nav ]** HiRO-Nav: Hybrid ReasOning Enables Efficient Embodied Navigation [[arxiv]](https://arxiv.org/abs/2604.08232) [[hjfy]](https://hjfy.top/arxiv/2604.08232) `RL`
  - 概览：提出HiRO-Nav混合推理智能体，以动作熵判断每一步采用快速反应还是深度思考，并先用混合监督微调冷启动、再以在线强化学习显式训练高熵关键动作的选择性推理。

- **[2026/04][ arXiv 2026 - 交通规则约束视觉语言导航 - Rule-VLN ]** Rule-VLN: Bridging Perception and Compliance via Semantic Reasoning and Geometric Rectification [[arxiv]](https://arxiv.org/abs/2604.16993) [[hjfy]](https://hjfy.top/arxiv/2604.16993) `Zero-Shot`
  - 概览：构建Rule-VLN城市规则合规导航基准，并提出零样本语义导航纠正模块SNRM，以粗到细视觉感知、认知地图和动态绕行规划识别并遵守交通与行为约束。

- **[2026/04][ arXiv 2026 - 在线SG-Memo自主探索 - Explore Like Humans ]** Explore Like Humans: Autonomous Exploration with Online SG-Memo Construction for Embodied Agents [[arxiv]](https://arxiv.org/abs/2604.19034) [[hjfy]](https://hjfy.top/arxiv/2604.19034) `Hierarchical`
  - 概览：提出ABot-Explorer，在仅使用RGB的在线探索过程中由大型VLM提取语义导航可及性锚点，并动态写入分层SG-Memo以优先探索门口、楼梯等结构通行节点；同时扩展InteriorGS并加入SNA和SG-Memo标注。

- **[2026/04][ arXiv 2026 - 异步连续视觉语言导航 - LiveVLN ]** LiveVLN: Breaking the Stop-and-Go Loop in Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2604.19536) [[hjfy]](https://hjfy.top/arxiv/2604.19536) `End-to-end`
  - 概览：提出LiveVLN异步运行时架构，将感知、规划与执行解耦并并行调度，以减少大模型推理造成的停走等待，同时保持连续机器人运动和及时的路径修正。

- **[2026/04][ arXiv 2026 - 真机可跑的视觉语言导航系统 ]** A Deployable Embodied Vision-Language Navigation System with Hierarchical Cognition and Context-Aware Exploration [[arxiv]](https://arxiv.org/abs/2604.21363) [[hjfy]](https://hjfy.top/arxiv/2604.21363) `Hierarchical`
  - 概览：提出可部署VLN系统，以高频感知—动作层和低频深度推理层异步运行、共享增量紧凑记忆图，并把分解子图逐步送入VLM；探索则联合推理结果与候选区域空间分布求解加权旅行修理工问题。

- **[2026/04][ arXiv 2026 - 故障感知示范学习安全导航 ]** Learning from Demonstration with Failure Awareness for Safe Robot Navigation [[arxiv]](https://arxiv.org/abs/2604.23360) [[hjfy]](https://hjfy.top/arxiv/2604.23360) `RL`
  - 概览：提出故障感知的离线强化学习导航框架，将碰撞等失败经历仅用于塑造危险区域的价值估计，同时限定策略从成功示范中学习，从而降低碰撞率并保持任务成功率。

- **[2026/04][ arXiv 2026 - 异步云端VLA边缘安全适配 - AsyncShield ]** AsyncShield: A Plug-and-Play Edge Adapter for Asynchronous Cloud-based VLA Navigation [[arxiv]](https://arxiv.org/abs/2604.24086) [[hjfy]](https://hjfy.top/arxiv/2604.24086) `Zero-Shot`
  - 概览：提出AsyncShield异步云端VLA适配器，以位姿缓冲和SE(2)运动学把网络时延转换为当前空间偏移，再把意图恢复与高频激光避障写成约束MDP，由PPO-Lagrangian策略在边缘端动态权衡。

- **[2026/04][ arXiv 2026 - 四足机器人分层姿态自适应导航新框架 - HiPAN ]** HiPAN: Hierarchical Posture-Adaptive Navigation for Quadruped Robots in Unstructured 3D Environments [[arxiv]](https://arxiv.org/abs/2604.26504) [[hjfy]](https://hjfy.top/arxiv/2604.26504) `Hierarchical`
  - 概览：提出HiPAN分层姿态自适应导航框架，高层从机载深度观测输出平面速度与身体姿态指令，低层控制器执行姿态适应运动；路径引导课程学习逐步把训练范围从反应式避障扩展到长时域战略导航。

- **[2026/04][ arXiv 2026 - 小米汽车×清华联合研发Walk With Me ]** Walk With Me: Long-Horizon Social Navigation for Human-Centric Outdoor Assistance [[arxiv]](https://arxiv.org/abs/2604.26839) [[hjfy]](https://hjfy.top/arxiv/2604.26839) `End-to-end`
  - 概览：提出Walk With Me无地图长程户外社交导航框架，以VLM将高层人类意图落地为目的地和粗航点，并由观察感知路由在高层安全推理与低层VLA动作生成之间切换。

- **[2026/04][ RA-L 2026 - 地图路径双策略协同VLN - CoMaR ]** Collaborative Map-Based and Route-Based Policy Learning for Continuous Vision-and-Language Navigation [[doi]](https://doi.org/10.1109/LRA.2026.3662659) [[github]](https://github.com/VIPL-EPP/CoMaR) `Dual Policy`
  - 概览：提出CoMaR，以地图策略负责全局空间推理、路线策略负责指令流程对齐，并通过双向信息交换协同决策连续环境中的下一航点。

- **[2026/04][ ACM CSUR 2026 - 基础语言模型驱动机器人导航综述 ]** Robot Navigation via Foundation Language Models: A Review [[doi]](https://doi.org/10.1145/3802539) `Survey`
  - 概览：从感知、规划、控制、人机交互与多机器人协同五个环节系统梳理基础语言模型驱动的机器人导航，并按室内、道路和越野环境比较数据集、仿真平台与评测指标，归纳空间推理、实时部署和跨场景泛化等挑战。

- **[2026/03][ 持续多模态记忆检索VLN智能体 - CMMR-VLN ]** CMMR-VLN: Vision-and-Language Navigation via Continual Multimodal Memory Retrieval [[arxiv]](https://arxiv.org/abs/2603.07997) [[hjfy]](https://hjfy.top/arxiv/2603.07997) `Agentic` `GPT-4o` `Matterport3D`
  - 概览：提出赋予LLM智能体结构化记忆与反思能力的VLN框架，以全景图像与显著地标索引多模态经验记忆，结合检索增强生成与反思式记忆更新策略，显著提升长程与陌生场景下的导航成功率。

- **[2026/03][ 拓扑感知全局动作推理VLN - TagaVLM ]** TagaVLM: Topology-Aware Global Action Reasoning for Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2603.02972) [[hjfy]](https://hjfy.top/arxiv/2603.02972) `End-to-end` `Qwen2-7B`
  - 概览：提出将拓扑结构显式注入VLM主干的端到端VLN框架，通过STAR-Att把拓扑边信息融入自注意力并以交错导航提示强化节点对齐，支持全局动作推理与路径纠正，在R2R未见环境取得大模型方法SOTA。

- **[2026/03][ VLN大模型Token缓存推理加速 - VLN-Cache ]** VLN-Cache: Enabling Token Caching for VLN Models with Visual/Semantic Dynamics Awareness [[arxiv]](https://arxiv.org/abs/2603.07080) [[hjfy]](https://hjfy.top/arxiv/2603.07080) `End-to-end` `Qwen2.5-VL-7B`
  - 概览：面向VLN大模型实时部署提出免训练的Token缓存框架，以视角对齐重映射与任务相关显著性过滤应对视觉与语义双重动态，在R2R-CE上实现最高1.52倍推理加速且保持导航成功率。

- **[2026/03][ arXiv 2026 - 分层记忆增强开源零样本VLN - HiMemVLN ]** HiMemVLN: Enhancing Reliability of Open-Source Zero-Shot Vision-and-Language Navigation with Hierarchical Memory System [[arxiv]](https://arxiv.org/abs/2603.14807) [[hjfy]](https://hjfy.top/arxiv/2603.14807) [[github]](https://github.com/lvkailin0118/HiMemVLN) `Zero-Shot`
  - 概览：针对开源多模态模型导航中的"导航失忆"问题，提出分层记忆系统增强视觉回忆与自定位能力，使开源零样本VLN在R2R-CE仿真与真实环境中的成功率提升约一倍。

- **[2026/03][ AAAI 2026 - 四足机器人视觉思维链VLN基准 - CoT-VLNBench ]** CoT-VLNBench: A Benchmark for Visual Chain-of-Thought Reasoning in Vision-Language-Navigation Robots [[aaai]](https://ojs.aaai.org/index.php/AAAI/article/view/40980) `Benchmark`
  - 概览：面向四足机器人导航的大规模视觉思维链推理基准，涵盖17.5万帧图像、525万个3D标注框与87.5万VQA对，覆盖室内外多样场景，并提出7B参数VLN基线模型超越现有方法。

- **[2026/03][ arXiv 2026 - LLM与VLM协同零样本导航 - ProFocus ]** ProFocus: Proactive Perception and Focused Reasoning in Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2603.05530) [[hjfy]](https://hjfy.top/arxiv/2603.05530) `Zero-Shot`
  - 概览：提出免训练渐进式框架，通过LLM与VLM协同将全景观察转为结构化自我中心语义地图以主动补全缺失视觉信息，并用分支多样化蒙特卡洛树搜索聚焦高价值历史航点推理，在R2R与REVERIE上取得零样本SOTA。

- **[2026/03][ arXiv 2026 - 观察推理修正解耦导航 - DecoVLN ]** DecoVLN: Decoupling Observation, Reasoning, and Correction for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2603.13133) [[hjfy]](https://hjfy.top/arxiv/2603.13133) [[github]](https://github.com/Allenxinn/DecoVLN) [[project]](https://allenxinn.github.io/DecoVLN/) `Hierarchical`
  - 概览：提出将观察、推理与修正解耦的VLN框架，以统一评分函数迭代优化长期记忆帧选择，并利用测地距离量化轨迹偏差进行状态-动作对级修正微调以缓解累积误差，已在真实环境部署验证。

- **[2026/03][ arXiv 2026 - 潜在视觉推理前瞻想象VLN - LatentPilot ]** LatentPilot: Scene-Aware Vision-and-Language Navigation by Dreaming Ahead with Latent Visual Reasoning [[arxiv]](https://arxiv.org/abs/2603.29165) [[hjfy]](https://hjfy.top/arxiv/2603.29165) `World Model`
  - 概览：提出在潜空间"前瞻想象"未来观测的VLN框架，通过飞轮式在线轨迹迭代采集机制学习动作条件下的视觉动态，部署时无需未来帧即可推理，在多个基准与真机测试中达到SOTA。

- **[2026/03][ arXiv 2026 - 轨迹多样性驱动鲁棒VLN - NavGRPO ]** Trajectory-Diversity-Driven Robust Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2603.15370) [[hjfy]](https://hjfy.top/arxiv/2603.15370) `RL`
  - 概览：提出目标导向的强化学习后训练框架NavGRPO，以组相对策略优化鼓励探索多样化轨迹，可即插即用于DUET、ScaleVLN等架构，在扰动条件下鲁棒性显著优于模仿学习策略。

- **[2026/03][ arXiv 2026 - 步进感知对比对齐VLN-CE后训练 - SACA ]** Let's Reward Step-by-Step: Step-Aware Contrastive Alignment for Vision-Language Navigation in Continuous Environments [[arxiv]](https://arxiv.org/abs/2603.09740) [[hjfy]](https://hjfy.top/arxiv/2603.09740) `RL`
  - 概览：针对VLN-CE中SFT误差累积与GRPO稀疏奖励的难题，提出步进感知对比对齐框架SACA，用逐步审计器将失败轨迹拆解为有效前缀与偏离点以提取密集监督信号，在VLN-CE基准上取得SOTA。

- **[2026/03][ arXiv 2026 - 智能体化VLN边缘部署框架 - AgentVLN ]** AgentVLN: Towards Agentic Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2603.17670) [[hjfy]](https://hjfy.top/arxiv/2603.17670) [[github]](https://github.com/Allenxinn/AgentVLN) `Agentic`
  - 概览：提出可在边缘计算平台部署的VLM-as-Brain智能体导航框架，以即插即用技能库解耦语义推理与感知规划，结合跨空间表征映射、上下文感知自校正与查询驱动感知思维链，在长时程VLN基准上超越SOTA。

- **[2026/03][ arXiv 2026 - 自适应探索-恢复-回忆零样本物体导航 - AERR-Nav ]** AERR-Nav: Adaptive Exploration-Recovery-Reminiscing Strategy for Zero-Shot Object Navigation [[arxiv]](https://arxiv.org/abs/2603.17712) [[hjfy]](https://hjfy.top/arxiv/2603.17712) `Zero-Shot` `MLLM`
  - 概览：提出零样本物体导航框架AERR-Nav，通过探索-恢复-回忆三状态自适应切换与快慢思考探索模式平衡探索与利用，在HM3D与MP3D多楼层环境取得零样本SOTA。

- **[2026/03][ ICLR 2026 - 全天候多场景终身VLN的Tucker自适应 - TuKA ]** All-day Multi-scenes Lifelong Vision-and-Language Navigation with Tucker Adaptation [[arxiv]](https://arxiv.org/abs/2603.14276) [[hjfy]](https://hjfy.top/arxiv/2603.14276) `End-to-end`
  - 概览：提出Tucker分解自适应方法TuKA，用高阶张量解耦共享与场景专属的多层次导航知识，并构建AlldayWalker智能体实现全天候多场景终身视觉语言导航。

- **[2026/03][ arXiv 2026 - 通用零样本具身导航 - SFCo-Nav ]** SFCo-Nav: Efficient Zero-Shot Visual Language Navigation via Collaboration of Slow LLM and Fast Attributed Graph Alignment [[arxiv]](https://arxiv.org/abs/2603.01477) [[hjfy]](https://hjfy.top/arxiv/2603.01477) `Zero-Shot` `Planning` `VLM`
  - 概览：SFCo-Nav将导航过程分解为三个协作模块：慢速LLM规划器负责制定战略性子目标链，每个子目标关联一个想象中的物体图；快速反应导航器实时构建物体图并执行子目标；轻量级异步桥梁模块通过对比想象图与感知图来评估导航置信度，仅在必要时触发慢速LLM。

- **[2026/03][ arXiv 2026 - 通用视觉语言导航 - SSMG-Nav ]** SSMG-Nav: Enhancing Lifelong Object Navigation with Semantic Skeleton Memory Graph [[arxiv]](https://arxiv.org/abs/2603.01813) [[hjfy]](https://hjfy.top/arxiv/2603.01813) `Memory` `Planning` `VLM`
  - 概览：SSMG-Nav提出语义骨架记忆图（SSMG）框架，将历史观测信息构建成以拓扑关键点（如房间中心、走廊拐角）为锚点的空间对齐记忆网络。

- **[2026/03][ arXiv 2026 - 通用视觉语言导航 - SaferPath ]** SaferPath: Hierarchical Visual Navigation with Learned Guidance and Safety-Constrained Control [[arxiv]](https://arxiv.org/abs/2603.01898) [[hjfy]](https://hjfy.top/arxiv/2603.01898) `Hierarchical` `End-to-end`
  - 概览：提出SaferPath分层视觉导航框架，先把视觉观测变换为可通行区域地图，再以MP-SVES在安全约束下优化学习模型给出的引导轨迹，最后由MPC控制器跟踪精炼后的路径。

- **[2026/03][ arXiv 2026 - 通用视觉语言导航 - CHOP ]** CHOP: Counterfactual Human Preference Labels Improve Obstacle Avoidance in Visuomotor Navigation Policies [[arxiv]](https://arxiv.org/abs/2603.02004) [[hjfy]](https://hjfy.top/arxiv/2603.02004) `Sim-to-Real` `Pretraining` `Human Preference`
  - 概览：提出CHOP，把机器人实际轨迹与相同观测下的反事实候选轨迹组成偏好对，由人工按碰撞风险和路径效率标注，再以聚合偏好微调视觉运动导航策略。

- **[2026/03][ arXiv 2026 - 通用视觉语言导航 - Self-Evolutionary ]** Agentic Self-Evolutionary Replanning for Embodied Navigation [[arxiv]](https://arxiv.org/abs/2603.02772) [[hjfy]](https://hjfy.top/arxiv/2603.02772) `Agentic`
  - 概览：提出自进化重规划方法SERP，用上下文学习与自动微分在运行时调整动作模型，并把环境压缩为图后执行图式思维链重规划，以在失败后同时更新计划与模型。

- **[2026/03][ arXiv 2026 - 通用具身导航基准 - CoFL ]** CoFL: Continuous Flow Fields for Language-Conditioned Navigation [[arxiv]](https://arxiv.org/abs/2603.02854) [[hjfy]](https://hjfy.top/arxiv/2603.02854) `Benchmark` `Zero-Shot` `End-to-end`
  - 概览：提出CoFL，将鸟瞰图和语言指令映射为工作空间连续流场，在任意位置预测局部运动向量，并通过数值积分从不同起点生成闭环轨迹；同时构建50万余对带流场与轨迹标注的BEV—指令数据。

- **[2026/03][ arXiv 2026 - 通用视觉语言导航 - DreamFlow ]** DreamFlow: Local Navigation Beyond Observation via Conditional Flow Matching in the Latent Space [[arxiv]](https://arxiv.org/abs/2603.02976) [[hjfy]](https://hjfy.top/arxiv/2603.02976) `Diffusion` `RL` `Planning`
  - 概览：DreamFlow提出一种基于条件流匹配的局部导航框架，通过潜在空间的环境特征预测，让机器人能够「预见」视野外的环境结构。

- **[2026/03][ arXiv 2026 - 通用视觉语言导航 - MA-CoNav ]** MA-CoNav: A Master-Slave Multi-Agent Framework with Hierarchical Collaboration and Dual-Level Reflection for Long-Horizon Embodied VLN [[arxiv]](https://arxiv.org/abs/2603.03024) [[hjfy]](https://hjfy.top/arxiv/2603.03024) `Agentic` `Hierarchical` `Memory`
  - 概览：受分布式认知理论启发，MA-CoNav采用主从式多智能体协作架构，将导航任务所需的感知、规划、执行和记忆功能解耦分配给专门智能体。

- **[2026/03][ arXiv 2026 - 通用具身导航基准 - RVN-Bench ]** RVN-Bench: A Benchmark for Reactive Visual Navigation [[arxiv]](https://arxiv.org/abs/2603.03953) [[hjfy]](https://hjfy.top/arxiv/2603.03953) `Benchmark` `RL` `Sim-to-Real`
  - 概览：平台不仅定义了碰撞感知导航任务和评估指标，还提供了标准化训练和测试工具，支持在线强化学习和离线学习。

- **[2026/03][ arXiv 2026 - 通用视觉语言导航 ]** Efficient Autonomous Navigation of a Quadruped Robot in Underground Mines on Edge Hardware [[arxiv]](https://arxiv.org/abs/2603.04470) [[hjfy]](https://hjfy.top/arxiv/2603.04470) `Navigation`
  - 概览：该系统融合激光雷达惯性里程计、先验地图扫描匹配定位、地形分割等技术，通过可见性全局规划与速度调控局部路径跟踪，实现了实时感知决策闭环。

- **[2026/03][ arXiv 2026 - 基于视觉语言锚定前沿的通用机器人导航方法 - OpenFrontier ]** OpenFrontier: General Navigation with Visual-Language Grounded Frontiers [[arxiv]](https://arxiv.org/abs/2603.05377) [[hjfy]](https://hjfy.top/arxiv/2603.05377) `Zero-Shot`
  - 概览：提出OpenFrontier，将导航表述为稀疏子目标识别与到达问题，并选择视觉前沿作为高层视觉语言先验的语义锚点；框架无需稠密三维语义地图、任务专项训练或模型微调即可执行零样本导航。

- **[2026/03][ arXiv 2026 - 通用视觉语言导航 ]** Lifelong Embodied Navigation Learning [[arxiv]](https://arxiv.org/abs/2603.06073) [[hjfy]](https://hjfy.top/arxiv/2603.06073) `Memory`
  - 概览：提出Uni-Walker终身导航框架，以Decoder Extension LoRA把知识拆为任务共享与任务专用分量；知识继承和专家协同激活迁移共享知识，专家子空间正交约束与导航思维链隔离专用知识以减轻遗忘。

- **[2026/03][ arXiv 2026 - 通用零样本具身导航 - History-Conditioned ]** History-Conditioned Spatio-Temporal Visual Token Pruning for Efficient Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2603.06480) [[hjfy]](https://hjfy.top/arxiv/2603.06480) `Zero-Shot` `VLA` `Sim-to-Real`
  - 概览：该方法无需重新训练或修改预训练模型，通过基于注意力机制的令牌重要性评估和查询引导的时空过滤，实现对当前视图的空间令牌选择和历史记忆的时空压缩。

- **[2026/03][ arXiv 2026 - 通用视觉语言导航 - SysNav ]** SysNav: Multi-Level Systematic Cooperation Enables Real-World, Cross-Embodiment Object Navigation [[arxiv]](https://arxiv.org/abs/2603.06914) [[hjfy]](https://hjfy.top/arxiv/2603.06914) `Hierarchical` `VLM`
  - 概览：提出SysNav系统，通过三层架构将语义推理、导航规划和运动控制解耦，实现了跨平台的高效目标导航。

- **[2026/03][ arXiv 2026 - 通用零样本具身导航 - T2Nav ]** T2Nav Algebraic Topology Aware Temporal Graph Memory and Loop Detection for ZeroShot Visual Navigation [[arxiv]](https://arxiv.org/abs/2603.06918) [[hjfy]](https://hjfy.top/arxiv/2603.06918) `Zero-Shot` `Memory` `Planning`
  - 概览：提出T2Nav零样本图导航系统，将视觉观测及环境匹配结果写入时序图记忆，以拓扑结构支持闭环检测、去除重复探索和路径规划，并处理以目标实例参考图像给出的导航任务。

- **[2026/03][ arXiv 2026 - 通用视觉语言导航 - RGBD ]** A Contrastive Fewshot RGBD Traversability Segmentation Framework for Indoor Robotic Navigation [[arxiv]](https://arxiv.org/abs/2603.06927) [[hjfy]](https://hjfy.top/arxiv/2603.06927) `Contrastive` `Transformer`
  - 概览：提出少样本RGB-D可通行区域分割框架，以负原型对比学习修正自由空间预测，并用两阶段注意力在水平与垂直方向对齐稀疏一维激光深度和RGB图像。

- **[2026/03][ arXiv 2026 - 融合异常检测的多地形机器人几何可通行性估计 - GSAT ]** GSAT: Geometric Traversability Estimation using Self-supervised Learning with Anomaly Detection for Diverse Terrains [[arxiv]](https://arxiv.org/abs/2603.07480) [[hjfy]](https://hjfy.top/arxiv/2603.07480) `End-to-end`
  - 概览：提出GSAT自监督可通行性估计方法，在潜在空间只用机器人经验正样本构建超球面，以异常检测区分不可通行区域，并联合训练异常分类和可通行性预测以利用不同平台的行驶经验。

- **[2026/03][ arXiv 2026 - 通用视觉语言导航 - PanoDP ]** PanoDP: Learning Collision-Free Navigation with Panoramic Depth and Differentiable Physics [[arxiv]](https://arxiv.org/abs/2603.07644) [[hjfy]](https://hjfy.top/arxiv/2603.07644) `Navigation`
  - 概览：提出PanoDP，以轻量CNN编码四视角全景深度，并用可微碰撞与运动可行性项提供稠密训练信号，使策略在部分可观测的静态和动态障碍环境中学习无碰撞导航。

- **[2026/03][ arXiv 2026 - 通用零样本具身导航 - From Reactive to Map-Based AI ]** From Reactive to Map-Based AI: Tuned Local LLMs for Semantic Zone Inference in Object-Goal Navigation [[arxiv]](https://arxiv.org/abs/2603.08086) [[hjfy]](https://hjfy.top/arxiv/2603.08086) `Zero-Shot` `GSM` `Memory`
  - 概览：提出地图式目标导航框架，用LoRA微调Llama-2从物体观测推断功能区域与目标存在概率，再把语义结果写入拓扑—栅格混合地图并以TSP排序探索区域。

- **[2026/03][ arXiv 2026 - 通用零样本具身导航 - R2F ]** R2F: Repurposing Ray Frontiers for LLM-free Object Navigation [[arxiv]](https://arxiv.org/abs/2603.08475) [[hjfy]](https://hjfy.top/arxiv/2603.08475) `Zero-Shot` `End-to-end` `VLM`
  - 概览：提出R2F，把射线边界解释为方向条件语义假设，在边界处稀疏存储沿射线累积的语言对齐特征，再以嵌入相似度评分边界并交由经典建图规划器跟踪，无需迭代调用大模型。

- **[2026/03][ arXiv 2026 - 通用视觉语言导航 - NaviNote ]** NaviNote: Enabling In-situ Spatial Annotation Authoring to Support Exploration and Navigation for Blind and Low Vision People [[arxiv]](https://arxiv.org/abs/2603.08837) [[hjfy]](https://hjfy.top/arxiv/2603.08837) `Agentic`
  - 概览：开发NaviNote，将视觉高精度定位与智能体架构结合，使盲人和低视力用户可通过语音在现场创建空间注释，并利用这些注释完成最后数米的定位与导航。

- **[2026/03][ arXiv 2026 - 通用视觉语言导航 - PM-Nav ]** PM-Nav: Priori-Map Guided Embodied Navigation in Functional Buildings [[arxiv]](https://arxiv.org/abs/2603.09113) [[hjfy]](https://hjfy.top/arxiv/2603.09113) `Hierarchical` `Planning`
  - 概览：提出PM-Nav导航框架，通过将环境地图转化为导航友好的语义先验地图，设计带有标注先验地图的分层思维链提示模板，实现精准路径规划，并构建多模型协同动作输出机制，完成导航定位决策与执行控制。

- **[2026/03][ arXiv 2026 - 通用空间感知VLN - SPAN-Nav ]** SPAN-Nav: Generalized Spatial Awareness for Versatile Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2603.09163) [[hjfy]](https://hjfy.top/arxiv/2603.09163) `End-to-end`
  - 概览：提出SPAN-Nav，以室内外4.2百万占用标注学习通用三维空间先验，将其压缩为单个空间令牌并显式注入动作推理，再通过多任务联合训练适配不同视觉语言导航任务。

- **[2026/03][ arXiv 2026 - 通用零样本具身导航 - Vision-and-Language ]** Implicit Geometry Representations for Vision-and-Language Navigation from Web Videos [[arxiv]](https://arxiv.org/abs/2603.09259) [[hjfy]](https://hjfy.top/arxiv/2603.09259) `Zero-Shot`
  - 概览：构建基于网络室内导览视频的视觉语言导航训练框架，配对描述增强与动作增强轨迹，并从RGB帧提取隐式几何表示以利用无需完整三维重建的视频片段。

- **[2026/03][ arXiv 2026 - 杂乱环境四足机器人实现高速安全自主避障 - SEA-Nav ]** SEA-Nav: Efficient Policy Learning for Safe and Agile Quadruped Navigation in Cluttered Environments [[arxiv]](https://arxiv.org/abs/2603.09460) [[hjfy]](https://hjfy.top/arxiv/2603.09460) `RL`
  - 概览：提出SEA-Nav四足机器人安全敏捷导航方法，以自适应碰撞状态初始化反复采样高风险片段，并配合课程式策略学习提高狭窄杂乱环境中的训练效率与避障能力。

- **[2026/03][ arXiv 2026 - 通用视觉语言导航 - Context-Nav ]** Context-Nav: Context-Driven Exploration and Viewpoint-Aware 3D Spatial Reasoning for Instance Navigation [[arxiv]](https://arxiv.org/abs/2603.09506) [[hjfy]](https://hjfy.top/arxiv/2603.09506) `Navigation`
  - 概览：提出Context-Nav，将完整文本描述与图像密集对齐形成探索价值图，并在发现候选实例后采样观察位姿、对齐局部坐标系，以三维空间关系验证目标是否满足描述。

- **[2026/03][ arXiv 2026 - 通用零样本具身导航 - BEACON ]** BEACON: Language-Conditioned Navigation Affordance Prediction under Occlusion [[arxiv]](https://arxiv.org/abs/2603.09961) [[hjfy]](https://hjfy.top/arxiv/2603.09961) `Zero-Shot` `VLM`
  - 概览：它结合四向RGB-D观测和语言指令，将空间线索注入视觉语言模型，并与深度信息融合，生成包含遮挡区域的局部可通行热图。

- **[2026/03][ arXiv 2026 - 通用视觉语言导航 - WalkGPT ]** WalkGPT: Grounded Vision-Language Conversation with Depth-Aware Segmentation for Pedestrian Navigation [[arxiv]](https://arxiv.org/abs/2603.10703) [[hjfy]](https://hjfy.top/arxiv/2603.10703) `Navigation` `VLM`
  - 概览：该模型通过多尺度查询投影器和校准文本投影器，能够在没有用户提示的情况下自动识别可通行区域和危险障碍物，并生成带有分割掩码的对话式导航建议。

- **[2026/03][ arXiv 2026 - 通用视觉语言导航 ]** Enhancing Lightweight Vision Language Models through Group Competitive Learning for Socially Compliant Navigation [[arxiv]](https://arxiv.org/abs/2603.11447) [[hjfy]](https://hjfy.top/arxiv/2603.11447) `Sim-to-Real` `VLM`
  - 概览：提出群体竞争学习GCL，以群体竞争目标GCO联合语义监督与分布正则，并用非对称群体优化AGO让轻量学习模型在较强引导模型的竞争信号下学习社会合规导航。

- **[2026/03][ arXiv 2026 - 用流匹配实现行人社交感知的统一导航 - FLUX ]** FLUX: Accelerating Cross-Embodiment Generative Navigation Policies via Rectified Flow and Static-to-Dynamic Learning [[arxiv]](https://arxiv.org/abs/2603.12806) [[hjfy]](https://hjfy.top/arxiv/2603.12806) `Zero-Shot`
  - 概览：提出FLUX统一生成式导航策略，以整流流的直线概率路径替代迭代去噪，并通过静态到动态课程与强化学习联合掌握目标到达和社会化动态避障。

- **[2026/03][ arXiv 2026 - 基于标识牌的大规模室内语义视觉导航 - SignNav ]** SignNav: Leveraging Signage for Semantic Visual Navigation in Large-Scale Indoor Environments [[arxiv]](https://arxiv.org/abs/2603.16166) [[hjfy]](https://hjfy.top/arxiv/2603.16166) `End-to-end`
  - 概览：提出SignNav大型室内标识导航任务并构建LSI-Dataset，同时设计START时空感知Transformer：空间模块把标识语义落地到物理环境，时间模块关联历史状态与当前观测，并以两阶段DAgger训练。

- **[2026/03][ arXiv 2026 - 通用零样本具身导航 - LightZeroNav ]** LightZeroNav: Zero-Shot Vision Language Navigation in Continuous Environments Based on Lightweight VLMs [[arxiv]](https://arxiv.org/abs/2603.16947) [[hjfy]](https://hjfy.top/arxiv/2603.16947) `Zero-Shot` `Memory` `VLM`
  - 概览：提出轻量零样本连续导航框架LightZeroNav，以目标导向感知压缩多源输入，用双记忆对比估计任务进度，并把动作执行与阶段切换分离为不同推理角色。

- **[2026/03][ arXiv 2026 - 通用视觉语言导航 - FloorPlan-VLN ]** FloorPlan-VLN: A New Paradigm for Floor Plan Guided Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2603.17437) [[hjfy]](https://hjfy.top/arxiv/2603.17437) `Sim-to-Real`
  - 概览：构建FloorPlan-VLN数据集，把语义户型图、简短指令与Matterport3D轨迹配对，并提出FP-Nav，以双视角时空对齐视频和辅助推理任务对齐观测、户型图与指令。

- **[2026/03][ arXiv 2026 - 通用视觉语言导航 - P$^{3}$Nav ]** P$^{3}$Nav: End-to-End Perception, Prediction and Planning for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2603.17459) [[hjfy]](https://hjfy.top/arxiv/2603.17459) `End-to-end` `Planning`
  - 概览：该框架通过对象级和地图级双视角提取互补信息增强感知，预测未来路径点以建模智能体潜在状态，并基于这些路径点前瞻性预测语义地图线索，从而减少对纯历史信息的依赖。

- **[2026/03][ arXiv 2026 - 通用视觉语言导航 - Context-Aware ]** Interpreting Context-Aware Human Preferences for Multi-Objective Robot Navigation [[arxiv]](https://arxiv.org/abs/2603.17510) [[hjfy]](https://hjfy.top/arxiv/2603.17510) `RL` `Memory` `Pretraining`
  - 概览：提出上下文偏好导航管线，由视觉语言模型提取环境上下文、大语言模型把用户反馈写成可更新规则，再将规则转成数值偏好向量以调节多目标强化学习策略。

- **[2026/03][ arXiv 2026 - 通用零样本具身导航 - GoalVLM ]** GoalVLM: VLM-driven Object Goal Navigation for Multi-Agent System [[arxiv]](https://arxiv.org/abs/2603.18210) [[hjfy]](https://hjfy.top/arxiv/2603.18210) `Zero-Shot` `Agentic` `VLM`
  - 概览：GoalVLM将视觉语言模型直接集成到决策循环中，通过SAM3实现文本提示的检测与分割，结合SpaceOM进行空间推理，使智能体能理解自由形式的语言目标，并基于零样本语义先验对探索边界进行评分。

- **[2026/03][ arXiv 2026 - 通用零样本具身导航 - SR-Nav ]** SR-Nav: Spatial Relationships Matter for Zero-shot Object Goal Navigation [[arxiv]](https://arxiv.org/abs/2603.18443) [[hjfy]](https://hjfy.top/arxiv/2603.18443) `Zero-Shot`
  - 概览：SR-Nav构建动态空间关系图，通过基础模型编码目标中心的空间关系，并随实时观测动态更新。

- **[2026/03][ arXiv 2026 - 基于滚动视界探索式斯坦纳树的无训练导航框架 - REST ]** REST: Receding Horizon Explorative Steiner Tree for Zero-Shot Object-Goal Navigation [[arxiv]](https://arxiv.org/abs/2603.18624) [[hjfy]](https://hjfy.top/arxiv/2603.18624) `Zero-Shot`
  - 概览：提出REST免训练目标导航框架，从在线RGB-D构建开放词汇3D地图，以采样规划生成机器人中心的安全信息路径树，再把各分支文本化为空间叙事供LLM进行由粗到细的下一路径选择。

- **[2026/03][ arXiv 2026 - 通用具身导航基准 - Meanings and Measurements ]** Meanings and Measurements: Multi-Agent Probabilistic Grounding for Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2603.19166) [[hjfy]](https://hjfy.top/arxiv/2603.19166) `Benchmark` `Agentic` `VLM`
  - 概览：提出MAPG框架，通过多智能体协作将复杂指令分解为结构化子任务，分别进行语义映射和度量计算，最后通过概率组合生成在3D空间中可执行的行动决策。

- **[2026/03][ arXiv 2026 - 通用具身导航基准 - NavTrust ]** NavTrust: Benchmarking Trustworthiness for Embodied Navigation [[arxiv]](https://arxiv.org/abs/2603.19229) [[hjfy]](https://hjfy.top/arxiv/2603.19229) `Benchmark`
  - 概览：NavTrust通过模拟真实场景中的输入干扰——包括图像色彩失真、深度信息误差和指令表述变化——构建统一基准测试平台。

- **[2026/03][ arXiv 2026 - 通用视觉语言导航 - CeRLP ]** CeRLP: A Cross-embodiment Robot Local Planning Framework for Visual Navigation [[arxiv]](https://arxiv.org/abs/2603.19602) [[hjfy]](https://hjfy.top/arxiv/2603.19602) `Planning`
  - 概览：该框架通过离线预校准解决单目深度估计的尺度模糊问题，还原精确的度量深度图像；同时设计视觉-扫描抽象模块，将多样化视觉输入转换为高度自适应的激光扫描数据，使导航策略具备跨平台鲁棒性。

- **[2026/03][ arXiv 2026 - 通用视觉语言导航 - Audio-Visual ]** Semantic Audio-Visual Navigation in Continuous Environments [[arxiv]](https://arxiv.org/abs/2603.19660) [[hjfy]](https://hjfy.top/arxiv/2603.19660) `Memory` `Transformer` `Audio-Visual`
  - 概览：面对目标声音可能间歇性消失的挑战，开发基于多模态Transformer的MAGNet模型，该模型能联合编码空间与语义目标表征，并融合历史信息与自运动线索，实现记忆增强的目标推理。

- **[2026/03][ arXiv 2026 - 通用视觉语言导航 - Co-Ego ]** Not an Obstacle for Dog, but a Hazard for Human: A Co-Ego Navigation System for Guide Dog Robots [[arxiv]](https://arxiv.org/abs/2603.20121) [[hjfy]](https://hjfy.top/arxiv/2603.20121) `Navigation`
  - 概览：该系统采用双分支避障框架，将机器人地面感知与用户的人体高度视角相融合，实现多层级导航安全。

- **[2026/03][ arXiv 2026 - 通用视觉语言导航 ]** Scene Representation using 360{\deg} Saliency Graph and its Application in Vision-based Indoor Navigation [[arxiv]](https://arxiv.org/abs/2603.20353) [[hjfy]](https://hjfy.top/arxiv/2603.20353) `Navigation`
  - 概览：提出360°显著性图，以节点、边、权重和角位置编码场景的视觉、语义与几何信息；导航时先用该图在拓扑地图中定位当前场景，再由嵌入几何估计下一步移动方向。

- **[2026/03][ arXiv 2026 - 通用零样本具身导航 - E-SocialNav ]** E-SocialNav: Efficient Socially Compliant Navigation with Language Models [[arxiv]](https://arxiv.org/abs/2603.20664) [[hjfy]](https://hjfy.top/arxiv/2603.20664) `Zero-Shot` `Transformer`
  - 概览：提出社会规范导航语言模型E-SocialNav，先以监督微调学习人类标注的导航行为，再用直接偏好优化校正动作选择，并以GPT-4o和Claude作为社会合规性评测参照。

- **[2026/03][ arXiv 2026 - 通用零样本具身导航 - Vision-Sharing ]** Does Peer Observation Help? Vision-Sharing Collaboration for Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2603.20804) [[hjfy]](https://hjfy.top/arxiv/2603.20804) `Zero-Shot` `Memory`
  - 概览：提出模型无关的协作框架Co-VLN，使独立导航智能体在识别到共同经过的位置时交换结构化视觉记忆，从而把同伴观测纳入各自的历史表示。

- **[2026/03][ arXiv 2026 - 通用视觉语言导航 - Vision-Language ]** Dynamic Control Barrier Function Regulation with Vision-Language Models for Safe, Adaptive, and Realtime Visual Navigation [[arxiv]](https://arxiv.org/abs/2603.21142) [[hjfy]](https://hjfy.top/arxiv/2603.21142) `End-to-end` `VLM`
  - 概览：提出的AlphaAdj框架将视觉语言模型（VLM）与控制系统结合，仅通过机器人第一视角的RGB图像，即可动态调整安全屏障的“保守程度”。

- **[2026/03][ arXiv 2026 - 实现动态场景下视觉语言导航 - DyGeoVLN ]** DyGeoVLN: Infusing Dynamic Geometry Foundation Model into Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2603.21269) [[hjfy]](https://hjfy.top/arxiv/2603.21269) `End-to-end`
  - 概览：提出DyGeoVLN，通过跨分支特征融合把动态几何基础模型的显式三维空间表示注入视觉语言导航，并采用无位姿、自适应分辨率的词元剪枝删除长时历史中的时空冗余信息。

- **[2026/03][ arXiv 2026 - 通用零样本具身导航 - Mind over Space ]** Mind over Space: Can Multimodal Large Language Models Mentally Navigate? [[arxiv]](https://arxiv.org/abs/2603.21577) [[hjfy]](https://hjfy.top/arxiv/2603.21577) `Zero-Shot` `Hierarchical` `Pretraining`
  - 概览：构建Video2Mental基准，要求模型从长第一人称视频建立层次认知地图并逐步规划地标路径；进一步提出NavMind，以细粒度认知地图为可学习中间表示，并按难度分层进行渐进监督微调。

- **[2026/03][ arXiv 2026 - 异构多智能体零训练协同导航 ]** Can a Robot Walk the Robotic Dog: Triple-Zero Collaborative Navigation for Heterogeneous Multi-Agent Systems [[arxiv]](https://arxiv.org/abs/2603.21723) [[hjfy]](https://hjfy.top/arxiv/2603.21723) `Agentic`
  - 概览：提出TZPP异构多机器人协作规划框架，由人形机器人担任任务协调者、四足机器人负责探索，并以多模态大模型引导路径可行性判断，在不进行专门训练、先验建图或仿真的条件下协同导航。

- **[2026/03][ arXiv 2026 - 通用视觉语言导航 - Human-Inspired ]** Human-Inspired Pavlovian and Instrumental Learning for Autonomous Agent Navigation [[arxiv]](https://arxiv.org/abs/2603.22170) [[hjfy]](https://hjfy.top/arxiv/2603.22170) `Navigation`
  - 概览：提出一种仿人脑的混合强化学习架构，融合了巴甫洛夫条件反射、工具性反应学习与模型规划三大模块。

- **[2026/03][ arXiv 2026 - 通用视觉语言导航 - Cross-Modal ]** Cross-Modal Reinforcement Learning for Navigation with Degraded Depth Measurements [[arxiv]](https://arxiv.org/abs/2603.22182) [[hjfy]](https://hjfy.top/arxiv/2603.22182) `RL`
  - 概览：开发跨模态Wasserstein自编码器，通过学习共享的潜在表示，使系统能够从灰度观测中推断深度相关特征。

- **[2026/03][ arXiv 2026 - 实现机器人非结构化环境高效自主导航 - CATNAV ]** CATNAV: Cached Vision-Language Traversability for Efficient Zero-Shot Robot Navigation [[arxiv]](https://arxiv.org/abs/2603.22800) [[hjfy]](https://hjfy.top/arxiv/2603.22800) `Zero-Shot`
  - 概览：提出零样本、具身感知的代价图生成框架，基于VLM语义结果推理，结合机器人形态和运动模式推断目标遍历风险，无需任务特定训练。

- **[2026/03][ arXiv 2026 - 状态训练增强长时导航记忆 - StateLinFormer ]** StateLinFormer: Stateful Training Enhancing Long-term Memory in Navigation [[arxiv]](https://arxiv.org/abs/2603.23571) [[hjfy]](https://hjfy.top/arxiv/2603.23571) `End-to-end`
  - 概览：提出StateLinFormer线性注意力导航模型，在相邻训练片段之间持续传递循环记忆状态而非每批重置，使模型近似在无限长序列上学习并保留跨长交互的上下文记忆。

- **[2026/03][ arXiv 2026 - 拓扑意图引导反应式导航 - IntentReact ]** IntentReact: Guiding Reactive Object-Centric Navigation via Topological Intent [[arxiv]](https://arxiv.org/abs/2603.25382) [[hjfy]](https://hjfy.top/arxiv/2603.25382) `GSM`
  - 概览：提出IntentReact物体中心反应式导航框架，以拓扑意图概括长程目标与局部可达关系，并用该高层意图约束实时视觉策略的动作选择。

- **[2026/03][ arXiv 2026 - 强化学习语义场景图导航 ]** Modernising Reinforcement Learning-Based Navigation for Embodied Semantic Scene Graph Generation [[arxiv]](https://arxiv.org/abs/2603.25415) [[hjfy]](https://hjfy.top/arxiv/2603.25415) `World Model`
  - 概览：更新具身语义场景图生成的模块化导航器，比较原子动作单头策略与动作分量多头策略、粗细离散动作集、课程学习和深度碰撞监督，以场景图完整度、执行安全及导航效率联合评估。

- **[2026/03][ arXiv 2026 - 揭示零样本机器人视觉语言导航三大核心局限 ]** Can Vision Foundation Models Navigate? Zero-Shot Real-World Evaluation and Lessons Learned [[arxiv]](https://arxiv.org/abs/2603.25937) [[hjfy]](https://hjfy.top/arxiv/2603.25937) `Benchmark`
  - 概览：构建视觉导航模型真实世界零样本评测，覆盖五种模型、两类机器人及五类室内外环境，并联合路径、目标识别、碰撞与视觉扰动指标分析几何理解、地点消歧和分布偏移问题。

- **[2026/03][ arXiv 2026 - 无监督探索与离线强化学习图像目标导航 - MINav ]** 120 Minutes and a Laptop: Minimalist Image-goal Navigation via Unsupervised Exploration and Offline RL [[arxiv]](https://arxiv.org/abs/2603.26441) [[hjfy]](https://hjfy.top/arxiv/2603.26441) `Zero-Shot`
  - 概览：提出MINav极简图像目标导航方法，以无监督探索收集数据、事后目标重标记和离线目标条件强化学习，在消费级笔记本上两小时内完成数据采集、训练和实机部署。

- **[2026/03][ arXiv 2026 - 实现机器人零样本自主导航 - SpatialAnt ]** SpatialAnt: Autonomous Zero-Shot Robot Navigation via Active Scene Reconstruction and Visual Anticipation [[arxiv]](https://arxiv.org/abs/2603.26837) [[hjfy]](https://hjfy.top/arxiv/2603.26837) `Zero-Shot`
  - 概览：提出SpatialAnt零样本导航框架，以物理落地策略为单目自建场景恢复绝对尺度，再利用噪声点云渲染未来观测进行反事实视觉预判，排除与语言指令矛盾的候选路径。

- **[2026/03][ arXiv 2026 - 多模态知识库增强VLN ]** Beyond Textual Knowledge-Leveraging Multimodal Knowledge Bases for Enhancing Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2603.26859) [[hjfy]](https://hjfy.top/arxiv/2603.26859) `End-to-end`
  - 概览：提出BTK框架，用Qwen3提取目标短语、Flux构建R2R-GP与REVERIE-GP生成图像知识库，并由BLIP-2从全景图构建环境文本知识库，再通过Goal-Aware Augmentor和Knowledge Augmentor融合这些知识。

- **[2026/03][ arXiv 2026 - 结构化观测语言高效VLN ]** Structured Observation Language for Efficient and Generalizable Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2603.27577) [[hjfy]](https://hjfy.top/arxiv/2603.27577) `End-to-end`
  - 概览：提出SOL-Nav，把RGB-D划分为网格并为每格提取语义、颜色与深度，形成紧凑结构化观测语言，再与导航指令拼接为纯文本输入预训练语言模型，以降低视觉预训练依赖。

- **[2026/03][ arXiv 2026 - 一个定位置，一个辨朝向 - RHO ]** RHO: Robust Holistic OSM-Based Metric Cross-View Geo-Localization [[arxiv]](https://arxiv.org/abs/2603.27758) [[hjfy]](https://hjfy.top/arxiv/2603.27758) `End-to-end`
  - 概览：构建含多种天气、光照与传感器噪声的CV-RHO跨视角定位基准，并提出双分支Pin-Pan架构联合估计位置和朝向。

- **[2026/03][ arXiv 2026 - 层级语义拓扑度量终身导航 - osmAG-Nav ]** osmAG-Nav: A Hierarchical Semantic Topometric Navigation Stack for Robust Lifelong Indoor Autonomy [[arxiv]](https://arxiv.org/abs/2603.28271) [[hjfy]](https://hjfy.top/arxiv/2603.28271) `Hierarchical`
  - 概览：提出osmAG-Nav层级语义拓扑度量导航栈，以兼容OpenStreetMap的osmAG室内地图统一长期定位、语义任务规划和局部运动执行，支持持续更新与跨楼层导航。

- **[2026/03][ arXiv 2026 - 实现高效开放词汇机器人自主导航 - DRIVE-Nav ]** DRIVE-Nav: Directional Reasoning, Inspection, and Verification for Efficient Open-Vocabulary Navigation [[arxiv]](https://arxiv.org/abs/2603.28691) [[hjfy]](https://hjfy.top/arxiv/2603.28691) `Zero-Shot`
  - 概览：提出DRIVE-Nav开放词汇导航框架，以持久化方向组织探索、通过加权快速行进法提取方向候选，并结合视觉语言提示和跨帧验证减少重复访问与语义误判。

- **[2026/03][ arXiv 2026 - 通用视觉语言导航 ]** Bootstrap Perception Under Hardware Depth Failure for Indoor Robot Navigation [[arxiv]](https://arxiv.org/abs/2603.28890) [[hjfy]](https://hjfy.top/arxiv/2603.28890) `Navigation`
  - 概览：提出硬件深度失效下的自举感知系统，以二维激光雷达作为几何锚点，保留ToF相机的有效像素并用其校准单目深度尺度，只在传感器缺失区域补入学习深度。

- **[2026/03][ AAAI 2026 - 高层指令空间导航 - SpNav ]** What You See is What You Reach: Towards Spatial Navigation with High-Level Human Instructions [[doi]](https://doi.org/10.1609/aaai.v40i15.38258) `VLM`
  - 概览：提出空间目标导航与空间区域导航任务，构建一万条AI2-THOR轨迹，并以SpNav通过VLM解析高层指令、空间指向和地图动作变换完成仿真与实景导航。

- **[2026/02][ Sensors 2026 - 大模型增强VLN综述 ]** Large-Scale Model-Enhanced Vision-Language Navigation: Recent Advances, Practical Applications, and Future Challenges [[doi]](https://doi.org/10.3390/s26072022) `Survey`
  - 概览：从指令理解、环境感知、高层规划与低层控制四个组件梳理大模型增强VLN，并总结数据、仿真、评价和边缘部署技术及其工程挑战。

- **[2026/02][ arXiv 2026 - 任务驱动生成式BEV地图学习 - MapDream ]** MapDream: Task-Driven Map Learning for Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2602.00222) [[hjfy]](https://hjfy.top/arxiv/2602.00222) [[project]](https://horizonrobotics.github.io/robot_lab/mapdream) `World Model`
  - 概览：提出"地图在环"框架，将地图构建形式化为自回归BEV图像生成并与动作预测联合学习，经监督预训练与强化微调实现端到端优化，在R2R-CE与RxR-CE上取得单目SOTA性能。

- **[2026/02][ arXiv 2026 - 回溯校正抗漂移VLN在线训练 - BudVLN ]** Nipping the Drift in the Bud: Retrospective Rectification for Robust Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2602.06356) [[hjfy]](https://hjfy.top/arxiv/2602.06356) `End-to-end`
  - 概览：针对模仿学习曝光偏差及DAgger式纠错的指令-状态错位问题，提出在线框架BudVLN，通过反事实重锚定与决策条件监督合成实现回溯校正，在R2R-CE与RxR-CE上取得SOTA成功率与SPL。

- **[2026/02][ arXiv 2026 - 面向零样本目标导航的高泛化性记忆-执行-评估框架 - MerNav ]** MerNav: A Highly Generalizable Memory-Execute-Review Framework for Zero-Shot Object Goal Navigation [[arxiv]](https://arxiv.org/abs/2602.05467) [[hjfy]](https://hjfy.top/arxiv/2602.05467) `Zero-Shot`
  - 概览：提出MerNav的Memory-Execute-Review框架，以层次记忆为决策提供环境信息，Execute模块处理常规动作，Review模块检测异常并复核、纠正行为，用于免训练和零样本物体目标导航。

- **[2026/02][ arXiv 2026 - 融入用户习惯的个性化物体导航基准 ]** User-Centric Object Navigation: A Benchmark with Integrated User Habits for Personalized Embodied Object Search [[arxiv]](https://arxiv.org/abs/2602.06459) [[hjfy]](https://hjfy.top/arxiv/2602.06459) `Benchmark`
  - 概览：构建UcON用户中心物体导航基准，收录约22600条用户放置习惯和489类目标物体，用于评测智能体在个性化家庭布置下的搜索能力；同时提出习惯检索模块，为目标物体提取相关习惯并据此推断可能位置。

- **[2026/02][ arXiv 2026 - 超像素图约束松弛实现类人高效导航 - SuReNav ]** SuReNav: Superpixel Graph-based Constraint Relaxation for Navigation in Over-constrained Environments [[arxiv]](https://arxiv.org/abs/2602.06807) [[hjfy]](https://hjfy.top/arxiv/2602.06807) `GSM`
  - 概览：提出SuReNav，以带区域约束的超像素图表示导航空间，用人类示范训练图神经网络判断最小软约束松弛，并交错执行约束松弛、路径规划和机器人运动，同时保持硬约束不可违反。

- **[2026/02][ arXiv 2026 - 基于自适应快慢双过程推理的目标导航 - Hydra-Nav ]** Hydra-Nav: Object Navigation via Adaptive Dual-Process Reasoning [[arxiv]](https://arxiv.org/abs/2602.09972) [[hjfy]](https://hjfy.top/arxiv/2602.09972) `End-to-end`
  - 概览：提出Hydra-Nav统一VLM，在分析探索历史并制定计划的慢系统与执行动作的快系统间自适应切换；通过空间—动作对齐、记忆—推理融合和迭代拒绝微调三阶段课程训练，并以成功率加权操作时间衡量搜索效率。

- **[2026/02][ arXiv 2026 - 视界自适应多轮强化学习长时程导航 - LongNav-R1 ]** LongNav-R1: Horizon-Adaptive Multi-Turn RL for Long-Horizon VLA Navigation [[arxiv]](https://arxiv.org/abs/2602.12351) [[hjfy]](https://hjfy.top/arxiv/2602.12351) `Zero-Shot`
  - 概览：提出LongNav-R1，将长时导航重构为VLA策略与具身环境的连续多轮交互，使模型从在线轨迹学习历史动作与远期结果；进一步以Horizon-Adaptive Policy Optimization适配不同序列长度的优势估计和时间信用分配。

- **[2026/02][ arXiv 2026 - 显式世界表征几何感知VLN - GTA ]** One Agent to Guide Them All: Empowering MLLMs for Vision-and-Language Navigation via Explicit World Representation [[arxiv]](https://arxiv.org/abs/2602.15400) [[hjfy]](https://hjfy.top/arxiv/2602.15400) `BEV`
  - 概览：提出解耦式MLLM导航框架，将低层空间状态估计与高层语义规划分开，并以可交互的度量世界表征保存一致几何信息；MLLM在该表征上进行反事实推理，再由度量约束保证动作物理可行。

- **[2026/02][ arXiv 2026 - 解耦大模型语义推理与确定性规划 - ReasonNavi ]** ReasonNavi: Human-Inspired Global Map Reasoning for Zero-Shot Embodied Navigation [[arxiv]](https://arxiv.org/abs/2602.15864) [[hjfy]](https://hjfy.top/arxiv/2602.15864) `Zero-Shot`
  - 概览：提出ReasonNavi，把顶视地图分割为房间并采样候选目标节点，由MLLM分阶段选择最符合物体、图像或文本目标的节点，再在在线占据图上用确定性规划器把所选航点落为可执行轨迹。

- **[2026/02][ arXiv 2026 - 面向条件化能力室内导航的视觉语言模型测试基准 - CapNav ]** CapNav: Benchmarking Vision Language Models on Capability-conditioned Indoor Navigation [[arxiv]](https://arxiv.org/abs/2602.18424) [[hjfy]](https://hjfy.top/arxiv/2602.18424) `Benchmark`
  - 概览：构建CapNav能力条件导航基准，以五类人或机器人主体的尺寸、移动能力和环境交互能力约束路径可行性，包含45个真实室内场景、473项导航任务和2365组问答，用于评测VLM对物理与操作限制的推理。

- **[2026/02][ arXiv 2026 - 全局-局部双智能体场景导航 ]** Global Commander and Local Operative: A Dual-Agent Framework for Scene Navigation [[arxiv]](https://arxiv.org/abs/2602.18941) [[hjfy]](https://hjfy.top/arxiv/2602.18941) `Zero-Shot`
  - 概览：提出DACo双智能体场景导航框架，由Global Commander负责高层动态子目标规划、Local Operative负责第一人称观测和细粒度执行，并通过自适应重规划在长时域任务中纠正指令漂移。

- **[2026/02][ arXiv 2026 - 开放词汇野外长距目标搜索 - WildOS ]** WildOS: Open-Vocabulary Object Search in the Wild [[arxiv]](https://arxiv.org/abs/2602.19308) [[hjfy]](https://hjfy.top/arxiv/2602.19308) `End-to-end`
  - 概览：提出WildOS长距离开放词汇目标搜索系统，以稀疏导航图保存空间记忆，由ExploRFM联合评估前沿可通行性、探索价值和目标相似度，并用粒子滤波估计远距目标位置。

- **[2026/02][ arXiv 2026 - 通用视觉语言导航 - Vision-Language ]** Enhancing Vision-Language Navigation with Multimodal Event Knowledge from Real-World Indoor Tour Videos [[arxiv]](https://arxiv.org/abs/2602.23937) [[hjfy]](https://hjfy.top/arxiv/2602.23937) `Hierarchical` `Memory` `Retrieval`
  - 概览：构建含8.6万节点和8.3万边的多模态时空知识图谱YE-KG，将室内导览视频抽取为“语义—动作—效果”事件；STE-VLN再以粗到细层次检索取回因果事件链，并与第一人称观测动态融合。

- **[2026/01][ arXiv 2026 - 显式空间感知与探索的零样本VLN - Spatial-VLN ]** Spatial-VLN: Zero-Shot Vision-and-Language Navigation With Explicit Spatial Perception and Exploration [[arxiv]](https://arxiv.org/abs/2601.12766) [[hjfy]](https://hjfy.top/arxiv/2601.12766) [[project]](https://yueluhhxx.github.io/Spatial-VLN-web/) `Zero-Shot`
  - 概览：针对零样本VLN中门交互、多房间导航与指令歧义三大空间难题，提出空间感知增强(SPE)与探索多专家推理(EMR)模块构建跨视角一致的空间表征，在VLN-CE上取得零样本SOTA并完成真机迁移。

- **[2026/01][ arXiv 2026 - 空间场景图零样本VLN - SpatialNav ]** SpatialNav: Leveraging Spatial Scene Graphs for Zero-Shot Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2601.06806) [[hjfy]](https://hjfy.top/arxiv/2601.06806) `Zero-Shot`
  - 概览：构建空间场景图(SSG)显式刻画已探索环境的全局空间结构与语义，融合智能体中心空间建图、罗盘对齐视觉表征与远距物体定位，在离散与连续环境中均大幅超越现有零样本导航智能体。

- **[2026/01][ CVPR 2026 - 统一多模态思维链隐式推理导航 - FantasyVLN ]** FantasyVLN: Unified Multimodal Chain-of-Thought Reasoning for Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2601.13976) [[hjfy]](https://hjfy.top/arxiv/2601.13976) [[github]](https://github.com/Fantasy-AMAP/fantasy-vln) `End-to-end`
  - 概览：提出统一隐式多模态思维链推理框架，用预训练视觉自回归模型将想象视觉token编码进紧凑潜空间，联合文本/视觉/多模态CoT训练，推理时直接完成指令到动作映射，延迟较显式CoT降低一个数量级。

- **[2026/01][ arXiv 2026 - 逆动力学增强VLN - NaVIDA ]** NaVIDA: Vision-Language Navigation with Inverse Dynamics Augmentation [[arxiv]](https://arxiv.org/abs/2601.18188) [[hjfy]](https://hjfy.top/arxiv/2601.18188) [[github]](https://github.com/waynechu1021/NAVIDA) `End-to-end` `Qwen2.5-VL-3B`
  - 概览：提出以逆动力学监督为显式目标的VLN框架，结合分层概率动作分块将轨迹组织为多步块以提供长程视觉线索，仅用3B参数即超越8B规模的SOTA方法并完成真机验证。

- **[2026/01][ arXiv 2026 - 自适应推理与语言记忆导航VLA - VLingNav ]** VLingNav: Embodied Navigation with Adaptive Reasoning and Visual-Assisted Linguistic Memory [[arxiv]](https://arxiv.org/abs/2601.08665) [[hjfy]](https://hjfy.top/arxiv/2601.08665) [[project]](https://wsakobe.github.io/VLingNav-web/) `End-to-end`
  - 概览：提出语言认知驱动的具身导航VLA模型，自适应思维链按需切换快慢思考，视觉辅助语言记忆支撑长时程导航，并构建最大规模推理标注数据集Nav-AdaCoT-2.9M，多基准SOTA且零样本迁移实机。

- **[2026/01][ arXiv 2026 - 序列长程VLN分层规划 - SeqWalker ]** SeqWalker: Sequential-Horizon Vision-and-Language Navigation with Hierarchical Planning [[arxiv]](https://arxiv.org/abs/2601.04699) [[hjfy]](https://hjfy.top/arxiv/2601.04699) [[github]](https://github.com/SeqWalker/SeqWalker-code) [[project]](https://seqwalker.github.io/seqwalker/) `Hierarchical`
  - 概览：提出分层规划框架SeqWalker求解多任务复杂指令下的序列长程VLN，高层规划器依据视觉观测筛选相关子指令，底层规划器以探索-验证策略纠正轨迹，并扩展IVLN数据集构建新基准。

- **[2026/01][ arXiv 2026 - 动态户外场景中自主移动机器人的长期具身导航系统 - CausalNav ]** CausalNav: A Long-term Embodied Navigation System for Autonomous Mobile Robots in Dynamic Outdoor Scenarios [[arxiv]](https://arxiv.org/abs/2601.01872) [[hjfy]](https://hjfy.top/arxiv/2601.01872) `Hierarchical`
  - 概览：提出CausalNav动态户外语义导航系统，以LLM把粗粒度地图和细粒度实体组织为多层Embodied Graph，并通过RAG执行开放词汇长程规划；图谱融合实时感知、显式处理动态物体并在时间窗内持续更新。

- **[2026/01][ arXiv 2026 - 下一代具身AI研究平台 - VirtualEnv ]** VirtualEnv: A Platform for Embodied AI Research [[arxiv]](https://arxiv.org/abs/2601.07553) [[hjfy]](https://hjfy.top/arxiv/2601.07553) `Agentic`
  - 概览：发布UE5仿真平台VirtualEnv，支持导航、物体操作、自适应多智能体协作、密室和程序化环境，并提供自然语言控制API及由LLM/VLM从多模态输入生成、验证和实时控制任务的流程。

- **[2026/01][ arXiv 2026 - 基于快慢交互推理的通用视觉语言导航 ]** Towards Open Environments and Instructions: General Vision-Language Navigation via Fast-Slow Interactive Reasoning [[arxiv]](https://arxiv.org/abs/2601.09111) [[hjfy]](https://hjfy.top/arxiv/2601.09111) `End-to-end`
  - 概览：提出slow4fast-VLN：快推理策略实时执行并把轨迹记录到历史库，慢推理模块分析记忆、反思并提取结构化经验，再将这些经验回写以持续优化快系统在开放场景中的决策。

- **[2026/01][ arXiv 2026 - 长时记忆赋能具身探索与场景问答 ]** Explore with Long-term Memory: A Benchmark and Multimodal LLM-based Reinforcement Learning Framework for Embodied Exploration [[arxiv]](https://arxiv.org/abs/2601.10744) [[hjfy]](https://hjfy.top/arxiv/2601.10744) `Benchmark`
  - 概览：新范式+新基准：提出LMEE长时记忆具身探索范式，融合多目标导航与记忆问答；构建LMEEBench基准，从导航效率、记忆问答双维度评估智能体认知与决策，数据集包含246类物体、9000+目标与问题、1982条真实探索轨迹。

- **[2026/01][ arXiv 2026 - 人形机器人局部导航中的空间选择性注意力与导航点引导方法 - FocusNav ]** FocusNav: Spatial Selective Attention with Waypoint Guidance for Humanoid Local Navigation [[arxiv]](https://arxiv.org/abs/2601.12790) [[hjfy]](https://hjfy.top/arxiv/2601.12790) `End-to-end`
  - 概览：提出了空间选择性注意力框架FocusNav：通过Waypoint-Guided Spatial Cross-Attention（WGSCA）机制，将导航意图与环境上下文对齐，确保特征聚合与预测轨迹空间锚定。

- **[2026/01][ arXiv 2026 - 城市环境下视觉语言模型的跨视角空间推理基准测试 - CityCube ]** CityCube: Benchmarking Cross-view Spatial Reasoning on Vision-Language Models in Urban Environments [[arxiv]](https://arxiv.org/abs/2601.14339) [[hjfy]](https://hjfy.top/arxiv/2601.14339) `Benchmark`
  - 概览：构建CityCube城市跨视角空间推理基准，覆盖车辆、无人机和卫星等平台的四类视点变化，提供5,022组多视图问答以评测五个认知维度和三类空间关系。

- **[2026/01][ arXiv 2026 - 双重验证可靠LLM导航 - DV-VLN ]** DV-VLN: Dual Verification for Reliable LLM-Based Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2601.18492) [[hjfy]](https://hjfy.top/arxiv/2601.18492) `Verification`
  - 概览：提出DV-VLN生成后验证框架，先用参数高效域内适配的LLaMA-2生成结构化导航思维链，再以真假验证和遮蔽实体验证两条通道检验候选动作，并聚合多次采样的验证结果重排序。

- **[2026/01][ arXiv 2026 - 面向目标导航的双立场协同辩论机制 - DSCD-Nav ]** DSCD-Nav: Dual-Stance Cooperative Debate for Object Navigation [[arxiv]](https://arxiv.org/abs/2601.21409) [[hjfy]](https://hjfy.top/arxiv/2601.21409) `Zero-Shot`
  - 概览：提出免训练DSCD-Nav，让任务—场景理解立场与安全—信息平衡立场针对同一候选动作集进行证据化协同辩论，再由导航共识仲裁器整合双方理由，并在选择不确定时触发轻量微探测。

- **[2026/01][ arXiv 2026 - 动态拓扑粒度自适应VLN - DGNav ]** Dynamic Topology Awareness: Breaking the Granularity Rigidity in Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2601.21751) [[hjfy]](https://hjfy.top/arxiv/2601.21751) `GSM`
  - 概览：提出DGNav处理连续VLN中的拓扑粒度刚性：场景感知自适应策略根据预测航点的离散程度动态调节建图阈值，动态图Transformer再融合视觉、语言和几何线索形成边权，以按环境复杂度调整节点密度与连通性。

- **[2026/01][ Visual Intelligence 2026 - 多模态LLM导航智能体 - NavGemini ]** NavGemini: a multi-modal LLM agent for vision-and-language navigation [[doi]](https://doi.org/10.1007/s44267-025-00105-x) `Agentic`
  - 概览：提出NavGemini，直接以Gemini-Pro-Vision联合处理当前观测和指令，并通过子任务拆分、指令缩减、回溯与终止检查控制上下文成本，完成零样本VLN。

- **[2026/01][ TCSVT 2026 - 空间感知与视角鲁棒VLN - SV-VLN ]** Spatial-Aware and Viewpoint-Robust Vision-Language Navigation [[doi]](https://doi.org/10.1109/TCSVT.2026.3682894) `3DGS`
  - 概览：提出包含航点、物体、房间和楼层的四层异构地图，并以三维高斯溅射筛选和补充稳健视角特征，支持长距离、跨楼层连续VLN。

- **[2026/X][ TIP 2026 - 单目VLN全景感知指令语义 - ThinkMatter ]** ThinkMatter: Panoramic-Aware Instructional Semantics for Monocular Vision-and-Language Navigation [[ieee]](https://ieeexplore.ieee.org/document/11367385) [[smu]](https://ink.library.smu.edu.sg/sis_research/10905) `End-to-end` `3DGS`
  - 概览：面向仅配备单目受限视野相机的低成本VLN-CE场景，提出基于3DGS的全景新视角生成与占据图-指令语义融合框架，让单目机器人"想得更多"，在仿真与真实环境中均验证有效。

- **[2026/X][ ACM TOMM 2026 - LLM辅助类人导航指令生成 - CaneSpeaker ]** CaneSpeaker: An LLM-Assisted Speaker for Generating Human-Like Navigation Instructions [[doi]](https://doi.org/10.1145/3785009) [[github]](https://github.com/zheng19845/CaneSpeaker) `Benchmark`
  - 概览：提出LLM辅助的Speaker模型CaneSpeaker，仅凭前视RGB图像生成多风格类人导航指令，并基于Matterport3D中17.8万条未标注路径合成跨任务增强数据集CANE缓解VLN数据稀缺。

- **[2026/X][ ICML 2026 - 三维交互链联合导航与操作 - 3D-IC ]** Joint Navigation and Manipulation Planning with 3D Interaction Chains [[openreview]](https://openreview.net/forum?id=oVB2xYWvpv) [[github]](https://github.com/kekeZ66/3D-IC) `Mobile Manipulation`
  - 概览：以共享三维特征图统一导航和操作表征，将找物、抓取、容器导航与放置组织为候选交互链，并用VLM可行性评分与转移代价联合选择和在线重规划。

- **[2025/12][ arXiv 2025 - 高效训练推理VLN基线 - Efficient-VLN ]** Efficient-VLN: A Simple yet Strong Baseline for Efficient Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2512.10310) [[hjfy]](https://hjfy.top/arxiv/2512.10310) `End-to-end`
  - 概览：提出简洁高效的VLN基线，通过KV缓存复用、防止动作泄漏的掩码训练与自适应数据收集策略，在显著降低训练与推理开销的同时保持主流基准上的领先性能。

- **[2025/12][ arXiv 2025 - 拓扑规划强化微调连续环境VLN - ETP-R1 ]** ETP-R1: Evolving Topological Planning with Reinforcement Fine-tuning for Vision-Language Navigation in Continuous Environments [[arxiv]](https://arxiv.org/abs/2512.20940) [[hjfy]](https://hjfy.top/arxiv/2512.20940) [[github]](https://github.com/Cepillar/ETP-R1) `RL` `Habitat`
  - 概览：将大规模数据预训练与GRPO强化微调范式引入基于拓扑图的VLN-CE模型，首次实现图式策略的闭环在线强化微调，在R2R-CE与RxR-CE基准上刷新SOTA。

- **[2025/12][ arXiv 2025 - 视觉提示与步级策略优化VLN智能体 - SeeNav-Agent ]** SeeNav-Agent: Enhancing Vision-Language Navigation with Visual Prompt and Step-Level Policy Optimization [[arxiv]](https://arxiv.org/abs/2512.02631) [[hjfy]](https://hjfy.top/arxiv/2512.02631) [[github]](https://github.com/WzcTHU/SeeNav-Agent) `RL`
  - 概览：提出双视角视觉提示缓解VLN智能体的感知幻觉，并设计步级可验证奖励与随机分组优势估计的SRGPO强化微调算法，为导航过程提供稠密奖励信号并显著提升成功率。

- **[2025/12][ arXiv 2025 - 双系统VLN基础模型 - DualVLN ]** Ground Slow, Move Fast: A Dual-System Foundation Model for Generalizable Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2512.08186) [[hjfy]](https://hjfy.top/arxiv/2512.08186) [[github]](https://github.com/InternRobotics/InternNav) [[project]](https://internrobotics.github.io/internvla-n1-dualvln.github.io/) `Hierarchical`
  - 概览：提出首个双系统VLN基础模型DualVLN(InternVLA-N1)，System 2用VLM预测中期像素目标，System 1以轻量扩散Transformer策略实时生成连续轨迹，实现"慢定位、快执行"的跨场景泛化导航。

- **[2025/12][ arXiv 2025 - 全动力学VLN评测基准 - VLNVerse ]** VLNVerse: A Benchmark for Vision-Language Navigation with Versatile, Embodied, Realistic Simulation and Evaluation [[arxiv]](https://arxiv.org/abs/2512.19021) [[hjfy]](https://hjfy.top/arxiv/2512.19021) [[project]](https://sihaoevery.github.io/vlnverse/) `Benchmark`
  - 概览：提出大规模VLN基准VLNVerse，以统一任务框架与基于物理的全动力学具身仿真取代传统"幽灵"智能体评测，统一多任务训练与评估并给出多任务基线模型，推动导航方法走向真实世界。

- **[2025/12][ arXiv 2025 - 人机协作视觉语言导航综述 ]** A Survey on Improving Human Robot Collaboration through Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2512.00027) [[hjfy]](https://hjfy.top/arxiv/2512.00027) `Survey`
  - 概览：综述视觉语言导航在人机协作和多机器人系统中的研究进展，重点分析双向通信、指令歧义消解、感知驱动协作及跨学科评测问题。

- **[2025/12][ arXiv 2025 - 通用零样本具身导航 - Dual-Relation ]** Nav-$R^2$ Dual-Relation Reasoning for Generalizable Open-Vocabulary Object-Goal Navigation [[arxiv]](https://arxiv.org/abs/2512.02400) [[hjfy]](https://hjfy.top/arxiv/2512.02400) `Zero-Shot` `Memory` `Planning`
  - 概览：提出面向开放词汇目标导航的双关系推理框架Nav-R2，显式地建模目标-环境（感知）和环境-动作（规划）两种关键关系，并将其整合到一个高效的推理流程中，且未引入额外模型参数。

- **[2025/12][ arXiv 2025 - 具身问答弃权能力基准发布 ]** When Robots Should Say "I Don't Know": Benchmarking Abstention in Embodied Question Answering [[arxiv]](https://arxiv.org/abs/2512.04597) [[hjfy]](https://hjfy.top/arxiv/2512.04597) `Benchmark`
  - 概览：构建AbstainEQA具身问答弃权基准，将OpenEQA问题改写为行动能力不足、指代不明、偏好依赖、信息不可得和错误预设五类歧义，并形成1,636个弃权样本与1,636个原始问题的平衡评测集。

- **[2025/12][ arXiv 2025 - 以用户需求为导向的视障人士专用视觉导航机器人 - GuideNav ]** GuideNav: User-Informed Development of a Vision-Only Robotic Navigation Assistant For Blind Travelers [[arxiv]](https://arxiv.org/abs/2512.06147) [[hjfy]](https://hjfy.top/arxiv/2512.06147) `End-to-end`
  - 概览：提出GuideNav视觉示教复现式辅助导航系统，以拓扑路线表示、视觉地点识别、时序滤波和相对位姿估计复现示范路径，并发布基于视障用户与导盲犬调研的GuideData。

- **[2025/12][ arXiv 2025 - 通用视觉语言导航 - REASAN ]** REASAN: Learning Reactive Safe Navigation for Legged Robots [[arxiv]](https://arxiv.org/abs/2512.09537) [[hjfy]](https://hjfy.top/arxiv/2512.09537) `Agentic` `End-to-end` `Transformer`
  - 概览：提出REASAN单激光雷达四足安全导航系统，由运动、安全屏障和导航三项强化学习策略及点云Transformer外感知估计器组成，分别在仿真中训练后协同执行实时反应式控制。

- **[2025/12][ arXiv 2025 - 网络规模人类轨迹语言引导城市导航 - UrbanNav ]** UrbanNav: Learning Language-Guided Urban Navigation from Web-Scale Human Trajectories [[arxiv]](https://arxiv.org/abs/2512.09607) [[hjfy]](https://hjfy.top/arxiv/2512.09607) `End-to-end`
  - 概览：提出UrbanNav可扩展城市导航框架，从网络规模人类步行视频构建语言指令、轨迹与地标对齐数据，并训练能泛化到未见城市的语言引导导航策略。

- **[2025/12][ arXiv 2025 - 通用视觉语言导航 - LISN ]** LISN: Language-Instructed Social Navigation with VLM-based Controller Modulating [[arxiv]](https://arxiv.org/abs/2512.09920) [[hjfy]](https://hjfy.top/arxiv/2512.09920) `Hierarchical`
  - 概览：构建语言指令社会导航基准LISN-Bench，并提出快慢分层Social-Nav-Modulator，由低频视觉语言模型调制代价地图和控制器参数、低层控制器实时避障执行。

- **[2025/12][ arXiv 2025 - 面向人类隐性需求的具身城市导航基准 - CitySeeker ]** CitySeeker: How Do VLMS Explore Embodied Urban Navigation With Implicit Human Needs? [[arxiv]](https://arxiv.org/abs/2512.16755) [[hjfy]](https://hjfy.top/arxiv/2512.16755) `End-to-end`
  - 概览：构建CitySeeker隐式需求城市导航基准，包含八座城市的6440条轨迹与七类需求场景，并评测回溯、空间认知增强和记忆检索策略对VLM长程决策的影响。

- **[2025/12][ arXiv 2025 - 通过场景想象促使视觉语言模型成为具身导航器 - ImagineNav++ ]** ImagineNav++: Prompting Vision-Language Models as Embodied Navigator through Scene Imagination [[arxiv]](https://arxiv.org/abs/2512.17435) [[hjfy]](https://hjfy.top/arxiv/2512.17435) `Hierarchical`
  - 概览：提出ImagineNav++无地图导航框架，由未来视图想象模块蒸馏人类导航偏好并生成候选观测，交给VLM选择信息量最高的视图；选择性中央凹记忆再以由稀到密的方式整合关键帧，维持长时空间一致性。

- **[2025/12][ arXiv 2025 - 度量感知视觉几何驱动的定位锚定导航策略 - LoGoPlanner ]** LoGoPlanner: Localization Grounded Navigation Policy with Metric-aware Visual Geometry [[arxiv]](https://arxiv.org/abs/2512.19629) [[hjfy]](https://hjfy.top/arxiv/2512.19629) `End-to-end`
  - 概览：提出LoGoPlanner端到端导航框架，微调长时域视觉几何主干以获得绝对度量尺度和隐式定位，再由历史观测重建周围稠密几何，并以这些辅助任务形成的隐式几何记忆条件化轨迹策略。

- **[2025/12][ arXiv 2025 - 面向终身具身导航的视觉上下文压缩长记忆导航 - AstraNav-Memory ]** AstraNav-Memory: Contexts Compression for Long Memory [[arxiv]](https://arxiv.org/abs/2512.21627) [[hjfy]](https://hjfy.top/arxiv/2512.21627) `End-to-end`
  - 概览：提出统一的终身具身导航框架：构建以图像为中心的上下文记忆，实现视觉、语言和决策的端到端耦合；集成高效视觉上下文压缩模块，将原生ViT的token数量压缩20倍，单帧仅用30个token实现高保真表示，使单个上下文能容纳数百帧历史图像，支撑大规模长期隐式记忆。

- **[2025/12][ arXiv 2025 - VL-LN Bench: 长程主动对话式目标导航新基准 ]** VL-LN Bench: Towards Long-horizon Goal-oriented Navigation with Active Dialogs [[arxiv]](https://arxiv.org/abs/2512.22342) [[hjfy]](https://hjfy.top/arxiv/2512.22342) `End-to-end`
  - 概览：提出允许智能体在导航中主动向Oracle提问的交互式实例目标导航IIGN，并构建VL-LN Bench，包含4.1万余条长时域对话增强轨迹及可自动回应查询的评测Oracle，用于联合训练和评测语言输出与导航动作。

- **[2025/12][ arXiv 2025 - 诊断大语言模型如何用语言指引视觉导航智能体 - VLN-MME ]** VLN-MME: Diagnosing MLLMs as Language-guided Visual Navigation agents [[arxiv]](https://arxiv.org/abs/2512.24851) [[hjfy]](https://hjfy.top/arxiv/2512.24851) `Benchmark`
  - 概览：构建VLN-MME模块化零样本导航评测框架，把传统VLN数据统一为可比较的MLLM智能体接口，并支持跨模型、智能体设计和任务的组件消融；其诊断显示CoT与自反思可能因上下文和3D空间落地不足而降低表现。

- **[2025/11][ arXiv 2025 - 语义进度推理VLN - Progress-Think ]** Progress-Think: Semantic Progress Reasoning for Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2511.17097) [[hjfy]](https://hjfy.top/arxiv/2511.17097) `End-to-end`
  - 概览：提出Progress-Think框架，将语义进度推理引入视觉语言导航，经自对齐进度预训练、进度引导策略预训练与进度-策略联合强化微调三阶段免标注训练，在R2R-CE和RxR-CE上取得SOTA成功率与效率。

- **[2025/11][ SIGSPATIAL 2025 - 结构化空间记忆空间CoT零样本VLN - SpatialGPT ]** SpatialGPT: Zero-Shot Vision-and-Language Navigation via Spatial CoT over Structured Spatial Memory [[doi]](https://dl.acm.org/doi/10.1145/3748636.3762753) `Zero-Shot`
  - 概览：提出SpatialGPT零样本VLN方法，在结构化空间记忆上执行空间思维链推理，使LLM智能体无需任务训练即可理解空间关系并完成指令导航。

- **[2025/11][ arXiv 2025 - 双过程思维零样本VLN系统 - R3 ]** Run, Ruminate, and Regulate: A Dual-process Thinking System for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2511.14131) [[hjfy]](https://hjfy.top/arxiv/2511.14131) [[github]](https://github.com/IAII-CAS/navigation_R3) `Zero-Shot`
  - 概览：提出双过程思维框架R3，轻量Transformer专家Runner高效执行常规导航，多模态大模型Ruminator按需进行思维链深度推理，Regulator依据导航进度调度快慢思考模式，在REVERIE上SPL显著超越SOTA。

- **[2025/11][ CVPR 2026 - 多模态3D场景图零样本具身导航 - MSGNav ]** MSGNav: Unleashing the Power of Multi-modal 3D Scene Graph for Zero-Shot Embodied Navigation [[arxiv]](https://arxiv.org/abs/2511.10376) [[hjfy]](https://hjfy.top/arxiv/2511.10376) [[github]](https://github.com/ylwhxht/MSGNav) `Zero-Shot`
  - 概览：提出以动态分配图像替代文本关系边的多模态3D场景图M3DSG及零样本导航系统MSGNav，引入开放词表更新与闭环推理模块，并针对"最后一英里"问题设计视点选择方法。

- **[2025/11][ CVPR 2026 - 经验与思维自进化零样本VLN智能体 - EvoNav ]** History to Future: Evolving Agent with Experience and Thought for Zero-shot Vision-and-Language Navigation [[cvf]](https://openaccess.thecvf.com/content/CVPR2026/papers/Dai_History_to_Future_Evolving_Agent_with_Experience_and_Thought_for_CVPR_2026_paper.pdf) `Agentic`
  - 概览：提出LLM零样本VLN-CE新范式EvoNav，以未来思维链F-CoT预测动作与地标辅助进度估计和方向选择，以历史经验链H-CoE总结轨迹与场景经验，协同进化智能体决策可靠性。

- **[2025/11][ arXiv 2025 - 室内光照黑盒对抗攻击 - ILA ]** Shedding Light on VLN Robustness: A Black-box Framework for Indoor Lighting-based Adversarial Attack [[arxiv]](https://arxiv.org/abs/2511.13132) [[hjfy]](https://hjfy.top/arxiv/2511.13132) `Benchmark`
  - 概览：提出黑盒室内光照对抗攻击框架ILA，设计静态SILA与动态DILA两种全局光照操纵模式，在三类导航任务上显著提高SOTA VLN模型的失败率，揭示其对真实光照变化的脆弱性。

- **[2025/11][ arXiv 2025 - 通用零样本具身导航 - Fast-SmartWay ]** Fast-SmartWay: Panoramic-Free End-to-End Zero-Shot Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2511.00933) [[hjfy]](https://hjfy.top/arxiv/2511.00933) `Zero-Shot` `End-to-end` `VLM`
  - 概览：提出端到端的零样本视觉语言导航框架Fast-SmartWay：该框架摒弃了典型的全景观察和航点预测器，仅使用三个前方RGB-D图像，结合自然语言指令，直接通过多模态大模型（MLLM）预测导航动作，降低了每一步的处理时间。

- **[2025/11][ arXiv 2025 - 通用视觉语言导航 - MacroNav ]** MacroNav: Multi-Task Context Representation Learning Enables Efficient Navigation in Unknown Environments [[arxiv]](https://arxiv.org/abs/2511.04320) [[hjfy]](https://hjfy.top/arxiv/2511.04320) `RL` `Sim-to-Real` `Representation`
  - 概览：提出多任务自监督表示学习方法，通过结合随机路径掩蔽（SPM）、视野预测（FOV）和掩蔽自编码（MAE）三种任务，同时满足导航所需的全局结构理解、局部几何识别和遮挡鲁棒性。

- **[2025/11][ arXiv 2025 - 通用零样本具身导航 - PanoNav ]** PanoNav: Mapless Zero-Shot Object Navigation with Panoramic Scene Parsing and Dynamic Memory [[arxiv]](https://arxiv.org/abs/2511.06840) [[hjfy]](https://hjfy.top/arxiv/2511.06840) `Zero-Shot` `Memory` `VLM`
  - 概览：提出PanoNav纯RGB无地图零样本导航框架，以全景场景解析向多模态大模型提供空间关系，并用动态有界记忆队列保存探索历史、辅助决策以避免局部循环。

- **[2025/11][ arXiv 2025 - 通用零样本具身导航 - Expand Your SCOPE ]** Expand Your SCOPE: Semantic Cognition over Potential-Based Exploration for Embodied Visual Navigation [[arxiv]](https://arxiv.org/abs/2511.08935) [[hjfy]](https://hjfy.top/arxiv/2511.08935) [[github]](https://github.com/mrwangyou/SCOPE) `Zero-Shot` `Memory` `VLM`
  - 概览：提出SCOPE零样本导航框架，以视觉语言模型估计探索边界的目标相关势能并组织为时空潜在图支持长程规划，再通过自我复议机制回看和修正先前决策。

- **[2025/11][ arXiv 2025 - 通用零样本具身导航 - PIGEON ]** PIGEON: VLM-Driven Object Navigation via Points of Interest Selection [[arxiv]](https://arxiv.org/abs/2511.13207) [[hjfy]](https://hjfy.top/arxiv/2511.13207) [[github]](https://github.com/pechpo/pigeon) `Zero-Shot` `Sim-to-Real` `Planning`
  - 概览：提出PIGEON，将探索边界、疑似目标、楼梯和楼层摘要表示为带原始第一人称观测的可执行兴趣点；VLM只选择关键兴趣点，低层规划器负责其间连续运动，并用可验证奖励微调本地VLM。

- **[2025/11][ arXiv 2025 - 通用具身导航基准 - RoboTidy ]** RoboTidy : A 3D Gaussian Splatting Household Tidying Benchmark for Embodied Navigation and Action [[arxiv]](https://arxiv.org/abs/2511.14161) [[hjfy]](https://hjfy.top/arxiv/2511.14161) `Benchmark` `VLA` `End-to-end`
  - 概览：提出RoboTidy基准测试：是用于语言引导的家庭整理的统一基准，支持视觉语言行动（VLA）和视觉语言导航（VLN）的训练和评估。

- **[2025/11][ arXiv 2025 - 通用视觉语言导航 - SocialNav ]** SocialNav: Training Human-Inspired Foundation Model for Socially-Aware Embodied Navigation [[arxiv]](https://arxiv.org/abs/2511.21135) [[hjfy]](https://hjfy.top/arxiv/2511.21135) `RL` `Hierarchical` `IL`
  - 概览：提出SocialNav社会导航基础模型，以分层“认知—动作”架构连接社会规范推理与低层轨迹生成；其7百万样本SocNav数据集含认知监督和多来源专家轨迹，并通过模仿学习与SAFE-GRPO分阶段训练。

- **[2025/11][ arXiv 2025 - 通用零样本具身导航 - MG-Nav ]** MG-Nav: Dual-Scale Visual Navigation via Sparse Spatial Memory [[arxiv]](https://arxiv.org/abs/2511.22609) [[hjfy]](https://hjfy.top/arxiv/2511.22609) `Zero-Shot` `Memory` `Pretraining`
  - 概览：设计稀疏空间记忆图（SMG）：这是一种区域中心化的多视图记忆图表示，能够高效地进行混合检索和节点级全局规划。

- **[2025/10][ arXiv 2025 - 通用视觉语言导航 - NavSpace ]** NavSpace: How Navigation Agents Follow Spatial Intelligence Instructions [[arxiv]](https://arxiv.org/abs/2510.08173) [[hjfy]](https://hjfy.top/arxiv/2510.08173) [[project]](https://navspace.github.io/) [[github]](https://github.com/TidalHarley/NavSpace) `Navigation` `VLM`
  - 概览：提出空间智能导航基准NavSpace：基于问卷调查，NavSpace包含1228个高质量的轨迹-指令对，覆盖垂直感知、精确移动、视角转换、空间关系、环境状态和空间结构等六种空间智能能力，为评估导航智能体的空间智能提供了全面的基准。

- **[2025/10][ arXiv 2025 - 通用视觉语言导航 - Dream to Recall ]** Dream to Recall: Imagination-Guided Experience Retrieval for Memory-Persistent Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2510.08553) [[hjfy]](https://hjfy.top/arxiv/2510.08553) [[github]](https://github.com/xyz9911/Memoir) `World Model` `Memory` `Retrieval`
  - 概览：开发Memoir框架：通过语言条件化的世界模型编码导航历史并生成想象轨迹作为检索查询，混合视角级记忆（HVM）存储观察和行为模式，以及经验增强的导航模型整合检索到的信息以进行稳健决策。

- **[2025/10][ arXiv 2025 - 通用视觉语言导航 - CompassNav ]** CompassNav: Steering From Path Imitation To Decision Understanding In Navigation [[arxiv]](https://arxiv.org/abs/2510.10154) [[hjfy]](https://hjfy.top/arxiv/2510.10154) [[project]](https://linengcs.github.io/CompassNav/) [[github]](https://github.com/linengcs/CompassNav) `Navigation` `VLM`
  - 概览：提出CompassNav，以Compass-Data-22k为所有可行动作标注A*测地距离，并设计差距感知混合奖励，在SFT后进行强化微调，使模型按候选动作相对质量而非单一路径模仿学习导航决策。

- **[2025/10][ arXiv 2025 - 通用视觉语言导航 - SUM-AgriVLN ]** SUM-AgriVLN: Spatial Understanding Memory for Agricultural Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2510.14357) [[hjfy]](https://hjfy.top/arxiv/2510.14357) [[github]](https://github.com/AlexTraveling/SUM-AgriVLN) `Memory`
  - 概览：提出空间理解记忆（SUM）模块，通过3D重建和表示实现空间理解和空间记忆的保存。

- **[2025/10][ arXiv 2025 - 通用视觉语言导航 - NavQ ]** NavQ: Learning a Q-Model for Foresighted Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2510.16457) [[hjfy]](https://hjfy.top/arxiv/2510.16457) `VLN`
  - 概览：构建跨模态未来编码器：将任务无关的Q特征与导航指令相结合，生成反映未来前景的动作分数，与基于历史信息的原始决策过程相结合，实现了A*风格的搜索策略。

- **[2025/10][ arXiv 2025 - 基于导航地图缓存与检索的目标导航 - EfficientNav ]** EfficientNav: Towards On-Device Object-Goal Navigation with Navigation Map Caching and Retrieval [[arxiv]](https://arxiv.org/abs/2510.18546) [[hjfy]](https://hjfy.top/arxiv/2510.18546) `Zero-Shot`
  - 概览：提出EfficientNav端侧目标导航框架，先以语义感知记忆检索裁剪导航地图中的冗余信息，再通过注意力式记忆聚类为各组独立计算并复用KV缓存，以适配小型本地LLM的容量和时延限制。

- **[2025/10][ arXiv 2025 - 通用零样本具身导航 - LaViRA ]** LaViRA: Language-Vision-Robot Actions Translation for Zero-Shot Vision Language Navigation in Continuous Environments [[arxiv]](https://arxiv.org/abs/2510.19655) [[hjfy]](https://hjfy.top/arxiv/2510.19655) `Zero-Shot` `Hierarchical` `Sim-to-Real`
  - 概览：提出分层导航框架LaViRA：针对零样本视觉语言导航（Zero-Shot VLN-CE），将导航动作解耦为语言动作（Language Action）、视觉动作（Vision Action）和机器人动作（Robot Action）三个层级，实现了从高层规划到底层控制的有效转化。

- **[2025/10][ arXiv 2025 - 通用零样本具身导航 - LagMemo ]** LagMemo: Language 3D Gaussian Splatting Memory for Multi-modal Open-vocabulary Multi-goal Visual Navigation [[arxiv]](https://arxiv.org/abs/2510.24118) [[hjfy]](https://hjfy.top/arxiv/2510.24118) [[project]](https://weekgoodday.github.io/lagmemo/) `Zero-Shot` `Memory`
  - 概览：提出LagMemo，在一次探索中构建具有空间—语义关联的语言3D高斯记忆；收到多模态开放词汇目标后查询候选位置，并用局部感知验证和动态匹配目标，同时整理GOAT-Core作为评测子集。

- **[2025/10][ arXiv 2025 - 通用视觉语言导航 - NaviTrace ]** NaviTrace: Evaluating Embodied Navigation of Vision-Language Models [[arxiv]](https://arxiv.org/abs/2510.26909) [[hjfy]](https://hjfy.top/arxiv/2510.26909) `Human Preference` `VLM`
  - 概览：构建NaviTrace视觉问答式导航基准，给定指令和人、四足、轮式或自行车实体类型，要求模型在图像空间输出二维轨迹；数据含1,000个场景、3,000余条专家轨迹，并以语义感知轨迹分数评测。

- **[2025/10][ ICCV 2025 - 单目与全景观测对齐 - monoVLN ]** monoVLN: Bridging the Observation Gap between Monocular and Panoramic Vision and Language Navigation [[doi]](https://doi.org/10.1109/ICCV51701.2025.00884) `Domain Adaptation`
  - 概览：提出monoVLN，以三维高斯表示弥合单目机器人观测与全景VLN训练设定之间的差异，在保持较低传感器需求的同时恢复可用于指令跟随的场景上下文。

- **[2025/10][ ACM MM 2025 - 可变环境视觉语言导航 - VLN-ChEnv ]** VLN-ChEnv: Vision-language Navigation in Changeable Environments [[doi]](https://doi.org/10.1145/3746027.3755202) `Robust VLN`
  - 概览：构建可变环境VLN设定，通过路径阻塞、地标变化和指令环境不一致等扰动评测导航鲁棒性，并提出相应适应方法处理执行过程中的场景变化。

- **[2025/09][ ICCV 2025 - 远程向导多轮对话导航 - DialNav ]** DialNav: Multi-turn Dialog Navigation with a Remote Guide [[arxiv]](https://arxiv.org/abs/2509.12894) [[hjfy]](https://hjfy.top/arxiv/2509.12894) `Benchmark`
  - 概览：提出协作式具身对话导航任务DialNav，导航智能体与远程向导通过多轮对话推断位置并抵达目标，发布含真人对话与导航轨迹的RAIN数据集及整体评测基准。

- **[2025/09][ ACM TOMM 2025 - 动作感知视觉文本对齐长指令VLN ]** Action-Aware Visual-Textual Alignment for Long-Instruction Vision-and-Language Navigation [[doi]](https://doi.org/10.1145/3748656) `End-to-end`
  - 概览：面向长指令VLN提出动作感知的视觉-文本对齐方法，显式对齐指令中的动作短语与视觉观测，充分利用长指令与长轨迹中的上下文信息以提升长程导航表现。

- **[2025/09][ CoRL 2025 - 指令图约束免训练VLN - GC-VLN ]** GC-VLN: Instruction as Graph Constraints for Training-free Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2509.10454) [[hjfy]](https://hjfy.top/arxiv/2509.10454) [[github]](https://github.com/bagh2178/GC-VLN) [[project]](https://bagh2178.github.io/GC-VLN/) `Zero-Shot`
  - 概览：提出免训练VLN框架GC-VLN，将指令分解为显式空间约束并构建航点-物体有向无环图，通过图约束优化求解导航路径，在VLN-CE基准上大幅超越现有零样本方法并完成真机泛化验证。

- **[2025/09][ arXiv 2025 - 层次多模态场景图快慢推理VLN - FSR-VLN ]** FSR-VLN: Fast and Slow Reasoning for Vision-Language Navigation with Hierarchical Multi-modal Scene Graph [[arxiv]](https://arxiv.org/abs/2509.13733) [[hjfy]](https://hjfy.top/arxiv/2509.13733) [[github]](https://github.com/HorizonRobotics/HoloAgent) [[project]](https://horizonrobotics.github.io/robot_lab/fsr-vln/) `GSM`
  - 概览：提出结合层次多模态场景图HMSG与快慢导航推理FSR的VLN系统，先快速检索候选房间/视图/物体再由VLM慢推理精选目标，时延降低82%并部署于Unitree G1人形机器人实现实时语音交互导航。

- **[2025/09][ ICML 2026 - 不确定性自适应推理VLN - AdaNav ]** AdaNav: Adaptive Reasoning with Uncertainty for Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2509.24387) [[hjfy]](https://hjfy.top/arxiv/2509.24387) `RL`
  - 概览：提出不确定性自适应推理模块UAR，以动作熵为策略先验并经启发式到强化学习训练逐步优化，使智能体按需触发推理，仅用6K样本即大幅提升R2R与RxR-CE导航成功率。

- **[2025/09][ arXiv 2025 - 多轮RL主动探索VLN - ActiveVLN ]** ActiveVLN: Towards Active Exploration via Multi-Turn RL in Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2509.12618) [[hjfy]](https://hjfy.top/arxiv/2509.12618) [[github]](https://github.com/arvillion/ActiveVLN) `RL`
  - 概览：提出两阶段框架ActiveVLN，先以少量专家轨迹模仿学习引导，再经多轮GRPO强化学习驱动智能体主动探索并自动收集多样轨迹，结合动态早停策略显著超越DAgger与此前RL后训练方法。

- **[2025/09][ arXiv 2025 - 具身推理导航基础模型 - Nav-R1 ]** Nav-R1: Reasoning and Navigation in Embodied Scenes [[arxiv]](https://arxiv.org/abs/2509.10884) [[hjfy]](https://hjfy.top/arxiv/2509.10884) [[github]](https://github.com/AIGeeksGroup/Nav-R1) [[project]](https://aigeeksgroup.github.io/Nav-R1) `RL`
  - 概览：构建Nav-CoT-110K思维链数据集冷启动，设计格式/理解/导航三重奖励的GRPO强化学习与Fast-in-Slow快慢推理范式，统一具身导航中的长时语义推理与低延迟实时控制。

- **[2025/09][ ICLR 2026 - 多机协作长程VLN基准 - CoNavBench ]** CoNavBench: Collaborative Long-Horizon Vision-Language Navigation Benchmark [[openreview]](https://openreview.net/forum?id=bMrH2PFMsi) [[project]](https://navcraft.github.io/) `Benchmark` `Qwen2.5-VL-3B` `Habitat`
  - 概览：构建含4048个单机与多机协作情节的长程VLN基准CoNavBench，提出场景图在环的自动化数据生成平台NavCraft校验任务交接与会合调度，并提供基于Qwen2.5-VL-3B的协作导航基线。

- **[2025/09][ ICLR 2026 - 宏微观专家混合的持续VLN - M3E ]** M3E: Continual Vision-and-Language Navigation via Mixture of Macro and Micro Experts [[openreview]](https://openreview.net/forum?id=pFh5ygjN3V) [[github]](https://github.com/YongliangJiang/M3E-Code) `Hierarchical`
  - 概览：提出宏微观专家混合框架M3E，以场景感知与实例感知双路由器分层激活策略与感知专家，结合动态动量更新在R2R/REVERIE域增量设定下缓解灾难性遗忘。

- **[2025/09][ IEEE Access 2025 - 动态概率策略与LLM零样本物体导航 ]** Language-Driven Zero-Shot Object Navigation via Dynamic Probabilistic Strategy and Large Language Models [[doi]](https://doi.org/10.1109/ACCESS.2025.3613059) `Zero-Shot` `RoboTHOR`
  - 概览：整合YOLO、BLIP与大语言模型进行语义解析与空间关系建模，构建概率加权距离网络并以动态概率策略结合启发式算法实时优化零样本物体导航路径。

- **[2025/09][ arXiv 2025 - 通用视觉语言导航 - T-araVLN ]** T-araVLN: Translator for Agricultural Robotic Agents on Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2509.06644) [[hjfy]](https://hjfy.top/arxiv/2509.06644) `VLN`
  - 概览：提出农业视觉语言导航方法T-araVLN，在AgriVLN智能体前加入指令翻译模块，把含噪、错误或复杂的自然语言指令改写为更明确的导航表示后再执行。

- **[2025/09][ arXiv 2025 - 可通行性感知拓扑导航 - TANGO ]** TANGO: Traversability-Aware Navigation with Local Metric Control for Topological Goals [[arxiv]](https://arxiv.org/abs/2509.08699) [[hjfy]](https://hjfy.top/arxiv/2509.08699) `Traversability`
  - 概览：提出TANGO，将局部可通行性估计与拓扑目标控制结合，在无需稠密三维地图或专门预训练控制器的条件下，把高层拓扑目标转化为安全局部运动。

- **[2025/09][ arXiv 2025 - 通用具身导航基准 - SocialNav-SUB ]** SocialNav-SUB: Benchmarking VLMs for Scene Understanding in Social Robot Navigation [[arxiv]](https://arxiv.org/abs/2509.08757) [[hjfy]](https://hjfy.top/arxiv/2509.08757) [[project]](https://larg.github.io/socialnav-sub/) [[github]](https://github.com/LARG/SocialNavSUB) `Benchmark` `VLM`
  - 概览：引入了用于评估VLMs在社交机器人导航场景中能力的VQA基准测试，使用SCAND数据集中的60个独特场景，评估VLMs与人类回答的一致性。

- **[2025/09][ arXiv 2025 - 通用视觉语言导航 - ObjectReact ]** ObjectReact: Learning Object-Relative Control for Visual Navigation [[arxiv]](https://arxiv.org/abs/2509.09594) [[hjfy]](https://hjfy.top/arxiv/2509.09594) [[project]](https://object-react.github.io/) [[github]](https://github.com/oravus/object-rel-nav) `GSM` `Planning`
  - 概览：提出基于物体相对控制的视觉导航方法ObjectReact，能够在没有严格依赖先前经验的情况下穿越新路线，将控制预测问题与解决图像匹配问题解耦，在跨实体部署时，对于训练测试和映射执行设置中的变化具有很高的不变性。

- **[2025/09][ arXiv 2025 - 通用零样本具身导航 - DreamNav ]** DreamNav: A Trajectory-Based Imaginative Framework for Zero-Shot Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2509.11197) [[hjfy]](https://hjfy.top/arxiv/2509.11197) `Zero-Shot` `Pretraining`
  - 概览：提出Trajectory Predictor，生成与指令语义一致的轨迹级动作策略，确保全局连贯的导航，克服了以往方法中点级决策与指令语义对齐不佳的局限。

- **[2025/09][ arXiv 2025 - 免调优多模态Token剪枝 - NAP ]** Walk and Read Less: Improving the Efficiency of Vision-and-Language Navigation via Tuning-Free Multimodal Token Pruning [[arxiv]](https://arxiv.org/abs/2509.15250) [[hjfy]](https://hjfy.top/arxiv/2509.15250) `Token Pruning`
  - 概览：提出免调优的NAP剪枝框架，分别从无关背景视图、回溯历史与低优先级词元压缩多模态上下文，在保持导航精度的同时降低VLN推理成本。

- **[2025/09][ arXiv 2025 - 通过视觉语言模型微调实现高效且泛化的具身语义导航 - FiLM-Nav ]** FiLM-Nav: Efficient and Generalizable Navigation via VLM Fine-tuning [[arxiv]](https://arxiv.org/abs/2509.16445) [[hjfy]](https://hjfy.top/arxiv/2509.16445) `Zero-Shot`
  - 概览：提出FiLM-Nav，直接以原始视觉轨迹历史和导航目标微调预训练VLM，使其选择下一探索前沿；训练混合ObjectNav、OVON、ImageNav和辅助空间推理任务，以学习任务动力学并增强未见类别泛化。

- **[2025/09][ arXiv 2025 - 通用零样本具身导航 - VLN-Zero ]** VLN-Zero: Rapid Exploration and Cache-Enabled Neurosymbolic Vision-Language Planning for Zero-Shot Transfer in Robot Navigation [[arxiv]](https://arxiv.org/abs/2509.18592) [[hjfy]](https://hjfy.top/arxiv/2509.18592) [[project]](https://vln-zero.github.io/) [[github]](https://github.com/VLN-Zero/vln-zero.github.io) `Zero-Shot` `GSM` `Planning`
  - 概览：零样本神经符号导航：引入了规划器，能够联合推理场景图、任务提示和实时观测，将自由形式的自然语言指令转化为满足约束条件的动作序列，无需微调或多轮推理。

- **[2025/09][ arXiv 2025 - 通用视觉语言导航 ]** Human-like Navigation in a World Built for Humans [[arxiv]](https://arxiv.org/abs/2509.21189) [[hjfy]](https://hjfy.top/arxiv/2509.21189) [[project]](https://reasonnav.github.io/) [[github]](https://github.com/ReasonNav/ReasonNav) `Navigation` `VLM`
  - 概览：提出模块化的导航系统ReasonNav，通过利用视觉语言模型的推理能力，将人类在人造环境中导航时的行为（如阅读标识、询问他人方向等）整合到机器人导航中，使机器人能够更高效地在大型复杂建筑中导航。

- **[2025/09][ arXiv 2025 - 通用视觉语言导航 - JanusVLN ]** JanusVLN: Decoupling Semantics and Spatiality with Dual Implicit Memory for Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2509.22548) [[hjfy]](https://hjfy.top/arxiv/2509.22548) [[project]](https://miv-xjtu.github.io/JanusVLN.github.io/) [[github]](https://github.com/MIV-XJTU/JanusVLN) `Memory` `VLM`
  - 概览：提出JanusVLN，将空间几何编码器与视觉语义编码器的历史KV分别压缩为固定大小的双隐式记忆，并保留初始与滑动窗口令牌作增量更新，以同时维持3D空间先验和语义历史。

- **[2025/09][ arXiv 2025 - 通用视觉语言导航 - CE-Nav ]** CE-Nav: Flow-Guided Reinforcement Refinement for Cross-Embodiment Local Navigation [[arxiv]](https://arxiv.org/abs/2509.23203) [[hjfy]](https://hjfy.top/arxiv/2509.23203) `RL` `Sim-to-Real` `IL`
  - 概览：提出两阶段（IL-then-RL）导航框架，通过解耦通用几何推理与特定实体（embodiment）的动态适应，实现了跨实体（不同机器人形态）的局部导航策略迁移。

- **[2025/09][ arXiv 2025 - 通用视觉语言导航 - OmniNav ]** OmniNav: A Unified Framework for Prospective Exploration and Visual-Language Navigation [[arxiv]](https://arxiv.org/abs/2509.25687) [[hjfy]](https://hjfy.top/arxiv/2509.25687) `Memory` `Sim-to-Real` `Multi-task`
  - 概览：提出统一框架：OmniNav是能够同时支持指令目标（instruct-goal）、目标对象（object-goal）、点目标（point-goal）以及前沿探索（frontier-based exploration）的统一架构。

- **[2025/09][ arXiv 2025 - 通用视觉语言导航 - COMRES-VLM ]** COMRES-VLM: Coordinated Multi-Robot Exploration and Search using Vision Language Models [[arxiv]](https://arxiv.org/abs/2509.26324) [[hjfy]](https://hjfy.top/arxiv/2509.26324) `Agentic` `Planning` `VLM`
  - 概览：提出COMRES-VLM，将实时前沿簇提取和拓扑骨架分析与VLM推理结合；VLM读取共享占据图、机器人状态及可选语言先验，为多机器人生成全局一致的探索与目标搜索航点。

- **[2025/09][ arXiv 2025 - 水下具身智能体感知、规划与导航基准环境 - OceanGym ]** OceanGym: A Benchmark Environment for Underwater Embodied Agents [[arxiv]](https://arxiv.org/abs/2509.26536) [[hjfy]](https://hjfy.top/arxiv/2509.26536) `Benchmark`
  - 概览：构建OceanGym水下具身智能体基准，覆盖八类任务并以多模态大模型智能体统一处理光学、声呐、记忆与序列决策，用于评测低能见度和动态洋流中的感知规划能力。

- **[2025/08][ AAAI 2026 - 单目全景想象VLN - MonoDream ]** MonoDream: Monocular Vision-Language Navigation with Panoramic Dreaming [[arxiv]](https://arxiv.org/abs/2508.02549) [[hjfy]](https://hjfy.top/arxiv/2508.02549) [[project]](https://horizonrobotics.github.io/robot_lab/monodream) `End-to-end` `NVILA-lite-2B`
  - 概览：提出轻量级单目VLA导航框架，学习统一导航表征并通过潜在全景想象任务从单目输入预测当前与未来全景RGB-D潜在特征，显著缩小单目智能体与全景RGB-D方法的性能差距。

- **[2025/08][ ACM MM 2025 - 开放词汇视觉语言建图指令定位 - OpenMap ]** OpenMap: Instruction Grounding via Open-Vocabulary Visual-Language Mapping [[arxiv]](https://arxiv.org/abs/2508.01723) [[hjfy]](https://hjfy.top/arxiv/2508.01723) [[github]](https://github.com/openmap-project/openmap) [[project]](https://openmap-project.github.io/openmap.github.io/) `GSM` `VLM+LLM`
  - 概览：提出零样本开放词汇视觉语言建图框架OpenMap，以结构-语义共识约束实现稳健的3D实例级聚合，并借助LLM辅助的指令到实例定位模块，在ScanNet200与Matterport3D上零样本超越现有基线。

- **[2025/08][ ICASSP 2026 - 动态记忆与LLM空间推理的零样本VLN - MSNav ]** MSNav: Zero-Shot Vision-and-Language Navigation with Dynamic Memory and LLM Spatial Reasoning [[arxiv]](https://arxiv.org/abs/2508.16654) [[hjfy]](https://hjfy.top/arxiv/2508.16654) `Zero-Shot` `Qwen3-4B`
  - 概览：提出记忆-空间-决策三模块协同的零样本VLN框架，动态地图记忆经选择性节点剪枝缓解长程记忆过载，微调Qwen-Spatial强化物体关系推理，在R2R与REVERIE上取得零样本SOTA。

- **[2025/08][ ACL 2026 - 技能混合VLN智能体 - SkillNav ]** Breaking Down and Building Up: Mixture of Skill-Based Vision-and-Language Navigation Agents [[arxiv]](https://arxiv.org/abs/2508.07642) [[hjfy]](https://hjfy.top/arxiv/2508.07642) `Agentic`
  - 概览：提出SkillNav框架，将导航分解为方向调整、垂直移动等可解释原子技能并由专门智能体分管，配合免训练VLM路由器动态选择技能智能体，在GSA-R2R上取得SOTA并提升对新指令风格与未见环境的泛化。

- **[2025/08][ AAAI 2026 - 自我纠错飞轮VLA导航后训练 - CorrectNav ]** CorrectNav: Self-Correction Flywheel Empowers Vision-Language-Action Navigation Model [[arxiv]](https://arxiv.org/abs/2508.10416) [[hjfy]](https://hjfy.top/arxiv/2508.10416) [[aaai]](https://ojs.aaai.org/index.php/AAAI/article/view/38942) `End-to-end`
  - 概览：提出"自我纠错飞轮"后训练范式，将训练集上的错误轨迹自动转化为感知与动作自纠错数据并多轮迭代训练，使单目RGB的VLA导航模型CorrectNav在R2R-CE与RxR-CE上大幅刷新SOTA并通过实机验证。

- **[2025/08][ arXiv 2025 - DAgger增强扩散策略VLN - DifNav ]** DAgger Diffusion Navigation: DAgger Boosted Diffusion Policy for Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2508.09444) [[hjfy]](https://hjfy.top/arxiv/2508.09444) [[github]](https://github.com/Tokishx/DifNav/) `Diffusion` `Habitat`
  - 概览：提出端到端扩散策略DifNav，将传统两阶段航点预测与规划统一，用条件扩散直接建模未来动作分布，并借助DAgger在线专家数据聚合缓解分布偏移与误差累积。

- **[2025/08][ arXiv 2025 - 记忆保留主动接地语言物体导航 - MAG-Nav ]** MAG-Nav: Language-Driven Object Navigation Leveraging Memory-Reserved Active Grounding [[arxiv]](https://arxiv.org/abs/2508.05021) [[hjfy]](https://hjfy.top/arxiv/2508.05021) `Zero-Shot` `VLM` `HM3D`
  - 概览：提出免训练的语言驱动物体导航框架，通过主动调整观察视角提升候选物体辨识度，并保留和回溯历史不确定观测以消解跨时刻歧义，在HM3D及四足机器人实机上验证开放描述目标的零样本泛化。

- **[2025/08][ arXiv 2025 - 好奇心驱动主动地理定位 - GeoExplorer ]** GeoExplorer: Active Geo-Localization with Curiosity-Driven Exploration [[arxiv]](https://arxiv.org/abs/2508.00152) [[hjfy]](https://hjfy.top/arxiv/2508.00152) `Active Exploration`
  - 概览：提出GeoExplorer，将目标导向与好奇心驱动的探索奖励结合，使智能体主动选择能减少位置不确定性的观测，在未知区域中提高地理定位效率。

- **[2025/08][ arXiv 2025 - 通用视觉语言导航 - IGL-Nav ]** IGL-Nav: Incremental 3D Gaussian Localization for Image-goal Navigation [[arxiv]](https://arxiv.org/abs/2508.00823) [[hjfy]](https://hjfy.top/arxiv/2508.00823) [[project]](https://gwxuan.github.io/IGL-Nav/) [[github]](https://github.com/GWxuan/IGL-Nav) `GSM` `Memory` `End-to-end`
  - 概览：设计粗粒度到细粒度的目标定位策略，先利用几何信息进行离散空间匹配实现粗粒度定位，再通过可微渲染优化求解精确定位，有效解决了6自由度相机姿态估计的复杂搜索空间问题。

- **[2025/08][ arXiv 2025 - 通用视觉语言导航 - HALO ]** HALO: Human Preference Aligned Offline Reward Learning for Robot Navigation [[arxiv]](https://arxiv.org/abs/2508.01539) [[hjfy]](https://hjfy.top/arxiv/2508.01539) [[project]](https://gamma.umd.edu/researchdirections/crowdmultiagent/halo/) `Sim-to-Real` `Planning` `Human Preference`
  - 概览：提出HALO离线奖励学习方法，以二元用户可行性反馈塑造动作偏好排序，并用Plackett-Luce损失训练视觉奖励模型；该奖励可用于离线策略学习，也可作为模型预测控制的附加代价。

- **[2025/08][ arXiv 2025 - 视觉提示具身导航 - VPN ]** VPN: Visual Prompt Navigation [[arxiv]](https://arxiv.org/abs/2508.01766) [[hjfy]](https://hjfy.top/arxiv/2508.01766) `End-to-end`
  - 概览：提出视觉提示导航VPN，让用户在二维俯视图上标记视觉轨迹而无需自然语言指令；构建离散与连续设定的R2R-VP、R2R-CE-VP数据集，并提出VPNet及视角级、轨迹级两种数据增强策略。

- **[2025/08][ arXiv 2025 - 通用零样本具身导航 - $NavA^3$ ]** $NavA^3$: Understanding Any Instruction, Navigating Anywhere, Finding Anything [[arxiv]](https://arxiv.org/abs/2508.04598) [[hjfy]](https://hjfy.top/arxiv/2508.04598) [[project]](https://navigationa3.github.io/) [[github]](https://github.com/linglingxiansen/NavA3) `Zero-Shot` `Hierarchical`
  - 概览：全局策略利用Reasoning-VLM解析高级指令并确定目标区域，局部策略则使用NaviAfford模型（Pointing-VLM）在目标区域内进行精确的目标对象定位和导航。

- **[2025/08][ arXiv 2025 - 通用视觉语言导航 - AgriVLN ]** AgriVLN: Vision-and-Language Navigation for Agricultural Robots [[arxiv]](https://arxiv.org/abs/2508.07406) [[hjfy]](https://hjfy.top/arxiv/2508.07406) [[github]](https://github.com/AlexTraveling/AgriVLN) `VLN` `VLM`
  - 概览：提出A2A基准测试，这是一个覆盖6种常见农业场景（农场、温室、森林、山区、花园和村庄）的视觉语言导航（VLN）基准测试，包含1560个episode，所有真实RGB视频都是由四足机器人前端摄像头在0.38米高度拍摄的，与实际部署条件一致。

- **[2025/08][ arXiv 2025 - 通用视觉语言导航 - Input-Adaptive ]** Harnessing Input-Adaptive Inference for Efficient VLN [[arxiv]](https://arxiv.org/abs/2508.09262) [[hjfy]](https://hjfy.top/arxiv/2508.09262) [[github]](https://github.com/Trustworthy-and-Responsible-AI-Lab/adaptive-vision-and-language-navigation) `VLN` `Transformer`
  - 概览：提出VLN输入自适应推理方法：空间层选择性处理全景视图，网络层按重要性阈值提前退出，时间层缓存已见视图以避免重复编码，从三个层面压缩历史感知计算。

- **[2025/08][ arXiv 2025 - 通用视觉语言导航 - GoViG ]** GoViG: Goal-Conditioned Visual Navigation Instruction Generation via Multimodal Reasoning [[arxiv]](https://arxiv.org/abs/2508.09547) [[hjfy]](https://hjfy.top/arxiv/2508.09547) [[github]](https://github.com/F1y1113/GoViG) `Navigation`
  - 概览：提出GoViG目标条件导航指令生成任务，仅根据起点与终点第一人称图像生成指令；模型先预测连接两端的中间视觉状态，再以自回归多模态模型生成落地指令，并比较单次与交错推理。

- **[2025/08][ arXiv 2025 - 分割Transformer开放词汇目标导航 - OVSegDT ]** OVSegDT: Segmenting Transformer for Open-Vocabulary Object Goal Navigation [[arxiv]](https://arxiv.org/abs/2508.11479) [[hjfy]](https://hjfy.top/arxiv/2508.11479) `End-to-end`
  - 概览：提出OVSegDT开放词汇物体目标导航方法，将目标分割掩码编码进Transformer策略观测，以空间位置线索提升未见类别和噪声分割条件下的导航鲁棒性。

- **[2025/08][ arXiv 2025 - 通用具身导航基准 - i2Nav-Robot ]** i2Nav-Robot: A Large-Scale Indoor-Outdoor Robot Dataset for Multi-Sensor Fusion Navigation [[arxiv]](https://arxiv.org/abs/2508.11485) [[hjfy]](https://hjfy.top/arxiv/2508.11485) [[github]](https://github.com/i2Nav-WHU/i2Nav-Robot) `Benchmark`
  - 概览：发布i2Nav-Robot室内外多传感器导航数据集，在全向轮式平台同步采集固态激光雷达、4D毫米波雷达、双目相机、IMU、GNSS和轮速计，包含10条共约17,060米序列及厘米级轨迹真值。

- **[2025/08][ arXiv 2025 - 通用视觉语言导航 - LookOut ]** LookOut: Real-World Humanoid Egocentric Navigation [[arxiv]](https://arxiv.org/abs/2508.14466) [[hjfy]](https://hjfy.top/arxiv/2508.14466) [[project]](https://sites.google.com/stanford.edu/lookout) `Navigation`
  - 概览：提出模型：设计通过时间聚合3D潜在特征来推理的框架LookOut，利用预训练的DINO特征编码器和无参数的反投影策略，有效解决了该任务，能够对环境的几何和语义约束进行建模，适用于环境的静态和动态部分。

- **[2025/08][ arXiv 2025 - 通用具身导航综述 ]** Sensing, Social, and Motion Intelligence in Embodied Navigation: A Comprehensive Survey [[arxiv]](https://arxiv.org/abs/2508.15354) [[hjfy]](https://hjfy.top/arxiv/2508.15354) [[github]](https://github.com/Franky-X/Awesome-Embodied-Navigation) `Survey`
  - 概览：提出TOFRA框架：将具身导航过程分解为五个关键阶段——状态转移、环境观测、信息融合、奖励策略构建和动作执行，为具身导航研究提供了统一的结构化分析框架。

- **[2025/07][ arXiv 2025 - 自进化VLN框架 - SE-VLN ]** SE-VLN: A Self-Evolving Vision-Language Navigation Framework Based on Multimodal Large Language Models [[arxiv]](https://arxiv.org/abs/2507.13152) [[hjfy]](https://hjfy.top/arxiv/2507.13152) `Agentic`
  - 概览：提出首个由多模态大模型驱动的自进化VLN框架，通过分层记忆、检索增强推理与反思三大模块让智能体在测试期持续积累经验并进化，在R2R等未见环境基准上显著超越现有SOTA。

- **[2025/07][ arXiv 2025 - 通用视觉语言导航 ]** Move to Understand a 3D Scene: Bridging Visual Grounding and Exploration for Efficient and Versatile Embodied Navigation [[arxiv]](https://arxiv.org/abs/2507.04047) [[hjfy]](https://hjfy.top/arxiv/2507.04047) `RL` `Memory` `End-to-end`
  - 概览：提出MTU3D，以在线查询表示从RGB-D帧直接构建空间记忆，把未探索区域表示为前沿查询并联合优化物体定位与前沿选择，再用超过百万条仿真和真实轨迹进行视觉—语言—探索预训练。

- **[2025/07][ arXiv 2025 - 通用视觉语言导航 - MOSU ]** MOSU: Autonomous Long-range Robot Navigation with Multi-modal Scene Understanding [[arxiv]](https://arxiv.org/abs/2507.04686) [[hjfy]](https://hjfy.top/arxiv/2507.04686) `Planning` `VLM`
  - 概览：结合了基于GPS和QGIS地图的全局路径规划以及多模态轨迹生成技术，用于局部导航细化。

- **[2025/07][ arXiv 2025 - 通用零样本具身导航 - LOVON ]** LOVON: Legged Open-Vocabulary Object Navigator [[arxiv]](https://arxiv.org/abs/2507.06747) [[hjfy]](https://hjfy.top/arxiv/2507.06747) [[project]](https://daojiepeng.github.io/LOVON/) [[github]](https://github.com/DaojiePENG/LOVON) `Zero-Shot` `Hierarchical`
  - 概览：提出统一框架LOVON，整合了LLMs、开放词汇视觉检测和L2MM，用于规划和执行复杂的开放世界长时域导航任务。

- **[2025/07][ arXiv 2025 - 通用视觉语言导航 - Vision-Language ]** View Invariant Learning for Vision-Language Navigation in Continuous Environments [[arxiv]](https://arxiv.org/abs/2507.08831) [[hjfy]](https://hjfy.top/arxiv/2507.08831) `End-to-end` `Contrastive`
  - 概览：提出视角不变学习策略VIL，该策略通过对比学习框架来学习稀疏且视角不变的特征，并引入教师-学生框架用于航点预测模块，以增强现有导航策略对相机视角变化的鲁棒性。

- **[2025/07][ arXiv 2025 - 通用视觉语言导航 - CogDDN ]** CogDDN: A Cognitive Demand-Driven Navigation with Decision Optimization and Dual-Process Thinking [[arxiv]](https://arxiv.org/abs/2507.11334) [[hjfy]](https://hjfy.top/arxiv/2507.11334) [[project]](https://yuehaohuang.github.io/CogDDN/) [[github]](https://github.com/yuehaohuang/CogDDN) `Navigation`
  - 概览：引入了双过程决策模块，该模块无需人工干预，通过自监督机制让经验直觉过程（Heuristic Process）继承理性分析过程（Analytic Process）的能力。

- **[2025/07][ arXiv 2025 - 通用零样本具身导航 - osmAG-LLM ]** osmAG-LLM: Zero-Shot Open-Vocabulary Object Navigation via Semantic Maps and Large Language Models Reasoning [[arxiv]](https://arxiv.org/abs/2507.12753) [[hjfy]](https://hjfy.top/arxiv/2507.12753) `Zero-Shot` `Pretraining` `Retrieval`
  - 概览：提出osmAG-LLM，以轻量文本语义地图提供环境上下文，并结合大语言模型先验在线推理目标位置，使系统能处理物体已移动或从未被建图的开放词汇目标查询。

- **[2025/07][ arXiv 2025 - 通用视觉语言导航 - Vision-and-Language ]** Rethinking the Embodied Gap in Vision-and-Language Navigation: A Holistic Study of Physical and Visual Disparities [[arxiv]](https://arxiv.org/abs/2507.13019) [[hjfy]](https://hjfy.top/arxiv/2507.13019) [[project]](https://crystalsixone.github.io/vln_pe.github.io/) [[github]](https://github.com/InternRobotics/InternNav) `Diffusion` `Planning`
  - 概览：系统性地评估了几种第一视角的VLN方法在物理机器人环境中的表现，包括单步离散动作预测的分类模型、密集轨迹点预测的扩散模型以及基于地图的无需训练的大语言模型（LLM）与路径规划的结合。

- **[2025/07][ arXiv 2025 - 通用零样本具身导航 - X-Nav ]** X-Nav: Learning End-to-End Cross-Embodiment Navigation for Mobile Robots [[arxiv]](https://arxiv.org/abs/2507.14731) [[hjfy]](https://hjfy.top/arxiv/2507.14731) [[project]](https://cross-embodiment-nav.github.io/) `Zero-Shot` `RL` `End-to-end`
  - 概览：设计两阶段学习框架：第一阶段利用深度强化学习（DRL）在大量随机生成的机器人实体上训练多个专家策略；第二阶段通过导航动作分块（Nav-ACT）结合Transformer模型，将专家策略的知识蒸馏到一个通用导航策略中，该通用策略可以直接将视觉和本体感知观测映射到低级控制指令，实现对新机器人实体的零样本（zero-shot）泛化。

- **[2025/07][ arXiv 2025 - 通用视觉语言导航 - Terrestrial-Aerial ]** Autonomous Exploration with Terrestrial-Aerial Bimodal Vehicles [[arxiv]](https://arxiv.org/abs/2507.21338) [[hjfy]](https://hjfy.top/arxiv/2507.21338) `Hierarchical` `Planning`
  - 概览：提出分层探索框架：为陆-空双模态车辆（TABV）设计，包含基于两种覆盖策略的双模态视点生成模块，以及充分利用机器人双模态运动能力的能量和时间感知决策机制。

- **[2025/07][ arXiv 2025 - 通用视觉语言导航 ]** Recursive Visual Imagination and Adaptive Linguistic Grounding for Vision Language Navigation [[arxiv]](https://arxiv.org/abs/2507.21450) [[hjfy]](https://hjfy.top/arxiv/2507.21450) `VLN`
  - 概览：提出自适应语言映射（ALG）机制：通过将指令的不同语义组件与ISR的神经网格在位置和语义上进行密集对齐，使智能体能够根据不同的语言组件自适应地激活不同的动作信号或场景记忆，从而实现更准确的视觉-语言匹配。

- **[2025/07][ RA-L 2025 - 复杂环境基础模型视觉导航 - EffoNAV ]** EffoNAV: An Effective Foundation-Model-Based Visual Navigation Approach in Challenging Environment [[doi]](https://doi.org/10.1109/LRA.2025.3572815) `Foundation Model`
  - 概览：提出EffoNAV，将预训练视觉基础模型的通用表征引入图像目标导航，并针对光照与外观变化进行特征匹配和策略学习，提高复杂环境中的鲁棒性。

- **[2025/07][ TPAMI 2025 - 层次目标区域图 - HOZ++ ]** HOZ++: Versatile Hierarchical Object-to-Zone Graph for Object Navigation [[doi]](https://doi.org/10.1109/TPAMI.2025.3552987) `Hierarchical Graph`
  - 概览：提出可在线更新的层次对象到区域图HOZ++，显式建模当前区域、目标区域及其连接关系，为未知环境中的目标搜索和跨区域路径规划提供结构化先验。

- **[2025/06][ Information Fusion 2025 - 细粒度对齐标注VLN指令生成 - FCA-NIG ]** Generating Vision-Language Navigation Instructions Incorporated Fine-Grained Alignment Annotations [[arxiv]](https://arxiv.org/abs/2506.08566) [[hjfy]](https://hjfy.top/arxiv/2506.08566) [[doi]](https://doi.org/10.1016/j.inffus.2025.104107) `Benchmark` `GLIP+OFA+CLIP`
  - 概览：提出生成式框架FCA-NIG，自动构建带子指令-子轨迹与实体-地标双层细粒度跨模态对齐标注的导航指令，生成的FCA-R2R增广数据集显著提升SF、EnvDrop、RecBERT等多种VLN智能体性能。

- **[2025/06][ TPAMI 2026 - 自我改进具身推理LLM导航 - EvolveNav ]** EvolveNav: Empowering LLM-Based Vision-Language Navigation via Self-Improving Embodied Reasoning [[arxiv]](https://arxiv.org/abs/2506.01551) [[hjfy]](https://hjfy.top/arxiv/2506.01551) [[github]](https://github.com/expectorlin/EvolveNav) `End-to-end`
  - 概览：提出自我改进具身推理范式，先以形式化CoT标签监督微调激活LLM的导航推理能力，再将模型自身推理输出作为自增强CoT标签进行自反思后训练，在R2R、REVERIE、CVDN与SOON上持续超越既有LLM导航方法。

- **[2025/06][ arXiv 2025 - 强化微调视觉语言导航 - VLN-R1 ]** VLN-R1: Vision-Language Navigation via Reinforcement Fine-Tuning [[arxiv]](https://arxiv.org/abs/2506.17221) [[hjfy]](https://hjfy.top/arxiv/2506.17221) [[github]](https://github.com/Qi-Zhangyang/GPT4Scene-and-VLN-R1) [[project]](https://vlnr1.github.io/) `RL` `Qwen2-VL` `Habitat`
  - 概览：提出VLN-R1框架，利用大型视觉语言模型将第一视角视频流直接转为连续导航动作，构建VLN-Ego数据集并采用SFT与时间衰减奖励强化微调的两阶段训练，以小模型实现高效具身导航。

- **[2025/06][ arXiv 2025 - 通用零样本具身导航 - NavBench ]** NavBench: Probing Multimodal Large Language Models for Embodied Navigation [[arxiv]](https://arxiv.org/abs/2506.01031) [[hjfy]](https://hjfy.top/arxiv/2506.01031) [[project]](https://navbench.github.io/) [[github]](https://github.com/NavBench/Evaluation_Code) `Zero-Shot` `Sim-to-Real` `VLM`
  - 概览：构建NavBench：以3,200个问答评测全局指令对齐、时间进度估计和局部观测—动作推理，并在72个室内场景的432个回合中评测逐步执行；同时提供将模型输出转为机器人动作的管线。

- **[2025/06][ arXiv 2025 - 通用视觉语言导航 - SEMNAV ]** SEMNAV: Enhancing Visual Semantic Navigation in Robotics through Semantic Segmentation [[arxiv]](https://arxiv.org/abs/2506.01418) [[hjfy]](https://hjfy.top/arxiv/2506.01418) [[github]](https://github.com/gramuah/semnav) `Sim-to-Real`
  - 概览：提出面向目标导航（OBJECTNAV）问题的视觉语义导航模型SEMNAV，利用机器人第一人称视角的语义分割来学习视觉观测与导航动作之间的映射关系。

- **[2025/06][ arXiv 2025 - 通用零样本具身导航 - DualMap ]** DualMap: Online Open-Vocabulary Semantic Mapping for Natural Language Navigation in Dynamic Changing Scenes [[arxiv]](https://arxiv.org/abs/2506.01950) [[hjfy]](https://hjfy.top/arxiv/2506.01950) [[project]](https://eku127.github.io/DualMap/) [[github]](https://github.com/Eku127/DualMap) `Zero-Shot`
  - 概览：提出双重建图表示方法，结合全局抽象地图用于高级候选选择和局部具体地图用于精确目标定位，有效管理和更新环境中的动态变化。

- **[2025/06][ arXiv 2025 - 通用零样本具身导航 - BeliefMapNav ]** BeliefMapNav: 3D Voxel-Based Belief Map for Zero-Shot Object Navigation [[arxiv]](https://arxiv.org/abs/2506.06487) [[hjfy]](https://hjfy.top/arxiv/2506.06487) [[github]](https://github.com/ZiboKNOW/BeliefMapNav) `Zero-Shot` `GSM` `Hierarchical`
  - 概览：提出零样本目标导航系统BeliefMapNav，通过构建3D体素信念图，将语言模型的语义推理与视觉嵌入相结合，实现了对目标位置的精确估计和高效的全局导航决策。

- **[2025/06][ arXiv 2025 - 通用零样本具身导航 - DyNaVLM ]** DyNaVLM: Zero-Shot Vision-Language Navigation System with Dynamic Viewpoints and Self-Refining Graph Memory [[arxiv]](https://arxiv.org/abs/2506.15096) [[hjfy]](https://hjfy.top/arxiv/2506.15096) `Zero-Shot` `Memory` `End-to-end`
  - 概览：提出DyNaVLM，让视觉语言模型从动态视角中自由选择连续导航目标，并以自精炼图记忆保存物体位置、检索增强决策及跨机器人共享，在无需任务微调时执行零样本导航。

- **[2025/06][ arXiv 2025 - 通用视觉语言导航 - Mem4Nav ]** Mem4Nav: Boosting Vision-and-Language Navigation in Urban Environments with a Hierarchical Spatial-Cognition Long-Short Memory System [[arxiv]](https://arxiv.org/abs/2506.19433) [[hjfy]](https://hjfy.top/arxiv/2506.19433) [[github]](https://github.com/TSYJ-He/Mem4Nav) `Agentic` `Hierarchical` `Memory`
  - 概览：提出层次化的空间认知长短期记忆系统Mem4Nav,通过结合稀疏八叉树索引和语义拓扑图，统一了细粒度几何信息和地标连通性，并设计一种可逆的Transformer记忆模块，能够无损地压缩和检索空间锚定的观测数据，同时开发短期记忆缓存用于高频本地查询，以及统一的检索机制动态平衡短期和长期记忆。

- **[2025/06][ Machine Intelligence Research 2025 - 多模态预训练知识目标导航 ]** Multimodal Pretrained Knowledge for Real-world Object Navigation [[doi]](https://doi.org/10.1007/s11633-024-1537-x) `Pretraining`
  - 概览：将多模态预训练知识用于真实世界物体导航，在关键位置进行视觉语言对齐并结合场景记忆，使机器人能利用语义先验搜索目标。

- **[2025/06][ CVPR 2025 - 场景地图提示调优指令生成 ]** Scene Map-based Prompt Tuning for Navigation Instruction Generation [[doi]](https://doi.org/10.1109/CVPR52734.2025.00647) `Prompt Tuning`
  - 概览：提出MAPINSTRUCTOR，将场景地图上下文编码进导航指令生成流程，并以参数高效提示调优适配语言模型，使生成指令更符合路径结构和关键地标。

- **[2025/06][ ACM ICMR 2025 - 户外多智能体协作VLN - MMCNav ]** MMCNav: MLLM-empowered Multi-agent Collaboration for Outdoor Visual Language Navigation [[doi]](https://doi.org/10.1145/3731715.3733393) `Multi-Agent`
  - 概览：提出由多模态大模型驱动的户外多智能体协作导航框架，通过角色分工、信息共享和协同决策解析复杂语言指令，提升单智能体难以覆盖的户外搜索能力。

- **[2025/05][ NeurIPS 2025 - 数据高效VLN推理策略 - Aux-Think ]** Aux-Think: Exploring Reasoning Strategies for Data-Efficient Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2505.11886) [[hjfy]](https://hjfy.top/arxiv/2505.11886) [[project]](https://horizonrobotics.github.io/robot_lab/aux-think) `End-to-end`
  - 概览：首次系统对比VLN中No-Think/Pre-Think/Post-Think三种推理策略并揭示推理时坍塌现象，提出训练时CoT监督、推理时直接预测动作的Aux-Think框架，并发布R2R-CoT-320k数据集。

- **[2025/05][ arXiv 2025 - 生成式视觉想象VLN - VISTA ]** VISTA: Generative Visual Imagination for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2505.07868) [[hjfy]](https://hjfy.top/arxiv/2505.07868) `Diffusion`
  - 概览：提出"想象-对齐"式导航框架VISTA，利用扩散模型根据指令与观测生成未来视觉想象，并通过感知对齐过滤器筛选想象以指导可解释的动作选择，在R2R与RoboTHOR上取得SOTA。

- **[2025/05][ arXiv 2025 - 通用视觉语言导航 - DOPE ]** DOPE: Dual Object Perception-Enhancement Network for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2505.00743) [[hjfy]](https://hjfy.top/arxiv/2505.00743) `VLN` `Transformer`
  - 概览：提出DOPE双物体感知增强网络，以文本语义提取器筛选指令中的关键物体与动作、TOPA增强文本物体表示，再由IOPA建模图像与文本中的跨模态物体关系。

- **[2025/05][ arXiv 2025 - 通用具身导航综述 - AI ]** A Survey of Robotic Navigation and Manipulation with Physics Simulators in the Era of Embodied AI [[arxiv]](https://arxiv.org/abs/2505.01458) [[hjfy]](https://hjfy.top/arxiv/2505.01458) `Survey` `Sim-to-Real` `Transformer`
  - 概览：系统比较物理模拟器在机器人导航与操作中的任务支持、硬件需求和仿真到现实迁移能力，并汇总相关数据集、指标、平台与方法，辅助按资源约束选择工具。

- **[2025/05][ arXiv 2025 - 通用视觉语言导航 - Model-Based ]** Learning to Drive Anywhere with Model-Based Reannotation [[arxiv]](https://arxiv.org/abs/2505.05592) [[hjfy]](https://hjfy.top/arxiv/2505.05592) [[project]](https://model-base-reannotation.github.io/) [[github]](https://github.com/NHirose/Learning-to-Drive-Anywhere-with-MBRA) `Navigation`
  - 概览：提出模型式重标注MBRA，用学习到的短时域专家为众包遥操作数据和无动作标签网络视频重标或生成动作，再把处理后的被动数据蒸馏为支持视觉目标与GPS航点的长时域策略LogoNav。

- **[2025/05][ arXiv 2025 - 通用视觉语言导航 - LOG-Nav ]** LOG-Nav: Efficient Layout-Aware Object-Goal Navigation with Hierarchical Planning [[arxiv]](https://arxiv.org/abs/2505.06131) [[hjfy]](https://hjfy.top/arxiv/2505.06131) `Hierarchical` `Memory`
  - 概览：提出高效的布局感知零样本目标导航方法LOG-Nav，该方法通过分层规划（全局拓扑规划和局部动态规划）实现复杂多室室内环境中的高效导航，且无需额外奖励或训练。

- **[2025/05][ arXiv 2025 - 通用视觉语言导航 - Learning to Reason and Navigate ]** Learning to Reason and Navigate: Parameter Efficient Action Planning with Large Language Models [[arxiv]](https://arxiv.org/abs/2505.07500) [[hjfy]](https://hjfy.top/arxiv/2505.07500) `Planning`
  - 概览：设计LGP和LAP两个模块，LLM目标规划器（LGP）用于从REVERIE指令中提取目标对象和房间；LoRA动作规划器（LAP）用于生成单步动作计划。

- **[2025/05][ arXiv 2025 - 通用视觉语言导航 - Dynam3D ]** Dynam3D: Dynamic Layered 3D Tokens Empower VLM for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2505.11383) [[hjfy]](https://hjfy.top/arxiv/2505.11383) [[github]](https://github.com/MrZihan/Dynam3D) `Hierarchical` `Memory` `Pretraining`
  - 概览：引入了3D视觉-语言模型（3D-VLM），该模型整合了来自通用特征场的3D patch特征和来自Dynam3D的3D实例-区域特征，平衡了细粒度几何和全局空间布局，以进行导航规划。

- **[2025/05][ arXiv 2025 - 通用视觉语言导航 - BadNAVer ]** BadNAVer: Exploring Jailbreak Attacks On Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2505.12443) [[hjfy]](https://hjfy.top/arxiv/2505.12443) `VLN` `Transformer` `VLM`
  - 概览：构建恶意查询基准：设计200个涵盖物理伤害、隐私侵犯、财产破坏和误导行为四类意图的恶意导航查询，作为评估MLLM驱动导航系统安全性的统一基准，与以往仅涉及少量视觉触发器和有限恶意行为的攻击不同，这些查询包含了各种物体和现实的恶意行为。

- **[2025/05][ arXiv 2025 - 通用视觉语言导航 - SayCoNav ]** SayCoNav: Utilizing Large Language Models for Adaptive Collaboration in Decentralized Multi-Robot Navigation [[arxiv]](https://arxiv.org/abs/2505.13729) [[hjfy]](https://hjfy.top/arxiv/2505.13729) `Agentic`
  - 概览：提出SayCoNav方法：利用大语言模型（LLMs）自动生成协作策略，实现异构机器人在去中心化环境中的自适应协作。

- **[2025/05][ arXiv 2025 - 通用视觉语言导航 - CoNav ]** CoNav: Collaborative Cross-Modal Reasoning for Embodied Navigation [[arxiv]](https://arxiv.org/abs/2505.16663) [[hjfy]](https://hjfy.top/arxiv/2505.16663) [[project]](https://abdd.top/CoNav/) [[github]](https://github.com/oceanhao/CoNav) `Pretraining`
  - 概览：提出协作跨模态推理框架CoNav：该框架允许3D-文本模型通过简单地共享文本假设来指导导航智能体，而无需大规模的三模态数据集。

- **[2025/05][ arXiv 2025 - 自适应文本想象导航 - ATD ]** Cross from Left to Right Brain: Adaptive Text Dreamer for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2505.20897) [[hjfy]](https://hjfy.top/arxiv/2505.20897) `LLM`
  - 概览：采用仿生双分支LLM分别建模当前状态与未来文本想象，通过共享隐空间将语言推理接入图导航决策，在较小参数规模下提升VLN性能与泛化。

- **[2025/05][ arXiv 2025 - 通用零样本具身导航 - Stairway to Success ]** Stairway to Success: An Online Floor-Aware Zero-Shot Object-Goal Navigation Framework via LLM-Driven Coarse-to-Fine Exploration [[arxiv]](https://arxiv.org/abs/2505.23019) [[hjfy]](https://hjfy.top/arxiv/2505.23019) `Zero-Shot` `Hierarchical` `Sim-to-Real`
  - 概览：提出多楼层零样本目标导航框架ASCENT，在线构建含楼梯和跨楼层拓扑的层次地图，并以边界排序结合大语言模型进行由楼层到局部目标的粗到细决策。

- **[2025/05][ ICRA 2025 - 知识历史感知连续VLN - VLN-KHVR ]** VLN-KHVR: Knowledge-And-History Aware Visual Representation for Continuous Vision-and-Language Navigation [[doi]](https://doi.org/10.1109/ICRA55743.2025.11127961) `Knowledge & History`
  - 概览：提出VLN-KHVR，将外部语义知识和历史观测共同注入视觉表征，强化指令与场景的跨模态对齐，以改善连续环境中的长期导航决策。

- **[2025/05][ TNNLS 2025 - 空间记忆与语义认知导航 ]** Visuomotor Navigation for Embodied Robots With Spatial Memory and Semantic Reasoning Cognition [[doi]](https://doi.org/10.1109/TNNLS.2024.3418857) `Spatial Memory`
  - 概览：构建由拓扑空间记忆图和语义关系图组成的双层表示，联合历史位置、物体关系与视觉运动控制，为具身机器人提供可记忆、可推理的导航策略。

- **[2025/05][ Science Robotics 2025 - 复杂离散地形四足高速导航 ]** High-speed control and navigation for quadrupedal robots on complex and discrete terrain [[doi]](https://doi.org/10.1126/scirobotics.ads6192) `RL`
  - 概览：提出面向复杂离散地形的四足机器人高速控制与导航框架，以地形感知、强化学习策略和运动安全约束协同处理跨越、转向及落足，在仿真和实机中验证高速通行能力。

- **[2025/04][ arXiv 2025 - 仿生空间认知VLN框架 - BrainNav ]** Endowing Embodied Agents with Spatial Reasoning Capabilities for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2504.08806) [[hjfy]](https://hjfy.top/arxiv/2504.08806) `Zero-Shot`
  - 概览：提出仿生空间认知导航框架BrainNav，以海马体记忆、视觉皮层感知等五大类脑模块结合双地图与双朝向策略，缓解真实环境VLN中的空间幻觉并实现零样本实时导航。

- **[2025/04][ ICASSP 2025 - 图感知推理与双向选择VLN - GAR ]** Exploring Graph-aware Reasoning and Bidirectional Selection for Vision-Language Navigation [[doi]](https://doi.org/10.1109/ICASSP49660.2025.10888565) `GSM` `State Space Model`
  - 概览：提出图感知推理模型GAR，将图神经推理融入结构化状态空间模型，并以双向选择机制同时利用历史与当前观察，在提升长序列导航推理能力的同时降低显存开销。

- **[2025/04][ arXiv 2025 - 通用具身导航基准 - FindAnything ]** FindAnything: Open-Vocabulary and Object-Centric Mapping for Robot Exploration in Any Environment [[arxiv]](https://arxiv.org/abs/2504.08603) [[hjfy]](https://hjfy.top/arxiv/2504.08603) `Benchmark` `Zero-Shot` `Memory`
  - 概览：提出开放词汇物体中心建图框架FindAnything，将像素级视觉语言特征按eSAM分割聚合为对象，再写入稠密体素子图，使自然语言查询能够对应到可扩展的三维几何表示。

- **[2025/04][ arXiv 2025 - 视觉语言模型助力机器人在未知环境中高效导航 - CL-CoTNav ]** CL-CoTNav: Closed-Loop Hierarchical Chain-of-Thought for Zero-Shot Object-Goal Navigation with Vision-Language Models [[arxiv]](https://arxiv.org/abs/2504.09000) [[hjfy]](https://hjfy.top/arxiv/2504.09000) `Zero-Shot`
  - 概览：提出CL-CoTNav，用人类示范轨迹生成的多轮问答数据微调VLM，并以层次思维链分步提取目标搜索知识；闭环机制再根据检测与推理置信度加权训练样本，抑制噪声和幻觉。

- **[2025/04][ arXiv 2025 - 扩散桥视觉导航 ]** Prior Does Matter: Visual Navigation via Denoising Diffusion Bridge Models [[arxiv]](https://arxiv.org/abs/2504.10041) [[hjfy]](https://hjfy.top/arxiv/2504.10041) `Diffusion`
  - 概览：提出NaviBridger，以先验动作分布替代高斯噪声作为去噪扩散桥起点，在生成导航动作时兼顾多模态分布建模、推理质量与采样效率。

- **[2025/04][ arXiv 2025 - 通用具身导航综述 ]** Multimodal Perception for Goal-oriented Navigation: A Survey [[arxiv]](https://arxiv.org/abs/2504.15643) [[hjfy]](https://hjfy.top/arxiv/2504.15643) `Survey`
  - 概览：从推理域视角综述目标导向多模态导航，按环境推理机制组织视觉、语言和声学导航方法，并比较不同任务共享的计算基础、特有能力与模态融合难点。

- **[2025/04][ arXiv 2025 - 通用视觉语言导航 - Vision-and-Language ]** Think Hierarchically, Act Dynamically: Hierarchical Multi-modal Fusion and Reasoning for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2504.16516) [[hjfy]](https://hjfy.top/arxiv/2504.16516) `Hierarchical` `Transformer`
  - 概览：提出MFRA多层融合推理架构，分层聚合视觉低层线索、语言语义与导航历史，再以指令引导注意力和动态上下文整合从融合表征中预测动作。

- **[2025/04][ arXiv 2025 - 通用视觉语言导航 - RSRNav ]** RSRNav: Reasoning Spatial Relationship for Image-Goal Navigation [[arxiv]](https://arxiv.org/abs/2504.17991) [[hjfy]](https://hjfy.top/arxiv/2504.17991) `Navigation`
  - 概览：提出RSRNav，在目标图像与当前观测之间构建空间相关性，并通过细粒度交叉相关和方向感知相关逐步细化该表示，再把空间关系作为策略网络的动作预测条件。

- **[2025/04][ Neurocomputing 2025 - 三维语义地图指令路径规划 ]** Instruction-guided path planning with 3D semantic maps for vision-language navigation [[doi]](https://doi.org/10.1016/j.neucom.2025.129457) `3D Semantic Map`
  - 概览：以高分辨率三维语义地图同时保留空间结构和物体语义，再将自然语言指令映射为地图约束并执行路径规划，减少二维或拓扑抽象造成的信息损失。

- **[2025/04][ AAAI 2025 - 噪声环境多声源视听导航 ]** Towards Audio-Visual Navigation in Noisy Environments: A Large-Scale Benchmark Dataset and an Architecture Considering Multiple Sound-Sources [[doi]](https://doi.org/10.1609/aaai.v39i14.33608) `Audio-Visual`
  - 概览：构建含多种声源与环境噪声的大规模BeDAViN视听导航数据集，并设计多声源感知架构，使智能体能在干扰条件下分离目标声音并联合视觉完成导航。

- **[2025/03][ CVPR 2025 - 视觉想象增强VLN - VLN-Imagine ]** Do Visual Imaginations Improve Vision-and-Language Navigation Agents? [[arxiv]](https://arxiv.org/abs/2503.16394) [[hjfy]](https://hjfy.top/arxiv/2503.16394) [[github]](https://github.com/akhilperincherry/VLN-Imagine) [[project]](https://www.akhilperincherry.com/VLN-Imagine-website/) `End-to-end`
  - 概览：利用文生图扩散模型将指令中的地标描述合成为视觉想象子目标，作为额外模态注入VLN智能体并辅以对齐辅助损失，使成功率提升约1个点、SPL最高提升0.5个点。

- **[2025/03][ IROS 2025 - 零样本VLN航点预测与回溯 - SmartWay ]** SmartWay: Enhanced Waypoint Prediction and Backtracking for Zero-Shot Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2503.10069) [[hjfy]](https://hjfy.top/arxiv/2503.10069) [[project]](https://sxyxs.github.io/smartway/) `Zero-Shot` `Habitat`
  - 概览：提出零样本VLN-CE框架，将掩码交叉注意力融合与占据感知损失增强的航点预测器同具备历史感知推理与自适应回溯的MLLM导航器结合，在仿真与真机上均超越已有零样本方法。

- **[2025/03][ Neural Networks 2025 - 域适应全景环境生成 - PanoGen++ ]** PanoGen++: Domain-Adapted Text-Guided Panoramic Environment Generation for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2503.09938) [[hjfy]](https://hjfy.top/arxiv/2503.09938) [[doi]](https://doi.org/10.1016/j.neunet.2025.107320) `Diffusion`
  - 概览：提出面向VLN的域适应全景环境生成框架，将预训练扩散模型与LoRA参数高效微调结合，通过掩码修复与递归外推两种方式生成多样化全景训练环境，在R2R、R4R与CVDN上均提升导航性能。

- **[2025/03][ arXiv 2025 - 动态多人交互人类感知VLN基准 - HA-VLN 2.0 ]** HA-VLN 2.0: An Open Benchmark and Leaderboard for Human-Aware Navigation in Discrete and Continuous Environments with Dynamic Multi-Human Interactions [[arxiv]](https://arxiv.org/abs/2503.14229) [[hjfy]](https://hjfy.top/arxiv/2503.14229) [[github]](https://github.com/UWMILab/HA-VLN) [[project]](https://ha-vln-project.vercel.app/) `Benchmark`
  - 概览：提出人类感知VLN开放基准HA-VLN 2.0，通过HAPS 2.0数据集与离散/连续双模拟器建模动态多人交互，在16844条社会性指令上评测主流智能体并提供公开排行榜与真机验证。

- **[2025/03][ arXiv 2025 - 语言驱动局部全局协同户外导航 - KiteRunner ]** KiteRunner: Language-Driven Cooperative Local-Global Navigation Policy with UAV Mapping in Outdoor Environments [[arxiv]](https://arxiv.org/abs/2503.08330) [[hjfy]](https://hjfy.top/arxiv/2503.08330) `Diffusion` `CLIP+GPT-4o`
  - 概览：将无人机实时正射影像生成的全局概率图与扩散模型驱动的局部路径生成相结合，并借助CLIP与GPT解析自然语言指令，实现开放世界户外长距离地面导航。

- **[2025/03][ arXiv 2025 - 通用视觉语言导航 - CREStE ]** CREStE: Scalable Mapless Navigation with Internet Scale Priors and Counterfactual Guidance [[arxiv]](https://arxiv.org/abs/2503.03921) [[hjfy]](https://hjfy.top/arxiv/2503.03921) [[project]](https://amrl.cs.utexas.edu/creste/) [[github]](https://github.com/ut-amrl/creste_public) `RL`
  - 概览：提出新的模型架构和蒸馏目标，用于从视觉基础模型中提取导航先验知识，学习开放集结构化的鸟瞰图（BEV）感知表示。

- **[2025/03][ arXiv 2025 - 通用视觉语言导航 - AutoSpatial ]** AutoSpatial: Visual-Language Reasoning for Social Robot Navigation through Efficient Spatial Reasoning Learning [[arxiv]](https://arxiv.org/abs/2503.07557) [[hjfy]](https://hjfy.top/arxiv/2503.07557) [[github]](https://github.com/Yanko96/AutoSpatial) `Hierarchical`
  - 概览：提出社会导航空间推理方法AutoSpatial，以少量人工监督配合自动标注的视觉问答对，并采用两轮层次化VQA训练，使模型分别学习全局场景与局部关系。

- **[2025/03][ arXiv 2025 - 通用零样本具身导航 ]** Reasoning in visual navigation of end-to-end trained agents: a dynamical systems approach [[arxiv]](https://arxiv.org/abs/2503.08306) [[hjfy]](https://hjfy.top/arxiv/2503.08306) [[project]](https://europe.naverlabs.com/research/publications/reasoning-in-visual-navigation-of-end-to-end-trained-agents/) `Zero-Shot` `Memory` `End-to-end`
  - 概览：以真实机器人导航回合研究端到端智能体的内部推理，通过动力学预测、潜在记忆探针、有限时域计划分析及价值函数对照，刻画感知、记忆与规划之间的关系。

- **[2025/03][ arXiv 2025 - 社会机器人注意力蒸馏 - ViLAM ]** ViLAM: Distilling Vision–Language Reasoning into Attention Maps for Social Robot Navigation [[arxiv]](https://arxiv.org/abs/2503.09820) [[hjfy]](https://hjfy.top/arxiv/2503.09820) `Distillation`
  - 概览：将视觉语言推理蒸馏为可解释注意力图，令社会机器人在动态人群环境中兼顾语义目标、社交约束与局部规划，并以轻量策略执行实时导航。

- **[2025/03][ IROS 2025 - 细粒度指令引导图推理 - OIKG ]** Fine-Grained Instruction-Guided Graph Reasoning for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2503.11006) [[hjfy]](https://hjfy.top/arxiv/2503.11006) [[doi]](https://doi.org/10.1109/IROS60139.2025.11247072) `VLN`
  - 概览：提出OIKG细粒度指令引导图推理框架：观察图交互模块解耦角度与视觉线索并以几何嵌入增强有向边，指令引导模块则提取地点和物体语义以对齐语言与可行轨迹。

- **[2025/03][ arXiv 2025 - 通用具身导航基准 - MoMa-Kitchen ]** MoMa-Kitchen: A 100K+ Benchmark for Affordance-Grounded Last-Mile Navigation in Mobile Manipulation [[arxiv]](https://arxiv.org/abs/2503.11081) [[hjfy]](https://hjfy.top/arxiv/2503.11081) [[project]](https://momakitchen.github.io/) [[github]](https://github.com/MoMaKitchen/MoMaKitchen) `Benchmark`
  - 概览：提出MoMa-Kitchen基准数据集，包含超过10万个样本，用于训练模型学习在移动操作任务中实现导航与操作无缝衔接的最优最终导航位置，覆盖相关问题。

- **[2025/03][ arXiv 2025 - 通用具身导航基准 - Beyond the Destination ]** Beyond the Destination: A Novel Benchmark for Exploration-Aware Embodied Question Answering [[arxiv]](https://arxiv.org/abs/2503.11117) [[hjfy]](https://hjfy.top/arxiv/2503.11117) [[github]](https://github.com/HCPLab-SYSU/EXPRESS-Bench) [[project]](https://hcplab-sysu.github.io/EXPRESS-Bench/) `Benchmark`
  - 概览：构建EXPRESS-Bench，包含777条探索轨迹和2,044个问题—轨迹对，并以探索—答案一致性指标联合评估探索可靠性与回答依据；同时提出Fine-EQA，将前沿探索和目标导向探索结合。

- **[2025/03][ arXiv 2025 - 通用视觉语言导航 - FlexVLN ]** FlexVLN: Flexible Adaptation for Diverse Vision-and-Language Navigation Tasks [[arxiv]](https://arxiv.org/abs/2503.13966) [[hjfy]](https://hjfy.top/arxiv/2503.13966) `Hierarchical` `Planning`
  - 概览：提出FlexVLN层次框架，由LLM规划器生成高层子目标、监督学习的指令跟随器执行低层动作，并以计划验证和多模型融合抑制规划幻觉，实现跨VLN数据集适配。

- **[2025/03][ arXiv 2025 - 通用视觉语言导航 - CTSAC ]** CTSAC: Curriculum-Based Transformer Soft Actor-Critic for Goal-Oriented Robot Exploration [[arxiv]](https://arxiv.org/abs/2503.14254) [[hjfy]](https://hjfy.top/arxiv/2503.14254) [[github]](https://github.com/ShengbenBi/CTSAC) `RL` `Sim-to-Real` `Transformer`
  - 概览：提出CTSAC，在Soft Actor-Critic感知网络中引入Transformer利用观测历史，并用周期复习式课程学习减轻阶段切换遗忘，再结合激光雷达聚类缩小仿真到现实差距。

- **[2025/03][ arXiv 2025 - 通用视觉语言导航 - Unseen from Seen ]** Unseen from Seen: Rewriting Observation-Instruction Using Foundation Models for Augmenting Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2503.18065) [[hjfy]](https://hjfy.top/arxiv/2503.18065) [[github]](https://github.com/SaDil13/VLN-RAM) `Navigation` `VLM`
  - 概览：提出RAM范式：通过改写人类标注的训练数据生成未见过的观察-指令对，无需依赖模拟器环境或网络收集的数据，将多种基础模型相结合实现数据增强。

- **[2025/03][ arXiv 2025 - 通用视觉语言导航 - RoboTron-Nav ]** RoboTron-Nav: A Unified Framework for Embodied Navigation Integrating Perception, Planning, and Prediction [[arxiv]](https://arxiv.org/abs/2503.18525) [[hjfy]](https://hjfy.top/arxiv/2503.18525) `Multi-task`
  - 概览：提出RoboTron-Nav，通过导航与具身问答多任务协作联合学习感知、规划和预测，并用自适应3D感知历史采样过滤冗余观测，再由大语言模型理解指令并生成动作。

- **[2025/03][ arXiv 2025 - 通用视觉语言导航 - AINav ]** AINav: Large Language Model-Based Adaptive Interactive Navigation [[arxiv]](https://arxiv.org/abs/2503.22942) [[hjfy]](https://hjfy.top/arxiv/2503.22942) `RL` `Pretraining`
  - 概览：提出AINav主动交互导航框架，以LLM驱动的原语技能树决定交互物体与执行顺序，以强化学习技能库执行运动和交互，并由Advisor触发、Arborist修改树结构实现在线重规划。

- **[2025/03][ arXiv 2025 - 通用视觉语言导航 - COSMO ]** COSMO: Combination of Selective Memorization for Low-cost Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2503.24065) [[hjfy]](https://hjfy.top/arxiv/2503.24065) `VLN` `Transformer`
  - 概览：提出COSMO轻量VLN架构，将状态空间模块与Transformer结合，并设计环形选择扫描RSS完成跨模态全局交互、双流CS3完成视觉—语言选择性交互，以降低导航计算成本。

- **[2025/03][ Science China Information Sciences 2025 - 具身导航系统综述 ]** Embodied navigation [[doi]](https://doi.org/10.1007/s11432-024-4303-8) `Survey`
  - 概览：系统综述具身导航的感知、规划控制与效率优化基础，进一步整理自动驾驶、通用助理和仿生导航等任务，并讨论真实部署、多智能体、安全和隐私问题。

- **[2025/02][ WACV 2025 - MLLM辅助目标定位VLN - GroundingMate ]** GroundingMate: Aiding Object Grounding for Goal-Oriented Vision-and-Language Navigation [[cvf]](https://openaccess.thecvf.com/content/WACV2025/html/Liu_GroundingMate_Aiding_Object_Grounding_for_Goal-Oriented_Vision-and-Language_Navigation_WACV_2025_paper.html) `Agentic` `MLLM`
  - 概览：提出即插即用、模型无关的GroundingMate框架，智能体在目标定位受挫时经多阶段自评估提取关键信息并向多模态大模型求助，无需重训练即可提升REVERIE与SOON上的物体定位表现。

- **[2025/02][ IEEE RA-L 2025 - 在线视觉语言地图连续环境VLN - OVL-MAP ]** OVL-MAP: An Online Visual Language Map Approach for Vision-and-Language Navigation in Continuous Environments [[doi]](https://doi.org/10.1109/LRA.2025.3540577) `GSM` `Habitat`
  - 概览：提出在线视觉语言地图算法OVL-MAP，由在线地图构建、航点预测与动作决策三模块组成，利用开放词汇语义分割动态增强场景理解，在Robo-VLN与R2R-CE上显著提升导航性能与未知环境泛化能力。

- **[2025/02][ arXiv 2025 - 标注语义地图记忆表示VLN - MapNav ]** MapNav: A Novel Memory Representation via Annotated Semantic Maps for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2502.13451) [[hjfy]](https://hjfy.top/arxiv/2502.13451) `End-to-end` `LLaVA-OneVision (Qwen2-7B)` `Habitat`
  - 概览：提出以标注语义地图ASM替代历史帧作为VLM导航记忆表示的端到端智能体MapNav，每步更新带文本标注的俯视语义地图，大幅降低存储与计算开销，在R2R-CE与RxR-CE上取得SOTA并完成真机部署。

- **[2025/02][ arXiv 2025 - 神经符号推理视觉语言导航 - VL-Nav ]** VL-Nav: Neuro-Symbolic Reasoning-based Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2502.00931) [[hjfy]](https://hjfy.top/arxiv/2502.00931) [[project]](https://sairlab.org/vlnav/) `GSM`
  - 概览：提出神经符号视觉语言导航系统VL-Nav，将符号化3D场景图与图像记忆融入VLM任务分解与重规划，并以神经语义线索耦合符号启发式函数实现高效探索，真实环境成功率达86.3%。

- **[2025/02][ arXiv 2025 - 检索增强导航指令生成 - NavRAG ]** NavRAG: Generating User Demand Instructions for Embodied Navigation through Retrieval-Augmented LLM [[arxiv]](https://arxiv.org/abs/2502.11142) [[hjfy]](https://hjfy.top/arxiv/2502.11142) [[github]](https://github.com/MrZihan/NavRAG) `Agentic`
  - 概览：提出基于检索增强LLM的导航指令生成框架，构建分层场景描述树并模拟多种用户角色生成贴近真实需求的指令，为861个场景自动标注超200万条数据，缓解VLN训练数据稀缺问题。

- **[2025/02][ RA-L 2025 - 真实到仿真到真实视觉导航与运动控制框架 - VR-Robo ]** VR-Robo: A Real-to-Sim-to-Real Framework for Visual Robot Navigation and Locomotion [[arxiv]](https://arxiv.org/abs/2502.01536) [[hjfy]](https://hjfy.top/arxiv/2502.01536) [[project]](https://vr-robo.github.io/) `RL` `3DGS`
  - 概览：提出Real-to-Sim-to-Real框架VR-Robo，基于3DGS重建照片级且物理可交互的数字孪生环境用于四足机器人视觉导航与运动策略的RL训练，实现RGB感知策略免微调真机部署。

- **[2025/02][ arXiv 2025 - 手绘地图引导移动机器人导航 ]** Mobile Robot Navigation Using Hand-Drawn Maps: A Vision Language Model Approach [[arxiv]](https://arxiv.org/abs/2502.00114) [[hjfy]](https://hjfy.top/arxiv/2502.00114) `VLM`
  - 概览：提出HAM-Nav，使用视觉语言模型同时理解手绘地图、实时相机观测与机器人位置，在地图比例、风格和几何存在误差时仍能生成可执行导航决策。

- **[2025/02][ arXiv 2025 - 通用视觉语言导航 - VertiFormer ]** VertiFormer: A Data-Efficient Multi-Task Transformer for Off-Road Robot Mobility [[arxiv]](https://arxiv.org/abs/2502.00543) [[hjfy]](https://hjfy.top/arxiv/2502.00543) [[github]](https://github.com/mhnazeri/VertiFormer) `Multi-task` `Transformer`
  - 概览：提出数据高效多任务Transformer模型VERTIFORMER，其通过统一的多模态潜在表示、可学习的掩码建模以及非自回归训练，能够在仅使用一小时训练数据的情况下，同时完成多种越野移动任务，例如正向和逆向运动学建模、行为克隆以及地形块重建等。

- **[2025/02][ arXiv 2025 - 通用零样本具身导航 - TRAVEL ]** TRAVEL: Training-Free Retrieval and Alignment for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2502.07306) [[hjfy]](https://hjfy.top/arxiv/2502.07306) `Zero-Shot` `Retrieval` `VLM`
  - 概览：提出基于模块化方法的Vision-Language Navigation（VLN）任务解决方案，该方法在零样本设置下利用现有的大型语言模型（LLMs）和视觉语言模型（VLMs），将问题分解为四个子模块，通过提取导航指令中的地标和访问顺序，检索最后地标的候选位置，生成路径假设，并计算与指令的对齐分数，最终评估路径保真度。

- **[2025/02][ arXiv 2025 - 通用零样本具身导航 - VL-Explore ]** VL-Explore: Zero-shot Vision-Language Exploration and Target Discovery by Mobile Robots [[arxiv]](https://arxiv.org/abs/2502.08791) [[hjfy]](https://hjfy.top/arxiv/2502.08791) [[project]](https://zhangyx.net/ClipRover/) `Zero-Shot` `Planning` `VLM`
  - 概览：提出VL-Explore，以单目视觉和CLIP在无先验地图、无目标先验条件下联合进行环境探索与目标发现，并将该管线部署到Open Rover无人地面车进行实时导航。

- **[2025/02][ arXiv 2025 - 通用具身导航基准 - OpenBench ]** OpenBench: A New Benchmark and Baseline for Semantic Navigation in Smart Logistics [[arxiv]](https://arxiv.org/abs/2502.09238) [[hjfy]](https://hjfy.top/arxiv/2502.09238) [[project]](https://ei-nav.github.io/OpenBench/) [[github]](https://github.com/EI-Nav/light-map-navigation) `Benchmark` `VLM`
  - 概览：构建面向住宅区末端配送的OpenBench室外语义导航基准，并提出OPEN系统：用OpenStreetMap作轻量地图、LLM理解配送指令、VLM完成全局定位、地图更新与门牌识别。

- **[2025/02][ arXiv 2025 - 房间专家图像目标导航 - REGNav ]** REGNav: Room Expert Guided Image-Goal Navigation [[arxiv]](https://arxiv.org/abs/2502.10785) [[hjfy]](https://hjfy.top/arxiv/2502.10785) `ImageNav`
  - 概览：提出REGNav，先以无监督学习在未标注房间图像上预训练房间专家，判断目标图像与当前观测是否来自同一房间，再通过两种融合方式把房间关系知识注入图像目标导航策略。

- **[2025/02][ arXiv 2025 - 通用具身导航基准 - CityEQA ]** CityEQA: A Hierarchical LLM Agent on Embodied Question Answering Benchmark in City Space [[arxiv]](https://arxiv.org/abs/2502.12532) [[hjfy]](https://hjfy.top/arxiv/2502.12532) `Benchmark` `Zero-Shot` `Agentic`
  - 概览：设计基于LLM的Planner模块解析任务指令并生成计划，Manager协调多模态感知模块并维护包含认知地图的记忆模块，监督和推进计划执行，Actor执行提供变尺度动作生成器，以有效应对大范围城市环境带来的行动挑战。

- **[2025/02][ arXiv 2025 - 通用零样本具身导航 - NavigateDiff ]** NavigateDiff: Visual Predictors are Zero-Shot Navigation Assistants [[arxiv]](https://arxiv.org/abs/2502.13894) [[hjfy]](https://hjfy.top/arxiv/2502.13894) [[project]](https://21styouth.github.io/NavigateDiff/) `Diffusion` `Zero-Shot` `RL`
  - 概览：引入了视觉预测器，结合多模态语言模型和扩散模型，用于生成未来的场景图像，以辅助机器人决策。

- **[2025/02][ arXiv 2025 - 通用视觉语言导航 - Mem2Ego ]** Mem2Ego: Empowering Vision-Language Models with Global-to-Ego Memory for Long-Horizon Embodied Navigation [[arxiv]](https://arxiv.org/abs/2502.14254) [[hjfy]](https://hjfy.top/arxiv/2502.14254) `Memory` `VLM`
  - 概览：提出整合全局记忆模块中的任务相关线索与智能体的自我视角观察的导航框架，以增强导航中的空间推理和决策能力。

- **[2025/02][ arXiv 2025 - 通用视觉语言导航 - Vision-and-Language ]** Ground-level Viewpoint Vision-and-Language Navigation in Continuous Environments [[arxiv]](https://arxiv.org/abs/2502.19024) [[hjfy]](https://hjfy.top/arxiv/2502.19024) `Sim-to-Real`
  - 概览：提出地面低视角导航方法GVNav，以加权历史观测补充时空上下文，并迁移HM3D与Gibson连接图作为空间先验，缓解人类视角指令与四足机器人低机位观测之间的错配。

- **[2025/02][ arXiv 2025 - 主动任务驱动的语言嵌入高斯绘制 - ATLAS Navigator ]** ATLAS Navigator: Active Task-driven LAnguage-embedded Gaussian Splatting [[arxiv]](https://arxiv.org/abs/2502.20386) [[hjfy]](https://hjfy.top/arxiv/2502.20386) `Hierarchical`
  - 概览：提出ATLAS Navigator层次语言高斯地图，以可在线更新的低维语言嵌入支持稀疏语义任务规划，同时保留稠密度量几何用于无碰撞局部导航，使自然语言任务能在未知环境中边建图边执行。

- **[2025/01][ ICLR 2025 - 场景自适应VLN任务与数据集 - GSA-VLN ]** General Scene Adaptation for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2501.17403) [[hjfy]](https://hjfy.top/arxiv/2501.17403) [[github]](https://github.com/honghd16/GSA-VLN) `Benchmark`
  - 概览：提出要求智能体在特定场景中执行指令的同时持续自适应的GSA-VLN任务与GSA-R2R数据集，用LLM三阶段指令编排管线扩充环境与指令风格多样性，并提出基于全局记忆的GR-DUET方法。

- **[2025/01][ arXiv 2025 - 动态家庭开放词汇实例导航 - OpenIN ]** OpenIN: Open-Vocabulary Instance-Oriented Navigation in Dynamic Domestic Environments [[arxiv]](https://arxiv.org/abs/2501.04279) [[hjfy]](https://hjfy.top/arxiv/2501.04279) `Open-Vocabulary`
  - 概览：提出OpenIN，统一文本和图像形式的需求级、语义级与实例级目标，并持续更新动态家庭环境中的实例位置，实现开放词汇、实例导向导航。

- **[2025/01][ arXiv 2025 - 通用具身导航综述 - AI ]** Semantic Mapping in Indoor Embodied AI -- A Survey on Advances, Challenges, and Future Directions [[arxiv]](https://arxiv.org/abs/2501.05750) [[hjfy]](https://hjfy.top/arxiv/2501.05750) `Survey` `Zero-Shot` `GSM`
  - 概览：分类框架：提出基于地图结构（如空间网格、拓扑图、密集几何图和混合图）和语义编码（显式特征与隐式特征）的分类框架，帮助更好地理解和比较不同方法。

- **[2025/01][ arXiv 2025 - 通用视觉语言导航 - Dual-BEV Nav ]** Dual-BEV Nav: Dual-layer BEV-based Heuristic Path Planning for Robotic Navigation in Unstructured Outdoor Environments [[arxiv]](https://arxiv.org/abs/2501.18351) [[hjfy]](https://hjfy.top/arxiv/2501.18351) `Sim-to-Real` `Planning`
  - 概览：提出Dual-BEV Nav：局部BEV规划器生成可通行候选路径，再将其投影到全局BEV可通行概率图选择航点，以双层启发式规划支持低质量定位与地图条件下的室外长程导航。

- **[2025/01][ TMM 2025 - 记忆观测协同连续VLN - MossVLN ]** MossVLN: Memory-Observation Synergistic System for Continuous Vision-Language Navigation [[doi]](https://doi.org/10.1109/TMM.2025.3586105) `Memory`
  - 概览：提出MossVLN，以观察驱动航点预测器融合深度空间线索和视觉语言对齐信息，并与历史记忆协同更新，提高连续环境中的航点选择和路径稳定性。

- **[2025/01][ TRO 2025 - 时间最优空间迭代向量场 ]** High-Efficiency Vector Field by Time-Optimal Spatial Iterative Learning [[doi]](https://doi.org/10.1109/TRO.2025.3610174) `Iterative Learning`
  - 概览：提出模型无关的时空迭代学习框架，将历史运行经验写入向量场，在保持线性计算复杂度、安全性与鲁棒性的同时优化移动机器人的通行时间。

- **[2025/X][ IROS 2025 - 反事实风格适应因果推理连续VLN - CVLN-Think ]** CVLN-Think: Causal Inference with Counterfactual Style Adaptation for Continuous Vision-and-Language Navigation [[doi]](https://doi.org/10.1109/iros60139.2025.11247004) `End-to-end`
  - 概览：提出融合因果推理的连续视觉语言导航模型CVLN-Think，通过风格因果调节器生成反事实风格观测以消除风格混杂因素，增强导航策略在未见环境下的鲁棒性与适应性。

- **[2024/12][ RSS 2025 - 统一具身导航任务视频VLA - Uni-NaVid ]** Uni-NaVid: A Video-based Vision-Language-Action Model for Unifying Embodied Navigation Tasks [[arxiv]](https://arxiv.org/abs/2412.06224) [[hjfy]](https://hjfy.top/arxiv/2412.06224) [[github]](https://github.com/jzhzhang/Uni-NaVid) [[project]](https://pku-epic.github.io/Uni-NaVid/) `End-to-end` `Vicuna-7B` `Habitat`
  - 概览：首个统一VLN、目标搜索、具身问答与人员跟随等多种具身导航任务的视频VLA模型，通过统一各任务的输入输出配置并在360万导航样本上训练，实现真实环境混合长程任务的无缝导航。

- **[2024/12][ TPAMI 2025 - 约束感知零样本连续环境VLN - CA-Nav ]** Constraint-Aware Zero-Shot Vision-Language Navigation in Continuous Environments [[arxiv]](https://arxiv.org/abs/2412.10137) [[hjfy]](https://hjfy.top/arxiv/2412.10137) `Zero-Shot`
  - 概览：提出约束感知导航器CA-Nav，将零样本连续环境VLN重构为约束感知的子指令序贯完成过程，由子指令管理器跟踪进度并动态生成约束引导的价值图，在R2R-CE和RxR-CE上零样本SOTA并完成真机部署。

- **[2024/12][ AAAI 2025 - 情景模拟与情景记忆VLN ]** Planning from Imagination: Episodic Simulation and Episodic Memory for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2412.01857) [[hjfy]](https://hjfy.top/arxiv/2412.01857) [[aaai]](https://ojs.aaai.org/index.php/AAAI/article/view/32679) `World Model`
  - 概览：受人类情景模拟与情景记忆机制启发，提出现实-想象混合记忆系统，使智能体能想象未来场景的高保真RGB图像并纳入记忆进行规划，在R2R与REVERIE未见环境上分别提升5%与7%成功率。

- **[2024/12][ CVPR 2025 - 房屋导览视频指令数据集 - RoomTour3D ]** RoomTour3D: Geometry-Aware Video-Instruction Tuning for Embodied Navigation [[arxiv]](https://arxiv.org/abs/2412.08591) [[hjfy]](https://hjfy.top/arxiv/2412.08591) [[project]](https://roomtour3d.github.io/) `Benchmark`
  - 概览：利用网络房屋导览视频构建几何感知的视频-指令数据集，结合3D重建自动生成约10万条开放词汇轨迹与20万条指令，显著提升CVDN、SOON、R2R与REVERIE等导航任务性能。

- **[2024/12][ RSS 2025 - 足式机器人VLA导航框架 - NaVILA ]** NaVILA: Legged Robot Vision-Language-Action Model for Navigation [[arxiv]](https://arxiv.org/abs/2412.04453) [[hjfy]](https://hjfy.top/arxiv/2412.04453) [[project]](https://navila-bot.github.io/) `Hierarchical` `VILA` `Isaac Sim`
  - 概览：提出面向足式机器人的两级VLA导航框架NaVILA，上层VLM将指令转化为"前进75厘米"等中级语言动作，下层视觉运动RL策略执行精细关节控制，实现四足与人形机器人在真实复杂环境中的指令跟随导航。

- **[2024/12][ RA-L 2024 - LLM指令分解高效强化学习VLN - DILLM-VLN ]** Boosting Efficient Reinforcement Learning for Vision-and-Language Navigation with Open-Sourced LLM [[doi]](https://doi.org/10.1109/lra.2024.3511402) [[github]](https://github.com/wangjw55/DILLM) `RL` `ChatGLM-6B` `Matterport3D`
  - 概览：提出DILLM-VLN，利用轻量级开源LLM(ChatGLM-6B)将复杂导航指令分解为简单可解释的子指令，结合级联多尺度注意力与多模态融合判别器判定子指令完成情况，逐段引导RL智能体高效学习导航。

- **[2024/12][ arXiv 2024 - 世界一致性VLN数据生成 - WCGEN ]** World-Consistent Data Generation for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2412.06413) [[hjfy]](https://hjfy.top/arxiv/2412.06413) `Diffusion`
  - 概览：提出兼顾多样性与世界一致性的VLN数据增强框架WCGEN，轨迹阶段以点云技术保证视点间空间连贯，视点阶段以新颖角度合成方法结合3D知识预测视角变化，显著提升智能体对未见环境的泛化能力。

- **[2024/12][ ICLR 2025 - 自精炼数据飞轮 - SRDF ]** Bootstrapping Language-Guided Navigation Learning with Self-Refining Data Flywheel [[arxiv]](https://arxiv.org/abs/2412.08467) [[hjfy]](https://hjfy.top/arxiv/2412.08467) [[github]](https://github.com/wz0919/VLN-SRDF) `End-to-end`
  - 概览：提出自精炼数据飞轮SRDF，让指令生成器与导航器协作迭代过滤并再生成指令-轨迹对，无需人工标注持续提升数据质量，训练的导航器在R2R测试集上以78% SPL首次超越人类表现(76%)。

- **[2024/12][ CVPR 2025 - 长时程VLN平台与基准 - LH-VLN ]** Towards Long-Horizon Vision-Language Navigation: Platform, Benchmark and Method [[arxiv]](https://arxiv.org/abs/2412.09082) [[hjfy]](https://hjfy.top/arxiv/2412.09082) [[github]](https://github.com/HCPLab-SYSU/LH-VLN) [[project]](https://hcplab-sysu.github.io/LH-VLN/) `Benchmark`
  - 概览：提出强调多阶段连续子任务的长时程视觉语言导航任务LH-VLN，构建自动数据生成平台NavGen与含3,260个任务的基准LHPR-VLN，并提出多粒度动态记忆模型MGDM作为基线方法。

- **[2024/12][ arXiv 2024 - 通用视觉语言导航 - SAME ]** SAME: Learning Generic Language-Guided Visual Navigation with State-Adaptive Mixture of Experts [[arxiv]](https://arxiv.org/abs/2412.05552) [[hjfy]](https://hjfy.top/arxiv/2412.05552) [[github]](https://github.com/GengzeZhou/SAME) `Navigation`
  - 概览：提出状态自适应混合专家模型SAME，根据语言指令粒度和动态观测选择任务共享知识与专用专家，把类别级搜索和细粒度指令跟随统一到同一导航智能体中。

- **[2024/12][ arXiv 2024 - 通用具身导航基准 - doScenes ]** doScenes: An Autonomous Driving Dataset with Natural Language Instruction for Human Interaction and Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2412.05893) [[hjfy]](https://hjfy.top/arxiv/2412.05893) [[github]](https://github.com/rossgreer/doScenes) `Benchmark`
  - 概览：doScenes集通过自然语言指令和引用标签对多模态传感器数据进行标注，弥合了指令和驾驶响应之间的差距，实现了上下文感知和自适应规划。

- **[2024/12][ arXiv 2024 - 语义空间层次表征 - SUSA ]** Agent Journey Beyond RGB: Hierarchical Semantic-Spatial Representation Enrichment for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2412.06465) [[hjfy]](https://hjfy.top/arxiv/2412.06465) `Semantic Map`
  - 概览：提出SUSA，将指令相关地标的文本语义与深度驱动的空间探索图结合，形成局部动作和全局路线共享的层次语义空间表征。

- **[2024/12][ arXiv 2024 - 通用视觉语言导航 - CogNav ]** CogNav: Cognitive Process Modeling for Object Goal Navigation with LLMs [[arxiv]](https://arxiv.org/abs/2412.10439) [[hjfy]](https://hjfy.top/arxiv/2412.10439) [[project]](https://yhancao.github.io/CogNav/) [[github]](https://github.com/yhanCao/CogNav_ObjNav) `Navigation`
  - 概览：提出一种在线构建的异构认知地图表示，该地图能够动态更新并通过提示LLM来确保高地图质量，为导航提供了更丰富的环境信息。

- **[2024/12][ arXiv 2024 - 通用视觉语言导航 - NAVCON ]** NAVCON: A Cognitively Inspired and Linguistically Grounded Corpus for Vision and Language Navigation [[arxiv]](https://arxiv.org/abs/2412.13026) [[hjfy]](https://hjfy.top/arxiv/2412.13026) `Navigation`
  - 概览：构建VLN语料库NAVCON，在R2R与RxR指令上定义四类认知和语言导航概念，以自动算法生成银标注，并将概念片段与智能体执行指令时的沿途图像对齐。

- **[2024/12][ arXiv 2024 - 通用视觉语言导航 - The One RING ]** The One RING: a Robotic Indoor Navigation Generalist [[arxiv]](https://arxiv.org/abs/2412.14401) [[hjfy]](https://hjfy.top/arxiv/2412.14401) [[project]](https://one-ring-policy.allen.ai/) `Navigation`
  - 概览：提出机器人室内导航通用策略RING，该策略在模拟中通过大规模随机生成的机器人实体进行训练，能够在未见过的实体上实现零样本泛化。

- **[2024/12][ arXiv 2024 - 平面图引导具身导航 - FloNa ]** FloNa: Floor Plan Guided Embodied Visual Navigation [[arxiv]](https://arxiv.org/abs/2412.18335) [[hjfy]](https://hjfy.top/arxiv/2412.18335) `Floor Plan`
  - 概览：提出利用建筑平面图与第一人称RGB观测的FloNa任务和模型，将全局楼层结构与局部视觉线索对齐，以支持未知室内环境中的目标定位和路径决策。

- **[2024/11][ arXiv 2024 - 零样本物体中心指令跟随 - OC-VLN ]** Zero-shot Object-Centric Instruction Following: Integrating Foundation Models with Traditional Navigation [[arxiv]](https://arxiv.org/abs/2411.07848) [[hjfy]](https://hjfy.top/arxiv/2411.07848) `Zero-Shot`
  - 概览：提出零样本物体中心指令跟随方法LIFGIF，将基础模型的开放词汇感知与基于因子图的传统SLAM导航栈相结合，构建OC-VLN评测数据集并在Boston Dynamics Spot实机上完成验证。

- **[2024/11][ arXiv 2024 - 泛化3DGS连续环境VLN - UnitedVLN ]** UnitedVLN: Generalizable Gaussian Splatting for Continuous Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2411.16053) [[hjfy]](https://hjfy.top/arxiv/2411.16053) `End-to-end` `3DGS`
  - 概览：提出基于泛化3DGS的VLN-CE预训练范式UnitedVLN，通过渲染未来环境的高保真图像与语义特征，联合利用外观级与语义级信息辅助导航决策，克服纯RGB或纯特征想象方法的局限。

- **[2024/11][ arXiv 2024 - 大规模3D语义理解与导航数据集 - VLA-3D ]** VLA-3D: A Dataset for 3D Semantic Scene Understanding and Navigation [[arxiv]](https://arxiv.org/abs/2411.03540) [[hjfy]](https://hjfy.top/arxiv/2411.03540) [[github]](https://github.com/HaochenZ11/VLA-3D) `Benchmark` `3D Scene Graph`
  - 概览：构建覆盖1.15万间真实扫描室内房间的VLA-3D数据集，提供2350万条物体语义关系、970万条指代表达以及点云、场景图和可通行自由空间标注，服务开放世界3D语义理解与语言导航。

- **[2024/11][ arXiv 2024 - 均衡搜索零样本语义导航 - VLN-Game ]** VLN-Game: Vision-Language Equilibrium Search for Zero-Shot Semantic Navigation [[arxiv]](https://arxiv.org/abs/2411.11609) [[hjfy]](https://hjfy.top/arxiv/2411.11609) `Game Search`
  - 概览：提出VLN-Game，将预训练视觉语言特征与三维重建融合为对象中心空间地图，先筛选有潜力的探索区域，再由博弈式视觉语言模型在候选目标间判断与对象名称或描述性语言最匹配的实例。

- **[2024/11][ arXiv 2024 - 任意物体精准局部导航 ]** Aim My Robot: Precision Local Navigation to Any Object [[arxiv]](https://arxiv.org/abs/2411.14770) [[hjfy]](https://hjfy.top/arxiv/2411.14770) `Local Navigation`
  - 概览：提出Aim My Robot，在无需预建地图或目标三维模型的条件下，从视觉目标描述估计局部相对位姿，并使机器人以厘米级精度到达指定物体附近。

- **[2024/11][ arXiv 2024 - 通用零样本具身导航 - TopV-Nav ]** TopV-Nav: Unlocking the Top-View Spatial Reasoning Potential of MLLM for Zero-shot Object Navigation [[arxiv]](https://arxiv.org/abs/2411.16425) [[hjfy]](https://hjfy.top/arxiv/2411.16425) `Zero-Shot`
  - 概览：提出TopV-Nav，以自适应视觉提示构建含语义的俯视图，动态缩放地图支持局部细粒度推理，并预测潜在目标位置以指导全局零样本目标探索。

- **[2024/11][ arXiv 2024 - 通用视觉语言导航 - CityWalker ]** CityWalker: Learning Embodied Urban Navigation from Web-Scale Videos [[arxiv]](https://arxiv.org/abs/2411.17820) [[hjfy]](https://hjfy.top/arxiv/2411.17820) [[project]](https://ai4ce.github.io/CityWalker/) [[github]](https://github.com/ai4ce/CityWalker) `IL`
  - 概览：设计简单且可扩展的数据处理范式：无需大量手动标注，仅依靠现成的视觉里程计（VO）模型从视频中提取动作监督信号，即可实现大规模模仿学习，降低了数据准备的成本和难度，使模型能够从海量数据中学习到复杂的导航策略。

- **[2024/10][ NeurIPS 2024 - 能量模型VLN导航策略 - ENP ]** Vision-Language Navigation with Energy-Based Policy [[arxiv]](https://arxiv.org/abs/2410.14250) [[hjfy]](https://hjfy.top/arxiv/2410.14250) `End-to-end`
  - 概览：提出能量化导航策略ENP，用能量模型显式建模专家的状态-动作联合分布以取代判别式行为克隆目标，可嵌入多种VLN架构并在R2R、REVERIE等基准上带来一致提升。

- **[2024/10][ NeurIPS 2024 - 在线3D场景图提示零样本目标导航 - SG-Nav ]** SG-Nav: Online 3D Scene Graph Prompting for LLM-based Zero-shot Object Navigation [[arxiv]](https://arxiv.org/abs/2410.08189) [[hjfy]](https://hjfy.top/arxiv/2410.08189) [[github]](https://github.com/bagh2178/SG-Nav) [[project]](https://bagh2178.github.io/SG-Nav/) `Zero-Shot` `LLM (Scene Graph)`
  - 概览：提出零样本物体目标导航框架SG-Nav，在线增量构建物体-组-房间层次化3D场景图并设计层级思维链提示，让LLM基于场景上下文推理目标位置，无需任何训练即大幅超越此前零样本方法。

- **[2024/10][ IROS 2024 - 多目标长时程VLN基准 - MG-VLN ]** MG-VLN: Benchmarking Multi-Goal and Long-Horizon Vision-Language Navigation with Language Enhanced Memory Map [[doi]](https://doi.org/10.1109/IROS58592.2024.10801689) `Benchmark`
  - 概览：基于REVERIE扩展提出多目标长时程VLN基准MG-VLN，要求智能体按序完成高层指令序列，并提出语言增强记忆地图利用先前子目标积累的环境信息提升长时程导航表现。

- **[2024/10][ CoRL 2024 - 野外视频学习语言条件导航策略 - LeLaN ]** LeLaN: Learning A Language-Conditioned Navigation Policy from In-the-Wild Videos [[arxiv]](https://arxiv.org/abs/2410.03603) [[hjfy]](https://hjfy.top/arxiv/2410.03603) [[project]](https://learning-language-navigation.github.io/) `End-to-end` `VLM`
  - 概览：利用VLM与机器人基础模型自动标注130余小时无动作野外第一视角视频，学习语言条件物体导航策略；逾1000次真实机器人测试中优于既有方法，并在边缘设备上实现约4倍推理加速。

- **[2024/10][ 预印本 2024 - 大语言模型机器人导航综述 ]** Recent Advances in Robot Navigation via Large Language Models: A Review [[doi]](https://doi.org/10.13140/RG.2.2.35284.41603) [[chinaxiv]](https://chinarxiv.org/items/chinaxiv-202503.00046) `Survey` `LLM`
  - 概览：按感知、规划、控制、交互与协同五个环节系统梳理LLM机器人导航研究，同时总结主要数据集和评测指标，并讨论多模态环境编码、实时部署、可靠性与泛化等开放挑战。

- **[2024/10][ arXiv 2024 - 通用零样本具身导航 - Open-Architecture ]** Open-Architecture End-to-End System for Real-World Autonomous Robot Navigation [[arxiv]](https://arxiv.org/abs/2410.06239) [[hjfy]](https://hjfy.top/arxiv/2410.06239) `Zero-Shot` `GSM` `Hierarchical`
  - 概览：提出实时在线自主导航框架OrionNav，能够在未知且不断变化的环境中，通过集成多级抽象的感知和规划流程，实现基于自然语言指令的机器人自主导航任务。

- **[2024/10][ arXiv 2024 - 自适应非抓取移动操作导航 ]** Interactive Navigation With Adaptive Non-Prehensile Mobile Manipulation [[arxiv]](https://arxiv.org/abs/2410.13418) [[hjfy]](https://hjfy.top/arxiv/2410.13418) `Model-Based Control`
  - 概览：在线辨识不同物体的SE(2)非抓取交互动力学，并将自适应模型接入MPPI控制，使移动机器人可通过推、绕等动作在未知物体动力学下联合导航与操作。

- **[2024/10][ arXiv 2024 - VLM推理零样本目标导航 - VLTNet ]** Zero-Shot Object Navigation with Vision-Language Models Reasoning [[arxiv]](https://arxiv.org/abs/2410.18570) [[hjfy]](https://hjfy.top/arxiv/2410.18570) `Zero-shot`
  - 概览：提出VLTNet，将视觉语言模型推理与Tree-of-Thought候选搜索结合，在无需目标类别专项训练的条件下完成语言驱动的零样本目标导航。

- **[2024/10][ Official Publication 2024 - LLM协作式粗粒度VLN - VLN-Copilot ]** LLM as Copilot for Coarse-Grained Vision-and-Language Navigation [[doi]](https://doi.org/10.1007/978-3-031-72652-1_27) `LLM`
  - 概览：提出VLN-Copilot，以混淆分数判断智能体何时需要协助，再让LLM分析当前困难并提供情境化指导；在REVERIE和CVDN-target上验证主动求助机制。

- **[2024/09][ ICRA 2025 - 开源LLM零样本连续环境VLN - Open-Nav ]** Open-Nav: Exploring Zero-Shot Vision-and-Language Navigation in Continuous Environment with Open-Source LLMs [[arxiv]](https://arxiv.org/abs/2409.18794) [[hjfy]](https://hjfy.top/arxiv/2409.18794) [[github]](https://github.com/YanyuanQiao/Open-Nav) [[project]](https://sites.google.com/view/opennav) `Zero-Shot`
  - 概览：探索用开源LLM实现连续环境零样本VLN，通过时空思维链将任务分解为指令理解、进度估计与决策，并以细粒度物体与空间知识增强场景感知，性能可比肩闭源GPT-4方案。

- **[2024/09][ ICRA 2025 - 物理接地VLM室外地形导航 - VLM-GroNav ]** Robot Navigation Using Physically Grounded Vision-Language Models in Outdoor Environments [[arxiv]](https://arxiv.org/abs/2409.20445) [[hjfy]](https://hjfy.top/arxiv/2409.20445) `Zero-Shot`
  - 概览：提出将VLM语义推理与本体感知物理量(打滑、下陷)在线融合的室外导航框架，动态更新地形可通行性估计并相应调整全局与局部规划，在腿式与轮式机器人真实实验中显著提升导航成功率。

- **[2024/09][ arXiv 2024 - 持续学习VLN范式 - VLNCL ]** Vision-Language Navigation with Continual Learning [[arxiv]](https://arxiv.org/abs/2409.02561) [[hjfy]](https://hjfy.top/arxiv/2409.02561) `End-to-end`
  - 概览：提出视觉语言导航持续学习范式VLNCL，采用脑启发的双循环情景记忆回放机制让智能体增量学习新环境同时巩固既有知识，缓解灾难性遗忘并提升未见环境泛化能力。

- **[2024/09][ arXiv 2024 - 渐进知识蒸馏轻量化VLN - MiniVLN ]** MiniVLN: Efficient Vision-and-Language Navigation by Progressive Knowledge Distillation [[arxiv]](https://arxiv.org/abs/2409.18800) [[hjfy]](https://hjfy.top/arxiv/2409.18800) `End-to-end` `Distillation`
  - 概览：提出覆盖预训练与导航微调的两阶段渐进知识蒸馏框架，分别传递细粒度跨模态知识与任务专属决策知识，使仅约教师12%参数的MiniVLN在R2R和REVERIE上达到接近教师的性能。

- **[2024/09][ NeurIPS 2024 - 日常物体触发的VLN后门攻击 - IPR Backdoor ]** Everyday Object Meets Vision-and-Language Navigation Agent via Backdoor [[neurips]](https://proceedings.neurips.cc/paper_files/paper/2024/hash/58e6c003c9fb3992265005ff6aef1913-Abstract-Conference.html) [[github]](https://github.com/Chenkehan21/VLN-ATT) `RL` `Security`
  - 概览：提出物体感知VLN后门范式IPR Backdoor，以门、画作和瑜伽球等日常物体充当隐蔽触发器，使智能体在未见物理或数字环境中执行预设异常行为，同时保持正常场景导航性能。

- **[2024/09][ arXiv 2024 - 实时开放词汇多目标地图 - OneMap ]** One Map to Find Them All: Real-time Open-Vocabulary Mapping for Zero-shot Multi-Object Navigation [[arxiv]](https://arxiv.org/abs/2409.11764) [[hjfy]](https://hjfy.top/arxiv/2409.11764) `Open-Vocabulary Map`
  - 概览：提出OneMap，在一次探索中增量构建带不确定性的实时开放词汇地图，使多个目标查询能复用同一语义空间记忆并进行零样本搜索。

- **[2024/09][ arXiv 2024 - 通用视觉语言导航 - ReMEmbR ]** ReMEmbR: Building and Reasoning Over Long-Horizon Spatio-Temporal Memory for Robot Navigation [[arxiv]](https://arxiv.org/abs/2409.13682) [[hjfy]](https://hjfy.top/arxiv/2409.13682) [[project]](https://nvidia-ai-iot.github.io/remembr/) [[github]](https://github.com/NVIDIA-AI-IOT/remembr) `Memory` `Retrieval`
  - 概览：介绍了ReMEmbR，用于构建和推理机器人导航中的长时序时空记忆，通过结合检索增强记忆和大模型（LLM）智能体，能够有效地处理机器人长时间积累的历史数据，并回答关于这些数据的自由形式问题。

- **[2024/08][ AAAI 2025 - 城市街景多模态LLM导航智能体 - FLAME ]** FLAME: Learning to Navigate with Multimodal LLM in Urban Environments [[arxiv]](https://arxiv.org/abs/2408.11051) [[hjfy]](https://hjfy.top/arxiv/2408.11051) [[github]](https://github.com/xyz9911/FLAME) [[project]](https://flame-sjtu.github.io) `End-to-end` `Flamingo`
  - 概览：提出基于Flamingo架构的城市视觉语言导航多模态LLM智能体FLAME，采用从单感知、多感知到端到端轨迹调优的三阶段训练策略适配街景导航，在Touchdown与Map2seq上显著超越此前方法。

- **[2024/08][ ACM MM 2024 - 先定位后规划室外VLN - Loc4Plan ]** Loc4Plan: Locating Before Planning for Outdoor Vision and Language Navigation [[arxiv]](https://arxiv.org/abs/2408.05090) [[hjfy]](https://hjfy.top/arxiv/2408.05090) `End-to-end`
  - 概览：受人类先定位后规划的导航习惯启发提出Loc4Plan框架，通过块感知空间定位(BAL)模块与空间感知动作规划(SAP)模块将智能体空间位置感知引入室外VLN，在Touchdown与map2seq基准上显著提升导航性能。

- **[2024/08][ arXiv 2024 - 通用视觉语言导航 - Perceive, Reflect, and Plan ]** Perceive, Reflect, and Plan: Designing LLM Agent for Goal-Directed City Navigation without Instructions [[arxiv]](https://arxiv.org/abs/2408.04168) [[hjfy]](https://hjfy.top/arxiv/2408.04168) `Agentic` `Memory`
  - 概览：提出Perceive—Reflect—Plan城市导航智能体：微调LLaVA估计地标方向与距离，以可检索记忆反思历史决策，再根据反思结果生成长程计划，在无逐步指令条件下导航至语言描述的目标。

- **[2024/08][ arXiv 2024 - 通用视觉语言导航 - UNMuTe ]** UNMuTe: Unifying Navigation and Multimodal Dialogue-like Text Generation [[arxiv]](https://arxiv.org/abs/2408.04423) [[hjfy]](https://hjfy.top/arxiv/2408.04423) `Navigation`
  - 概览：提出两模块计算模型UNMuTe，能够同时执行基于对话形式的文本指令导航，并生成有助于导航者朝目标物体移动的问题-答案对。

- **[2024/08][ arXiv 2024 - 通用具身导航基准 - RoboSense ]** RoboSense: Large-scale Dataset and Benchmark for Egocentric Robot Perception and Navigation in Crowded and Unstructured Environments [[arxiv]](https://arxiv.org/abs/2408.15503) [[hjfy]](https://hjfy.top/arxiv/2408.15503) [[github]](https://github.com/suhaisheng/RoboSense) `Benchmark`
  - 概览：基于RoboSense定义了6个标准化基准任务，包括多视图3D检测、LiDAR 3D检测、多模态3D检测、多目标跟踪、运动预测和占用预测，为相关导航研究的发展提供了评估和公平比较的基准。

- **[2024/08][ Official Publication 2024 - 智能制造LLM协作机器人导航 ]** An LLM-based vision and language cobot navigation approach for Human-centric Smart Manufacturing [[doi]](https://doi.org/10.1016/j.jmsy.2024.04.020) `LLM`
  - 概览：将LLM自然语言解析、代码触发和路径规划接入协作机器人导航，并在三维重建的智能制造场景中验证单目标与多目标工具取用任务。

- **[2024/07][ ECCV 2024 - 可微场景语义与双层控制具身导航交互 - DISCO ]** DISCO: Embodied Navigation and Interaction via Differentiable Scene Semantics and Dual-level Control [[arxiv]](https://arxiv.org/abs/2407.14758) [[hjfy]](https://hjfy.top/arxiv/2407.14758) [[github]](https://github.com/AllenXuuu/DISCO) `Hierarchical` `GSM` `ALFRED`
  - 概览：在线学习包含物体语义与可供性的可微场景表示，并以全局规划和局部交互组成的粗到细双层控制完成移动操作，在ALFRED未见场景中即使没有逐步指令也显著提升任务成功率。

- **[2024/07][ ECCV 2024 - BEV感知与大模型导航指令生成 - BEVInstructor ]** Navigation Instruction Generation with BEV Perception and Large Language Models [[arxiv]](https://arxiv.org/abs/2407.15087) [[hjfy]](https://hjfy.top/arxiv/2407.15087) [[github]](https://github.com/FanScy/BEVInstructor) `End-to-end` `MLLM` `BEV`
  - 概览：融合透视与鸟瞰图特征形成包含3D几何和物体语义的MLLM视觉提示，再以实例引导的迭代精炼逐步改进路线描述，在R2R、REVERIE和UrbanWalk上提升导航指令生成质量。

- **[2024/07][ ECCV 2024 - 大模型导航推理VLN - NavGPT-2 ]** NavGPT-2: Unleashing Navigational Reasoning Capability for Large Vision-Language Models [[arxiv]](https://arxiv.org/abs/2407.12366) [[hjfy]](https://hjfy.top/arxiv/2407.12366) [[github]](https://github.com/GengzeZhou/NavGPT-2) `End-to-end` `InstructBLIP` `Matterport3D`
  - 概览：提出将冻结的大型视觉语言模型与拓扑图导航策略网络相结合的VLN框架NavGPT-2，在保留LLM生成语言化导航推理能力的同时，弥合了LLM导航范式与专用VLN模型间的性能差距。

- **[2024/07][ ICARM 2024 - 视觉指令对齐奖励设计 - RewardVLN ]** RewardVLN: An Improved Agent Navigation Based On Visual-Instruction Alignment [[doi]](https://doi.org/10.1109/ICARM62033.2024.10715935) `RL`
  - 概览：针对VLN强化学习中奖励稀疏的问题，基于视觉观测与指令子片段的对齐程度设计改进的密集奖励，引导智能体更忠实地沿指令路径导航，在标准VLN基准上提升导航性能。

- **[2024/07][ AAAI 2025 - 可供性导向零样本连续VLN - AO-Planner ]** Affordances-Oriented Planning using Foundation Models for Continuous Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2407.05890) [[hjfy]](https://hjfy.top/arxiv/2407.05890) [[github]](https://github.com/chen-judge/AO-Planner) [[project]](https://chen-judge.github.io/AO-Planner/) `Zero-Shot` `GPT-4V+SAM`
  - 概览：提出零样本连续VLN规划框架AO-Planner，用SAM分割可行地面生成视觉可供性提示引导LLM选取候选路径点并规划低层路径，再由PathAgent高层推理选径，在R2R-CE上取得零样本SOTA。

- **[2024/07][ arXiv 2024 - 基础模型时代VLN综述 ]** Vision-and-Language Navigation Today and Tomorrow: A Survey in the Era of Foundation Models [[arxiv]](https://arxiv.org/abs/2407.07035) [[hjfy]](https://hjfy.top/arxiv/2407.07035) [[github]](https://github.com/zhangyuejoslin/VLN-Survey-with-Foundation-Models) `Survey`
  - 概览：以语言、智能体与世界三要素组织基础模型时代的VLN研究，系统讨论LLM/VLM在多模态理解、规划、动态环境和跨域泛化中的作用与局限。

- **[2024/07][ arXiv 2024 - 有向保真轨迹规划 - PRET ]** PRET: Planning with Directed Fidelity Trajectory for Vision and Language Navigation [[arxiv]](https://arxiv.org/abs/2407.11487) [[hjfy]](https://hjfy.top/arxiv/2407.11487) `Graph Planning`
  - 概览：以有向图边特征序列表示导航路径，通过指令与有向保真轨迹的全局对齐选择候选节点，在保留方向性和全局决策范围的同时降低计算开销。

- **[2024/07][ arXiv 2024 - VLM地形穿越机器人系统 - SARO ]** SARO: Space-Aware Robot System for Terrain Crossing via Vision-Language Model [[arxiv]](https://arxiv.org/abs/2407.16412) [[hjfy]](https://hjfy.top/arxiv/2407.16412) `VLM`
  - 概览：提出SARO，以VLM高层推理分解地形穿越任务，闭环执行子任务，并用概率退火选择强化学习策略完成低层控制，面向多种室内外三维地形验证零样本泛化。

- **[2024/07][ arXiv 2024 - 障碍环境鲁棒VLN - ObVLN ]** Navigating Beyond Instructions: Vision-and-Language Navigation in Obstructed Environments [[arxiv]](https://arxiv.org/abs/2407.21452) [[hjfy]](https://hjfy.top/arxiv/2407.21452) `Robust VLN`
  - 概览：构建含指令与现实不匹配障碍的R2R-UNO数据集，并提出结合课程训练和虚拟图更新的ObVLN，使智能体能在路径受阻时调整导航而非机械复现原指令。

- **[2024/06][ arXiv 2024 - 元能力引导交互式链式蒸馏VLN - MAGIC ]** MAGIC: Meta-Ability Guided Interactive Chain-of-Distillation for Effective-and-Efficient Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2406.17960) [[hjfy]](https://hjfy.top/arxiv/2406.17960) [[github]](https://github.com/CrystalSixone/VLN-MAGIC) `End-to-end` `Distillation` `Matterport3D`
  - 概览：提出元能力知识蒸馏与教师—学生交互式链式蒸馏，通过能力级和样本级动态加权实现多轮协同进化；仅教师约5%参数的MAGIC-S即可取得强R2R导航性能并满足实时部署。

- **[2024/06][ CoRL 2024 - 零样本通用指令导航系统 - InstructNav ]** InstructNav: Zero-shot System for Generic Instruction Navigation in Unexplored Environment [[arxiv]](https://arxiv.org/abs/2406.04882) [[hjfy]](https://hjfy.top/arxiv/2406.04882) [[github]](https://github.com/LYX0501/InstructNav) [[project]](https://sites.google.com/view/instructnav) `Zero-Shot` `GPT-4V` `Habitat`
  - 概览：提出无需任何导航训练与预建地图的通用指令导航系统，以动态导航思维链DCoN统一多类指令的规划过程，并用多源价值地图将语言规划转化为可执行轨迹，首次零样本完成R2R-CE任务。

- **[2024/06][ CVPR 2024 - 零样本语义音视频导航LLM智能体 - RILA ]** RILA: Reflective and Imaginative Language Agent for Zero-Shot Semantic Audio-Visual Navigation [[cvf]](https://openaccess.thecvf.com/content/CVPR2024/html/Yang_RILA_Reflective_and_Imaginative_Language_Agent_for_Zero-Shot_Semantic_Audio-Visual_CVPR_2024_paper.html) `Zero-Shot` `SoundSpaces`
  - 概览：提出反思与想象语言智能体RILA，用多模态模型将感知转为文本后由LLM规划器主动探索并自适应剔除不准确的感知描述，辅以LLM助手构建房间布局，实现零样本语义音视频导航。

- **[2024/06][ NeurIPS 2024 - 人类感知动态环境VLN基准 - HA-VLN ]** Human-Aware Vision-and-Language Navigation: Bridging Simulation to Reality with Dynamic Human Interactions [[arxiv]](https://arxiv.org/abs/2406.19236) [[hjfy]](https://hjfy.top/arxiv/2406.19236) [[github]](https://github.com/lpercc/HA3D_simulator) [[project]](https://ha-vln-project.vercel.app/) `Benchmark` `HA3D`
  - 概览：提出人类感知VLN任务HA-VLN，构建融合动态人类活动的HA3D模拟器与HA-R2R数据集，并给出VLN-CM与VLN-DT两种智能体基线，推动VLN从静态仿真走向含人动态真实场景。

- **[2024/06][ RO-MAN 2024 - 交互式指令纠错VLN - I2EDL ]** I2EDL: Interactive Instruction Error Detection and Localization [[arxiv]](https://arxiv.org/abs/2406.05080) [[hjfy]](https://hjfy.top/arxiv/2406.05080) `Agentic` `Habitat`
  - 概览：提出交互式VLN任务IVLN-CE与智能体I2EDL，导航中检测到指令错误时才触发用户交互并将错误精确定位到指令片段以请求更正，同时设计交互次数加权成功率(SIN)新指标。

- **[2024/06][ CoRL 2024 - 3D特征场VLN模拟到现实迁移 - 3DFF ]** Sim-to-Real Transfer via 3D Feature Fields for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2406.09798) [[hjfy]](https://hjfy.top/arxiv/2406.09798) [[github]](https://github.com/MrZihan/Sim2Real-VLN-3DFF) `GSM` `CLIP` `Habitat`
  - 概览：提出基于语义可通行地图与3D特征场的模拟到现实迁移方案，赋予单目机器人全景可通行性感知与全景语义理解，将高性能全景VLN模型平滑部署到真实单目机器人。

- **[2024/06][ arXiv 2024 - 通用零样本具身导航 - Why Only Text ]** Why Only Text: Empowering Vision-and-Language Navigation with Multi-modal Prompts [[arxiv]](https://arxiv.org/abs/2406.02208) [[hjfy]](https://hjfy.top/arxiv/2406.02208) [[github]](https://github.com/honghd16/VLN-MP) `Zero-Shot`
  - 概览：提出视觉语言导航多模态提示任务VLN-MP，在文本指令中加入精确或相似的地标图像；配套免训练提示转换流程、R2R等四套多模态数据及可接入现有VLN模型的图像提示融合模块。

- **[2024/06][ arXiv 2024 - 通用具身导航基准 ]** Human-centered In-building Embodied Delivery Benchmark [[arxiv]](https://arxiv.org/abs/2406.17898) [[hjfy]](https://hjfy.top/arxiv/2406.17898) [[project]](https://prsorg.github.io/) [[github]](https://github.com/PRS-Organization/prs-delivery) `Benchmark` `Hierarchical`
  - 概览：构建以极地科考站为原型的多层楼宇配送仿真环境，包含自主角色、可移动抓取机器人和交互物品，并发布13K条服务指令数据；同时提供由多模态大模型完成指令解析、目标搜索与动作执行的基线。

- **[2024/05][ TPAMI 2024 - 大模型可校正地标发现VLN - CONSOLE ]** Correctable Landmark Discovery via Large Models for Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2405.18721) [[hjfy]](https://hjfy.top/arxiv/2405.18721) [[github]](https://github.com/expectorlin/CONSOLE) `End-to-end` `ChatGPT+CLIP`
  - 概览：将VLN重构为可校正地标发现问题，利用ChatGPT生成地标共现常识先验并通过可学习共现打分模块依据实际观测动态校正，缓解大模型先验与真实场景不一致的问题。

- **[2024/05][ TNNLS 2024 - 分层强化学习内在子目标发现 - DISH ]** Discovering Intrinsic Subgoals for Vision-and-Language Navigation via Hierarchical Reinforcement Learning [[doi]](https://doi.org/10.1109/tnnls.2024.3398300) `Hierarchical`
  - 概览：提出DISH方法，通过分层强化学习在潜在空间自动发现内在子目标，高层策略生成子目标、低层策略据此执行动作，无需昂贵的子目标标注即可提升VLN智能体的跨环境泛化能力。

- **[2024/04][ CVPR 2024 - 神经辐射前瞻探索连续VLN - HNR ]** Lookahead Exploration with Neural Radiance Representation for Continuous Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2404.01943) [[hjfy]](https://hjfy.top/arxiv/2404.01943) [[github]](https://github.com/MrZihan/HNR-VLN) `World Model` `Habitat`
  - 概览：提出分层神经辐射表示模型HNR，无需真实移动即可预测候选位置未来环境的多层级语义特征，支持前瞻式并行评估多条候选路径，显著提升连续环境VLN性能。

- **[2024/04][ CVPR 2024 - 因果学习去偏VLN - GOAT ]** Vision-and-Language Navigation via Causal Learning [[arxiv]](https://arxiv.org/abs/2404.10241) [[hjfy]](https://hjfy.top/arxiv/2404.10241) [[github]](https://github.com/CrystalSixone/VLN-GOAT) `End-to-end` `Transformer` `Matterport3D`
  - 概览：提出基于因果学习的统一VLN框架GOAT，通过后门与前门因果干预消除视觉与语言中的数据集偏差混杂因子，在R2R、REVERIE等多个基准上显著提升未见环境泛化能力。

- **[2024/03][ CVPR 2024 - 开放词表检测与全知图迭代VLN - OVER-NAV ]** OVER-NAV: Elevating Iterative Vision-and-Language Navigation with Open-Vocabulary Detection and StructurEd Representation [[arxiv]](https://arxiv.org/abs/2403.17334) [[hjfy]](https://hjfy.top/arxiv/2403.17334) `GSM` `HAMT/CMA`
  - 概览：提出OVER-NAV框架，结合LLM与开放词表检测器蒸馏多模态关键对应信息并构建全知图(Omnigraph)结构化表示，无需额外标注即可显著提升迭代视觉语言导航性能。

- **[2024/03][ CVPR 2024 - 体素化3D环境表示VLN - VER ]** Volumetric Environment Representation for Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2403.14158) [[hjfy]](https://hjfy.top/arxiv/2403.14158) [[github]](https://github.com/DefaultRui/VLN-VER) `End-to-end` `Transformer`
  - 概览：提出体素化环境表示VER，经2D-3D采样将多视角特征聚合到统一3D体素空间，并以3D占据、房间布局与目标框多任务学习增强场景理解，在R2R、REVERIE等基准取得SOTA。

- **[2024/03][ TPAMI 2025 - 解耦推理链LLM视觉语言导航 - NavCoT ]** NavCoT: Boosting LLM-Based Vision-and-Language Navigation via Learning Disentangled Reasoning [[arxiv]](https://arxiv.org/abs/2403.07376) [[hjfy]](https://hjfy.top/arxiv/2403.07376) [[github]](https://github.com/expectorlin/NavCoT) `End-to-end` `LLaMA2-7B`
  - 概览：提出导航思维链NavCoT，通过参数高效域内训练让LLM依次想象下一步观测、选择匹配候选并决策动作的解耦推理，R2R上较GPT-4方法相对提升约7%。

- **[2024/03][ arXiv 2024 - 持续视觉语言导航基准 - CVLN ]** Continual Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2403.15049) [[hjfy]](https://hjfy.top/arxiv/2403.15049) `Benchmark`
  - 概览：提出持续视觉语言导航范式CVLN与指令跟随、对话引导两类基准，让智能体跨场景域增量学习，并给出困惑度回放(PerpR)与情景自回放(ESR)两个基线以对抗灾难性遗忘。

- **[2024/03][ IROS 2024 - VLN指令错误检测与定位基准 - R2RIE-CE ]** Mind the Error! Detection and Localization of Instruction Errors in Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2403.10700) [[hjfy]](https://hjfy.top/arxiv/2403.10700) `Benchmark` `Transformer` `Habitat`
  - 概览：首次构建含多类人为指令错误的VLN-CE基准数据集，正式定义指令错误检测与定位任务并提出跨模态Transformer基线方法，揭示SOTA VLN方法在错误指令下成功率最多下降25%。

- **[2024/03][ arXiv 2024 - 模型驱动端到端点机器人导航 - NeuPAN ]** NeuPAN: Direct Point Robot Navigation With End-to-End Model-Based Learning [[arxiv]](https://arxiv.org/abs/2403.06828) [[hjfy]](https://hjfy.top/arxiv/2403.06828) `Model-Based`
  - 概览：提出NeuPAN，将原始点云经端到端可微模型直接映射为机器人动作，并把学习动力学嵌入模型预测控制，减少传统感知、规划、控制级联的误差传播。

- **[2024/03][ arXiv 2024 - 高斯溅射视觉导航 - GaussNav ]** GaussNav: Gaussian Splatting for Visual Navigation [[arxiv]](https://arxiv.org/abs/2403.11625) [[hjfy]](https://hjfy.top/arxiv/2403.11625) `3DGS`
  - 概览：提出GaussNav，以三维高斯表示重建并渲染环境视图，将几何一致的场景记忆用于实例图像目标导航，缓解视角差异对目标匹配的影响。

- **[2024/03][ arXiv 2024 - 实例感知视觉语言地图 - IVLMap ]** IVLMap: Instance-Aware Visual Language Grounding for Consumer Robot Navigation [[arxiv]](https://arxiv.org/abs/2403.19336) [[hjfy]](https://hjfy.top/arxiv/2403.19336) [[project]](https://ivlmap.github.io/) `Visual-Language Map`
  - 概览：融合RGB-D重建、开放词汇视觉语言特征与实例分割，构建可按序号和属性区分同类物体的IVLMap，并由LLM将自然语言转换为实例级导航目标。

- **[2024/02][ RSS 2024 - 视频VLM端到端VLN - NaVid ]** NaVid: Video-based VLM Plans the Next Step for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2402.15852) [[hjfy]](https://hjfy.top/arxiv/2402.15852) [[github]](https://github.com/jzhzhang/NaVid-VLN-CE) [[project]](https://pku-epic.github.io/NaVid/) `End-to-end` `Vicuna-7B` `Habitat`
  - 概览：首个仅凭单目RGB视频流即可执行VLN的视频大模型，无需地图、里程计或深度输入即达SOTA导航性能，并显著缩小Sim-to-Real泛化差距。

- **[2024/02][ AAAI 2024 - 驾驶视频增强室外VLN - VLN-Video ]** VLN-Video: Utilizing Driving Videos for Outdoor Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2402.03561) [[hjfy]](https://hjfy.top/arxiv/2402.03561) `End-to-end` `Transformer`
  - 概览：提出VLN-Video方法，利用美国多城市驾驶视频结合模板填充指令生成与图像旋转相似度动作预测器自动构建室外VLN预训练数据，经三个代理任务预训练后在Touchdown基准上任务完成率提升2.1%达到新SOTA。

- **[2024/01][ ACL 2024 - 地图引导GPT提示与自适应路径规划 - MapGPT ]** MapGPT: Map-Guided Prompting with Adaptive Path Planning for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2401.07314) [[hjfy]](https://hjfy.top/arxiv/2401.07314) [[github]](https://github.com/chen-judge/MapGPT) [[project]](https://chen-judge.github.io/MapGPT/) `Zero-Shot` `GPT-4/GPT-4V`
  - 概览：将GPT-4/GPT-4V用作零样本导航智能体，把在线构建的拓扑地图转化为提示以激发全局探索，并通过自适应路径规划机制实现多步路径推理，免训练即取得强导航性能。

- **[2024/01][ arXiv 2024 - Voronoi场景图零样本目标导航 - VoroNav ]** VoroNav: Voronoi-based Zero-shot Object Navigation with Large Language Model [[arxiv]](https://arxiv.org/abs/2401.02695) [[hjfy]](https://hjfy.top/arxiv/2401.02695) `Zero-shot`
  - 概览：以Voronoi结构选择信息丰富的探索航点，并将路径、远景和场景语义组织为LLM提示，在探索收益、路径效率与常识先验之间联合决策零样本目标导航。

- **[2023/12][ CVPR 2024 - 具身导航通用大模型 - NaviLLM ]** Towards Learning a Generalist Model for Embodied Navigation [[arxiv]](https://arxiv.org/abs/2312.02010) [[hjfy]](https://hjfy.top/arxiv/2312.02010) [[github]](https://github.com/LaVi-Lab/NaviLLM) `End-to-end` `Vicuna-7B`
  - 概览：提出首个具身导航通用大模型NaviLLM，通过基于模式的指令(schema-based instructions)将多种具身任务统一为生成式问题，在CVDN、SOON、ScanQA等基准取得SOTA并对未见任务展现零样本泛化能力。

- **[2023/12][ NeurIPS 2023 - 频域增强数据增广VLN - FDA ]** Frequency-enhanced Data Augmentation for Vision-and-Language Navigation [[openreview]](https://openreview.net/pdf?id=eKFrXWb0sT) [[github]](https://github.com/hekj/FDA) `End-to-end` `Matterport3D`
  - 概览：提出频域增强数据增广方法FDA，通过混入其他图像的高频分量扰动训练观测，增强VLN智能体对高频视觉信息的捕捉与泛化能力，在R2R、RxR等多个基准上稳定提升性能。

- **[2023/12][ arXiv 2023 - 通用零样本具身导航 - VLFM ]** VLFM: Vision-Language Frontier Maps for Zero-Shot Semantic Navigation [[arxiv]](https://arxiv.org/abs/2312.03275) [[hjfy]](https://hjfy.top/arxiv/2312.03275) `Zero-Shot` `Sim-to-Real` `Pretraining`
  - 概览：提出零样本语义导航方法VLFM，从深度观测构建占据图和探索边界，以视觉语言模型生成语言落地价值图，并选择最可能通向目标物体的边界执行探索。

- **[2023/11][ RA-L 2024 - VLN-CE碰撞规避 - Safe-VLN ]** Safe-VLN: Collision Avoidance for Vision-and-Language Navigation of Autonomous Robots Operating in Continuous Environments [[arxiv]](https://arxiv.org/abs/2311.02817) [[hjfy]](https://hjfy.top/arxiv/2311.02817) `End-to-end` `Habitat`
  - 概览：针对VLN-CE中长期被忽视的碰撞问题提出Safe-VLN算法，利用模拟2D LiDAR占据掩码约束航点预测器避开障碍区域，并采用碰撞后重选导航策略，在R2R-CE上显著降低碰撞率并提升导航性能。

- **[2023/11][ arXiv 2023 - 通用具身导航综述 ]** Advances in Embodied Navigation Using Large Language Models: A Survey [[arxiv]](https://arxiv.org/abs/2311.00530) [[hjfy]](https://hjfy.top/arxiv/2311.00530) [[github]](https://github.com/Rongtao-Xu/Awesome-LLM-EN) `Survey` `Pretraining` `Transformer`
  - 概览：综述大语言模型在具身导航中的应用，比较代表性模型、方法、导航数据集及其优缺点，并归纳多模态融合、实时推理效率和训练成本等挑战。

- **[2023/10][ RA-L 2025 - 多机器人协同语义导航 - Co-NavGPT ]** Co-NavGPT: Multi-Robot Cooperative Visual Semantic Navigation Using Vision Language Models [[arxiv]](https://arxiv.org/abs/2310.07937) [[hjfy]](https://hjfy.top/arxiv/2310.07937) [[project]](https://sites.google.com/view/co-navgpt2) `Zero-Shot` `Habitat`
  - 概览：提出以视觉语言模型为全局规划器的多机器人协同目标导航框架，将多机子地图融合为统一全局地图并由VLM分配探索前沿，无需任务训练即在HM3D上超越基线并完成四足机器人实机验证。

- **[2023/10][ arXiv 2023 - 通用视觉语言导航 - LangNav ]** LangNav: Language as a Perceptual Representation for Navigation [[arxiv]](https://arxiv.org/abs/2310.07889) [[hjfy]](https://hjfy.top/arxiv/2310.07889) `Pretraining` `Representation`
  - 概览：提出LangNav，把图像描述和物体检测结果转换为离散语言感知表示，再微调语言模型结合当前描述、轨迹历史和指令选取动作，面向少样本和跨仿真环境迁移。

- **[2023/09][ ICRA 2024 - 多专家讨论零样本VLN - DiscussNav ]** Discuss Before Moving: Visual Language Navigation via Multi-expert Discussions [[arxiv]](https://arxiv.org/abs/2309.11382) [[hjfy]](https://hjfy.top/arxiv/2309.11382) [[github]](https://github.com/LYX0501/DiscussNav) [[project]](https://sites.google.com/view/discussnav) `Zero-Shot` `GPT-4`
  - 概览：受专家会诊启发提出零样本VLN智能体DiscussNav，让具备不同专长的大模型充当领域专家，导航体每步移动前主动与专家讨论指令理解、环境感知等关键子任务后再行动。

- **[2023/09][ arXiv 2023 - 场景图驱动动态规划 - SayNav ]** SayNav: Grounding Large Language Models for Dynamic Planning to Navigation in New Environments [[arxiv]](https://arxiv.org/abs/2309.04077) [[hjfy]](https://hjfy.top/arxiv/2309.04077) `Agentic`
  - 概览：提出SayNav，在探索中增量构建三维场景图，并让LLM基于局部子图动态生成多目标高层计划，再由预训练点目标策略执行短程导航。

- **[2023/09][ arXiv 2023 - 通用视觉语言导航 - Find What You Want ]** Find What You Want: Learning Demand-conditioned Object Attribute Space for Demand-driven Navigation [[arxiv]](https://arxiv.org/abs/2309.08138) [[hjfy]](https://hjfy.top/arxiv/2309.08138) [[project]](https://sites.google.com/view/demand-driven-navigation) [[github]](https://github.com/whcpumpkin/Demand-driven-navigation) `Pretraining`
  - 概览：提出需求驱动导航DDN，使智能体按用户需求而非固定物体名称寻找可替代目标；方法从大语言模型提取物体文本属性，并用CLIP对齐视觉属性空间以指导目标搜索。

- **[2023/08][ ICCV 2023 - 实体地标对齐自适应预训练 - GELA ]** Grounded Entity-Landmark Adaptive Pre-training for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2308.12587) [[hjfy]](https://hjfy.top/arxiv/2308.12587) [[github]](https://github.com/CSir1996/VLN-GELA) `End-to-end`
  - 概览：在R2R上构建实体短语与环境地标人工对齐标注的GEL-R2R数据集，提出实体-地标自适应预训练范式显式监督细粒度跨模态对齐，在R2R与CVDN两个下游任务上均达到SOTA。

- **[2023/08][ ICCV 2023 - 鸟瞰图场景图 - BSG ]** Bird's-Eye-View Scene Graph for Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2308.04758) [[hjfy]](https://hjfy.top/arxiv/2308.04758) [[github]](https://github.com/DefaultRui/BEV-Scene-Graph) `GSM`
  - 概览：提出鸟瞰图场景图BSG，在3D检测监督下用多步BEV表示编码室内场景布局与几何线索，结合局部网格级与全局图级决策评分改进动作预测，在REVERIE、R2R、R4R上显著超越现有方法。

- **[2023/08][ ICCV 2023 - 世界模型心智规划VLN-CE - DreamWalker ]** DREAMWALKER: Mental Planning for Continuous Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2308.07498) [[hjfy]](https://hjfy.top/arxiv/2308.07498) [[github]](https://github.com/hanqingwangai/Dreamwalker) `World Model` `Habitat`
  - 概览：提出基于世界模型的连续环境VLN智能体DreamWalker，将连续环境抽象为离散结构化的内部世界表示，在执行动作前于其中模拟并评估候选计划，实现可解释的心智前瞻规划。

- **[2023/07][ ICCV 2023 - 网格记忆地图 - GridMM ]** GridMM: Grid Memory Map for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2307.12907) [[hjfy]](https://hjfy.top/arxiv/2307.12907) [[github]](https://github.com/MrZihan/GridMM) `GSM`
  - 概览：构建自顶向下、自我中心且动态增长的网格记忆地图统一表征已访问环境，并提出指令相关性聚合方法捕捉各网格区域的细粒度视觉线索，在REVERIE、R2R、SOON及R2R-CE上均表现优越。

- **[2023/07][ ICCV 2023 - VLN大规模数据生成 - ScaleVLN ]** Scaling Data Generation in Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2307.15644) [[hjfy]](https://hjfy.top/arxiv/2307.15644) [[github]](https://github.com/wz0919/ScaleVLN) [[cvf]](https://openaccess.thecvf.com/content/ICCV2023/papers/Wang_Scaling_Data_Generation_in_Vision-and-Language_Navigation_ICCV_2023_paper.pdf) `End-to-end` `DUET` `Habitat`
  - 概览：提出VLN大规模数据生成范式ScaleVLN，利用HM3D与Gibson的1200余个逼真环境合成490万条指令-轨迹对用于预训练与微调，使现有智能体性能大幅提升并显著缩小与人类表现的差距。

- **[2023/07][ arXiv 2023 - 细粒度行为干预评测 ]** Behavioral Analysis of Vision-and-Language Navigation Agents [[arxiv]](https://arxiv.org/abs/2307.10790) [[hjfy]](https://hjfy.top/arxiv/2307.10790) `Benchmark`
  - 概览：通过生成针对停止、转向、目标物体和房间等技能的语言干预，度量HAMT动作预测的变化，从而诊断VLN智能体的细粒度能力、偏差及其与整体任务性能的关系。

- **[2023/06][ AAAI 2024 - 对话式音视频具身导航 - CAVEN ]** CAVEN: An Embodied Conversational Agent for Efficient Audio-Visual Navigation in Noisy Environments [[arxiv]](https://arxiv.org/abs/2306.04047) [[hjfy]](https://hjfy.top/arxiv/2306.04047) [[aaai]](https://ojs.aaai.org/index.php/AAAI/article/view/28167) `RL` `SoundSpaces`
  - 概览：提出对话式音视频具身导航框架CAVEN，将任务建模为预算感知的部分可观测半马尔可夫决策过程，使智能体能与Oracle进行双向自然语言对话获取指引，显著提升嘈杂环境下音频目标导航成功率。

- **[2023/06][ ACL Findings 2024 - 自我修正规划零样本VLN - CorNav ]** CorNav: Autonomous Agent with Self-Corrected Planning for Zero-Shot Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2306.10322) [[hjfy]](https://hjfy.top/arxiv/2306.10322) [[acl]](https://aclanthology.org/2024.findings-acl.745.pdf) `Zero-Shot` `UE5`
  - 概览：提出零样本VLN框架CorNav，以LLM决策并结合环境反馈修正后续规划与动作，辅以多领域专家解析指令与理解场景，并基于UE5构建逼真仿真器与零样本多任务基准NavBench。

- **[2023/06][ CVPR 2023 - 自适应分区感知分层规划 - AZHP ]** Adaptive Zone-aware Hierarchical Planner for Vision-Language Navigation [[cvf]](https://openaccess.thecvf.com/content/CVPR2023/papers/Gao_Adaptive_Zone-Aware_Hierarchical_Planner_for_Vision-Language_Navigation_CVPR_2023_paper.pdf) [[github]](https://github.com/chengaopro/AZHP) `Hierarchical`
  - 概览：提出自适应分区感知分层规划器AZHP，通过场景自适应分区划分与目标导向分区选择设定子目标并分层执行，结合分层强化学习与课程学习，在REVERIE、SOON、R2R上取得SOTA。

- **[2023/05][ AAAI 2024 - LLM显式推理VLN智能体 - NavGPT ]** NavGPT: Explicit Reasoning in Vision-and-Language Navigation with Large Language Models [[arxiv]](https://arxiv.org/abs/2305.16986) [[hjfy]](https://hjfy.top/arxiv/2305.16986) [[github]](https://github.com/GengzeZhou/NavGPT) `Zero-Shot` `GPT-4`
  - 概览：提出基于LLM的零样本VLN智能体NavGPT，在每步导航中显式进行指令分解、地标识别、进度追踪与计划调整等推理，揭示了GPT-4零样本执行导航任务的潜力与可解释性。

- **[2023/05][ NeurIPS 2023 - 文本条件全景环境生成 - PanoGen ]** PanoGen: Text-Conditioned Panoramic Environment Generation for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2305.19195) [[hjfy]](https://hjfy.top/arxiv/2305.19195) [[github]](https://github.com/jialuli-luka/PanoGen) [[project]](https://pano-gen.github.io/) `Diffusion` `Stable Diffusion`
  - 概览：利用文本条件扩散模型与递归外绘(outpainting)生成无限多样的全景导航环境，缓解VLN训练环境稀缺问题，在R2R、R4R、CVDN的预训练与微调中均显著提升导航性能。

- **[2023/05][ arXiv 2023 - 通用视觉语言导航 - GeoVLN ]** GeoVLN: Learning Geometry-Enhanced Visual Representation with Slot Attention for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2305.17102) [[hjfy]](https://hjfy.top/arxiv/2305.17102) `VLN` `Transformer`
  - 概览：提出GeoVLN，以深度图和法向图补充RGB观测，利用局部槽注意力与CLIP生成几何增强表示，再通过多路注意力对齐指令短语和候选视图。

- **[2023/05][ 软件学报 2025 - 物体目标导航综述 ]** Survey on Object Goal Navigation for Embodied AI [[doi]](https://doi.org/10.13328/j.cnki.jos.007250) `Survey`
  - 概览：从任务类型、模型结构与技术演进三条主线系统梳理物体目标导航，总结数据集、评价指标和训练范式，并分析视觉语言匹配、探索、记忆与避障等关键挑战。

- **[2023/04][ TPAMI 2024 - 演化拓扑规划连续环境VLN - ETPNav ]** ETPNav: Evolving Topological Planning for Vision-Language Navigation in Continuous Environments [[arxiv]](https://arxiv.org/abs/2304.03047) [[hjfy]](https://hjfy.top/arxiv/2304.03047) [[github]](https://github.com/MarSaKi/ETPNav) `Hierarchical` `Transformer` `Habitat`
  - 概览：提出演化拓扑规划框架，在线自组织拓扑地图抽象连续环境，将VLN分解为高层跨模态长程规划与底层避障控制，在R2R-CE、RxR-CE等基准上大幅刷新SOTA。

- **[2023/04][ arXiv 2023 - 通用视觉语言导航 - Vision-and-Language ]** Improving Vision-and-Language Navigation by Generating Future-View Image Semantics [[arxiv]](https://arxiv.org/abs/2304.04907) [[hjfy]](https://hjfy.top/arxiv/2304.04907) `Pretraining`
  - 概览：提出VLN-SIG未来视图语义生成方法，通过全景遮蔽、轨迹遮蔽和动作条件图像生成三项预训练任务学习预测下一视图，并在导航微调时加入语义一致性损失。

- **[2023/03][ Applied Intelligence 2025 - 多级注意力子指令连续VLN - MLANet ]** MLANet: Multi-Level Attention Network with Sub-instruction for Continuous Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2303.01396) [[hjfy]](https://hjfy.top/arxiv/2303.01396) [[github]](https://github.com/RavenKiller/MLANet) [[doi]](https://doi.org/10.1007/s10489-025-06544-9) `End-to-end` `Habitat`
  - 概览：面向连续环境VLN提出多级注意力网络，配合无需标注、提速28倍的快速子指令算法FSA，动态融合高低层语言语义与视觉特征以增强复杂指令理解与实时导航。

- **[2023/03][ CVPR 2023 - 语言双向导航智能体 - LANA ]** Lana: A Language-Capable Navigator for Instruction Following and Generation [[arxiv]](https://arxiv.org/abs/2303.08409) [[hjfy]](https://hjfy.top/arxiv/2303.08409) [[github]](https://github.com/wxh1996/LANA-VLN) `End-to-end` `Transformer` `Matterport3D`
  - 概览：提出同时具备指令跟随与路径描述生成能力的语言双向导航智能体LANA，单一模型联合学习两项任务即可媲美单任务模型，并使智能体行为可通过自然语言自我解释。

- **[2023/03][ CVPR 2023 - 知识增强推理VLN - KERM ]** KERM: Knowledge Enhanced Reasoning for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2303.15796) [[hjfy]](https://hjfy.top/arxiv/2303.15796) [[github]](https://github.com/xiangyangli-cn/KERM) `End-to-end` `DUET` `Matterport3D`
  - 概览：提出知识增强推理模型KERM，为导航视图检索知识图谱事实，经净化、事实感知交互与指令引导聚合模块融合视觉、历史与知识特征，在REVERIE、R2R和SOON上均获提升。

- **[2023/03][ arXiv 2023 - 情景场景记忆导航 - ESceme ]** ESceme: Vision-and-Language Navigation with Episodic Scene Memory [[arxiv]](https://arxiv.org/abs/2303.01032) [[hjfy]](https://hjfy.top/arxiv/2303.01032) `Memory`
  - 概览：提出情景场景记忆ESceme，将历史访问场景压缩为可检索记忆，在导航决策中补充长期环境上下文，以兼顾未见场景泛化与推理效率。

- **[2023/02][ ACL 2023 - 指令翻译器VLN - VLN-Trans ]** VLN-Trans: Translator for the Vision and Language Navigation Agent [[arxiv]](https://arxiv.org/abs/2302.09230) [[hjfy]](https://hjfy.top/arxiv/2302.09230) [[github]](https://github.com/HLR/VLN-trans) `End-to-end` `Matterport3D`
  - 概览：为导航智能体设计"翻译器"模块，将复杂指令转换为聚焦可见地标与可执行动作的易读子指令表示，并构建合成子指令数据集与三项翻译任务，提升R2R等基准上的指令跟随性能。

- **[2023/01][ arXiv 2023 - 通用零样本具身导航 - ESC ]** ESC: Exploration with Soft Commonsense Constraints for Zero-shot Object Navigation [[arxiv]](https://arxiv.org/abs/2301.13166) [[hjfy]](https://hjfy.top/arxiv/2301.13166) `Zero-Shot` `Pretraining`
  - 概览：提出零样本目标导航方法ESC，使用视觉语言模型进行开放词汇目标定位、用语言模型推断房间与物体常识，并将常识转化为软逻辑约束指导探索动作。

- **[2022/12][ arXiv 2022 - 通用视觉语言导航 - BEVBert ]** BEVBert: Multimodal Map Pre-training for Language-guided Navigation [[arxiv]](https://arxiv.org/abs/2212.04385) [[hjfy]](https://hjfy.top/arxiv/2212.04385) `Pretraining`
  - 概览：提出BEVBert地图预训练范式，以局部度量地图聚合并去重观测、以全局拓扑图建模长程依赖，再学习空间感知的多模态地图表示用于语言引导导航。

- **[2022/11][ arXiv 2022 - CLIP零样本视觉语言导航 - CLIP-Nav ]** CLIP-Nav: Using CLIP for Zero-Shot Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2211.16649) [[hjfy]](https://hjfy.top/arxiv/2211.16649) `Zero-Shot` `CLIP`
  - 概览：探索CLIP在零样本视觉语言导航中的语言接地能力，用自然语言指代表达配合CLIP打分逐步引导智能体决策，在REVERIE上超越监督基线并展现更强跨环境泛化。

- **[2022/11][ NAACL 2024 - 联邦具身导航后门攻防 - NAW/PBA ]** Navigation as Attackers Wish? Towards Building Robust Embodied Agents under Federated Learning [[arxiv]](https://arxiv.org/abs/2211.14769) [[hjfy]](https://hjfy.top/arxiv/2211.14769) [[project]](https://styleszhang.github.io/pba/) [[acl]](https://aclanthology.org/2024.naacl-long.57/) `RL` `Security` `Matterport3D`
  - 概览：针对联邦VLN提出通过污染客户端本地轨迹植入后门的Navigation as Wish攻击，并以视觉—语言对齐差异识别恶意客户端的Prompt-Based Aggregation防御，在保护场景隐私的同时增强聚合鲁棒性。

- **[2022/10][ NeurIPS 2022 - 弱监督多粒度地图学习 - WS-MGMap ]** Weakly-Supervised Multi-Granularity Map Learning for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2210.07506) [[hjfy]](https://hjfy.top/arxiv/2210.07506) [[github]](https://github.com/PeihaoChen/WS-MGMap) `GSM` `Habitat`
  - 概览：提出弱监督多粒度地图学习框架WS-MGMap，融合物体细粒度细节与语义区域信息构建导航地图，并借助弱监督物体定位辅助任务提升连续环境VLN成功率。

- **[2022/10][ NeurIPS 2022 - 音频视觉语言具身导航 - AVLEN ]** AVLEN: Audio-Visual-Language Embodied Navigation in 3D Environments [[arxiv]](https://arxiv.org/abs/2210.07940) [[hjfy]](https://hjfy.top/arxiv/2210.07940) [[github]](https://github.com/merlresearch/avlen) `Hierarchical` `SoundSpaces`
  - 概览：提出音频-视觉-语言具身导航框架AVLEN，通过分层强化学习让智能体在追踪声源目标的同时适时向人类请求语言指令，提升3D环境中音频目标导航的鲁棒性。

- **[2022/10][ CVPR 2023 - 合成指令规模化模仿学习 - MARVAL ]** A New Path: Scaling Vision-and-Language Navigation with Synthetic Instructions and Imitation Learning [[arxiv]](https://arxiv.org/abs/2210.03112) [[hjfy]](https://hjfy.top/arxiv/2210.03112) [[github]](https://github.com/google-research-datasets/RxR) `End-to-end` `Transformer`
  - 概览：用Marky指令生成器在500余栋新环境中自动构建420万条合成指令-轨迹对，证明纯模仿学习训练的Transformer导航智能体可超越依赖强化学习的方法，大幅刷新RxR基准纪录。

- **[2022/10][ CVPR 2023 - 持久环境迭代式VLN基准 - IVLN ]** Iterative Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2210.03087) [[hjfy]](https://hjfy.top/arxiv/2210.03087) [[github]](https://github.com/Bill1235813/IVLN) [[project]](https://jacobkrantz.github.io/ivln) `Benchmark` `Habitat`
  - 概览：提出在持久环境中跨回合保持记忆的迭代式VLN评测范式，构建覆盖80个室内场景、约400条游览路线的离散与连续版Iterative R2R基准，凸显建图对长期导航的价值。

- **[2022/08][ ECCV 2022 - 无标注3D环境自动构建VLN数据 - HM3D-AutoVLN ]** Learning from Unlabeled 3D Environments for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2208.11781) [[hjfy]](https://hjfy.top/arxiv/2208.11781) [[project]](https://cshizhe.github.io/projects/hm3d_autovln.html) `End-to-end` `HM3D`
  - 概览：利用2D-3D伪标注与跨视角一致性从900栋无标注HM3D建筑中自动构建大规模VLN数据集HM3D-AutoVLN，显著提升导航模型在未见环境中的泛化性能。

- **[2022/06][ NeurIPS 2022 - 多模态目标嵌入零样本物体导航 - ZSON ]** ZSON: Zero-Shot Object-Goal Navigation using Multimodal Goal Embeddings [[arxiv]](https://arxiv.org/abs/2206.12403) [[hjfy]](https://hjfy.top/arxiv/2206.12403) [[github]](https://github.com/gunagg/zson) `Zero-Shot` `CLIP` `Habitat`
  - 概览：将图像目标编码进CLIP多模态语义嵌入空间，在无标注3D环境中大规模训练语义目标导航智能体，实现按自然语言指令零样本寻找任意物体的开放世界ObjectNav。

- **[2022/05][ ACL SRW 2022 - 显式物体关系对齐 - EXOR ]** Explicit Object Relation Alignment for Vision and Language Navigation [[acl]](https://aclanthology.org/2022.acl-srw.24/) `End-to-end`
  - 概览：提出显式物体关系对齐智能体EXOR，将指令中的地标及其与智能体间的空间关系显式对齐到视觉模态，在R2R上大幅超越基线并展现可解释的空间推理能力。

- **[2022/04][ CVPR 2022 - 强化结构化状态演化 - SEvol ]** Reinforced Structured State-Evolution for Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2204.09280) [[hjfy]](https://hjfy.top/arxiv/2204.09280) `RL`
  - 概览：提出结构化状态演化模型SEvol，以图结构取代向量状态保留环境布局线索，结合强化布局线索挖掘器(RLM)与结构化演化模块(SEM)，在R2R、R4R上为多种VLN模型带来大幅提升。

- **[2022/04][ arXiv 2022 - 通用视觉语言导航 - Sim-2-Sim ]** Sim-2-Sim Transfer for Vision-and-Language Navigation in Continuous Environments [[arxiv]](https://arxiv.org/abs/2204.09667) [[hjfy]](https://hjfy.top/arxiv/2204.09667) `VLN`
  - 概览：研究从拓扑式VLN模拟器向连续VLN-CE环境的sim-to-sim迁移，将已训练智能体接入低层控制，并通过分解两类环境差异定位连续导航中的性能损失来源。

- **[2022/03][ CVPR 2022 - 跨模态语义地图学习连续环境导航 - CM2 ]** Cross-modal Map Learning for Vision and Language Navigation [[arxiv]](https://arxiv.org/abs/2203.05137) [[hjfy]](https://hjfy.top/arxiv/2203.05137) [[github]](https://github.com/ggeorgak11/CM2) [[project]](https://ggeorgak11.github.io/CM2-project/) `GSM` `Habitat`
  - 概览：提出跨模态地图学习框架CM2，以指令为条件预测自我中心语义地图中视野外的区域并回归路径点序列，实现连续环境下的语言引导导航。

- **[2022/03][ CVPR 2022 - 环境编辑数据增广 - EnvEdit ]** EnvEdit: Environment Editing for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2203.15685) [[hjfy]](https://hjfy.top/arxiv/2203.15685) [[github]](https://github.com/jialuli-luka/EnvEdit) `End-to-end` `Matterport3D`
  - 概览：提出环境编辑数据增广方法EnvEdit，通过编辑现有环境的风格、物体外观与类别合成新训练环境，提升智能体对未见环境的泛化能力，在R2R与多语言RxR上取得SOTA。

- **[2022/03][ arXiv 2022 - 通用视觉语言导航 - Vision-and-Language ]** Bridging the Gap Between Learning in Discrete and Continuous Environments for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2203.02764) [[hjfy]](https://hjfy.top/arxiv/2203.02764) `IL`
  - 概览：提出候选航点预测器，把离散VLN智能体的高层动作映射到连续环境可达航点，并通过细化Matterport3D连接图和航点增强缩小离散训练与连续控制之间的差距。

- **[2022/03][ arXiv 2022 - 通用零样本具身导航 - CoWs on Pasture ]** CoWs on Pasture: Baselines and Benchmarks for Language-Driven Zero-Shot Object Navigation [[arxiv]](https://arxiv.org/abs/2203.10421) [[hjfy]](https://hjfy.top/arxiv/2203.10421) `Zero-Shot`
  - 概览：提出无需微调的CLIP on Wheels零样本目标导航框架，并构建PASTURE基准，覆盖罕见物体、属性描述和遮挡目标，在三个环境的九万余回合中比较21种基线。

- **[2022/02][ CVPR 2022 - 双尺度图Transformer拓扑图导航 - DUET ]** Think Global, Act Local: Dual-scale Graph Transformer for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2202.11742) [[hjfy]](https://hjfy.top/arxiv/2202.11742) [[github]](https://github.com/cshizhe/VLN-DUET) `GSM` `Transformer` `Matterport3D`
  - 概览：提出双尺度图Transformer DUET，在线构建拓扑地图并将粗粒度全局规划与细粒度局部决策联合编码，显著提升REVERIE、SOON等目标导向VLN基准性能。

- **[2021/12][ NeurIPS 2021 - 细粒度对齐监督VLN数据集 - Landmark-RxR ]** Landmark-RxR: Solving Vision-and-Language Navigation with Fine-Grained Alignment Supervision [[neurips]](https://papers.nips.cc/paper/2021/hash/0602940f23884f782058efac46f64b0f-Abstract.html) [[github]](https://github.com/hekj/Landmark-RxR) `Benchmark` `Matterport3D`
  - 概览：构建人工标注的细粒度VLN数据集Landmark-RxR，并提出软硬两种形式的焦点导向奖励与重初始化评测机制，从细粒度层面强化视觉语言导航的跨模态对齐监督。

- **[2021/11][ CVPR 2022 - 地标驱动导航指令生成 - Marky-mT5 ]** Less is More: Generating Grounded Navigation Instructions from Landmarks [[arxiv]](https://arxiv.org/abs/2111.12872) [[hjfy]](https://hjfy.top/arxiv/2111.12872) [[github]](https://github.com/google-research-datasets/RxR) `End-to-end` `mT5`
  - 概览：提出两阶段指令生成系统Marky-mT5，先检测全景图中的视觉地标再由多语言多模态编解码器生成接地导航指令，人类跟随其指令的成功率达71%接近人类指令水平，为VLN大规模数据增广铺路。

- **[2021/10][ ICCV 2021 - 自驱动通信视觉对话导航 - SCoA ]** Self-Motivated Communication Agent for Real-World Vision-Dialog Navigation [[cvf]](https://openaccess.thecvf.com/content/ICCV2021/html/Zhu_Self-Motivated_Communication_Agent_for_Real-World_Vision-Dialog_Navigation_ICCV_2021_paper.html) `RL`
  - 概览：提出自驱动通信智能体SCoA，通过"是否提问"与"问什么"双策略在模仿与强化学习联合框架下自适应向人求助，摆脱对预定义提问位置和昂贵对话标注的依赖。

- **[2021/10][ arXiv 2021 - 通用视觉语言导航 - Vision-and-Language ]** History Aware Multimodal Transformer for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2110.13309) [[hjfy]](https://hjfy.top/arxiv/2110.13309) `RL` `Hierarchical` `Memory`
  - 概览：提出历史感知多模态Transformer(HAMT)，用分层视觉Transformer编码单帧、全景空间关系及长时序历史，再联合文本和当前观测预测动作并以强化学习优化策略。

- **[2021/09][ arXiv 2021 - 通用视觉语言导航 - ROS-X-Habitat ]** ROS-X-Habitat: Bridging the ROS Ecosystem with Embodied AI [[arxiv]](https://arxiv.org/abs/2109.07703) [[hjfy]](https://hjfy.top/arxiv/2109.07703) `System`
  - 概览：发布ROS-X-Habitat接口，以ROS标准通信连接Habitat具身智能体、Gazebo及建图规划组件，使同一导航算法能够在Habitat仿真与ROS机器人软件栈之间互操作。

- **[2021/09][ arXiv 2021 - 通用视觉语言导航 - Language-Aligned ]** Language-Aligned Waypoint (LAW) Supervision for Vision-and-Language Navigation in Continuous Environments [[arxiv]](https://arxiv.org/abs/2109.15207) [[hjfy]](https://hjfy.top/arxiv/2109.15207) `VLN`
  - 概览：提出语言对齐航点监督LAW，使偏离参考路径后的纠正动作仍对应尚未完成的子指令，并设计子指令完成度指标衡量连续环境中智能体实际遵循了多少语言内容。

- **[2021/05][ arXiv 2021 - 通用视觉语言导航 - VISITRON ]** VISITRON: Visual Semantics-Aligned Interactively Trained Object-Navigator [[arxiv]](https://arxiv.org/abs/2105.11589) [[hjfy]](https://hjfy.top/arxiv/2105.11589) `IL` `Pretraining` `Transformer`
  - 概览：提出VISITRON多模态Transformer导航器，对齐环境物体语义与对话历史，并用二分类交互头学习何时继续导航、何时向人提问，以适配协作式视觉对话导航。

- **[2021/04][ ICCV 2021 - 物体与房间信息序列BERT导航 - ORIST ]** The Road to Know-Where: An Object-and-Room Informed Sequential BERT for Indoor Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/2104.04167) [[hjfy]](https://hjfy.top/arxiv/2104.04167) [[github]](https://github.com/YuankaiQi/ORIST) `End-to-end` `BERT` `Matterport3D`
  - 概览：提出物体与房间信息感知的序列BERT模型ORIST，将物体级与房间级细粒度视觉信息对齐到指令编码，并设计房间感知奖励函数提升室内导航的指令对齐能力。

- **[2021/03][ CVPR 2021 - 场景导向目标导航基准 - SOON ]** SOON: Scenario Oriented Object Navigation with Graph-based Exploration [[arxiv]](https://arxiv.org/abs/2103.17138) [[hjfy]](https://hjfy.top/arxiv/2103.17138) [[github]](https://github.com/ZhuFengdaaa/SOON) `Benchmark` `Matterport3D`
  - 概览：提出场景导向目标导航新任务SOON与大规模FAO基准，智能体从任意起点依据场景描述由粗到细定位目标物体，并设计图结构探索方法GBE取得最优性能。

- **[2020/12][ CVPR 2021 - 拓扑地图Transformer规划VLN ]** Topological Planning with Transformers for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2012.05292) [[hjfy]](https://hjfy.top/arxiv/2012.05292) `Hierarchical` `Transformer`
  - 概览：受机器人学模块化思想启发，用跨模态注意力Transformer在拓扑地图上预测导航计划，再交由低层控制器鲁棒执行，在自由移动环境中超越端到端方法且计划可解释。

- **[2020/11][ CVPR 2021 - 循环视觉语言BERT导航策略 - RecBERT ]** A Recurrent Vision-and-Language BERT for Navigation [[arxiv]](https://arxiv.org/abs/2011.13922) [[hjfy]](https://hjfy.top/arxiv/2011.13922) [[github]](https://github.com/YicongHong/Recurrent-VLN-BERT) `End-to-end` `BERT` `Matterport3D`
  - 概览：提出循环视觉-语言BERT(RecBERT)，通过引入循环状态单元将多模态BERT转化为可处理部分可观测输入的导航策略网络，刷新R2R与REVERIE基准成绩。

- **[2020/11][ EMNLP 2020 - 通用具身导航基准 - Room-Across-Room ]** Room-Across-Room: Multilingual Vision-and-Language Navigation with Dense Spatiotemporal Grounding [[acl]](https://aclanthology.org/2020.emnlp-main.356/) `Benchmark`
  - 概览：构建多语言视觉语言导航数据集Room-Across-Room(RxR)，提供英语、印地语和泰卢固语路线指令，并以词级时空对齐将语言片段对应到导航轨迹。

- **[2020/05][ ACL 2020 - 分解子指令逐步执行的长程VLN - BabyWalk ]** BabyWalk: Going Farther in Vision-and-Language Navigation by Taking Baby Steps [[arxiv]](https://arxiv.org/abs/2005.04625) [[hjfy]](https://hjfy.top/arxiv/2005.04625) [[github]](https://github.com/Sha-Lab/babywalk) `RL` `LSTM`
  - 概览：提出将长指令分解为短"婴儿步"子任务并借助记忆缓冲逐段执行的方法，先模仿学习后课程强化学习，显著提升VLN智能体在R4R/R6R/R8R长路径任务上的泛化能力。

- **[2020/04][ ECCV 2020 - 连续环境视觉语言导航基准 - VLN-CE ]** Beyond the Nav-Graph: Vision-and-Language Navigation in Continuous Environments [[arxiv]](https://arxiv.org/abs/2004.02857) [[hjfy]](https://hjfy.top/arxiv/2004.02857) [[github]](https://github.com/jacobkrantz/VLN-CE) `Benchmark` `CMA` `Habitat`
  - 概览：将VLN任务从离散导航图拓展到连续3D环境，在Habitat中重建R2R轨迹构建VLN-CE基准，并提供Seq2Seq与跨模态注意力(CMA)基线。

- **[2020/04][ EMNLP 2020 - 子指令感知VLN与FGR2R数据集 ]** Sub-Instruction Aware Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/2004.02707) [[hjfy]](https://hjfy.top/arxiv/2004.02707) [[github]](https://github.com/YicongHong/Fine-Grained-R2R) `End-to-end`
  - 概览：为R2R每条指令标注子指令及对应路径片段构建FGR2R数据集，并提出子指令注意力与移位模块让智能体逐条跟踪执行子指令，在多个SOTA导航智能体上均带来性能提升。

- **[2020/04][ ECCV 2020 - 网络图文预训练视觉语言导航 - VLN-BERT ]** Improving Vision-and-Language Navigation with Image-Text Pairs from the Web [[arxiv]](https://arxiv.org/abs/2004.14973) [[hjfy]](https://hjfy.top/arxiv/2004.14973) [[github]](https://github.com/arjunmajum/vln-bert) `Pre-training` `BERT` `Matterport3D`
  - 概览：提出VLN-BERT视觉语言Transformer兼容性模型，先在网络图文对上预训练视觉语义对齐能力，再在路径-指令数据上微调，使全观测VLN成功率较此前最佳方法提升4个百分点。

- **[2020/03][ arXiv 2020 - 通用视觉语言导航 - Vision-Dialog ]** Vision-Dialog Navigation by Exploring Cross-modal Memory [[arxiv]](https://arxiv.org/abs/2003.06745) [[hjfy]](https://hjfy.top/arxiv/2003.06745) `Memory` `Transformer`
  - 概览：提出跨模态记忆网络CMN，以语言记忆建模当前问答与对话历史的关系，以视觉记忆关联当前视图和既往动作，从而联合利用对话与视觉历史进行导航决策。

- **[2020/02][ CVPR 2020 - VLN预训练通用智能体 - PREVALENT ]** Towards Learning a Generic Agent for Vision-and-Language Navigation via Pre-training [[arxiv]](https://arxiv.org/abs/2002.10638) [[hjfy]](https://hjfy.top/arxiv/2002.10638) [[github]](https://github.com/weituo12321/PREVALENT) `End-to-end` `Transformer`
  - 概览：首个VLN预训练-微调范式，在大规模图文-动作三元组上自监督预训练编码器获得通用视觉语言表征，可即插即用提升R2R、CVDN、HANNA等多个导航任务性能。

- **[2020/02][ TPAMI 2020 - VLN策略学习与适应 - RCM+SIL ]** Vision-Language Navigation Policy Learning and Adaptation [[doi]](https://doi.org/10.1109/tpami.2020.2972281) `RL`
  - 概览：RCM(CVPR 2019)的期刊扩展版，提出强化跨模态匹配方法，以指令-轨迹跨模态匹配为内在奖励进行策略学习，并通过自监督模仿学习(SIL)在未见环境中实现策略自适应。

- **[2019/12][ ECCV 2020 - 音视频具身导航仿真平台 - SoundSpaces ]** SoundSpaces: Audio-Visual Navigation in 3D Environments [[arxiv]](https://arxiv.org/abs/1912.11474) [[hjfy]](https://hjfy.top/arxiv/1912.11474) [[github]](https://github.com/facebookresearch/sound-spaces) `Benchmark` `Habitat`
  - 概览：提出音视频具身导航任务与SoundSpaces声学仿真平台，为Replica和Matterport3D场景渲染逼真双耳空间音频，使智能体联合利用视觉与听觉导航发声目标。

- **[2019/12][ arXiv 2019 - 通用视觉语言导航 - VALAN ]** VALAN: Vision and Language Agent Navigation [[arxiv]](https://arxiv.org/abs/1912.03241) [[hjfy]](https://hjfy.top/arxiv/1912.03241) `RL`
  - 概览：发布VALAN分布式深度强化学习框架，在SEED RL之上提供适配VLN和视觉对话导航的环境、智能体与训练抽象，并以指令条件室内导航展示完整用法。

- **[2019/11][ CVPR 2020 - 自监督辅助推理任务VLN - AuxRN ]** Vision-Language Navigation with Self-Supervised Auxiliary Reasoning Tasks [[arxiv]](https://arxiv.org/abs/1911.07883) [[hjfy]](https://hjfy.top/arxiv/1911.07883) `End-to-end` `Attention/LSTM`
  - 概览：提出AuxRN框架，引入解释历史动作、估计导航进度、预测下一朝向与评估轨迹一致性四个自监督辅助推理任务，挖掘环境语义信息作为额外训练信号，显著提升VLN智能体的泛化导航性能。

- **[2019/09][ EMNLP 2019 - 语言预训练与随机采样鲁棒导航 - PRESS ]** Robust Navigation with Language Pretraining and Stochastic Sampling [[arxiv]](https://arxiv.org/abs/1909.02244) [[hjfy]](https://hjfy.top/arxiv/1909.02244) [[github]](https://github.com/xjli/r2r_vln) `End-to-end` `BERT`
  - 概览：提出PRESS方法，用预训练BERT编码导航指令，并以随机路径采样替代学生强制训练缓解曝光偏差，显著提升VLN在未见环境中的鲁棒性与成功率。

- **[2019/07][ arXiv 2019 - 通用视觉语言导航 - Vision-and-Dialog ]** Vision-and-Dialog Navigation [[arxiv]](https://arxiv.org/abs/1907.04957) [[hjfy]](https://hjfy.top/arxiv/1907.04957) `Planning`
  - 概览：构建Cooperative Vision-and-Dialog Navigation数据集，收录两千余段Navigator与Oracle协作对话，并定义根据目标物体和对话历史在未知住宅中导航的任务。

- **[2019/04][ CVPR 2020 - 远程物体指代表达导航基准 - REVERIE ]** REVERIE: Remote Embodied Visual Referring Expression in Real Indoor Environments [[arxiv]](https://arxiv.org/abs/1904.10151) [[hjfy]](https://hjfy.top/arxiv/1904.10151) [[github]](https://github.com/YuankaiQi/REVERIE) `Benchmark` `Matterport3D`
  - 概览：提出远程具身视觉指代表达任务与基准REVERIE，要求智能体依据简洁高层指令在未见室内环境中导航并定位远处目标物体，并给出交互式导航-指示器基线模型。

- **[2019/04][ NAACL 2019 - 回译与环境Dropout数据增强 - EnvDrop ]** Learning to Navigate Unseen Environments: Back Translation with Environmental Dropout [[arxiv]](https://arxiv.org/abs/1904.04195) [[hjfy]](https://hjfy.top/arxiv/1904.04195) [[github]](https://github.com/airsplay/R2R-EnvDrop) `End-to-end` `Attention/LSTM`
  - 概览：提出"环境Dropout"结合回译的半监督数据增强方案，通过随机丢弃视觉特征模拟未见新环境并自动生成增广指令-路径对，有效缓解VLN智能体在未见环境中的泛化难题。

- **[2019/04][ arXiv 2019 - 通用视觉语言导航 - Habitat ]** Habitat: A Platform for Embodied AI Research [[arxiv]](https://arxiv.org/abs/1904.01201) [[hjfy]](https://hjfy.top/arxiv/1904.01201) `End-to-end`
  - 概览：发布Habitat具身AI平台，由高吞吐量3D模拟器Habitat-Sim和任务训练评测库Habitat-API组成，支持导航、指令跟随与具身问答的可配置大规模实验。

- **[2019/03][ CVPR 2019 - 进度估计辅助回退导航 - Regretful ]** The Regretful Agent: Heuristic-Aided Navigation through Progress Estimation [[arxiv]](https://arxiv.org/abs/1903.01602) [[hjfy]](https://hjfy.top/arxiv/1903.01602) [[github]](https://github.com/chihyaoma/regretful-agent) [[project]](https://chihyaoma.github.io/project/2019/02/25/regretful.html) `End-to-end` `Attention/LSTM`
  - 概览：提出Regretful Agent，以学习到的进度估计器作为启发式信号，引入回退(regret)模块让智能体在导航置信度下降时回溯至先前位置重新决策，显著提升R2R未见环境导航成功率。

- **[2019/03][ CVPR 2019 - 回溯自我修正导航 - FAST ]** Tactical Rewind: Self-Correction via Backtracking in Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/1903.02547) [[hjfy]](https://hjfy.top/arxiv/1903.02547) [[github]](https://github.com/Kelym/FAST) `End-to-end` `Attention/LSTM`
  - 概览：提出FAST导航框架，将VLN建模为对已访问边界节点的评分搜索问题，利用局部与全局信号让智能体在偏离路线时高效回溯并自我修正，兼顾贪心策略的速度与束搜索的准确率。

- **[2019/03][ arXiv 2019 - 通用具身导航基准 - StreetLearn ]** The StreetLearn Environment and Dataset [[arxiv]](https://arxiv.org/abs/1903.01292) [[hjfy]](https://hjfy.top/arxiv/1903.01292) `Benchmark` `RL` `Memory`
  - 概览：发布StreetLearn交互式第一人称导航环境，以Google Street View提供大范围真实街景，并配套目标驱动导航任务、基线智能体和可用于强化学习的数据接口。

- **[2019/01][ ICLR 2019 - 进度估计自监控导航智能体 - Self-Monitoring ]** Self-Monitoring Navigation Agent via Auxiliary Progress Estimation [[arxiv]](https://arxiv.org/abs/1901.03035) [[hjfy]](https://hjfy.top/arxiv/1901.03035) [[github]](https://github.com/chihyaoma/selfmonitoring-agent) `End-to-end` `LSTM`
  - 概览：提出自监控导航智能体，通过视觉-文本共同定位与辅助进度估计器实时监控指令完成进度，显著提升VLN路径对齐与成功率。

- **[2018/11][ CVPR 2019 - 强化跨模态匹配与自监督模仿学习 - RCM ]** Reinforced Cross-Modal Matching and Self-Supervised Imitation Learning for Vision-Language Navigation [[arxiv]](https://arxiv.org/abs/1811.10092) [[hjfy]](https://hjfy.top/arxiv/1811.10092) `RL` `LSTM`
  - 概览：提出强化跨模态匹配(RCM)方法，以循环重构内在奖励强化指令与轨迹的跨模态对齐，并结合自监督模仿学习(SIL)探索未见环境提升泛化。

- **[2018/11][ CVPR 2019 - 街景自然语言导航与空间推理基准 - Touchdown ]** Touchdown: Natural Language Navigation and Spatial Reasoning in Visual Street Environments [[arxiv]](https://arxiv.org/abs/1811.12354) [[hjfy]](https://hjfy.top/arxiv/1811.12354) [[github]](https://github.com/lil-lab/touchdown) `Benchmark` `StreetView`
  - 概览：提出Touchdown任务与数据集，要求智能体在真实街景环境中跟随自然语言指令导航并按空间描述定位隐藏目标，含9,326条指令-演示配对，空间推理表达比既有资源更丰富。

- **[2018/06][ NeurIPS 2018 - 说话者-跟随者数据增广模型 - Speaker-Follower ]** Speaker-Follower Models for Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/1806.02724) [[hjfy]](https://hjfy.top/arxiv/1806.02724) [[github]](https://github.com/ronghanghu/speaker_follower) [[project]](https://ronghanghu.com/speaker_follower/) `End-to-end` `LSTM`
  - 概览：提出说话者-跟随者框架，利用说话者模型合成指令进行数据增广，并在推理阶段以语用推断为候选路径打分重排，大幅提升VLN成功率。

- **[2018/03][ ECCV 2018 - 模型无关与基于模型RL结合的前瞻规划VLN - RPA ]** Look Before You Leap: Bridging Model-Free and Model-Based Reinforcement Learning for Planned-Ahead Vision-and-Language Navigation [[arxiv]](https://arxiv.org/abs/1803.07729) [[hjfy]](https://hjfy.top/arxiv/1803.07729) `RL`
  - 概览：提出RPA框架首次将模型无关与基于模型的强化学习结合用于VLN，通过环境模型预测未来状态与奖励实现前瞻规划，提升R2R未见环境中的导航泛化能力。

- **[2017/11][ CVPR 2018 - VLN任务开山之作与R2R基准 - R2R ]** Vision-and-Language Navigation: Interpreting visually-grounded navigation instructions in real environments [[arxiv]](https://arxiv.org/abs/1711.07280) [[hjfy]](https://hjfy.top/arxiv/1711.07280) [[github]](https://github.com/peteanderson80/Matterport3DSimulator) [[project]](https://bringmeaspoon.org/) `Benchmark` `Matterport3D`
  - 概览：VLN任务开山之作，基于真实拍摄的Matterport3D环境构建仿真器与Room-to-Room(R2R)数据集，正式定义视觉语言导航任务并给出seq2seq基线。

- **[2010/X][ AISTATS 2010 - 模仿学习的高效归约 - SMILe ]** Efficient Reductions for Imitation Learning [[pmlr]](https://proceedings.mlr.press/v9/ross10a.html) `RL`
  - 概览：揭示模仿学习中监督式训练的复合误差随任务时长二次增长的问题，提出前向训练与随机混合迭代学习(SMILe)算法将误差降至近线性，为VLN在线纠错与学生强制训练奠定理论基础。

---

<sub>条目格式与主目录一致（标题行 + 概览行 + 技术标签徽章）。内容以 [MIT License](./LICENSE) 发布 © 2026 20bytes；论文版权归原作者及出版方所有。[← 返回主目录](README.md)</sub>
