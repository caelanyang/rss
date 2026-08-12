# Meta's 4-bit 30B in 24 GB of VRAM, NVIDIA's 448 ms full-duplex turns, and an agent runtime that forks 5× faster than Docker

**来源：** AI Dev Signals (Marktechpost)  
**日期：** 2026-08-12  
**查看原邮件：** <https://mail.google.com/mail/u/1/#search/subject%3A%22Meta%27s%204-bit%2030B%20in%2024%20GB%20of%20VRAM%2C%20NVIDIA%27s%20448%20ms%20full-duplex%20turns%2C%20and%20an%20agent%20runtime%20that%20forks%205%C3%97%20faster%20than%20Docker%22>

---

Six releases. Six runtime envelopes. 4 GB, 24 GB, 80 GB, or nothing.

> **译文：** 六个版本。六个运行时容量。4 GB、24 GB、80 GB，或者不提供。

30B quantized to 4-bit and fitted into 24 GB. A 1.78 GiB GGUF under a non-commercial license. 11B of speech-to-speech behind an 80 GB requirement and a research-only tag. And a Git-like trace that forks a live agent process, not just its files.

> **译文：** 30 字节量化为 4 位，并装入 24 GB 空间。一个 1.78 GiB 的 GGUF，采用非商业许可。11 字节的语音转换数据，占用 80 GB 空间，并标记为仅供研究使用。还有一个类似 Git 的跟踪工具，它会派生一个实时代理进程，而不仅仅是它的文件。

No benchmark decided anything this week. VRAM ceilings, license text and deployment targets did. Meta got a 30B under 20 GB with 4-bit weights. webAI shipped a 1.78 GiB checkpoint you may not deploy for revenue. NVIDIA published permissive weights and then tagged them research-only. ByteDance published no weights, no parameter count, and no API. Read the spec line before the eval table.

> **译文：** 本周没有任何基准测试结果能决定任何事情。真正起作用的是显存上限、许可协议文本和部署目标。Meta 的显存容量为 300 亿字节，占用空间不到 20 GB，权重为 4 位。webAI 发布了一个 1.78 GiB 的检查点，但你可能无法将其用于盈利用途。NVIDIA 发布了宽松的权重，然后又将其标记为仅供研究使用。字节跳动没有发布任何权重、参数数量或 API。在查看评估表之前，请先阅读规格说明。

Muse Glimmer VRAM envelope

VoiceChat turn-taking latency

01 · Meta · Open weights

Meta AI Releases Muse Glimmer: A 30B Open-Weights Agentic Model That Runs on One Consumer GPU

> **译文：** Meta AI 发布 Muse Glimmer：一款可在单张消费级 GPU 上运行的 300 亿开放权重智能体模型

A 30B model used to be a data-center line item. At full precision Muse Glimmer needs over 55 GB. Meta compresses the weights to roughly 4-bit, which brings the language model under 20 GB, and the whole thing fits a 24 GB card — KV cache, perception encoder and drafter sharing the headroom. No network call.

> **译文：** 一个 30B 的模型曾经是数据中心的一项重要资源。Muse Glimmer 在全精度下需要超过 55GB 的内存。Meta 将权重压缩到大约 4 位，使语言模型的大小降至 20GB 以下，整个模型可以装进一张 24GB 的存储卡——KV 缓存、感知编码器和绘图器共享剩余空间。无需网络调用。

Two quantized builds ship. K-Quant-17GB targets 24 GB VRAM at 1.0% average degradation across 15 benchmarks; K-Quant-Dynamic targets 32 GB at 0.2%. Speed comes from DFlash, a block-diffusion drafter predicting 16 tokens per forward pass: on an RTX 5090 throughput moves from 74.9 to 233.4 tok/s, a 3.1x speedup. It leads MCP Atlas at 75.5 against Gemma4-31B’s 54.2 and Qwen3.6-27B’s 62.5, and trails Qwen3.6-27B on OSWorld-Verified, 65.9 to 75.6. Apache 2.0.

> **译文：** 提供两种量化版本。K-Quant-17GB 目标配置 24 GB 显存，在 15 项基准测试中平均性能下降 1.0%；K-Quant-Dynamic 目标配置 32 GB 显存，性能下降 0.2%。速度提升得益于 DFlash，这是一款块扩散式数据提取器，每次前向传播可预测 16 个令牌：在 RTX 5090 显卡上，吞吐量从 74.9 tok/s 提升至 233.4 tok/s，速度提升 3.1 倍。在 MCP Atlas 测试中，其性能为 75.5，领先于 Gemma4-31B 的 54.2 和 Qwen3.6-27B 的 62.5；但在 OSWorld-Verified 测试中，其性能略逊于 Qwen3.6-27B，分别为 65.9 和 75.6。Apache 2.0。

02 · webAI · Formal logic webAI Releases TwIL-LM: A 1.7B and 3B Formal-Logic Model Family for Autoformalization on Local Hardware

> **译文：** 02 · webAI · 形式逻辑 webAI 发布 TwIL-LM：用于本地硬件自动形式化的 17 亿和 3 亿形式逻辑模型系列

The small-model pitch is usually cost. webAI’s is verification. TwIL-LM translates English into first-order logic and checks whether a conclusion follows from its premises — a job that wants a checker, not a conversationalist. The 3B Q4_K_M GGUF is 1.78 GiB and runs on CPU or 4 GB of VRAM.

> **译文：** 小型模型的卖点通常是成本。webAI 的卖点则是验证。TwIL-LM 将英语翻译成一阶逻辑，并检查结论是否由前提推导而出——这项工作需要的是验证器，而不是对话器。3B Q4_K_M GGUF 的大小为 1.78 GiB，可在 CPU 或 4 GB 显存上运行。

The announcement frames the release around beating gpt-oss-120b on four of five formal-reasoning lanes. The shipped checkpoint trails it on the six-lane average, 0.4488 to 0.5192. The unambiguous win is throughput: 482-token generations and 32.9 answers per second against the 120B’s 4.2. Both checkpoints ship under the webAI Non-Commercial License 1.0 — revenue-generating deployment needs a separate agreement.

> **译文：** 此次发布公告重点强调了该版本在五个形式推理测试通道中的四个通道上超越了 gpt-oss-120b。在六个通道的平均测试结果上，该版本略逊一筹，分别为 0.4488 和 0.5192。但最显著的优势在于吞吐量：该版本每秒可生成 482 个令牌并给出 32.9 个答案，而 gpt-oss-120b 仅为 4.2 个。这两个版本均采用 webAI 非商业许可 1.0 版发布——用于盈利性部署需要另行签署协议。

03 · NVIDIA · Voice AI

NVIDIA Releases NemotronLabs VoiceChat 11B: An Open Full-Duplex Speech-to-Speech Model with ~450 ms Turn-Taking and Live Tool Calling

> **译文：** NVIDIA 发布 NemotronLabs VoiceChat 11B：一款开放式全双工语音对语音模型，具有约 450 毫秒的轮流语音交互速度和实时工具调用功能

A voice agent has been three models in a trench coat: ASR, then an LLM, then TTS, every handoff adding latency and losing information. VoiceChat 11B does streaming speech understanding and speech generation in one hybrid Mamba/Transformer network. It listens while it speaks, so a user can barge in mid-turn and the agent yields.

> **译文：** 语音代理过去常常采用三种不同的模式：自动语音识别 (ASR)、语言逻辑模型 (LLM) 和文本转语音 (TTS)，每次切换都会增加延迟并丢失信息。VoiceChat 11B 在一个混合的 Mamba/Transformer 网络中实现了流式语音理解和语音生成。它边听边说，因此用户可以在发言过程中突然插话，而代理会自动让位。

Measured smooth turn-taking latency is 448 ms on Full-Duplex-Bench 1.0 at TOR 0.82, with a take-over rate of 1.00 at 480 ms on user interruption. It is the first open full-duplex model to call tools while the conversation keeps flowing, emitting on a side channel while an operator-defined on-hold line covers the silence. Weights are permissive OpenMDW-1.1, but NVIDIA labels the checkpoint research-only, caps it at five tools per session, and wants one 80 GB GPU. There is no hosted API.

> **译文：** 在 TOR 0.82 的条件下，使用 Full-Duplex-Bench 1.0 测试测得的平滑轮流延迟为 448 毫秒，用户中断时接管率为 1.00，延迟为 480 毫秒。它是首个开放式全双工模型，能够在对话持续进行的同时调用工具，并通过侧信道发送消息，同时由操作员定义的保持线路来覆盖静默期。权重采用宽松的 OpenMDW-1.1 标准，但 NVIDIA 将此检查点标记为仅供研究使用，限制每个会话最多使用五个工具，并要求配备一块 80 GB 的 GPU。目前没有托管 API。

Agents, MCP integrations, and LLM-powered apps are entering codebases faster than security programs can track them. This guide gives AI/ML engineers, platform engineers, and AppSec teams a practical see–fix–protect framework, with the checklists and templates to start today.

> **译文：** 代理、MCP 集成和 LLM 驱动的应用程序正以远超安全程序跟踪速度的速度涌入代码库。本指南为 AI/ML 工程师、平台工程师和应用安全团队提供了一个实用的“发现-修复-保护”框架，其中包含清单和模板，可帮助您立即上手。

04 · ByteDance Seed · Multimodal

ByteDance Seed Introduces SeedRealtime: a Native Audio-Visual Full-Duplex LLM That Watches, Listens and Speaks in One Model

> **译文：** 字节跳动Seed推出SeedRealtime：一款原生音视频全双工LLM，可在单一模型中实现观看、聆听和说话功能。

Every other release here has somewhere to run. This one has nowhere, and that is why it is in the issue. SeedRealtime fuses audio, video and text in one end-to-end architecture and moves turn-taking inside the model, replacing the external voice-activity detector most real-time stacks still depend on.

> **译文：** 这里的其他版本都有运行环境，唯独这个版本没有，所以才出现在这个问题里。SeedRealtime 将音频、视频和文本融合到一个端到端的架构中，并将轮流交互机制移到模型内部，取代了大多数实时协议栈仍然依赖的外部语音活动检测器。

The demos are the evidence. At a noisy group dinner it binds names to faces and keeps each voice tied to its identity. At a museum it holds an instruction and speaks up unprompted when the object enters frame. Watching an espresso workflow it interrupts when whole beans go into the portafilter. ByteDance’s own human eval reports pacing issues halved versus cascaded stacks — no benchmark, no latency numbers. It is live in the Doubao app. There is no technical report, no parameter count, no weights, and no announced API.

> **译文：** 演示就是最好的证明。在嘈杂的聚餐中，它能将名字与面孔对应起来，并将每个声音与其身份关联起来。在博物馆里，它能识别指示牌，并在展品进入画面时主动发出语音提示。在观察意式咖啡制作流程时，当咖啡豆进入手柄时，它会立即打断。字节跳动自己的人工评估报告显示，与级联堆栈相比，速度问题减少了一半——但没有基准测试，也没有延迟数据。它已在豆宝应用中上线。目前没有技术报告、参数数量、权重，也没有公布任何API。

05 · Pokee AI · Long context

Pokee AI Releases Pokee-Isaac 28B: A 10M-Token Context Agentic Model Built to Run Inside the Customer Boundary

> **译文：** Pokee AI 发布 Pokee-Isaac 28B：一个拥有 1000 万个令牌的上下文代理模型，旨在客户边界内运行

Long context has been a cloud feature, which excludes everyone whose data is not permitted to leave the boundary at all. Isaac is a 28B text-only model with a 10M-token window, built to be deployed inside that boundary — VPC, on-premises, or on-device.

> **译文：** 长上下文一直是云平台的一项特性，它排除了所有数据完全不允许离开边界的用户。Isaac 是一个 280 亿文本模型，具有 1000 万个令牌窗口，旨在部署在该边界内——无论是 VPC、本地部署还是设备端部署。

It stays above 93.3% on RULER at every tested length, ending at 93.3% at 10M, where GPT-5.6 Luna and Gemini 3.5 Flash Lite track it to 512K and then overflow at 1M. It leads BFCL v4 at 70.94 to Luna’s 70.61 — the report calls that parity, not a lead — and loses Terminal-Bench 2.1, resolving 56 of 86 text-compatible tasks against Luna’s 60. Weights are not published; deployment is licensed. Pokee publishes measurements only from a single B200-class GPU, so the single-GPU-from-an-RTX-4090 claim is vendor guidance, not a reported result.

> **译文：** 在 RULER 测试中，该模型在所有测试长度下均保持 93.3% 以上的准确率，在 10M 长度下仍为 93.3%。GPT-5.6 Luna 和 Gemini 3.5 Flash Lite 在 512K 长度下与其表现相当，但在 1M 长度下则出现溢出。该模型在 BFCL v4 测试中以 70.94% 的准确率领先于 Luna 的 70.61%——报告称两者表现相当，而非领先——但在 Terminal-Bench 2.1 测试中则逊色，仅解决了 86 个文本兼容任务中的 56 个，而 Luna 解决了 60 个。权重未公布；部署需获得许可。Pokee 仅公布了来自单个 B200 级 GPU 的测量结果，因此关于 RTX 4090 单 GPU 测试结果的说法仅为厂商建议，并非实际报告结果。

Northeastern & Stanford · Agent runtime

Meet Shepherd: An Open-Source Python Substrate That Lets Meta-Agents Fork, Replay, and Revert Any Agent Run

> **译文：** Shepherd 简介：一个开源的 Python 底层框架，允许元代理 fork、重放和回滚任何代理运行。

A coding agent at step 10 is holding edited files, a running dev server, installed packages, and a warm prompt cache. It misreads a traceback and rewrites a file that was already correct. Now you have two bad options: patch forward, growing the context and the token bill, or restart, re-paying every model and tool call while reproducing nothing exactly, because runs are non-deterministic.

> **译文：** 在步骤 10 中，编码代理持有已编辑的文件、正在运行的开发服务器、已安装的软件包以及预热提示缓存。它错误地读取了回溯信息，并重写了原本正确的文件。现在你面临两个糟糕的选择：要么向前修补，但这会增加上下文和令牌成本；要么重新启动，重新执行每个模型和工具调用，但由于运行结果不确定，你将无法完全重现问题。

What you want is step eight. Git versions files, not a live process or a cache, so no existing runtime offers it. Shepherd records an agent run as a Git-like trace of typed events, where each commit covers the agent process and the filesystem together, copy-on-write. A branch therefore carries live state, not just files. Core operations are mechanized in Lean, and permissions are declared in the signature — a May[GitRepo, ReadOnly] binding compiles down to that run’s writable roots and is enforced at the syscall jail.

> **译文：** 你需要的是第八步。Git 版本控制的是文件，而不是实时进程或缓存，因此现有的运行时环境都不支持此功能。Shepherd 将代理运行记录为类似 Git 的类型化事件跟踪，其中每次提交都会同时覆盖代理进程和文件系统，并采用写时复制 (copy-on-write) 机制。因此，分支承载的是实时状态，而不仅仅是文件。核心操作在 Lean 中实现了自动化，权限在签名中声明——`May[GitRepo, ReadOnly]` 绑定会编译到该运行的可写根目录，并在系统调用 jail 中强制执行。

Reported: forks 5× faster than Docker and over 95% prompt-cache reuse on replay. Once a run is forkable, a meta-agent can sit on top of it. Live supervision raised CooperBench pair-coding pass rates from 28.8% to 54.7%. Branching exploration beat baselines across four benchmarks by up to 11 points while cutting wall-clock time by up to 58%. Forking rollouts for Tree-RL moved TerminalBench-2 from 34.2% to 39.4%. MIT-licensed, pip install shepherd-ai , Python 3.11+, early alpha.

> **译文：** 据报道：fork 速度比 Docker 快 5 倍，重放时提示缓存重用率超过 95%。一旦运行可以 fork，元智能体就可以在其上运行。实时监督将 CooperBench 结对编程的通过率从 28.8% 提高到 54.7%。分支探索在四个基准测试中比基线高出 11 分，同时将实际运行时间缩短了 58%。Tree-RL 的 fork 部署将 TerminalBench-2 的通过率从 34.2% 提高到 39.4%。MIT 许可，使用 pip 安装 shepherd-ai，支持 Python 3.11+，早期 alpha 版本。