# The 276B AI model that beats its 975B teacher — on one GPU



**来源：** Marktechpost AI (AI Dev Signals)  

**日期：** 2026-08-03  

**查看原邮件：** <https://mail.google.com/mail/u/1/#search/subject%3A%22The%20276B%20AI%20model%20that%20beats%20its%20975B%20teacher%20%E2%80%94%20on%20one%20GPU%22>



---



AI DEV SIGNALS · AUGUST 3, 2026

Eight releases. One question. What can you actually run?

> **译文：** 八个版本。一个问题：你到底能运行哪些程序？

A 2.4-trillion-parameter flagship you rent, a 276B model that fits on one GPU, a cyber model you cannot download at all, a video model whose weights are still in transit — and one pipeline you can run start to finish today.

> **译文：** 一个拥有 2.4 万亿个参数的旗舰模型可供租用，一个 2760 亿的模型可以安装在一个 GPU 上，一个网络模型根本无法下载，一个权重仍在传输中的视频模型——以及一个今天就可以从头到尾运行的流水线。

Every release this week splits in two: the thing announced and the thing you can run. Qwen announces 2.4 trillion parameters; the deployable artifact is an API today and a 27B checkpoint later. Cogent announces a frontier cyber model; the deployable piece is the harness around it. AMD open-sources everything except commercial rights. Read each story for the second half.

> **译文：** 本周的每个版本都分为两部分：发布内容和可运行版本。Qwen 宣布拥有 2.4 万亿个参数；目前可部署的组件是一个 API，稍后会推出一个 270 亿的检查点。Cogent 发布了前沿网络安全模型；可部署的组件是围绕该模型构建的框架。AMD 开源了除商业权利之外的所有内容。请阅读每篇文章的后半部分。

2.4T — Qwen3.8-Max total parameters. 180 GB — Inkling-Small NVFP4 VRAM floor. 0.630 — Ontology 1 P@10 score.

> **译文：** 2.4T — Qwen3.8-Max 总参数。180 GB — Inkling-Small NVFP4 显存最低要求。0.630 — Ontology 1 P@10 得分。

01 · ALIBABA QWEN · FRONTIER MOE

Alibaba Qwen Releases Qwen3.8-Max: A 2.4 Trillion Parameter MoE Model and the Most Capable One in the Qwen Family to Date

> **译文：** 阿里巴巴Qwen发布Qwen3.8-Max：参数规模达2.4万亿的Qwen系列迄今为止性能最强的产品

A frontier flagship used to mean a closed API and nothing else. Qwen3.8-Max ships as a hosted, OpenAI-compatible endpoint today — and Alibaba says the open weights follow next week, alongside an open Qwen3.8-27B. The 27B, not the 2.4T flagship, is the checkpoint that fits ordinary on-premise hardware.

> **译文：** 过去，旗舰级产品通常意味着封闭的API，除此之外别无其他。而Qwen3.8-Max今天以托管式、兼容OpenAI的端点形式发布——阿里巴巴表示，下周将推出开放权重，以及开放的Qwen3.8-27B。需要注意的是，Qwen3.8-27B（而非2.4T旗舰版）才是适用于普通本地部署硬件的基准测试产品。

Context runs to 1M tokens. Pricing is $2.00 input and $6.00 output per 1M tokens, with implicit cache reads at $0.25 — cached input is eight times cheaper than fresh, so prefix stability drives cost more than prompt length. It scores 86.6 on Terminal-Bench 2.1, and against its own predecessor FrontierSWE jumps from 40.7 to 73.5. The activated-parameter count is still undisclosed, so open-weights serving cost cannot yet be modeled.

> **译文：** Context 的运行规模为 100 万个代币。定价为每 100 万个代币的输入 2 美元，输出 6 美元，隐式缓存读取成本为 0.25 美元——缓存输入比全新输入便宜八倍，因此前缀稳定性比提示符长度更能影响成本。它在 Terminal-Bench 2.1 上的得分为 86.6，与它的前身 FrontierSWE 相比，得分从 40.7 跃升至 73.5。激活参数的数量尚未公开，因此目前还无法对开放权重服务成本进行建模。

02 · THINKING MACHINES LAB · OPEN WEIGHTS

Thinking Machines Lab Releases Inkling-Small: A 276B Total, 12B Active Open Weights Multimodal MoE Model

> **译文：** Thinking Machines Lab 发布 Inkling-Small：一个包含 2760 亿个总权重、120 亿个有效开放权重的多模态 MoE 模型

The student beat the teacher. Inkling-Small is a quarter the size of the 975B Inkling, distilled from it in part — and it comes out ahead on SWE-bench Verified at 80.2% versus 77.6%, on Humanity's Last Exam at 31.6% versus 29.7%, and on ARC-AGI-2 at 40.1% versus 36.5%. Weights ship under Apache 2.0.

> **译文：** 学生战胜了老师。Inkling-Small 的大小只有 975B Inkling 的四分之一，部分代码源自后者——并且在 SWE-bench Verified 测试中表现更佳，得分分别为 80.2% 和 77.6%；在 Humanity's Last Exam 测试中得分分别为 31.6% 和 29.7%；在 ARC-AGI-2 测试中得分分别为 40.1% 和 36.5%。权重基于 Apache 2.0 协议发布。

The deployment story is the NVFP4 checkpoint: 180 GB aggregated VRAM on a single B300, against 600 GB for BF16. It reasons natively over text, images and audio with a 1M-token context. The honest trade: factual recall regressed, with SimpleQA Verified falling to 20.6% from Inkling's 43.9%.

> **译文：** 部署方面，NVFP4 是一个关键节点：单台 B300 显卡集成了 180 GB 的 VRAM，而 BF16 则需要 600 GB。它能够原生处理文本、图像和音频，并支持 100 万个令牌的上下文。但需要注意的是：事实回忆率有所下降，SimpleQA 验证率从 Inkling 的 43.9% 降至 20.6%。

03 · COGENT · SECURITY

Cogent AI Team Releases VR-1: A Frontier Cyber Reasoning Model That Composes and Verifies Enterprise Attack Paths

> **译文：** Cogent AI团队发布VR-1：一款前沿网络推理模型，可构建并验证企业攻击路径

Most cyber benchmarks reward describing an attack. IntrusionBench, released alongside VR-1, scores nothing for narration — the agent has to execute the chain and produce checkable evidence. VR-1 is post-trained for exactly that: investigating under partial information, composing evidence across cloud, identity, code and CI/CD, and verifying the actual objective.

> **译文：** 大多数网络安全基准测试都侧重于描述攻击过程。与 VR-1 一同发布的 IntrusionBench 对描述攻击过程不予评分——智能体必须执行攻击链并生成可验证的证据。VR-1 正是为此而进行后训练：在信息不完整的情况下进行调查，整合来自云端、身份、代码和 CI/CD 的证据，并验证攻击的实际目标。

Cogent reports roughly twice as many proven attack paths at about a quarter of the cost, measured as black-box pass@3 against Kimi K3, Claude Opus 4.8 and GLM-5.2 — and says plainly that harness-matched, the gap nearly closes, and its own black-box success rate stays under 30%. The model is gated to vetted enterprises; the model-agnostic AI Harness is the broadly deployable piece.

> **译文：** Cogent 报告称，其已验证的攻击路径数量约为其他方案的两倍，而成本却只有四分之一左右（以针对 Kimi K3、Claude Opus 4.8 和 GLM-5.2 的黑盒 pass@3 测试结果衡量）。Cogent 还明确指出，如果配合相应的 AI Harness，两者的差距几乎可以忽略不计，其自身的黑盒测试成功率也保持在 30% 以下。该模型仅限经过审核的企业使用；而与模型无关的 AI Harness 则是可广泛部署的组件。

04 · ONTON · SEARCH

Onton Releases Ontology 1: A Neurosymbolic Search Model That is 2.7x More Accurate than the World's Best E-commerce Search Engines

> **译文：** Onton发布本体1：一种神经符号搜索模型，其准确率比全球最佳电子商务搜索引擎高2.7倍

There is no product filter for "pet-friendly." Ontology 1 does not trust the seller's label either — it reasons from properties more likely to be objective, like fiber, weave and construction, in an explicit knowledge graph you can inspect, and flags claims the product data contradicts.

> **译文：** 没有“宠物友好型”的产品筛选器。本体1也不信任卖家的标签——它基于更客观的属性进行推理，例如纤维、编织方式和结构，这些属性都存储在一个您可以查看的显式知识图谱中，并标记出与产品数据相矛盾的说法。

On Subtext-Decor-90, scored by three independent LLM judges, it reaches P@10 0.630 against Google Shopping's 0.543 and Amazon's 0.469 — while indexing roughly 1% of their catalogs, winning 52 of 90 queries outright. Judge agreement is modest (Krippendorff's alpha 0.465), but all three judges rank the engines identically. Live on Onton.com; no public API or open weights.

> **译文：** 在由三位独立的LLM评委评分的Subtext-Decor-90数据集上，该搜索引擎的P@10得分达到0.630，高于Google Shopping的0.543和Amazon的0.469——尽管其索引的商品目录仅占Google Shopping和Amazon商品目录的约1%，但在90次查询中却赢得了52次。评委间的一致性不高（Krippendorff's alpha值为0.465），但三位评委对该搜索引擎的排名完全一致。该搜索引擎已上线Onton.com；目前没有公开的API或权重数据。

05 · AMD · FULLY OPEN MOE

AMD Releases Instella-MoE-16B-A3B: A Fully Open Mixture-of-Experts LLM With 2.8B Active Parameters Trained On Instinct GPUs

> **译文：** AMD发布Instella-MoE-16B-A3B：一款完全开放的混合专家LLM模型，拥有28亿个活跃参数，基于Instinct GPU进行训练。

Most "open" releases give you a checkpoint. AMD is publishing weights from every training stage, plus data mixtures, training configs and inference code — a complete end-to-end MoE recipe trained from scratch on Instinct MI300X and MI325X. The model holds 16B total parameters and activates 2.8B per token: 2 shared experts plus 6 routed from 64.

> **译文：** 大多数“开源”版本都会提供一个检查点。AMD 发布了每个训练阶段的权重，以及数据混合、训练配置和推理代码——一个完整的端到端 MoE 模型，该模型在 Instinct MI300X 和 MI325X 上从零开始训练。该模型总共包含 160 亿个参数，每个 token 激活 28 亿个参数：2 个共享专家加上从 64 个专家中路由的 6 个。

Gated MLA and FarSkip-Collective deliver a 12.7% pre-training speedup and up to 39.2% lower time to first token under expert parallelism. The base checkpoint averages 76.7, the strongest among fully open models. The catch: weights ship under a research-only ResearchRAIL license — the MIT-licensed training code is the more reusable asset.

> **译文：** 门控 MLA 和 FarSkip-Collective 可实现 12.7% 的预训练速度提升，并在专家并行处理下将首次获取 token 的时间缩短高达 39.2%。基础检查点平均性能为 76.7，在所有完全开源的模型中表现最佳。需要注意的是：权重以仅供研究使用的 ResearchRAIL 许可证发布——而采用 MIT 许可证的训练代码才是更具可重用的资源。

06 · SUPABASE · AGENT EVALS

Supabase Releases Evals: an Open Source Benchmark That Scores Claude Code, Codex and OpenCode on Real Supabase Tasks

> **译文：** Supabase 发布评估报告：一个开源基准测试，用于评估 Claude Code、Codex 和 OpenCode 在实际 Supabase 任务上的性能

Most agent benchmarks run against mocks. Every Supabase Evals scenario boots a real containerized stack — agents call the actual MCP server and CLI, then get scored by deterministic checks plus LLM-as-a-judge, with one retry before grading. It is Apache-2.0 and runs locally via pnpm.

> **译文：** 大多数代理基准测试都使用模拟对象。而 Supabase Evals 的每个场景都会启动一个真实的容器化堆栈——代理会调用实际的 MCP 服务器和 CLI，然后通过确定性检查和 LLM 作为评判标准进行评分，评分前允许一次重试。它基于 Apache 2.0，并通过 pnpm 在本地运行。

Skills mattered least for top models, most for smaller ones: Sonnet 5 rose from 78% to 100% with skills loaded, GPT-5.6 Sol from 89% to 100%. One finding worth quoting to your team: Codex reads roughly 8 docs pages per scenario versus about 2 for Claude Code, which checks docs in under 40% of scenarios even with skills loaded.

> **译文：** 技能对顶级模型的影响最小，对小型模型的影响最大：Sonnet 5 在加载技能后准确率从 78% 提升至 100%，GPT-5.6 Sol 从 89% 提升至 100%。一项值得团队注意的发现是：Codex 平均每个场景读取约 8 页文档，而 Claude Code 平均每个场景仅读取约 2 页文档，即使加载了技能，Claude Code 的文档检查率也低于 40%。

07 · MINIMAX · VIDEO GENERATION

MiniMax Releases MiniMax H3: An Omni-Modal Video Model That Generates 15-Second 2K Clips With Native Stereo Audio

> **译文：** MiniMax发布MiniMax H3：一款全模态视频模型，可生成15秒2K视频片段，并带有原生立体声音频。

One model reads text, images, video and audio as unified context and returns 2K video with native stereo sound, 4–15 seconds. The H3-VAE tokenizer delivers a stated 4× gain in effective sequence length. API today; open weights promised in the coming days, not yet shipped.

> **译文：** 该模型可将文本、图像、视频和音频作为统一上下文读取，并返回时长 4-15 秒、带有原生立体声的 2K 视频。H3-VAE 分词器据称可将有效序列长度提升 4 倍。API 现已发布；承诺在未来几天内开放权重，但尚未发布。

08 · DEEPSEEK · MODEL UPDATE

DeepSeek Upgrades DeepSeek-V4-Flash-0731 with Major Agentic and Coding Gains

> **译文：** DeepSeek 对 DeepSeek-V4-Flash-0731 进行升级，在代理和编码方面均有重大改进

Same 284B/13B-active MIT-licensed architecture; the jump is post-training only. Terminal Bench 2.1 moves from 61.8 to 82.7, and API pricing sits at $0.14 per 1M input and $0.28 per 1M output tokens. All benchmark numbers are vendor-reported on an unreleased harness — run your own evals first.

> **译文：** 架构依然是 284B/13B 活跃 MIT 许可；此次性能提升仅在训练后出现。Terminal Bench 2.1 的得分从 61.8 提升至 82.7，API 定价为每百万个输入令牌 0.14 美元，每百万个输出令牌 0.28 美元。所有基准测试数据均由厂商在未发布的测试框架上提供——请先自行进行评估。

ONE MORE THING…

MARKTECHPOST · HANDS-ON TUTORIAL

A Tutorial on GeoAI: Designing Footprint Extraction from NAIP Imagery Using U-Net, Grounding DINO, SAM, and Mask R-CNN

> **译文：** GeoAI教程：使用U-Net、Grounding DINO、SAM和Mask R-CNN从NAIP影像中提取足迹。

After seven releases where the deployable artifact is an API, a partnership or a license, here is the counterpoint: a complete pipeline where everything runs. Raw NAIP aerial imagery in, cleaned and regularized building-footprint polygons out, end to end in one Colab notebook.

> **译文：** 在前七个版本中，可部署的组件都是 API、合作伙伴关系或许可证之后，现在我们带来了一个截然不同的方案：一个完整的流程，所有环节都在同一个 Colab notebook 中完成。从输入原始 NAIP 航拍图像，到输出经过清理和规范化的建筑物轮廓多边形，整个流程都在同一个 Colab notebook 中完成。

You train a U-Net with a ResNet-34 encoder on 512-pixel georeferenced chips, run sliding-window inference on an unseen scene, orthogonalize the predicted masks into polygons, and score IoU and F1. Then you compare three paradigms on the same scene: your trained model, zero-shot Grounding DINO plus SAM from text prompts, and a pretrained Mask R-CNN — and extend the pipeline to any real area using Microsoft Planetary Computer imagery and Overture Maps labels.

> **译文：** 您使用 ResNet-34 编码器在 512 像素的地理参考芯片上训练一个 U-Net，对一个未见过的场景运行滑动窗口推理，将预测的掩码正交化为多边形，并计算 IoU 和 F1 值。然后，您在同一场景上比较三种范式：您训练的模型、基于文本提示的零样本 Grounding DINO 加 SAM 以及预训练的 Mask R-CNN——并将该流程扩展到任何真实区域，使用 Microsoft 行星计算机图像和 Overture Maps 标签。

▮ AI Dev Signals · by Marktechpost AI Media

Every number above is taken from the primary source and the Marktechpost coverage linked in each story, August 2026 — versions, access tiers and availability change fast.

> **译文：** 以上所有数字均来自主要来源和 Marktechpost 报道中链接的内容，截至 2026 年 8 月——版本、访问级别和可用性变化很快。

© 2026 Marktechpost AI Media Inc. All rights reserved.

> **译文：** © 2026 Marktechpost AI Media Inc. 保留所有权利。