# 🚨 Muse Glimmer's 16-token block drafter, NVFP4 weights on one H100, and video in an 8× compressed latent

**来源：** Marktechpost AI (AI Dev Signals)  
**日期：** 2026-08-15  
**查看原邮件：** <https://mail.google.com/mail/u/1/#search/subject%3A%22%F0%9F%9A%A8%20Muse%20Glimmer%27s%2016-token%20block%20drafter%2C%20NVFP4%20weights%20on%20one%20H100%2C%20and%20video%20in%20an%208%C3%97%20compressed%20latent%22>

---

🚨 Muse Glimmer's 16-token block drafter, NVFP4 weights on one H100, and video in an 8× compressed latent

> **译文：** 🚨 Muse Glimmer 的 16 代币区块选牌器，NVFP4 权重在一个 H100 上，以及 8 倍压缩潜在视频

Home

Promotions

Home

Posts

🚨 Muse Glimmer's 16-token block drafter, NVFP4 weights on one H100, and video in an 8× compressed latent

> **译文：** 🚨 Muse Glimmer 的 16 代币区块选牌器，NVFP4 权重在一个 H100 上，以及 8 倍压缩潜在视频

🚨 Muse Glimmer's 16-token block drafter, NVFP4 weights on one H100, and video in an 8× compressed latent

> **译文：** 🚨 Muse Glimmer 的 16 代币区块选牌器，NVFP4 权重在一个 H100 上，以及 8 倍压缩潜在视频

3B active out of 30B. 4-bit weights in 24 GB at 1.0% degradation. An escalation router sending 7% of calls upstream. Six releases, zero new base models, and one paper arguing the metrics underneath all of it are broken.

> **译文：** 300亿用户中只有30亿用户处于活跃状态。24GB内存中4位权重数据性能下降1.0%。升级路由器将7%的呼叫发送到上游。发布了六个版本，没有新的基础模型，只有一篇论文指出所有这些底层指标都存在问题。

Aug 14, 2026

Together with NVIDIA

/

AI Dev Signals · August 13, 2026

Nobody scaled parameters this week.

Precision, decoding and routing did.

A 1M-hour human-video pre-training ladder. Two frontier updates that are post-training runs on a frozen base. A 30B MoE with 3B active behind an escalation router. And 30B weights quantized into 24 GB at 1.0% degradation.

> **译文：** 一个包含 100 万小时人类视频预训练的阶梯模型。两次前沿更新，是在冻结的基准模型上进行的训练后运行。一个 300 亿 MoE 集群，其中 30 亿处于激活状态，位于升级路由器之后。以及 300 亿权重被量化为 24 GB，降级率为 1.0%。

Presented by Mend.io Securing AI Agents, MCP Servers & LLM Apps — a practical see–fix–protect framework, with the checklists to start today. Get the guide →

> **译文：** 由 Mend.io 出品的《保护 AI 代理、MCP 服务器和 LLM 应用》——一套实用的“发现-修复-保护”框架，并附有可立即开始使用的检查清单。获取指南 →

Look at what shipped between August 10 and today. Not one lab announced a larger base model. SpaceXAI froze the Grok 4.5 foundation and spent the delta on a supplemental run, regenerated SFT trajectories and agentic RL. Google’s model card calls 3.7 Flash an algorithmic refinement of the reasoning foundation, not a new pretraining run. NVIDIA shipped a sparse 30B with 3B active, NVFP4 weights, multi-token prediction, and a router that decides when the frontier model is needed at all. Meta reached 24 GB through 4-bit quantization plus a 16-token block-diffusion drafter. LTX rebuilt the decoder and moved motion into an 8x compressed latent. Dyna scaled the pre-training corpus instead, four orders of magnitude of unlabelled human video. Parameter count was not the variable this week. Training stage, numeric precision, decode strategy and routing were.

> **译文：** 看看8月10日到今天这段时间都发布了哪些产品。没有一家实验室宣布推出更大的基础模型。SpaceXAI冻结了Grok 4.5的基础模型，并将节省下来的空间用于补充运行、重新生成SFT轨迹和智能强化学习。谷歌的模型卡片将3.7 Flash称为推理基础的算法改进，而不是新的预训练运行。NVIDIA发布了一个稀疏的30B模型，其中包含3B个活跃节点、NVFP4权重、多标记预测以及一个用于决定何时需要前沿模型的路由器。Meta通过4位量化和一个16标记块扩散草稿器达到了24GB的大小。LTX重建了解码器，并将运动信息转移到一个压缩了8倍的潜在数据中。Dyna则扩展了预训练语料库，增加了四个数量级的未标注人类视频。本周的重点不是参数数量，而是训练阶段、数值精度、解码策略和路由。

74% cost cut by routing

6.8s for ten seconds of video

24 GB holds a 30B agent

⭐ Featured · Sponsored by NVIDIA

LTX · Open weights world model

The Video Production Stack Now Fits on One Desk: LTX-2.5 Launches as NVIDIA-Accelerated Open Weights World Model

> **译文：** 视频制作全套设备现在都能放在一张桌子上：LTX-2.5 作为 NVIDIA 加速的 Open Weights World 模型发布。

The render farm was the studio door. LTX-2.5 is an open weights world model for video generation, real-time applications and physical AI, optimized for local inference on NVIDIA RTX GPUs and DGX Spark. VRAM requirements are cut far enough that a frontier world model runs on hardware creators already own, and additional clips carry no per-generation fee or metered credit.

> **译文：** 渲染农场就是工作室的入口。LTX-2.5 是一款开放权重世界模型，适用于视频生成、实时应用和物理人工智能，并针对 NVIDIA RTX GPU 和 DGX Spark 上的本地推理进行了优化。其显存需求大幅降低，使得这款前沿世界模型能够在创作者已有的硬件上运行，而且额外的片段无需按生成次数付费或按流量计费。

The speed number is the one to hold onto. In LTX’s published image-to-video benchmark, a 10-second clip takes 6.8 seconds on-prem running on 2x NVIDIA GB200 , and 23.7 seconds through the LTX API. The fastest closed alternatives listed — Omni Flash, Grok 1.5, Veo 3.1 — land at 52 to 70 seconds. Seedance 2.0 is 196, FLUX 3 is 259, Seedance 2.5 is 317, and Kling 3.0 Pro is 398. On-prem, generation finishes faster than the clip’s own runtime.

> **译文：** 速度才是关键。在 LTX 公布的图像转视频基准测试中，一段 10 秒的视频片段在本地部署的 2 块 NVIDIA GB200 显卡上运行耗时 6.8 秒，而通过 LTX API 则耗时 23.7 秒。列出的速度最快的封闭式替代方案——Omni Flash、Grok 1.5 和 Veo 3.1——耗时 52 到 70 秒。Seedance 2.0 耗时 196 秒，FLUX 3 耗时 259 秒，Seedance 2.5 耗时 317 秒，Kling 3.0 Pro 耗时 398 秒。在本地部署中，视频生成速度甚至比视频片段本身的运行时间还要快。

LTX rebuilt the pipeline rather than bolting features onto an older core. A new diffusion video decoder cuts artifacts in high-motion scenes while holding the high compression ratio. Native multishot renders a full sequence as one output, keeping character, scene and voice consistent across cuts, on a custom Gemma 4 language backbone with a dedicated prompt enhancer. Diffusion Fidelity Rendering builds motion and structure in an 8x temporally compressed latent space, then generates high-fidelity keyframes to anchor detail, with keyframe count adapting to scene complexity and compute budget.

> **译文：** LTX 重构了整个渲染管线，而非在旧核心上简单地添加新功能。全新的扩散视频解码器能够有效减少高运动场景中的伪影，同时保持高压缩比。原生多镜头渲染技术能够将整个序列渲染为一个输出，确保角色、场景和语音在不同镜头间保持一致，其底层语言采用定制的 Gemma 4，并配备了专用的提示增强器。扩散保真渲染技术在 8 倍时间压缩的潜在空间中构建运动和结构，然后生成高保真关键帧来锚定细节，关键帧数量会根据场景复杂性和计算预算进行调整。

A separate pretrained physical AI checkpoint gives robotics teams a fine-tuning base for non-cinematic domain data, and a stronger distilled model targets production-volume deployment. LTX describes the family as the most used open world model, with more than 33 million downloads. Weights ship on Hugging Face, natively in ComfyUI on day one, and through the LTX API — free for organizations under $10M in annual recurring revenue, with full control of hardware, customization and IP.

> **译文：** 一个独立的预训练物理AI检查点为机器人团队提供了一个针对非电影领域数据的微调基础，而更强大的精简模型则面向生产规模部署。LTX称该模型系列是使用最广泛的开放世界模型，下载量超过3300万次。权重数据在Hugging Face上发布，在ComfyUI发布首日即可原生使用，并通过LTX API提供——年经常性收入低于1000万美元的企业可免费使用，并拥有对硬件、定制和知识产权的完全控制权。

Read the full breakdown →

Read on Marktechpost →

· Announcement

· GitHub

· Hugging Face

· Docs

· NVIDIA local AI series

Disclosure: Marktechpost’s coverage of this release was sponsored by NVIDIA. All performance figures above are LTX’s own published numbers.

> **译文：** 声明：Marktechpost 对此次发布的报道由 NVIDIA 赞助。以上所有性能数据均为 LTX 自行公布的数据。

🔥 The signals

01 · Dyna Robotics · Robotics

Dyna Robotics Introduces Dyna-2: A World-Action Model Pre-Trained on 1 Million Hours of Human Video

> **译文：** Dyna Robotics推出Dyna-2：一款基于100万小时人类视频预训练的世界动作模型

Robot learning has been bottlenecked by action-labelled data, and that data has to be deliberately produced by teleoperation. One arm, one operator, one demonstration at a time. Dyna-2 asks whether video of people doing ordinary things — footage nobody had to stage — can stand in for it.

> **译文：** 机器人学习一直受限于动作标注数据，而这些数据必须通过远程操作刻意生成。每次只能进行一次演示，由一名操作员、一个机械臂完成。Dyna-2 项目旨在探究，人们进行日常活动的视频——无需任何人为安排的素材——是否可以替代动作标注数据。

Pre-training used more than one million hours of egocentric human video, roughly 170 years of continuous waking experience. On a nested ladder from 1,000 to 1,000,000 hours, mean normalized score across 14 post-trained tasks rose 20% → 28% → 45% → 53%. The law transfers: zero-shot action MSE on 39 robot tasks the model never saw fits 0.306·D^-0.0713 . Joint video-and-action denoising beat action-only on 39 of 39 tasks at every action scale. No weights and no API — deployment today means buying a vendor-operated Dyna robot cell.

> **译文：** 预训练使用了超过一百万小时的以自我为中心的人类视频，相当于大约170年的连续清醒状态经验。在从1000小时到100万小时的嵌套阶梯中，14项后训练任务的平均归一化得分分别提高了20%、28%、45%和53%。该规律具有迁移性：模型从未接触过的39项机器人任务的零样本动作均方误差(MSE)符合0.306·D^-0.0713。在所有39项任务中，视频和动作联合去噪在所有动作尺度上均优于仅动作去噪。无需权重和API——如今部署该模型意味着购买由供应商运营的Dyna机器人单元。

Read on Marktechpost →

· Technical report

· Announcement

· xdof ABC eval set

02 · SpaceXAI · Frontier model

SpaceXAI Releases Grok 4.6: A 500K-Context Frontier Model Tuned for Long-Running Agents, Coding, and Knowledge Work

> **译文：** SpaceXAI 发布 Grok 4.6：一个针对长时间运行的智能体、编码和知识工作优化的 50 万上下文前沿模型

The base model did not change. SpaceXAI held the foundation constant and spent the improvement on a longer supplemental training run, regenerated supervised fine-tuning trajectories, and reinforcement learning in agentic environments. A generational bump without a new pre-training bill.

> **译文：** 基础模型并未改变。SpaceXAI 保持了模型的基本架构不变，并将改进的重点放在了更长时间的补充训练、重新生成监督式微调轨迹以及在智能体环境中进行强化学习上。这相当于在无需额外预训练成本的情况下实现了性能的代际提升。

It scores 61 on the Artificial Analysis Intelligence Index, up from 56, tied with GPT-5.6 Sol Max. 500K context, text and image in, and a new xhigh reasoning-effort level. Read the losses first: DeepSWE v1.1 lands at 65.9% against 73% for GPT-5.6 Sol Max, and Terminal-Bench v3.0 at 26% is last of the four models listed. The bolded wins on GDPval-AA v2 and AA-Briefcase sit inside Artificial Analysis’ confidence intervals, and Claude Opus 5 is absent from the comparison set. Pricing is $2 / $6 per 1M below 200K prompt tokens, doubling above it. No open weights.

> **译文：** 它在人工智能分析智能指数 (AII) 上的得分从 56 分上升至 61 分，与 GPT-5.6 Sol Max 并列。该模型包含 50 万个上下文、文本和图像，并采用了全新的 xhigh 推理难度级别。首先来看它的不足之处：DeepSWE v1.1 的得分为 65.9%，而 GPT-5.6 Sol Max 的得分为 73%；Terminal-Bench v3.0 的得分仅为 26%，在列出的四个模型中排名垫底。在 GDPval-AA v2 和 AA-Briefcase 测试中以粗体显示的得分均在人工智能分析的置信区间内，而 Claude Opus 5 则未包含在比较集中。定价为：低于 20 万个提示代币时，每百万个代币 2 美元/6 美元；高于 20 万个提示代币时，价格翻倍。目前没有开放权重。

Read on Marktechpost →

· Announcement

· Docs

· Release notes

03 · Google DeepMind · Model pricing

Google AI Just Released Gemini 3.7 Flash: A Coding and Agent Model at $0.75/1M Input Tokens

> **译文：** Google AI刚刚发布了Gemini 3.7 Flash：一个编码和代理模型，每百万输入令牌收费0.75美元。

The same move, one day later, at a different lab. The model card describes 3.7 Flash as a refinement of 3.6 Flash with algorithmic improvements to the core reasoning foundation — not a new pretraining run. Three weeks separate the two releases.

> **译文：** 一天后，在另一个实验室也进行了同样的操作。模型卡片将 3.7 Flash 描述为 3.6 Flash 的改进版，改进之处在于核心推理基础的算法——而不是新的预训练。这两个版本发布间隔三周。

The coding gains are real. FrontierCode 1.1 Main goes from 34.4% to 43.6%, DeepSWE v1.1 reaches 65.3%, and WebDev Arena posts 1588 Elo against 1538. AutomationBench moves from 17.0% to 30.4%, ahead of Claude Sonnet 5 at 10.7% and GPT-5.6 Terra at 23.6%. But price is the argument: $0.75 / $3.75 per 1M tokens, introductory until December 31, 2026, then $1.50 / $7.50. GPT-5.6 Terra still leads DeepSWE, Terminal-bench and OSWorld-2.0, and CharXiv Reasoning regressed slightly to 84.5%. API and enterprise only — nothing to self-host.

> **译文：** 编码能力的提升是实实在在的。FrontierCode 1.1 Main 的准确率从 34.4% 提升至 43.6%，DeepSWE v1.1 达到 65.3%，WebDev Arena 的 Elo 评分从 1538 提升至 1588。AutomationBench 的准确率从 17.0% 提升至 30.4%，领先于 Claude Sonnet 5（10.7%）和 GPT-5.6 Terra（23.6%）。但价格才是关键：每百万代币 0.75 美元/3.75 美元，优惠期至 2026 年 12 月 31 日，之后价格将调整为 1.50 美元/7.50 美元。GPT-5.6 Terra 仍然领先于 DeepSWE、Terminal-bench 和 OSWorld-2.0，而 CharXiv Reasoning 的准确率略有回落至 84.5%。仅限 API 和企业版——不支持自托管。

Read on Marktechpost →

· Announcement

· Model card

· API docs

Sponsored · Mend.io

Securing AI Agents, MCP Servers & LLM Apps: A Practical Framework

> **译文：** 保障人工智能代理、MCP 服务器和 LLM 应用的安全：一个实用的框架

Agents, MCP integrations, and LLM-powered apps are entering codebases faster than security programs can track them — and their behavior isn’t defined by code alone. This guide gives AI/ML engineers, platform engineers, and AppSec teams a practical see–fix–protect framework, with the checklists and templates to start today.

> **译文：** 代理、MCP 集成和 LLM 驱动的应用程序正以远超安全程序追踪速度的速度涌入代码库——而且它们的行为并非仅由代码决定。本指南为 AI/ML 工程师、平台工程师和应用安全团队提供了一个实用的“发现-修复-保护”框架，其中包含可立即上手使用的清单和模板。

Inside: the agentic AI attack surface map across five layers, from prompt injection to poisoned MCP tools. A 12-point misconfiguration checklist covering agent and MCP permission and config checks. Triage at AI speed — what to automate, what to keep human. Runtime guardrail architectures, prompt hardening, and policy enforcement for AI in production. Plus an agentic AI maturity roadmap: a self-assessment aligned to NIST AI RMF, OWASP AIMA, ISO/IEC 42001, and the EU AI Act.

> **译文：** 内容包括：涵盖五层架构的智能体人工智能攻击面图，从即时注入到恶意MCP工具；一份包含12项配置错误的检查清单，涵盖智能体和MCP的权限和配置检查；以人工智能的速度进行分类——哪些操作自动化，哪些操作需要人工处理；运行时防护架构、即时强化以及生产环境中人工智能的策略执行；以及智能体人工智能成熟度路线图：一份符合NIST AI RMF、OWASP AIMA、ISO/IEC 42001和欧盟人工智能法案的自评估工具。

Get the framework →

Download the guide → · Our writeup of the framework

> **译文：** 下载指南 → · 我们撰写的框架说明

04 · NVIDIA · Agent infrastructure

NVIDIA AI Releases Nemotron 3.5 Lightning: A 30B Open MoE with 3B Active Parameters, and NeMo Switchyard Model Router

> **译文：** NVIDIA AI 发布 Nemotron 3.5 Lightning：一款拥有 30 位开放式 MoE 和 30 位活动参数的路由器，以及 NeMo Switchyard 模型路由器

Long-running agents spend most of their token budget on tool calls, result validation, and subagent delegation. Every one of those steps goes to a frontier reasoning model by default. Two artifacts shipped together to break that default: a small model for the execution layer, and a router that decides when the expensive model is actually needed.

> **译文：** 长时间运行的智能体会将大部分令牌预算用于工具调用、结果验证和子智能体委托。默认情况下，这些步骤都会调用一个前沿推理模型。为了打破这种默认设置，我们同时提供了两个组件：一个用于执行层的小型模型，以及一个用于判断何时真正需要调用高成本模型的路由器。

Lightning is a 30B mixture-of-experts with 3B active parameters on a hybrid Mamba-2 + MoE + Attention stack, 1M-token context, pre-trained on more than 20 trillion tokens with an NVFP4 recipe. NVIDIA reports up to 4x output speed against similar-sized models, and 86% accuracy on PinchBench while completing 10,000 tasks 30% faster than Qwen3.6 35B. Switchyard is the other half: LangChain benchmarked 145 multi-turn agentic tasks, and the escalation router cut cost 74% versus a frontier-only baseline while sending 7% of calls to the frontier model, at roughly a 6-point accuracy tradeoff. OpenMDW-1.1, commercial use permitted, single-GPU on 1x DGX Spark or 1x H100.

> **译文：** Lightning 是一个包含 300 亿个专家混合模型，拥有 30 亿个活跃参数，采用 Mamba-2 + MoE + Attention 混合技术栈，处理 100 万个 token 的上下文，并使用 NVFP4 配方在超过 20 万亿个 token 上进行预训练。NVIDIA 报告称，与类似规模的模型相比，其输出速度最高可达 4 倍，在 PinchBench 测试中准确率达到 86%，完成 10,000 个任务的速度比 Qwen3.6 350 快 30%。Switchyard 是另一半：LangChain 对 145 个多轮代理任务进行了基准测试，结果表明，升级路由器在将 7% 的调用发送到前端模型的同时，将成本降低了 74%（相比仅使用 frontier 模型的基准），准确率损失约为 6 个百分点。OpenMDW-1.1 允许商业用途，支持单 GPU，可在 1 个 DGX Spark 或 1 个 H100 上运行。

Read on Marktechpost →

· Hugging Face

· Switchyard GitHub

· NVIDIA blog

· LangChain benchmark

05 · Meta AI · Local agents

Meta AI Releases Muse Glimmer: A 30B Open-Weights Agentic Model That Runs on One Consumer GPU

> **译文：** Meta AI 发布 Muse Glimmer：一款可在单张消费级 GPU 上运行的 300 亿开放权重智能体模型

A 30B model needs over 55 GB at full precision, which is a datacenter conversation. Meta compressed it to roughly 4-bit and added block-level speculative decoding, so it answers fast enough to sit inside a real agent loop on one card, with no network call. Apache 2.0, distilled from Muse Spark.

> **译文：** 一个 30 亿位的模型在全精度下需要超过 55 GB 的空间，这已经是数据中心级别的开销了。Meta 将其压缩到大约 4 位，并添加了块级推测解码，因此响应速度足够快，可以运行在单卡上的真实代理循环中，无需网络调用。基于 Apache 2.0，源自 Muse Spark。

Two quantized builds ship: K-Quant-Dynamic targets 32 GB VRAM at 0.2% average degradation, K-Quant-17GB targets 24 GB at 1.0%, averaged across 15 common benchmarks. Speed comes from DFlash, a block-diffusion drafter predicting 16 tokens per forward pass — on an RTX 5090 throughput moves from 74.9 to 233.4 tok/s, a 3.1x speedup; Apple M5 Max goes 26.6 to 50.2. Against Gemma4-31B and Qwen3.6-27B it leads MCP Atlas at 75.5 versus 54.2 and 62.5, DeepSearch QA at 74.6, and SWE-Bench Pro at 51.2. It trails Qwen3.6-27B on OSWorld-Verified (65.9 against 75.6) and TerminalBench 2.1. The pattern holds: wins on agentic orchestration, losses on computer-use and terminal work.

> **译文：** 提供两种量化版本：K-Quant-Dynamic 目标使用 32 GB 显存，平均性能下降 0.2%；K-Quant-17GB 目标使用 24 GB 显存，平均性能下降 1.0%（基于 15 项常用基准测试）。速度提升主要得益于 DFlash，这是一款块扩散式数据提取器，每次前向传播可预测 16 个令牌——在 RTX 5090 上，吞吐量从 74.9 tok/s 提升至 233.4 tok/s，速度提升 3.1 倍；在 Apple M5 Max 上，吞吐量从 26.6 tok/s 提升至 50.2 tok/s。在与 Gemma4-31B 和 Qwen3.6-27B 的对比中，其在 MCP Atlas 测试中以 75.5 的成绩领先于 54.2 和 62.5，在 DeepSearch QA 测试中以 74.6 的成绩领先，在 SWE-Bench Pro 测试中以 51.2 的成绩领先。在 OSWorld-Verified (65.9 对 75.6) 和 TerminalBench 2.1 测试中，它落后于 Qwen3.6-27B。模式依然成立：在代理编排方面表现出色，但在计算机使用和终端工作方面则表现不佳。

Read on Marktechpost →

· Meta blog

· Hugging Face

· Model details

· DFlash paper

From Marktechpost · our own repo

Same theme, smaller scale: Token Saver keeps a 200-page PDF out of the context window and hands the model a page-cited slice instead. MIT, one-click .mcpb for Claude Desktop, retrieval recall@5 of 0.90 on 30 gold questions, and the eval you can re-run yourself. Star it on GitHub →

> **译文：** 同样的主题，规模更小：Token Saver 将 200 页的 PDF 文件从上下文窗口中移除，而是向模型提供页码引用的片段。MIT 许可，一键生成适用于 Claude Desktop 的 .mcpb 文件，在 30 个黄金问题上检索召回率达到 0.90（5 次检索），并且您可以自行重新运行评估。在 GitHub 上为它点赞 →

One more thing…

Xiaomi MiLM Plus · Evaluation

Xiaomi’s MiLM Plus Releases PROVE: Perception-Aligned Object Removal Metrics RC-S and RC-T With a Real-World Video Benchmark

> **译文：** 小米 MiLM Plus 发布 PROVE：感知对齐物体移除指标 RC-S 和 RC-T，并提供真实世界视频基准测试

Every story above made something cheaper. This one asks whether you would notice if cheaper made it worse. Object removal models have improved faster than the metrics used to judge them, and the reason is structural: erasure is ill-posed and one-to-many, so no single ground truth exists to compare against.

> **译文：** 以上每个案例都旨在降低成本。而本文则提出这样一个问题：如果成本降低导致性能下降，你是否能够察觉？对象移除模型的改进速度远超用于评价它们的指标，其原因在于结构性问题：擦除操作本身就是一个不适定问题，且涉及一对多关系，因此不存在一个可供比较的单一标准。

The consequences are specific and uncomfortable. PSNR, SSIM and LPIPS assume point-to-point correspondence, so they reward copy-paste over genuine erasure, and residual shadows occupy too few pixels to be penalized. Cutting diffusion inference steps improves PSNR and SSIM while visual quality collapses. On ROSE-Bench, progressively blurring the masked region degrades neither ReMOVE nor CFD — both eventually score better than their own unblurred baselines.

> **译文：** 其后果具体而令人不安。PSNR、SSIM 和 LPIPS 假设点对点对应，因此它们奖励复制粘贴而非真正的擦除，而残留阴影所占像素太少，无法进行惩罚。减少扩散推理步骤可以提高 PSNR 和 SSIM，但视觉质量会急剧下降。在 ROSE-Bench 测试中，逐步模糊掩蔽区域既不会降低 ReMOVE 也不会降低 CFD 的性能——最终两者的得分都优于各自未模糊的基线。

PROVE’s answer is local distribution matching instead of global aggregation. RC-S and RC-T score only the edited region, using sliding-window Maximum Mean Discrepancy over DINOv2 features, and neither needs a reference video. Against human rankings from 20 participants, RC-S reaches 0.59 average Kendall’s τ and 0.66 Spearman’s ρ , against 0.26/0.29 for ReMOVE and 0.16/0.18 for CFD. It prefers the clean image over blurred and region-swapped variants in 100% of RORD-Val cases, runs at 134.6 ms/frame on one RTX 4090, and is 13.7x cheaper than CFD. Apache 2.0, accepted at ACM MM 2026.

> **译文：** PROVE 的答案是局部分布匹配而非全局聚合。RC-S 和 RC-T 仅对编辑区域进行评分，使用基于 DINOv2 特征的滑动窗口最大均值差异 (MSID)，且均不需要参考视频。与 20 位参与者的人工评分相比，RC-S 的平均 Kendall's τ 值为 0.59，Spearman's ρ 值为 0.66，而 ReMOVE 和 CFD 的相应值分别为 0.26/0.29 和 0.16/0.18。在 100% 的 RORD-Val 测试中，RC-S 都优先选择干净的图像而非模糊或区域交换的变体。在单张 RTX 4090 显卡上，RC-S 的运行时间为 134.6 毫秒/帧，比 CFD 的计算成本低 13.7 倍。该算法已获得 Apache 2.0 许可，并被 ACM MM 2026 接收。

Get the code →

Read on Marktechpost → · Paper · Project page · PROVE-Bench dataset

> **译文：** 在 Marktechpost 上阅读更多内容 → · 论文 · 项目页面 · PROVE-Bench 数据集