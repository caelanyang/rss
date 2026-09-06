# MARKTECHPOST: ARC Prize, Agentic AI, and Voice Upgrades

**来源：** Marktechpost AI  
**日期：** 2026-09-05  
**查看原邮件：** <https://mail.google.com/mail/u/1/#search/subject%3A%22MARKTECHPOST%3A%20ARC%20Prize%2C%20Agentic%20AI%2C%20and%20Voice%20Upgrades%22>

---

Hey there, This issue covers ARC Prize insights on OpenAI's Astra harness alongside major updates across Agentic AI, Physical AI, and AI Infrastructure, including releases like Meta's Muse Spark 1.3 and Anthropic's Claude 5.1 series. It also highlights advancements in Voice AI and ML/CV tools, featuring Google's Lyria 3.5, Microsoft's MAI-Image-2.6, and LlamaIndex's Extract Turbo.

> **译文：** 大家好，本期涵盖 ARC Prize 对 OpenAI Astra 测试框架的洞见，以及 Agentic AI、Physical AI 和 AI 基础设施领域的主要更新，包括 Meta 的 Muse
> Spark 1.3 和 Anthropic 的 Claude 5.1 系列等发布。本期还重点介绍了语音 AI 和 ML/CV 工具的进展，包括 Google 的 Lyria 3.5、Microsoft
> 的 MAI-Image-2.6 和 LlamaIndex 的 Extract Turbo。

Agentic AI

ARC Prize ran OpenAI's Astra twice on the same benchmark. Basic setup: 62.7%, $26,098. A setup that let the model keep its reasoning between steps: 98.6%, $17,332. Same model, same effort setting. Higher score, lower bill. The difference is the harness - the software giving a model its tools, memory and permissions. Agent = model + harness.

> **译文：** ARC Prize 在同一基准测试上运行了 OpenAI 的 Astra 两次。基础设置：62.7%，花费 $26,098。允许模型在步骤之间保留推理过程的设置：98.6%，花费
> $17,332。同一模型，同一努力程度设置。得分更高，费用更低。差异在于测试框架——即为模型提供工具、记忆和权限的软件。智能体 = 模型 + 测试框架。

Takeaway: A benchmark score belongs to a whole system, not the model on the box. Ask which harness produced it. No answer means no comparison.

> **译文：** 要点：基准测试得分属于整个系统，而非包装盒上的模型。要问是哪个测试框架产生了这个分数。没有答案就意味着无法比较。

Also this week

1. Meta AI Released Muse Spark 1.3: An Agentic Coding Model That Uses ~20% Fewer Tool Calls and ~25% Fewer Tokens Than Muse Spark 1.2

> **译文：** 1. Meta AI 发布 Muse Spark 1.3：一款 Agentic 编码模型，比 Muse Spark 1.2 减少约 20% 的工具调用和约 25% 的 Token 使用量

2. Anthropic Releases Claude Fable 5.1 and Claude Mythos 5.1: 52.6% on Terminal-Bench-Science and 75% Cheaper Cache Reads

> **译文：** 2. Anthropic 发布 Claude Fable 5.1 和 Claude Mythos 5.1：在 Terminal-Bench-Science 上取得 52.6% 的成绩，缓存读取成本降低
> 75%

3. OpenClaw Releases OpenClaw 2.0: Guided Model Setup, 575 ms Control UI Startup, and One Trust Boundary Per Gateway

> **译文：** 3. OpenClaw 发布 OpenClaw 2.0：引导式模型设置、575 毫秒控制界面启动，以及每个网关单一信任边界

4. Google introduces a new capability to our latest Gemini models: agentic video understanding. This allows developers to process long-form video content with more accuracy, while using up to 88% less tokens.

> **译文：** 4. Google 为最新的 Gemini 模型引入了一项新功能：智能体视频理解。这使得开发者能够更准确地处理长格式视频内容，同时最多可减少 88% 的 Token 使用量。

5. SpaceXAI Launches Grok Bot Marketplace for Instant AI Teammates

> **译文：** 5. SpaceXAI 推出 Grok Bot 市场，用于即时获取 AI 队友

6. Hermes Desktop now sets up local models in one click.

> **译文：** 6. Hermes Desktop 现已支持一键设置本地模型。

Physical AI

1. Generalist AI Releases GEN-1.5: A Robot Foundation Model That Learns New Tasks From One 3–12 Second Demo

> **译文：** 1. Generalist AI 发布 GEN-1.5：一款机器人基础模型，可从单个 3–12 秒的演示中学习新任务

2. Axis Robotics Open-Sources One of the Largest Franka Arm Simulation Datasets for Physical AI

> **译文：** 2. Axis Robotics 开源 Physical AI 领域最大的 Franka 机械臂仿真数据集之一

AI Infrastructure

1. Extropic Introduces Z1T Models for Energy-Efficient Thermodynamic AI Chips

> **译文：** 1. Extropic 推出 Z1T 模型，用于能效更高的热力学 AI 芯片

2. Perplexity Open Sources Lily: A Rust + Metal Inference Engine for Qwen3.6-35B-A3B on Apple Silicon

> **译文：** 2. Perplexity 开源 Lily：一款面向 Apple Silicon 上 Qwen3.6-35B-A3B 的 Rust + Metal 推理引擎

3. Unsloth AI GLM-5.3-Flash run 3.3x faster locally, Local GGUF inference is now 1.6–3.4× faster with optimized decoding and bonus multi-token prediction.

> **译文：** 3. Unsloth AI GLM-5.3-Flash 本地运行速度提升 3.3 倍，通过优化解码和额外的多 Token 预测，本地 GGUF 推理速度现已提升 1.6–3.4 倍。

4. Just announced at IFA, NVIDIA PAIR automatically links systems across your local network and sends inference requests wherever there’s available capacity, helping agents run more efficiently.

> **译文：** 4. 刚刚在 IFA 上宣布，NVIDIA PAIR 可自动连接本地网络中的系统，并将推理请求发送到任何有可用容量的位置，帮助智能体更高效地运行。

5. Meet Switchyard: A Rust Proxy and Library That Routes and Translates LLM Traffic Across OpenAI and Anthropic APIs

> **译文：** 5. 认识一下 Switchyard：一款 Rust 代理和库，可在 OpenAI 和 Anthropic API 之间路由和转换 LLM 流量

Voice AI

1. Lyria 3.5, Google’s best-sounding music generation model, is now available in AI Studio, via the Gemini API, and in the Gemini app

> **译文：** 1. Lyria 3.5，Google 音质最佳的音乐生成模型，现已在 AI Studio、Gemini API 和 Gemini 应用中提供

2. Phonely Launches Alma, a Voice LLM That’s 63% Faster and 84% Cheaper Than OpenAI

> **译文：** 2. Phonely 推出 Alma，一款比 OpenAI 快 63% 且便宜 84% 的语音 LLM

3. Google AI introduces three new voice-activated features that can change the way you use Google Workspace products

> **译文：** 3. Google AI 推出三项新的语音激活功能，可改变您使用 Google Workspace 产品的方式

4. Meta Superintelligence Labs Releases Muse Voice Transcribe: One Real-Time Model for Streaming ASR, Diarization, and Endpointing

> **译文：** 4. Meta Superintelligence Labs 发布 Muse Voice Transcribe：一款用于流式 ASR、说话人分离和端点检测的实时模型

ML/CV/Data Science/OCR

* Microsoft Releases MAI-Image-2.6, Tops Image AI Price-Quality Charts

> **译文：** * 微软发布 MAI-Image-2.6，登顶图像AI性价比排行榜

* Ant Group releases Ling-3.0-flash-VL, built on Ling-3.0-flash with visual understanding and visual agent capabilities.

> **译文：** * 蚂蚁集团发布 Ling-3.0-flash-VL，基于 Ling-3.0-flash 构建，具备视觉理解与视觉智能体能力。

* Google DeepMind’s WeatherNext 3 Trains on Weather Station Observations to Deliver 5 km Global Forecasts, Refreshed Every Hour

> **译文：** * 谷歌 DeepMind 的 WeatherNext 3 基于气象站观测数据训练，提供每5公里分辨率、每小时更新的全球预报

* Lama Index launched Extract Turbo: A super fast VLM-powered document extraction solution, 3-5x faster than all other comparable OCR solutions, including LlamaParse tiers.

> **译文：** * Llama Index 推出 Extract Turbo：一款超高速 VLM 驱动的文档提取解决方案，比所有其他同类 OCR 方案（包括 LlamaParse 各版本）快 3-5 倍。

* GitHub introduced Project HydraFusion (research preview) in Copilot, orchestrating multiple AI models to plan, build, critique, and complete coding tasks.

> **译文：** * GitHub 在 Copilot 中引入 Project HydraFusion（研究预览版），通过编排多个 AI 模型来规划、构建、评审并完成编码任务。

----------Until next week,

The Marktechpost Team