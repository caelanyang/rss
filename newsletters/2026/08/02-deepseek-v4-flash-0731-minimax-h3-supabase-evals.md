# 🚨 DeepSeek V4-Flash 0731, MiniMax H3, Supabase evals

**来源：** Marktechpost AI  
**日期：** 2026-08-02  
**查看原邮件：** <https://mail.google.com/mail/u/1/#search/subject%3A%22%F0%9F%9A%A8%20DeepSeek%20V4-Flash%200731%2C%20MiniMax%20H3%2C%20Supabase%20evals%22>

---

Same architecture, better post-training. Native stereo video. And the benchmark that caught Codex reading 4× more docs than Claude Code.
Aug 1, 2026
Together with MongoDB
AI Dev Signals · August 1, 2026 · The Frozen Target
Nobody trained a new model.
The numbers moved anyway.
A checkpoint that only changed its post‑training. A drafter trained against a frozen target. A decoder rewired into an encoder. And one genuinely new architecture, to prove the rule.
Presented by MongoDB    Event Venue Operator — an agentic demo on Atlas with three‑layer memory and Voyage embeddings. Clone it →
Almost everything below left the model alone. DeepSeek shipped the same 284B architecture with new post‑training. Tencent froze the target and trained a drafter around it. Liquid AI converted decoders it already had. Supabase changed the skills, not the agents. The exception is MiniMax H3, which rebuilt the whole stack — and is the one thing here you cannot download.
82.7
up from 61.8 preview
4.79
against 3.00 for MTP
99.4%
tokens saved, 233 pages
🔥 The signals
01 · DeepSeek · Model update
DeepSeek Upgrades DeepSeek-V4-Flash-0731 with Major Agentic and Coding Gains
An upgrade usually means a new architecture. This one means a new curriculum. The model card says the architecture and size are unchanged. The gains come from re‑post‑training alone.
Terminal Bench 2.1 moves 61.8 to 82.7. DeepSWE moves 7.3 to 54.4. It beats V4‑Pro (Preview) on every agentic benchmark DeepSeek published. Output pricing is $0.28 per 1M tokens against $0.87 for deepseek-v4-pro . Weights are MIT and ungated, but self‑hosting still wants roughly 110 GB at 3‑bit. Every figure is vendor‑reported on a harness that has not been released.
Read on Marktechpost →
·  Model card
·  Technical report
·  Pricing
·  DSpark paper
02 · MiniMax · Video model
MiniMax Releases MiniMax H3: An Omni-Modal Video Model That Generates 15-Second 2K Clips With Native Stereo Audio
A video stack used to be a drawer of expert models. Text‑to‑video, image‑to‑video, first‑and‑last‑frame, subject reference, editing. H3 folds them into one pretraining paradigm where the relationships are expressed in natural language.
Output is 2K, four to fifteen seconds, integer durations only, with native stereo. H3‑VAE’s compression delivers a stated 4× gain in effective sequence length, which is what makes native 2K economical. Training throughput is up nearly 30%. Open weights are promised in the coming days, not shipped, so the API is the only path today.
Read on Marktechpost →
·  Announcement
·  API docs
03 · Supabase · Benchmark
Supabase Releases Evals: an Open Source Benchmark That Scores Claude Code, Codex and OpenCode on Real Supabase Tasks
Most agent benchmarks grade against mocks. This one boots a containerized stack and a real CLI, then asks the agent to build a schema or fix a broken RLS policy. Scoring mixes deterministic checks with LLM‑as‑a‑judge, and the agent gets one retry.
Agents pass most scenarios with no skill loaded. Opus 5 and Kimi K3 both scored 100% unaided in the Build stage. Skills mattered further down: Sonnet 5 went 78% to 100%, GPT‑5.4 mini 78% to 89%. The odd finding is docs usage. Codex reads roughly eight docs pages per scenario against about two for Claude Code. Apache‑2.0, and it runs locally on pnpm .
Read on Marktechpost →
·  Announcement
·  GitHub
·  Leaderboard
From our sponsor
Want agent memory modelled on a real cluster instead of a diagram? Run MongoDB’s Event Venue Operator →
04 · Tencent · Inference
Tencent Open-Sources AngelSpec: A Unified Training Framework for MTP and Block-Parallel Speculative Decoding on Hy3 Models
Speculative decoding usually hunts for one drafter that averages well. Real traffic is not an average. Open‑ended chat rewards short proposals. Code and maths reward long predictable blocks. AngelSpec ships two drafters instead of one compromise.
DFly reaches 4.79 mean accepted length on Hy3‑A21B, against 3.69 for DFlash and 3.00 for MTP. On Qwen3‑8B it takes every math and code benchmark, though DSpark stays ahead on MT‑Bench at 3.77 to 3.67. The target backbone and LM head stay frozen throughout, so verification preserves the original distribution. Seven checkpoints ship on Hugging Face and ModelScope.
Read on Marktechpost →
·  Paper
·  GitHub
·  Docs
·  Hugging Face
05 · Liquid AI · Encoders
Liquid AI Releases LFM2.5-Encoder-230M and LFM2.5-Encoder-350M: Bidirectional Encoders That Stay Fast at 8K Context on CPU
Nobody demos an encoder. Everybody runs one, underneath the classifier, the intent router, the PII filter. Liquid AI did not train these from scratch. It converted decoders it already had, using a bidirectional mask, non‑causal short convolutions, and a 30% mask rate.
The 350M posts an 81.02 mean across 17 tasks, ranking fourth of 14. The three models above it are all larger, and the top one is nearly ten times its size. The 230M runs one 8K forward pass on CPU in about 28 seconds, against over 90 for ModernBERT‑base. License is the LFM Open License v1.0, and every load call needs trust_remote_code=True .
Read on Marktechpost →
·  Announcement
·  Model card
·  Eval code
06 · Marktechpost · Open source
Meet Token Saver: An Open-Source MCP Extension Using Local Hybrid RAG to Cut Claude PDF Token Costs
A 200‑page PDF is not a one‑time charge

相同的架构，更优的后训练。原生立体视频。以及一项基准测试，该测试发现 Codex 阅读的文档数量是 Claude Code 的 4 倍。

2026 年 8 月 1 日

与 MongoDB 合作

AI 开发信号 · 2026 年 8 月 1 日 · 冻结目标

没有人训练新的模型。

但数据依然发生了变化。

一个仅更改后训练的检查点。一个针对冻结目标训练的绘图器。一个解码器被重新连接到编码器。以及一个真正的新架构，以证明这一规则。

由 MongoDB 呈现 活动场地运营商 — 基于 Atlas 的智能体演示，采用三层内存和 Voyage 嵌入。克隆它 →

以下几乎所有内容都保持了模型不变。DeepSeek 发布了相同的 284B 架构，并采用了新的后训练。腾讯冻结了目标，并围绕它训练了一个绘图器。Liquid AI 转换了它已有的解码器。Supabase 更改了技能，但没有更改智能体。例外情况是 MiniMax H3，它重建了整个堆栈——也是这里唯一无法下载的内容。

82.7

较预览版 61.8 有所提升

4.79

对比 MTP 的 3.00

99.4%

已保存 233 页

🔥 信号

01 · DeepSeek · 模型更新

DeepSeek 升级 DeepSeek-V4-Flash-0731，在代理和编码方面均有显著提升

升级通常意味着新的架构。而这次升级意味着新的课程。模型卡显示架构和大小保持不变。性能提升仅来自重新训练。

Terminal Bench 2.1 将分数从 61.8 提升至 82.7。DeepSWE 将分数从 7.3 提升至 54.4。在 DeepSeek 发布的所有代理基准测试中，它都优于 V4-Pro（预览版）。输出定价为每百万个代币 0.28 美元，而 deepseek-v4-pro 为 0.87 美元。权重采用 MIT 许可且未设门槛，但自托管仍需要大约 110 GB 的 3 位分辨率空间。所有数据均来自尚未发布的测试平台，由供应商提供。

在 Marktechpost 阅读全文 →

· 模型卡

· 技术报告

· 定价

· DSpark 论文

02 · MiniMax · 视频模型

MiniMax 发布 MiniMax H3：一款全模态视频模型，可生成 15 秒 2K 视频片段，并带有原生立体声音频

以往的视频堆栈就像一个专家模型的抽屉，包含文本转视频、图像转视频、首帧和末帧识别、主题参考、编辑等功能。H3 将它们整合到一个预训练范式中，其中关系以自然语言表达。

输出为 2K 分辨率，时长 4 到 15 秒，仅支持整数时长，并带有原生立体声。 H3-VAE 的压缩技术据称可将有效序列长度提升 4 倍，这正是原生 2K 格式经济高效的原因。训练吞吐量提升近 30%。开放权重将在未来几天内发布，但尚未正式发布，因此目前只能通过 API 获取。

阅读 Marktechpost 上的文章 →

· 公告

· API 文档

03 · Supabase · 基准测试

Supabase 发布评估工具：一款开源基准测试工具，用于评估 Claude Code、Codex 和 OpenCode 在真实 Supabase 任务上的表现

大多数智能体基准测试都使用模拟对象进行评分。而这款测试工具会启动一个容器化的堆栈和一个真实的 CLI，然后要求智能体构建模式或修复损坏的 RLS 策略。评分机制结合了确定性检查和 LLM 作为评判标准，智能体可以重试一次。

智能体在未加载任何技能的情况下通过了大多数场景。Opus 5 和 Kimi K3 在构建阶段均获得了 100% 的分数。技能的重要性进一步提升：Sonnet 5 的准确率从 78% 提升至 100%，GPT-5.4 mini 的准确率从 78% 提升至 89%。一个奇怪的发现是文档使用情况。Codex 平均每个场景阅读约 8 页文档，而 Claude Code 则约为 2 页。它使用 Apache-2.0 许可证，并在本地通过 pnpm 运行。

在 Marktechpost 上阅读更多内容 →

· 公告

· GitHub

· 排行榜

来自我们的赞助商

想要基于真实集群而非图表来模拟代理内存？运行 MongoDB 的 Event Venue Operator →

04 · 腾讯 · 推理

腾讯开源 AngelSpec：一个用于 Hy3 模型上 MTP 和块并行推测解码的统一训练框架

推测解码通常会寻找一个平均表现良好的草案生成器。但实际流量并非平均值。开放式聊天会奖励简短的提案。代码和数学会奖励较长且可预测的块。AngelSpec 提供两个草案生成器，而不是一个折衷方案。

DFly 在 Hy3-A21B 数据集上的平均接受长度达到 4.79，而 DFlash 和 MTP 分别为 3.69 和 3.00。在 Qwen3-8B 数据集上，DFly 在所有数学和代码基准测试中均胜出，尽管 DSpark 在 MT-Bench 测试中以 3.77 对 3.67 领先。目标骨干网和 LM 头在整个验证过程中保持冻结状态，因此验证过程保留了原始分布。Hugging Face 和 ModelScope 均包含七个检查点。

在 Marktechpost 上阅读 →

· 论文

· GitHub

· 文档

· Hugging Face
05 · Liquid AI · 编码器

Liquid AI 发布 LFM2.5-Encoder-230M 和 LFM2.5-Encoder-350M：在 CPU 上处理 8K 上下文时仍能保持高速的双向编码器

没有人演示编码器。每个人都在分类器、意图路由器和 PII 过滤器下面运行编码器。Liquid AI 并没有从头开始训练这些编码器。它转换了已有的解码器，使用了双向掩码、非因果短卷积和 30% 的掩码率。

350M 在 17 项任务中取得了 81.02 的平均分，在 14 个模型中排名第四。排在它前面的三个模型都比它大，排名第一的模型几乎是它的十倍。230M 在 CPU 上运行一次 8K 前向传播大约需要 28 秒，而 ModernBERT-base 则需要 90 多秒。许可证为 LFM 开源许可证 v1.0，每次加载调用都需要设置 trust_remote_code=True。

在 Marktechpost 上阅读更多内容 →

· 公告

· 模型卡

· 评估代码

06 · Marktechpost · 开源
Token Saver 简介：一款使用本地混合 RAG 降低 Claude PDF Token 成本的开源 MCP 扩展

200 页的 PDF 并非一次性收费。