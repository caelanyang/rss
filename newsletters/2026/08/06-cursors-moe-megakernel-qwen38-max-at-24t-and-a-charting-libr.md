# 🚨 Cursor's MoE megakernel, Qwen3.8-Max at 2.4T, and a charting library that ships 10M points in 258 KiB

**来源：** Marktechpost AI (AI Dev Signals)  
**日期：** 2026-08-06  
**查看原邮件：** <https://mail.google.com/mail/u/1/#search/subject%3A%22%F0%9F%9A%A8%20Cursor%27s%20MoE%20megakernel%2C%20Qwen3.8-Max%20at%202.4T%2C%20and%20a%20charting%20library%20that%20ships%2010M%20points%20in%20258%20KiB%22>

---

🚨 Cursor's MoE megakernel, Qwen3.8-Max at 2.4T, and a charting library that ships 10M points in 258 KiB

> **译文：** 🚨 Cursor 的 MoE 超大型内核、2.4T 的 Qwen3.8-Max 以及一个仅 258 KiB 即可生成 1000 万个点的图表库

Home

Posts

🚨 Cursor's MoE megakernel, Qwen3.8-Max at 2.4T, and a charting library that ships 10M points in 258 KiB

> **译文：** 🚨 Cursor 的 MoE 超大型内核、2.4T 的 Qwen3.8-Max 以及一个仅 258 KiB 即可生成 1000 万个点的图表库

🚨 Cursor's MoE megakernel, Qwen3.8-Max at 2.4T, and a charting library that ships 10M points in 258 KiB

> **译文：** 🚨 Cursor 的 MoE 超大型内核、2.4T 的 Qwen3.8-Max 以及一个仅 258 KiB 即可生成 1000 万个点的图表库

Cursor open-sources its MoE training megakernel. Alibaba ships Qwen3.8-Max at 2.4T parameters. Reflex releases XY. GenOffice, pixel-native RAG, SkillSpector auditing, PerceptionBench evals, and YC's agent harness

> **译文：** Cursor 开源了其 MoE 训练巨型内核。阿里巴巴发布了参数量高达 2.4T 的 Qwen3.8-Max。Reflex 发布了 XY。GenOffice、像素级原生 RAG、SkillSpector 审计、PerceptionBench 评估以及 YC 的代理框架也相继问世。

Aug 5, 2026

Together with Mend

AI Dev Signals · August 4, 2026

Render, don’t parse. Patch, don’t rewrite.Eight releases that keep the source bytes.

> **译文：** 渲染，而非解析。修补，而非重写。八个版本，保留了源代码字节。

Screenshot tiles into FAISS instead of a text extractor. Dirty-block OOXML splicing instead of a full re-serialize. Exact f64 columns in Python behind a WebGL2 canvas. One deterministic megakernel instead of a scheduled dispatch. And a 2.4T MoE whose activated-parameter count is still unpublished.

> **译文：** 将屏幕截图平铺到 FAISS 中，而不是使用文本提取器。采用脏块 OOXML 拼接，而不是完全重新序列化。在 WebGL2 画布后方的 Python 中使用精确的 f64 列。使用一个确定性的巨型内核，而不是定时分发。以及一个 2.4T 的 MoE，其激活参数数量尚未公布。

Presented by Mend.io Securing AI Agents, MCP Servers & LLM Apps — agent behavior is not defined by code alone. Get the framework →

> **译文：** 由 Mend.io 呈现：保护 AI 代理、MCP 服务器和 LLM 应用——代理行为并非仅由代码定义。获取框架 →

Every layer below used to be lossy at the boundary. HTML parsing drops layout. Re-serializing a .docx drops formatting. Per-row draw calls force you to decimate before you plot. A single aggregate accuracy drops the failure mode. All eight releases move the same way: keep the canonical representation, emit a diff against it, and surface the loss where one is unavoidable.

> **译文：** 之前每一层在边界处都会有损。HTML 解析会丢失布局。重新序列化 .docx 文件会丢失格式。逐行绘制调用会强制你在绘图前进行数据抽取。单一聚合精度可以消除故障模式。所有八个版本都遵循相同的原则：保持规范表示，生成差异对比，并在不可避免的情况下显示损失。

2.37×

MoK MXFP8 forward speedup 258 KiB

XY export, 10M points 2.4T

Qwen3.8-Max total parameters

🔥 The signals 01 · Cursor · MoE training

Cursor Open-Sources Mixture-of-Kittens (MoK): A Deterministic MoE Training Megakernel for GB300 NVL72 Racks

> **译文：** Cursor Open-Sources Mixture-of-Kittens (MoK)：用于 GB300 NVL72 机架的确定性 MoE 训练 Megakernel

The MoE layer used to be a compute problem. On a 72-GPU NVLink domain it became a scheduling problem, and the MoE layer can consume more than half of end-to-end training time. Cursor fused every communication and computation step into one deterministic megakernel and took the CPU out of the loop.

> **译文：** MoE 层曾经是一个计算难题。在 72 个 GPU 的 NVLink 域上，它变成了一个调度难题，而且 MoE 层会消耗超过一半的端到端训练时间。Cursor 将所有通信和计算步骤融合到一个确定性的超内核中，从而将 CPU 从循环中移除。

Pull-based dispatch plus push-based combine cut dispatch signalling from 103 µs to 18 µs, roughly 5.8x. Against the fastest public baseline it runs up to 2.37x for MXFP8 forward, 1.78x MXFP8 backward, 1.92x BF16 forward, 1.58x BF16 backward. End to end on 512 GPUs, tokens per second per GPU moved from 760.9 to 1,070.2. Apache-2.0, but the floor is Blackwell SM100/SM103, CUDA 13.0+ and PyTorch 2.10+.

> **译文：** 基于拉取的调度与基于推送的调度相结合，将调度信号处理时间从 103 微秒缩短至 18 微秒，提升约 5.8 倍。与目前最快的公开基准相比，其 MXFP8 正向性能提升高达 2.37 倍，MXFP8 反向性能提升高达 1.78 倍，BF16 正向性能提升高达 1.92 倍，BF16 反向性能提升高达 1.58 倍。在 512 个 GPU 上进行端到端测试，每个 GPU 的每秒令牌数从 760.9 提升至 1070.2。测试环境为 Apache 2.0，但最低配置要求为 Blackwell SM100/SM103、CUDA 13.0+ 和 PyTorch 2.10+。

Read on Marktechpost →

· GitHub

· Technical details 02 · Alibaba Qwen · Frontier model

> **译文：** · 技术细节 02 · 阿里巴巴 Qwen · 前沿模型

Alibaba Qwen Releases Qwen3.8-Max: A 2.4 Trillion Parameter MoE Model and the Most Capable One in the Qwen Family to Date

> **译文：** 阿里巴巴Qwen发布Qwen3.8-Max：参数规模达2.4万亿的Qwen系列迄今为止性能最强的产品

A flagship release usually arrives with one number you are meant to remember. This one arrives with a number that is missing. Alibaba has not disclosed the activated-parameter count, so serving cost for the 2.4T checkpoint cannot be modeled yet. Open weights for Qwen3.8-Max and Qwen3.8-27B are promised next week.

> **译文：** 旗舰版本通常会有一个需要你记住的数字。但这次却缺少一个数字。阿里巴巴尚未公布激活参数的数量，因此目前还无法估算2.4T检查点的服务成本。Qwen3.8-Max和Qwen3.8-27B的开放权重预计将于下周公布。

The model page lists a 1M-token context window, with maximum input at 991K tokens and 983K when thinking is enabled. Pricing is $2.00 per 1M input tokens and $6.00 per 1M output, with implicit cache reads at $0.25 — cached input is eight times cheaper than fresh, so prefix stability drives cost more than prompt length. It scores 86.6 on Terminal-Bench 2.1 and 92.6 on GPQA Diamond, but reports 67.7 on SWE-bench Pro and 73.5 on FrontierSWE against Fable 5’s 80.0 and 88.8. The gains are multimodal and agentic, not reasoning.

> **译文：** 该模型页面列出了一个 100 万个令牌的上下文窗口，最大输入量为 99.1 万个令牌，启用思考功能后为 98.3 万个令牌。定价为每 100 万个输入令牌 2 美元，每 100 万个输出令牌 6 美元，隐式缓存读取费用为 0.25 美元——缓存输入比全新输入便宜八倍，因此前缀稳定性驱动的成本高于提示符长度。该模型在 Terminal-Bench 2.1 和 GPQA Diamond 测试中分别获得 86.6 分和 92.6 分，但在 SWE-bench Pro 和 FrontierSWE 测试中分别获得 67.7 分和 73.5 分，而 Fable 5 的得分分别为 80.0 分和 88.8 分。性能提升体现在多模态和智能体方面，而非推理方面。

Read on Marktechpost →

· Announcement

· Model page

· Qwen Studio 03 · Reflex · Python charting

Reflex Open Sources XY: A Rust-Backed Super-Fast Python Charting Library That Keeps 100 Million Point Charts Interactive

> **译文：** Reflex 开源 XY：一个基于 Rust 的超快速 Python 图表库，可保持 1 亿个点的图表的交互性

Every Python charting stack makes one drawable object per row, so past a few hundred thousand points you start sampling before you plot. XY draws a screen-bounded representation instead and leaves the exact f64 columns in Python, so hover, selection and zoom drilldown still return original rows.

> **译文：** 每个 Python 图表堆栈都会为每一行创建一个可绘制对象，因此当数据点超过几十万个后，在绘制之前就会开始采样。而 XY 则绘制屏幕边界内的表示，并在 Python 中保留精确的 f64 列，因此悬停、选择和缩放钻取操作仍然会返回原始行。

Render time holds at 0.071 s for 10,000 points and 0.081 s at 100 million. At 10M the benchmark reports 0.083 s against 2.804 s for Matplotlib WebAgg and 3.367 s for Plotly scattergl; Plotly does not complete at 50M. A 10-million-point interactive scatter exports to 258 KiB of HTML against a stated 259 MiB for the Plotly equivalent, and the payload stays near 258 KiB from 1M through 100M rows. Apache-2.0 — and version 0.0.1 early alpha, which argues against critical paths.

> **译文：** 渲染时间在 1 万个点时保持在 0.071 秒，在 1 亿个点时保持在 0.081 秒。在 1000 万个点时，基准测试报告的渲染时间为 0.083 秒，而 Matplotlib WebAgg 为 2.804 秒，Plotly scattergl 为 3.367 秒；Plotly 在 5000 万个点时无法完成渲染。一个 1000 万个点的交互式散点图导出为 258 KiB 的 HTML 文件，而 Plotly 的同等功能则需要 259 MiB，并且在 100 万行到 1 亿行之间，有效载荷始终保持在 258 KiB 左右。Apache 2.0 和 0.0.1 早期 alpha 版本，这表明关键路径可能存在问题。

Read on Marktechpost →

· GitHub

· Benchmarks

· Blog

Sponsored · CopilotKit

Your agent already works. Channels SDK gives it somewhere to work with people.

> **译文：** 您的代理程序已经可以运行。Channels SDK 为它提供了一个与用户交互的平台。

CopilotKit has released the Channels SDK, an open source library that puts an existing agent inside Slack and Microsoft Teams without a rewrite per platform. The connection is AG-UI, so LangGraph, CrewAI, Mastra, Pydantic AI, Google ADK and a plain HTTP agent you wrote yourself all work. Your model and orchestration layer stay where they are.

> **译文：** CopilotKit 发布了 Channels SDK，这是一个开源库，可以将现有的代理程序集成到 Slack 和 Microsoft Teams 中，无需针对每个平台进行重写。连接方式基于 AG-UI，因此 LangGraph、CrewAI、Mastra、Pydantic AI、Google ADK 以及您自己编写的纯 HTTP 代理程序均可正常工作。您的模型和编排层无需改动。

A channel is a transport and a rendering target, not a second agent. Messages are authored once as JSX and lowered into Block Kit in Slack and Adaptive Cards in Teams. Generative UI, human-in-the-loop approvals, tools, persistence, slash commands and mentions all ship. @copilotkit/channels 0.5.0 is live on npm under MIT; deployment needs Node.js 22+, an ESM project, and a long-running process.

> **译文：** 频道是一种传输和渲染目标，而非第二个代理。消息以 JSX 格式编写一次，即可在 Slack 中被导入 Block Kit，在 Teams 中被导入 Adaptive Cards。生成式 UI、人工审批、工具、持久化、斜杠命令和提及功能均已发布。@copilotkit/channels 0.5.0 已在 npm 上发布，采用 MIT 许可证；部署需要 Node.js 22+、一个 ESM 项目以及一个长时间运行的进程。

Read the breakdown →

Channels SDK on GitHub → · AG-UI protocol · CopilotKit 04 · Genspark · Office suite

> **译文：** GitHub 上的 Channels SDK → · AG-UI 协议 · CopilotKit 04 · Genspark · Office 套件

Genspark Open Sources GenOffice: A Free, Ad-Free AI Office Suite for macOS and Windows with Docs, Sheets, Slides, PDF

> **译文：** Genspark 开源 GenOffice：一款免费、无广告的 AI 办公套件，适用于 macOS 和 Windows，包含文档、表格、幻灯片和 PDF 文件。

Every alternative office suite breaks a Word document eventually, because it re-serializes the whole file on save. GenOffice archives the original by hash and never touches it. Only dirty blocks become OOXML fragments and get spliced back into the original document.xml. Untouched blocks keep their original bytes, and every other zip entry is copied verbatim.

> **译文：** 其他所有办公软件最终都会破坏 Word 文档，因为它们会在保存时重新序列化整个文件。GenOffice 会根据哈希值对原始文件进行归档，并且不会对其进行任何修改。只有脏数据块会变成 OOXML 片段，并被拼接回原始的 document.xml 文件中。未修改的数据块会保留其原始字节，而其他所有压缩条目都会被原样复制。

Five Electron apps over one engine layer, Apache-2.0, signed installers for Apple Silicon and Windows x64 at version 0.4.110. Sheets pairs the Univer core with a Rust xlsx sidecar using calamine and IronCalc; Slides and the docx engine are in-house. The team says one engineer, one week, roughly $10,000 in tokens for the Alpha — and Alpha is the operative word: AI runs through a signed-in Genspark account and consumes credits, with no local model key by default.

> **译文：** 五个基于同一引擎层（Apache 2.0）的 Electron 应用，版本为 0.4.110，并为 Apple Silicon 和 Windows x64 平台提供了签名安装程序。Sheets 应用将 Univer 核心与使用 calamine 和 IronCalc 的 Rust xlsx sidecar 组件结合使用；Slides 应用和 docx 引擎则由团队自主开发。团队表示，Alpha 版本仅花费一名工程师一周时间，约 1 万美元的代币——注意是“Alpha”这个词：人工智能需要通过已登录的 Genspark 账户运行并消耗积分，默认情况下没有本地模型密钥。

Read on Marktechpost →

· GitHub

· Download

· Security notes 05 · Marktechpost · RAG tutorial

Pixel-Native RAG: A Practical Guide to Visual Document Indexing

> **译文：** 像素原生 RAG：可视化文档索引实用指南

A parser is per-site glue code. A renderer is one code path for HTML, PDF, scanned fax and spreadsheet export alike. This build skips text extraction entirely: render pages as images, slice them into overlapping tiles, embed with SigLIP, CLIP or an optional Qwen3-VL backend, and search a FAISS index.

> **译文：** 解析器是每个站点的粘合代码。渲染器是一条统一的代码路径，可用于导出 HTML、PDF、扫描传真和电子表格等多种格式的文件。此版本完全跳过了文本提取：将页面渲染为图像，将其分割成重叠的图块，嵌入 SigLIP、CLIP 或可选的 Qwen3-VL 后端，并搜索 FAISS 索引。

Tiles are 1024×1024 with 128px of vertical overlap, so a sentence or table row is not split across two embeddings. OCR-based BM25 runs alongside dense retrieval and the two are combined with reciprocal rank fusion; tile scores are max-pooled per document. The tutorial measures Recall@1, @3, @5 and MRR, trains a residual contrastive adapter on mined pseudo-queries, and serves the whole thing behind a FastAPI POST /search.

> **译文：** 图块尺寸为 1024×1024，垂直重叠 128 像素，因此句子或表格行不会被分割到两个嵌入向量中。基于 OCR 的 BM25 与密集检索并行运行，两者通过倒数排序融合进行结合；每个文档的图块得分进行最大池化。本教程测量 Recall@1、@3、@5 和 MRR，在挖掘出的伪查询上训练残差对比适配器，并通过 FastAPI POST /search 请求提供所有服务。

Read on Marktechpost →

· Full codes

· PixelRAG upstream 06 · NVIDIA · Skill security

Building an Advanced AI Skill Security Auditing Pipeline with NVIDIA SkillSpector, LangGraph, YARA Rules, SARIF, and CI Policy Gates

> **译文：** 利用 NVIDIA SkillSpector、LangGraph、YARA Rules、SARIF 和 CI Policy Gates 构建高级 AI 技能安全审计管道

Agent skills are code you install from strangers. This walkthrough builds a synthetic skill marketplace with clean, risky, malicious and MCP-based examples, then scans each one through SkillSpector’s LangGraph inspection pipeline and keeps the evidence for every finding.

> **译文：** 代理技能是指您从陌生人处安装的代码。本教程构建了一个包含干净、有风险、恶意和基于 MCP 的示例的合成技能市场，然后使用 SkillSpector 的 LangGraph 检查流程扫描每个示例，并保留每次发现的证据。

It covers risk scores, categorized findings, confidence levels and analyzer completeness; SARIF and Markdown export; baseline suppressions that survive a deliberately introduced regression; organization-specific YARA rules; a custom secret analyzer added as an extra LangGraph node; and a CI gate that blocks on score, severity, confidence and rule id. The malicious sample exercises prompt injection, env harvesting, credential access and a staged exec chain. Needs Python >=3.12.

> **译文：** 它涵盖风险评分、分类结果、置信度级别和分析器完整性；SARIF 和 Markdown 导出；能够抵御故意引入的回归的基线抑制；特定于组织的 YARA 规则；作为额外 LangGraph 节点添加的自定义密钥分析器；以及一个基于评分、严重性、置信度和规则 ID 进行阻止的 CI 门控。恶意样本演示了提示注入、环境收集、凭证访问和分阶段执行链。需要 Python 3.12 或更高版本。

Read on Marktechpost →

· Full codes

· SkillSpector 07 · Moonshot · Eval tutorial

Evaluating Multimodal Vision Models with Moonshot PerceptionBench Using Robust Data Loading and Automated Judging

> **译文：** 利用 Moonshot PerceptionBench 进行多模态视觉模型评估，采用稳健的数据加载和自动评判

One overall accuracy score tells you a model is worse. It never tells you where. PerceptionBench measures fine-grained visual perception across OCR, counting, localization, contextual reasoning, comparison, depth understanding and hallucination detection, and this harness reports each capability separately.

> **译文：** 单一的总体准确率评分只能告诉你模型性能较差，却无法指出具体劣势所在。PerceptionBench 能够衡量精细的视觉感知能力，涵盖光学字符识别 (OCR)、计数、定位、上下文推理、比较、深度理解和幻觉检测等多个方面，并且该测试工具会分别报告每项能力的表现。

The pipeline handles resilient multi-stage dataset streaming, base64 image decoding and interleaved image placeholders, then runs three backends: a blind-prior baseline that needs no API key or GPU, OpenAI-compatible multimodal APIs, and local Hugging Face vision-language models. Judging is rule-based with optional LLM assistance, and results carry bootstrap confidence intervals broken out by capability, multi-image questions, image resolution and answer format.

> **译文：** 该流程可处理弹性多阶段数据集流、base64 图像解码和交错图像占位符，然后运行三个后端：一个无需 API 密钥或 GPU 的盲先验基线、兼容 OpenAI 的多模态 API 以及本地 Hugging Face 视觉语言模型。评判基于规则，并可选地使用 LLM 辅助，结果包含按能力、多图像问题、图像分辨率和答案格式细分的 bootstrap 置信区间。

Read on Marktechpost →

· Tutorial codes

Sponsored · Datalab

Marker v2: documents in, Markdown out — 76.0 on olmOCR-bench at 2.9 pages per second

> **译文：** Marker v2：文档输入，Markdown 输出 — 在 olmOCR-bench 测试中获得 76.0 分，速度为每秒 2.9 页

The story above about keeping the original applies to your ingestion layer too. Marker takes PDFs, scans, DOCX and PPTX and returns Markdown, JSON or HTML with tables, inline math and reading order intact — not a flattened text blob with the structure stripped out.

> **译文：** 上面关于保留原始文件的描述同样适用于您的数据导入层。Marker 可以读取 PDF、扫描件、DOCX 和 PPTX 文件，并返回 Markdown、JSON 或 HTML 文件，其中表格、行内公式和阅读顺序都保持完整——而不是结构被剥离的扁平化文本块。

Datalab rewrote Marker as a three-mode pipeline. Version 2 scores 76.0 on olmOCR-bench and sustains 2.9 pages per second on a single B200 — over 5x MinerU’s pipeline backend, and ahead of Docling on both accuracy and speed. Apache-2.0, fully open source.

> **译文：** Datalab 将 Marker 重写为一个三模式流水线。版本 2 在 olmOCR-bench 测试中获得 76.0 分，在单台 B200 打印机上可稳定达到每秒 2.9 页的处理速度——是 MinerU 流水线后端速度的 5 倍以上，并且在准确率和速度方面均优于 Docling。采用 Apache-2.0 许可，完全开源。

Get Marker on GitHub → datalab-to/marker → · Marker v2 vs MinerU, Docling, LiteParse

> **译文：** 在 GitHub 上获取 Marker → datalab-to/marker → · Marker v2 与 MinerU、Docling、LiteParse 的对比

One more thing…

Y Combinator · Agent harness

Y Combinator Open-Sources QM: An MIT-Licensed Multiplayer Agent Harness That Runs In Slack And The Web

> **译文：** Y Combinator 开源 QM：一款可在 Slack 和 Web 上运行的 MIT 许可多人代理框架

Most agents are designed as personal assistants. Stretch one assistant across a whole company and it gets complicated fast. QM does the opposite. Every person and every room gets its own scoped memory, files, keychain view, permissions, crons, web apps and durable sandbox. The same identity carries between Slack and the web app.

> **译文：** 大多数代理都被设计成个人助理。如果把一个助理扩展到整个公司，很快就会变得非常复杂。QM 则反其道而行之。每个人和每个房间都有自己专属的内存空间、文件、钥匙串视图、权限、定时任务、Web 应用和持久沙箱。Slack 和 Web 应用之间使用相同的身份。

Every turn runs through a headless core over Postgres, and the agent has a small fixed tool surface with one execute tool that runs inside the scope’s own sandbox. Pi, OpenCode, Codex and Claude Code all drive the same core, so a deployment is not tied to one vendor. Three org security postures gate tool calls — Strict pauses every harness tool call, Auto screens external data with a classifier, Dangerous removes both — and hard denials for recursive deletes and destructive SQL apply in all three.

> **译文：** 所有操作都通过基于 Postgres 的无头核心运行，代理程序拥有一个小型固定工具界面，其中包含一个在自身沙箱范围内运行的执行工具。Pi、OpenCode、Codex 和 Claude Code 都驱动同一个核心，因此部署并不依赖于单一供应商。三种组织安全策略控制工具调用——严格模式会暂停所有工具调用，自动模式会使用分类器筛选外部数据，危险模式则会移除所有外部数据——并且所有三种策略都强制禁止递归删除和破坏性 SQL 操作。

Here is the part that makes it worth the closer. YC runs QM across accounting, legal, events and engineering, including building QM itself — and still calls the release early and buggy. That is the honest version of a dogfooding claim.

> **译文：** 关键就在这里。YC 将 QM 应用于会计、法务、活动和工程等各个部门，包括 QM 本身的开发——即便如此，他们仍然承认 QM 版本发布过早且存在 bug。这才是真正诚实的“内部测试”声明。

Get QM on GitHub →

Read on Marktechpost → · Project page · Deployment · Threat model

> **译文：** 在 Marktechpost 上阅读更多内容 → · 项目页面 · 部署 · 威胁模型

Sponsor AI Dev Signals

Put your product in front of the people who build with it.

> **译文：** 把你的产品展示给那些使用它进行开发的人。

This list is engineers, researchers, and founders who read a release note before they read a press release. No banner farms, no interstitials. One sponsor per issue, written in your voice, placed where people are already reading.

> **译文：** 这份名单上的人员都是工程师、研究人员和创始人，他们会在阅读新闻稿之前先阅读产品发布说明。我们不投放横幅广告，也不投放插页式广告。每期只刊登一位赞助商的广告，广告文案会用您的语言撰写，并放置在读者经常阅读的位置。

Newsletter placements, article sponsorship, product launches, GitHub and Hugging Face repo promotion, and webinars. Tell us the goal and we will send the media kit and available dates.

> **译文：** 新闻稿发布、文章赞助、产品发布、GitHub 和 Hugging Face 代码库推广以及网络研讨会。请告诉我们您的目标，我们将发送媒体资料包和可预约日期。

Book a placement →

See one in action — this issue’s placement for Mend.io →

> **译文：** 看看实际应用——本期 Mend.io 的专题报道 →

🚀 Join the community

Reddit

·

X

·

LinkedIn

·

Telegram

▮ AI Dev Signals · by Marktechpost AI Media

Every number above is taken from the primary source and the Marktechpost coverage linked in each story, August 2026 — versions, access tiers and availability change fast.

> **译文：** 以上所有数字均来自主要来源和 Marktechpost 报道中链接的内容，截至 2026 年 8 月——版本、访问级别和可用性变化很快。

© 2026 Marktechpost AI Media Inc. All rights reserved.

> **译文：** © 2026 Marktechpost AI Media Inc. 保留所有权利。

Keep Reading

View more

The newsletter platform built for AI Devs

Subscribe© 2026 Marktechpost AI Media Inc.beehiivPowered by beehiiv

> **译文：** 订阅© 2026 Marktechpost AI Media Inc.beehiiv 由 beehiiv 提供技术支持