# 🚨 A 30B at 57.00 on SWE-Bench Verified, ~86% throughput at 1% packet loss, and one 12-second demo → 59% robot success



**来源：** AI Dev Signals (Marktechpost)  

**日期：** 2026-08-26  

**查看原邮件：** <https://mail.google.com/mail/u/1/#search/subject%3A%22%F0%9F%9A%A8%20A%2030B%20at%2057.00%20on%20SWE-Bench%20Verified%2C%20~86%25%20throughput%20at%201%25%20packet%20loss%2C%20and%20one%2012-second%20demo%20%E2%86%92%2059%25%20robot%20success%22>



---



🚨 A 30B at 57.00 on SWE-Bench Verified, ~86% throughput at 1% packet loss, and one 12-second demo → 59% robot success

> **译文：** 🚨 在 SWE-Bench 验证中，30B 进程得分 57.00，丢包率 1% 时吞吐量约为 86%，完成一次 12
> 秒演示后，机器人成功率达到 59%。

Home

Promotions

Home

Posts

🚨 A 30B at 57.00 on SWE-Bench Verified, ~86% throughput at 1% packet loss, and one 12-second demo → 59% robot success

> **译文：** 🚨 在 SWE-Bench 验证中，30B 进程得分 57.00，丢包率 1% 时吞吐量约为 86%，完成一次 12
> 秒演示后，机器人成功率达到 59%。

🚨 A 30B at 57.00 on SWE-Bench Verified, ~86% throughput at 1% packet loss, and one 12-second demo → 59% robot success

> **译文：** 🚨 在 SWE-Bench 验证中，30B 进程得分 57.00，丢包率 1% 时吞吐量约为 86%，完成一次 12
> 秒演示后，机器人成功率达到 59%。

Granite 4.2 reserves agentic RL for the 8B and 30B. Pipette scores the configuration, not the model. MetaRoCE skips the reorder buffer entirely, and GEN-1.5 adapts in ten gradient steps.

> **译文：** Granite 4.2 将主动强化学习保留给 8B 和 30B 处理器。Pipette 对配置而非模型进行评分。MetaRoCE
> 完全跳过重排序缓冲区，而 GEN-1.5 则在十个梯度步长内进行自适应。

Aug 26, 2026

Together with NVIDIA

AI Dev Signals · August 25, 2026

Open weights. Local agents.

Six releases that remove a unit of cost.

Granite 4.2 reserves agentic RL for the 8B and 30B. Pipette scores the configuration, not the model. MetaRoCE skips the reorder buffer entirely, and GEN-1.5 adapts in ten gradient steps.

> **译文：** Granite 4.2 将主动强化学习保留给 8B 和 30B 处理器。Pipette 对配置而非模型进行评分。MetaRoCE
> 完全跳过重排序缓冲区，而 GEN-1.5 则在十个梯度步长内进行自适应。

Presented by NVIDIA

LTX-2.5

— an open weights world model, NVIDIA-accelerated, generating a 10-second clip in 6.8 seconds on-prem.

> **译文：** — 一个开放权重世界模型，NVIDIA 加速，在本地环境中 6.8 秒内生成 10 秒的视频片段。

Read the launch →

Every release below removes a unit somebody was being charged for. Granite ships open weights instead of an API key. Perplexity runs the whole harness on hardware you own and charges nothing for local steps. GLiNER2.5 makes a forty-word clause cost the same to find as a two-word name. GEN-1.5 turns tens of thousands of gradient steps into ten. Pipette tells you what a configuration actually costs on the device you ship on, and MetaRoCE stops one dropped packet from stranding a cluster. Six layers of the stack. One move.

> **译文：** 以下每个版本都移除了之前需要付费的功能。Granite 提供开放权重，而非 API 密钥。Perplexity
> 可在您拥有的硬件上运行整个框架，并且本地步骤不收费。GLiNER2.5 使查找一个 40 个单词的子句与查找一个 2
> 个单词的名称的成本相同。GEN-1.5 将数万个梯度步骤简化为 10 个。Pipette 会告诉您在所使用的设备上配置的实际成本，而
> MetaRoCE 可防止因丢包而导致集群中断。六层协议栈，一次操作即可完成。

57.00

Granite 30B, SWE-Bench Verified

~86%

MetaRoCE throughput at 1% loss

59%

one demo, zero gradient steps

🔥 The signals

01 · IBM · Open models

IBM Releases Granite 4.2: Bringing Native Reasoning and Agentic RL to Open Enterprise Models

> **译文：** IBM发布Granite 4.2：将原生推理和智能体强化学习引入开放企业模型

An open enterprise model used to mean an instruction-following assistant you were allowed to self-host. Granite 4.2 is built around reasoning instead. Every size emits a chain of thought before it answers, and the chat template exposes a thinking / low-effort / non-thinking switch. The architecture is deliberately boring — dense, decoder-only, no MoE. The training pipeline is the story.

> **译文：** 过去，开放式企业模式指的是允许用户自行托管的指令式助手。而 Granite 4.2
> 则围绕推理机制构建。每个规模的助手在回答问题前都会发出一段思考过程，聊天模板则提供了一个思考/低投入/非思考模式的切换开关。其架构刻意追求简洁——密集、仅包含解码器、不涉及任何应用领域。训练流程才是关键所在。

Three sizes, 3B / 8B / 30B, all Apache 2.0, all pre-trained from scratch on roughly 15 trillion tokens, then post-trained through a multi-stage RL chain. The agentic RL block — SWE, Terminal, Search — runs only on the 8B and 30B, and that one choice explains most of the capability gap across sizes. The 30B reports 57.00 on SWE-Bench Verified and 29.24 on Terminal-Bench 2.1; the 8B, 47.67 and 20.56. IBM also shipped Granite Speech 5.0 Turbo CTC at

> **译文：** 三种规格：3B、8B 和 30B，全部基于 Apache 2.0，均使用约 15
> 万亿个代币进行从零开始的预训练，然后通过多阶段强化学习链进行后训练。智能强化学习模块（软件工程、终端、搜索）仅在 8B 和 30B
> 上运行，这一选择解释了不同规格之间性能差异的大部分原因。30B 在 SWE-Bench Verified 测试中得分为 57.00，在
> Terminal-Bench 2.1 测试中得分为 29.24；8B 的相应得分分别为 47.67 和 20.56。IBM 还发布了
> Granite Speech 5.0 Turbo CTC。

470M parameters with no LLM backbone at all.

Read on Marktechpost →

·

IBM Research blog

·

Hugging Face

·

GitHub

02 · Liquid AI · On-device benchmarks

Liquid AI Open-Sources Pipette: A Reproducible Benchmarking Suite That Measures On-Device Models, Quantization, Runtime and Hardware Together

> **译文：** Liquid AI 开源移液器：一套可复现的基准测试套件，可同时衡量设备端模型、量化、运行时间和硬件性能。

A model card reports quality under server-class, full-precision conditions. Nobody ships that. Pipette changes the unit of measurement from the model to the deployed configuration: model + quantization + runtime + device. Built with Artificial Analysis as an independent methodology validator.

> **译文：** 模型卡可在服务器级、全精度条件下报告质量。目前市面上还没有这样的产品。Pipette 将测量单位从模型转换为部署配置：模型 +
> 量化 + 运行时间 + 设备。它采用人工智能分析作为独立的方法验证器。

The launch dataset covers five performance metrics across more than 1,000 configurations and 30+ models, at context lengths from 256 to 8,192 tokens, verified on a MacBook Pro M5 Max, an iPhone 17 Pro and a Galaxy S26 Ultra. The comparison that makes the case: at

> **译文：** 该发布数据集涵盖了超过 1000 种配置和 30 多个型号的五项性能指标，上下文长度从 256 到 8192 个令牌不等，并在
> MacBook Pro M5 Max、iPhone 17 Pro 和 Galaxy S26 Ultra 上进行了验证。以下对比结果足以说明问题：

Q4_K_M on the Galaxy, Granite-4.0-H-350M keeps 78.4% of its decode throughput out to 4,096 input tokens while Granite-4.0-350M keeps 33.8%. Same parameter count, opposite answer. One caveat worth reading twice: the quality scores come from H100 reference runs matched to on-device performance, not measured on the phone.

> **译文：** 在 Galaxy 设备上，Q4_K_M 测试中，Granite-4.0-H-350M 在处理 4096
> 个输入标记时，解码吞吐量保持率为 78.4%，而 Granite-4.0-350M 则为
> 33.8%。参数数量相同，结果却截然相反。需要特别注意的是：这些质量评分来自与设备性能相匹配的 H100 参考测试，而非在手机上直接测量的结果。

Read on Marktechpost →

·

Technical details

·

Leaderboard

·

GitHub

03 · Perplexity · Agent infrastructure

Perplexity Ships Portable Computer on NVIDIA DGX Spark: Local Harness, OS-Enforced Sandbox, and Zero Per-Token Cost for Local Steps

> **译文：** Perplexity推出基于NVIDIA DGX Spark的便携式计算机：本地部署、操作系统强制沙箱以及本地步骤零令牌成本

Most local AI ships a model and leaves you to build the rest. Portable Computer ships the harness, orchestrator, planner, tool router, sandbox and connectors as one packaged system on a DGX Spark. Every task starts on the device. When a step needs the live web or frontier reasoning, the orchestrator stops, runs a PII classifier over the context, shows you exactly what would leave the machine, and waits.

> **译文：**
> 大多数本地人工智能解决方案只提供模型，其余部分需要用户自行构建。而便携式计算机则将框架、编排器、规划器、工具路由器、沙箱和连接器作为一个打包系统，安装在
> DGX Spark 上。每个任务都在设备上启动。当某个步骤需要实时网络或前沿推理时，编排器会停止运行，对上下文运行 PII
> 分类器，准确地显示哪些内容需要从机器输出，然后等待。

On Perplexity’s own 53-task Local Knowledge Work Bench, Computer with PPLX 27B scored 85.4% against 77.6% for the open-source Pi harness on the identical model. The honest number is Terminal Bench 2.1: 59.6% fully local at effectively zero marginal cost, 73.0% with adviser escalation at roughly $0.415 per rollout, against 82.4% at about $0.65 for Claude Opus 5 alone. Escalation narrows the gap without closing it. The hardware gate is real — a GB10-class box, or an RTX GPU with 24 GB of VRAM, Linux first.

> **译文：** 在 Perplexity 自家的 53 项本地知识工作台测试中，搭载 PPLX 27B 的计算机得分
> 85.4%，而搭载相同型号开源 Pi 外设的计算机得分为 77.6%。更客观的数据来自 Terminal Bench 2.1：完全本地化后得分为
> 59.6%，边际成本几乎为零；如果采用顾问升级，每次部署成本约为 0.415 美元，则得分为 73.0%；相比之下，仅使用 Claude
> Opus 5 的本地化后得分为 82.4%，每次部署成本约为 0.65 美元。升级可以缩小差距，但无法完全消除差距。硬件门槛确实存在——需要一台
> GB10 级别的服务器，或者配备 24GB 显存的 RTX GPU，并且优先考虑 Linux 系统。

Read on Marktechpost →

·

Product page

·

NVIDIA local AI blog

Sponsored · NVIDIA

The video production stack now fits on one desk

LTX-2.5 is an open weights world model for video generation, real-time applications and physical AI, optimized by NVIDIA for local inference on RTX GPUs and DGX Spark. Native multishot generation renders a full sequence as one coherent output, holding a character’s look shot to shot. A custom Gemma 4 language backbone sharpens complex multi-subject prompts, and a new diffusion video decoder cuts artifacts in high-motion scenes. One person at a desk can lock a branded character with a quick LoRA fine-tune. No studio, no cloud, no IP leaving the machine.

> **译文：** LTX-2.5 是一款开放权重世界模型，适用于视频生成、实时应用和物理 AI，由 NVIDIA 针对 RTX GPU 和 DGX
> Spark 上的本地推理进行了优化。原生多镜头生成功能可将完整序列渲染为一个连贯的输出，确保角色在镜头间的视觉效果保持一致。定制的 Gemma
> 4 语言骨架可锐化复杂的多主体提示，而全新的扩散视频解码器则可消除高速运动场景中的伪影。只需一人即可在办公桌前通过 LoRa
> 快速微调锁定品牌角色。无需工作室，无需云端，IP 也不会离开机器。

In LTX’s published image-to-video benchmark, a 10-second clip takes 6.8 seconds on-prem on 2x NVIDIA GB200 and 23.7 seconds through the LTX API, against 52 to 70 seconds for the fastest closed alternatives listed. Weights are on Hugging Face, native in ComfyUI on day one, and free for organizations under $10M in annual recurring revenue. LTX reports more than 33 million downloads across the family.

> **译文：** 在 LTX 公布的图像转视频基准测试中，一段 10 秒的视频片段在本地部署的 2 块 NVIDIA GB200 显卡上耗时
> 6.8 秒，而通过 LTX API 则耗时 23.7 秒，相比之下，其他最快的封闭式替代方案则需要 52 到 70 秒。Hugging Face
> 是 ComfyUI 的原生应用，并且在发布首日即可使用，对于年经常性收入低于 1000 万美元的企业用户免费。LTX
> 报告称，其产品系列的总下载量已超过 3300 万次。

Read the LTX-2.5 launch →

LTX newsroom →

·

Open weights

·

GitHub

·

Docs

04 · Fastino · Information extraction

Fastino Releases GLiNER2.5: A Boundary-Prediction Architecture That Removes Span Enumeration From Information Extraction

> **译文：** Fastino发布GLiNER2.5：一种无需跨度枚举即可进行信息抽取的边界预测架构

Extraction has been a choice between rigid cheap encoders and flexible expensive LLMs. GLiNER2.5 stops enumerating every candidate span against a width grid and predicts where an entity starts and ends instead. Remove the width axis and the ceiling on entity length goes with it: a forty-word indemnification clause now costs the same to locate as a two-word name.

> **译文：** 提取过程一直需要在刚性廉价编码器和灵活昂贵的语言逻辑模型 (LLM) 之间做出选择。GLiNER2.5
> 不再逐个枚举每个候选跨度与宽度网格，而是预测实体的起始和结束位置。移除宽度轴后，实体长度的上限也随之消失：现在定位一个四十字的赔偿条款与定位一个两字名称的成本相同。

Three Apache 2.0 checkpoints at 74M, 194M and 287M, all CPU-runnable through pip install gliner2[local]

> **译文：** 三个 Apache 2.0 检查点，大小分别为 74M、194M 和 287M，均可通过 pip install
> gliner2[local] 在 CPU 上运行。

, shipping with max_len=4096

. Across 16 zero-shot benchmarks the multilingual checkpoint reaches 56.17 overall macro F1 against 56.09 for GLiNER2 — close to flat, with the gain concentrated in XNLI, which jumps to 62.30 from 37.55. Joint entity-relation decoding returns schema-valid graphs by construction, which deletes a post-hoc validation layer. No inference provider hosts the checkpoints, so self-hosting is the deployment path.

> **译文：** 在 16 项零样本基准测试中，多语言检查点总体宏 F1 值达到 56.17，而 GLiNER2 为
> 56.09，两者基本持平，提升主要集中在 XNLI 上，其 F1 值从 37.55 跃升至
> 62.30。联合实体关系解码通过构造返回符合模式的图，从而省去了事后验证层。由于没有推理提供程序托管检查点，因此采用自托管部署方式。

Read on Marktechpost →

·

Technical blog

·

GitHub

·

Hugging Face

05 · Meta · AI networking

Meta AI Introduces MetaRoCE: A Clean-Sheet RDMA Transport Built for AI-Scale Ethernet

> **译文：** Meta AI推出MetaRoCE：专为AI规模以太网打造的全新RDMA传输协议

Standard RoCE assumes the network delivers every frame in order, leans on PFC, and discourages the packet spraying that large multiplane fabrics need. MetaRoCE inverts the assumption. The fabric is treated as lossy; ordering, path selection and recovery move into the NIC. Packets spray across many paths, arrive out of order by design, and write straight to their final memory location — no reorder buffer, no head-of-line blocking.

> **译文：** 标准 RoCE 假设网络按顺序传输每个帧，依赖于 PFC，并且不鼓励大型多平面网络所需的散播数据包。MetaRoCE
> 则颠覆了这一假设。网络被视为有损网络；排序、路径选择和恢复都由网卡 (NIC)
> 负责。数据包会散播到多条路径上，设计上就是乱序到达，并直接写入最终的内存位置——没有重排序缓冲区，也没有队头阻塞。

On a 64-node AMD GPU cluster running RCCL collectives on AMD Pensando NICs, MetaRoCE holds roughly 86% throughput at 1% packet loss and keeps delivering useful bandwidth at 10%, converging rather than collapsing. It asks the switch for two things every switch already has, ECN marking and ECMP, which means it also runs on fabrics you do not control. Not deployable yet: the spec, the compliance suite and

> **译文：** 在运行于 AMD Pensando 网卡上的 64 节点 AMD GPU 集群上，使用 RCCL 聚合，MetaRoCE 在
> 1% 丢包率下可保持约 86% 的吞吐量，并在 10%
> 丢包率下仍能提供有效带宽，且性能稳定而非崩溃。它需要交换机提供两项所有交换机都已具备的功能：ECN 标记和
> ECMP，这意味着它也可以运行在您无法控制的网络结构上。目前尚无法部署：规范、合规性套件和

libsoftmetaroce are expected at the OCP Global Summit in October 2026.

> **译文：** libsoftmetaroce 预计将于 2026 年 10 月参加 OCP 全球峰会。

Read on Marktechpost →

·

Meta Engineering

From our sponsor

Want a frontier world model running on the GPU already in your machine?

> **译文：** 想在机器自带的GPU上运行前沿世界模型吗？

See LTX-2.5 →

One more thing…

Generalist AI · Robot foundation models

Generalist AI Releases GEN-1.5: A Robot Foundation Model That Learns New Tasks From One 3–12 Second Demo

> **译文：** Generalist AI 发布 GEN-1.5：一款机器人基础模型，可通过 3-12 秒演示学习新任务

Teaching a robot a new task has meant collecting data and running tens of thousands of gradient steps. GEN-1.5 takes 3 to 12 seconds of sensorimotor data, dropped into a 30-second context window, and does the task. No gradient updates. No fine-tuning. No task-specific programming. Generalist calls it physical prompting.

> **译文：** 以往教机器人执行新任务需要收集数据并运行数万步梯度迭代。而 GEN-1.5 只需 3 到 12 秒的感知运动数据，将其放入 30
> 秒的上下文窗口中，即可完成任务。无需梯度更新，无需微调，也无需针对特定任务进行编程。通用机器人专家称之为物理提示。

Across 10 diverse manipulation tasks, one-shot in-context prompting averaged 59% success (±10% std. dev.) straight from the pretrained model. Ten gradient steps on five minutes of data per task raised that to 83% (±9%). Those ten steps move the weights on held-out tasks by less than 0.15%, which suggests the fine-tune is reconfiguring knowledge the model already has rather than building new representations.

> **译文：**
> 在10项不同的操作任务中，预训练模型直接进行单次情境提示的平均成功率为59%（标准差±10%）。对每项任务5分钟的数据进行10步梯度调整后，成功率提升至83%（标准差±9%）。这10步调整对保留任务的权重影响小于0.15%，表明微调是对模型已有知识的重新配置，而非构建新的表征。

None of it was designed in: no architectural changes, no meta-learning loop, no auxiliary objectives. It emerged from more than eight months of continuous pretraining, the way one-shot prompting emerged in GPT-3. A demonstration recorded entirely in simulation works as a prompt for the real robot, despite pretraining containing no simulation data. The tasks are short-horizon and the company says so plainly. There are no weights, no API and no pricing page — read this as a signal about scaling, not as a product.

> **译文：** 这一切都不是预先设计好的：没有架构变更，没有元学习循环，也没有辅助目标。它源于超过八个月的持续预训练，就像 GPT-3
> 的单次提示功能一样。一段完全在模拟环境中录制的演示视频可以作为真实机器人的提示，尽管预训练过程中没有包含任何模拟数据。任务是短期的，公司也明确说明了这一点。没有权重，没有
> API，也没有定价页面——这应该被视为一个关于规模化的信号，而不是一个产品。

Read the research post →

Read on Marktechpost →

·

Announcement thread