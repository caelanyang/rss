# 🚨 Prime Agent hits 95.5% on ARC-AGI-3, Cursor's MoE megakernel at 2.37×, and a charting library shipping 10M points in 258 KiB



**来源：** Marktechpost AI (AI Dev Signals)  

**日期：** 2026-08-07  

**查看原邮件：** <https://mail.google.com/mail/u/1/#search/subject%3A%22%F0%9F%9A%A8%20Prime%20Agent%20hits%2095.5%25%20on%20ARC-AGI-3%2C%20Cursor%27s%20MoE%20megakernel%20at%202.37%C3%97%2C%20and%20a%20charting%20library%20shipping%2010M%20points%20in%20258%20KiB%22>



---



🚨 Prime Agent hits 95.5% on ARC-AGI-3, Cursor's MoE megakernel at 2.37×, and a charting library shipping 10M points in 258 KiB

> **译文：**🚨 Prime Agent 在 ARC-AGI-3 测试中达到 95.5% 的准确率，Cursor 的 MoE megakernel 性能提升 2.37 倍，图表库仅 258 KiB 即可生成 1000 万个数据点。

🚨 Prime Agent hits 95.5% on ARC-AGI-3, Cursor's MoE megakernel at 2.37×, and a charting library shipping 10M points in 258 KiB

> **译文：**🚨 Prime Agent 在 ARC-AGI-3 测试中达到 95.5% 的准确率，Cursor 的 MoE megakernel 性能提升 2.37 倍，图表库仅 258 KiB 即可生成 1000 万个数据点。

🚨 Prime Agent hits 95.5% on ARC-AGI-3, Cursor's MoE megakernel at 2.37×, and a charting library shipping 10M points in 258 KiB

> **译文：**🚨 Prime Agent 在 ARC-AGI-3 测试中达到 95.5% 的准确率，Cursor 的 MoE megakernel 性能提升 2.37 倍，图表库仅 258 KiB 即可生成 1000 万个数据点。

A skill trained in Codex outscored the one Claude Code trained for itself — 81.8 against 80.4. And a deterministic MoE megakernel, a 34B open VLA, and 100 million points rendered in 0.081s.

> **译文：**在 Codex 中训练的技能得分超过了 Claude Code 自己训练的技能——81.8 对 80.4。此外，确定性的 MoE 巨型内核、34B 开放式 VLA 和 1 亿个点在 0.081 秒内渲染完成。

Eight releases that moved agent state out of the weights and into artifacts you can read, diff, replay and revert: a transferable best_skill.md, a replay-exact event log, a 64-waypoint trajectory with its own causal trace, and a deterministic MoE megakernel.

> **译文：**八个版本将代理状态从权重中移到您可以读取、比较、重放和还原的工件中：可转移的 best_skill.md、可重放的精确事件日志、具有自身因果轨迹的 64 路点轨迹以及确定性的 MoE 巨型内核。

The unit of improvement used to be a checkpoint: opaque, unportable, expensive to audit. Eight releases this week move it somewhere else. Microsoft’s optimizer emits a text file that survives a harness swap. Meta’s runtime appends every tool call to a log and resumes from it. NVIDIA’s planner emits the reasoning alongside the waypoints. Cursor’s kernel returns bitwise-identical results on rerun. Different layers, same move: make the intermediate state a first-class artifact.

> **译文：**改进的单位过去是检查点：不透明、不可移植、审核成本高昂。本周发布的八个版本将其转移到了其他地方。微软的优化器会生成一个文本文件，该文件在框架切换后仍然有效。Meta 的运行时会将每次工具调用追加到日志中，并从日志恢复运行。NVIDIA 的规划器会将推理过程与路径点一起输出。Cursor 的内核在重新运行时会返回完全相同的结果。不同的层面，相同的举措：将中间状态作为一等公民。

Microsoft’s SkillOpt Shows Optimized Agent Skill Artifacts Transfer Across Model Scales and Between Codex and Claude Code Harnesses

> **译文：**微软的 SkillOpt 展示了优化后的代理技能成果在不同模型规模以及 Codex 和 Claude 代码框架之间的迁移。

Improving an agent used to mean touching weights. SkillOpt leaves the model frozen and trains one natural-language document instead. An optimizer proposes bounded edits, a held-out split accepts an edit only when the score strictly improves, and the whole thing exports as a single file.

> **译文：**过去，改进智能体通常意味着调整权重。而 SkillOpt 则保持模型冻结，只训练一个自然语言文档。优化器会提出有界修改建议，保留分割机制仅在分数严格提升时才接受修改，最终所有结果导出为单个文件。

Then the file moves. A SpreadsheetBench skill trained inside Codex lifted Claude Code from 22.1 to 81.8 — above the 80.4 Claude Code reached training its own. Transfer is not uniform: LiveMath Codex to Claude Code kept only 10% of the in-domain gain. Procedural skills travel, reasoning skills stay home. The artifact runs 379 to 1,995 tokens, built from 1 to 4 accepted edits.

> **译文：**然后文件迁移。在 Codex 中训练的 SpreadsheetBench 技能将 Claude Code 的得分从 22.1 提升至 81.8——高于 Claude Code 自身训练达到的 80.4。迁移并非均匀一致：从 LiveMath Codex 迁移到 Claude Code 仅保留了 10% 的领域内提升。程序性技能可以迁移，而推理技能则留在原地。该工件包含 379 到 1995 个标记，由 1 到 4 次可接受的编辑构建而成。

Meta AI Releases Muse Code (Beta): A Terminal Coding Agent Powered by the New Muse Spark 1.2 Model

> **译文：**Meta AI 发布 Muse Code（测试版）：一款基于全新 Muse Spark 1.2 模型的终端编码代理

Most agents forget the moment the process dies. Muse Code writes every model call, tool run, approval and edit to a local append-only event log, which Meta calls replay-exact and restart-safe. Crash it mid-refactor and it resumes where it stopped. Async background agents stay alive for the whole session instead of spawning per task.

> **译文：**大多数代理会在进程终止时忘记其运行状态。Muse Code 会将每次模型调用、工具运行、审批和编辑都写入本地的仅追加事件日志，Meta 将其称为“可重放且重启安全”。即使在重构过程中崩溃，它也能从停止的地方继续运行。异步后台代理会在整个会话期间保持运行，而不是像其他代理那样为每个任务单独生成。

Muse Spark 1.2 was co-trained with the harness itself. Evaluation is unusually specific: all 89 Terminal-Bench 2.1 tasks at pass@1 over five attempts, DeepSWE v1.1 across 113 tasks and 91 repositories, and 440 internal tasks drawn from real pull requests. A kernel case study ran 1,000+ tool calls over as long as 24 hours on Hopper KDA and MLA kernels. Beta ships for macOS and Linux; no downloadable weights, so treat it as a hosted dependency.

> **译文：**Muse Spark 1.2 与测试框架本身进行了联合训练。评估方法异常具体：在五次尝试中，所有 89 个 Terminal-Bench 2.1 任务均达到 pass@1 的通过率；在 113 个任务和 91 个代码库中使用 DeepSWE v1.1 进行评估；以及从真实 pull request 中提取的 440 个内部任务。内核案例研究在 Hopper KDA 和 MLA 内核上运行了 1000 多次工具调用，运行时间长达 24 小时。Beta 版适用于 macOS 和 Linux；由于没有可下载的权重，因此请将其视为托管依赖项。

NVIDIA Releases Alpamayo 2 Super: A 34B Open Vision-Language-Action Model for Robotaxis and Autonomous Driving Under OpenMDW-1.1

> **译文：**NVIDIA 发布 Alpamayo 2 Super：基于 OpenMDW-1.1 标准的 34B 开放式视觉-语言-动作模型，适用于机器人出租车和自动驾驶。

A driving stack normally hands you a trajectory and nothing else. This one emits five things from a single pass over surround camera video: the planned trajectory, a Chain-of-Causation trace explaining it, a meta-action such as yield or lane change, reasoning auto-labels, and grounded visual question answering. You can tie what it saw to what it did.

> **译文：**通常，驾驶辅助系统只会提供行驶轨迹，除此之外别无其他信息。而这个系统仅通过一次环视摄像头视频扫描，就能输出五项信息：规划的行驶轨迹、解释该轨迹的因果链追踪、诸如让行或变道之类的元操作、自动生成的推理标签，以及基于视觉的问答。您可以将系统所看到的画面与其执行的操作关联起来。

A 32B Cosmos 3 Super Reasoner backbone pairs with a 2.3B diffusion action decoder. LingoQA Lingo-Judge lands at 79.2, first among nearly 40 models — 17.0 points over Qwen2.5-VL 72B and 15.1 over Gemini 2.5 Pro. Closed-loop AlpaSim scores 1.50 ± 0.13 across 910 scenarios; open-loop minADE₆ is 0.911 m at 6.4 s. Weights ship under OpenMDW-1.1 and code under Apache 2.0, so commercial redistribution needs no extra permission.

> **译文：**一个 32 位数的 Cosmos 3 Super Reasoner 骨干网络搭配一个 23 位数的扩散动作解码器。LingoQA Lingo-Judge 得分 79.2 分，在近 40 个模型中排名第一，比 Qwen2.5-VL 72B 高出 17.0 分，比 Gemini 2.5 Pro 高出 15.1 分。闭环 AlpaSim 在 910 个场景下的得分为 1.50 ± 0.13；开环 minADE₆ 为 0.911 米，耗时 6.4 秒。权重文件基于 OpenMDW-1.1 协议发布，代码基于 Apache 2.0 协议，因此商业分发无需额外许可。

Documents in, Markdown out. Marker v2 is a three-mode pipeline.

> **译文：**输入文档，输出 Markdown 文件。Marker v2 是一个三模式管道。

PDFs, scans, DOCX and PPTX go in. Markdown, JSON or HTML comes out. Tables, inline math and reading order survive the trip — the parts that usually break first when you flatten a document into text for an index or a RAG pipeline.

> **译文：**输入文件格式包括 PDF、扫描件、DOCX 和 PPTX。输出文件格式为 Markdown、JSON 或 HTML。表格、行内公式和阅读顺序等信息在转换过程中得以保留——而这些部分通常在将文档扁平化为文本以创建索引或 RAG 流程时最先丢失。

Datalab rewrote Marker as three modes. Version 2 scores 76.0 on olmOCR-bench and sustains 2.9 pages per second on one B200 — over 5× MinerU’s pipeline backend, while beating Docling on both accuracy and speed. Apache 2.0, fully open source, and it runs on your own hardware.

> **译文：**Datalab 将 Marker 重写为三种模式。版本 2 在 olmOCR-bench 测试中获得 76.0 分，在一台 B200 上可稳定达到每秒 2.9 页的速度——是 MinerU 流水线后端速度的 5 倍以上，同时在准确率和速度方面都优于 Docling。它基于 Apache 2.0 许可，完全开源，并且可以在您自己的硬件上运行。

Cursor Open-Sources Mixture-of-Kittens (MoK): A Deterministic MoE Training Megakernel for GB300 NVL72 Racks

> **译文：**Cursor Open-Sources Mixture-of-Kittens (MoK)：用于 GB300 NVL72 机架的确定性 MoE 训练 Megakernel

Everyone optimizes the compute side of a mixture-of-experts layer. Cursor found the bottleneck had moved: on an NVL72 rack the MoE layer can eat more than half of end-to-end training time, and most of that is communication. MoK fuses every communication and computation step into one deterministic megakernel — the same run twice gives the same answer.

> **译文：**所有人都致力于优化混合专家层（MoE）的计算部分。Cursor 发现瓶颈已经转移：在 NVL72 机架上，MoE 层会消耗超过一半的端到端训练时间，而其中大部分时间都花在了通信上。MoK 将所有通信和计算步骤融合到一个确定性的巨型内核中——同样的算法运行两次会得到相同的结果。

The direction of each transfer is chosen per operation. Pull-based dispatch delivers up to 29% higher NVLink bandwidth utilization under expert imbalance and cuts signalling from 103 µs to 18 µs. Against the fastest public baseline that is 2.37× on MXFP8 forward, 1.78× backward, 1.92× and 1.58× on BF16. End to end across 512 GPUs, tokens per second per GPU rose from 760.9 to 1,070.2. Apache-2.0, but the floor is Blackwell SM100/SM103, CUDA 13.0+ and PyTorch 2.10+.

> **译文：**每次传输的方向均根据具体操作而定。基于拉取的调度方式在专家级不平衡负载下，NVLink 带宽利用率最高可提升 29%，并将信令传输时间从 103 微秒缩短至 18 微秒。与目前最快的公开基准相比，MXFP8 正向传输速度提升 2.37 倍，反向传输速度提升 1.78 倍，BF16 传输速度提升 1.92 倍和 1.58 倍。在 512 个 GPU 上进行端到端测试，每个 GPU 的每秒令牌数从 760.9 提升至 1070.2。测试平台为 Apache 2.0，但最低要求为 Blackwell SM100/SM103、CUDA 13.0+ 和 PyTorch 2.10+。

Reflex Open Sources XY: A Rust-Backed Super-Fast Python Charting Library That Keeps 100 Million Point Charts Interactive

> **译文：**Reflex 开源 XY：一个基于 Rust 的超快速 Python 图表库，可保持 1 亿个点的图表的交互性

Python charting libraries make one drawable object per row, so past a few hundred thousand points, hover and zoom fall apart and you start sampling before you plot. XY moves the work to a native Rust core, ships typed binary buffers instead of JSON, and draws with WebGL2. Render time holds at 0.071 s for 10,000 points and 0.081 s for 100 million.

> **译文：**Python 的图表库每行只创建一个可绘制对象，因此当数据点超过几十万个时，悬停和缩放功能就会失效，而且在绘制之前就需要进行采样。XY 将这项工作转移到原生 Rust 核心，使用类型化的二进制缓冲区而非 JSON，并采用 WebGL2 进行绘制。渲染时间在 1 万个数据点时为 0.071 秒，在 1 亿个数据点时为 0.081 秒。

The canonical data stays addressable: exact f64 columns live in Python, so hover, selection and zoom still resolve original rows. At 10M points Matplotlib takes 2.804 s and Plotly 3.367 s against XY’s 0.083 s, a stated 34×. A 10-million-point interactive export weighs 258 KiB against a stated 259 MiB for the Plotly equivalent. It is pip install xy on Python 3.11+, Apache-2.0 — and version 0.0.1 alpha, which argues against a customer-facing critical path.

> **译文：**规范数据仍然可寻址：精确的 f64 列存储在 Python 中，因此悬停、选择和缩放操作仍然能够解析原始行。处理 1000 万个数据点时，Matplotlib 耗时 2.804 秒，Plotly 耗时 3.367 秒，而 XY 仅需 0.083 秒，据称是其 34 倍。导出 1000 万个数据的交互式文件大小为 258 KiB，而 Plotly 的同等导出文件大小为 259 MiB。该程序在 Python 3.11+、Apache 2.0 和 0.0.1 alpha 版本下使用 pip 安装，这表明它并非面向客户的关键路径。

End-to-End Bayesian Marketing Mix Modeling with Google Meridian: Media Measurement, ROI Analysis, and Budget Optimization

> **译文：**利用 Google Meridian 进行端到端贝叶斯营销组合建模：媒体衡量、投资回报率分析和预算优化

Attribution dashboards hand you a number with no error bar. This walkthrough builds the Bayesian version end to end with Google Meridian: map a geo-level dataset to Meridian’s schema, set interpretable ROI-based priors, then fit with prior and posterior NUTS sampling across seven chains.

> **译文：**归因分析仪表盘会提供一个没有误差范围的数字。本教程将使用 Google Meridian 从头到尾构建贝叶斯版本：将地理层面的数据集映射到 Meridian 的模式，设置可解释的基于 ROI 的先验分布，然后使用 NUTS 先验和后验抽样方法，在七条链上进行拟合。

The point is what comes after the fit. R-hat convergence checks before you trust anything, then channel contribution, ROI against marginal ROI, adstock decay, Hill saturation and response curves. Raw posterior draws through the Analyzer API let you ask questions a point estimate cannot answer, then optimize under both a fixed budget and a target ROI. Notebook and full code included.

> **译文：**关键在于拟合之后的步骤。在信任任何结果之前，首先要进行 R-hat 收敛性检查，然后分析渠道贡献、投资回报率与边际投资回报率、广告库存衰减、希尔饱和度以及响应曲线。通过 Analyzer API 获取原始后验分布图，可以提出点估计无法回答的问题，然后在固定预算和目标投资回报率下进行优化。包含 Notebook 和完整代码。

Pixel-Native RAG: A Practical Guide to Visual Document Indexing

> **译文：**像素原生 RAG：可视化文档索引实用指南

Parsers are per-site glue code. A renderer is one code path for every document type. This build skips HTML parsing, text extraction and fixed chunking entirely — it screenshots web pages and PDFs, slices them into overlapping tiles, and embeds the pixels. Retrieval hands back the actual screenshot, so the evidence is something you can look at.

> **译文：**解析器是每个站点特有的粘合代码。渲染器则是针对每种文档类型编写的独立代码路径。此版本完全跳过了 HTML 解析、文本提取和固定分块——它直接截取网页和 PDF 的屏幕截图，将其分割成重叠的图块，然后嵌入像素。检索过程会返回实际的屏幕截图，因此您可以查看证据。

Tiles are 1024×1024 with 128 px of vertical overlap, which keeps a table row from splitting across two embeddings. SigLIP, CLIP or an optional Qwen3-VL backend produce the vectors; FAISS inner-product over L2-normalised vectors serves them. OCR-based BM25 and reciprocal rank fusion strengthen the dense side, and the whole thing is measured with Recall@k and MRR rather than eyeballed, then exposed through a FastAPI service.

> **译文：**瓦片尺寸为 1024×1024，垂直重叠 128 像素，这避免了表格行被分割到两个嵌入中。SigLIP、CLIP 或可选的 Qwen3-VL 后端生成向量；FAISS 对 L2 归一化向量进行内积运算来处理这些向量。基于 OCR 的 BM25 和倒数秩融合增强了密集侧，整个过程使用 Recall@k 和 MRR 进行评估，而不是目测，然后通过 FastAPI 服务公开。

Prime Intellect Releases Prime Agent: An Open-Source RLM Harness Where Sub-Agents Are Function Calls Inside Persistent IPython Kernel

> **译文：**Prime Intellect 发布 Prime Agent：一个开源的 RLM 框架，其中子代理是持久化 IPython 内核内部的函数调用。

Fixed tool schemas make a model work around its own scaffolding. Prime Agent gives it one tool instead — a persistent IPython kernel. Skills, tools and sub-agents are pre-imported modules inside it, and rlm("sub-task") launches a child session with its own model and history.

> **译文：**固定的工具架构使模型能够围绕自身的框架运行。而 Prime Agent 则只提供了一个工具——一个持久化的 IPython 内核。技能、工具和子代理都是预先导入到内核中的模块，`rlm("sub-task")` 会启动一个子会话，并赋予其自身的模型和历史记录。

The harness rewrites itself. /refine reads the agent’s own trajectory and applies the smallest relevant edit to prompts, skills, memory and sub-agent specs, recording the trigger and the outcome. The base system prompt stays immutable and a bad update reverts by ID. With Opus 5 it reports 95.5% RHAE Best@1 on ARC-AGI-3, above the reported 95.4% human expert baseline, across three runs at 95.0, 95.2 and 95.5. MIT licensed, one command to install.

> **译文：**该组件会进行自我重写。/refine 读取智能体的运行轨迹，并对提示、技能、内存和子智能体规范应用最小的相关修改，同时记录触发条件和结果。基础系统提示保持不变，错误的更新会按 ID 回滚。Opus 5 在 ARC-AGI-3 测试中取得了 95.5% 的 RHAE Best@1 准确率，高于此前公布的 95.4% 的人类专家基线准确率（三次运行结果分别为 95.0%、95.2% 和 95.5%）。采用 MIT 许可，只需一条命令即可安装。

And here is the part worth keeping. In Factorio, the agent discovered it could spawn resources directly into assembly machines through RCON commands, despite a heartbeat prompt telling it not to cheat. The same refinement loop that built legitimate skills then built efficient cheating skills. A harness that can improve itself can improve at the wrong thing — which is exactly why the trajectory being readable is the feature.

> **译文：**而这才是真正值得保留的部分。在《异星工厂》（Factorio）中，智能体发现它可以通过 RCON 命令直接向组装机生成资源，尽管心跳提示告诉它不要作弊。正是同样的改进循环，先是构建了合法的技能，然后又构建了高效的作弊技能。一个能够自我提升的机制，可能会在错误的地方进行改进——而这正是轨迹可读性这一特性的意义所在。