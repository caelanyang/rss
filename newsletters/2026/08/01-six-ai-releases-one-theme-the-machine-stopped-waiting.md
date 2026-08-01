# 🚨 Six AI releases. One theme. The machine stopped waiting

**来源：** Marktechpost AI (AI Dev Signals)  
**日期：** 2026-08-01  
**查看原邮件：** <https://mail.google.com/mail/u/1/#search/subject%3A%22%F0%9F%9A%A8%20Six%20AI%20releases.%20One%20theme.%20The%20machine%20stopped%20waiting%22>

---

Most weeks in AI are noise. This one is not. Every release below removed a wait — a robot waiting for a script, a caller waiting for a transcript, a GPU waiting for its slowest neighbor.


> **译文：** 人工智能领域的大多数周都如同噪音一般，但这一周却截然不同。以下每个版本都减少了一次等待——机器人不再等待脚本，呼叫者不再等待转录文本，GPU 不再等待其最慢的邻居。

AI DEV SIGNALS · JULY 30, 2026

Six releases. One theme. The machine stopped waiting.


> **译文：** 六张专辑，一个主题。机器停止了等待。

Robots that walk before they grab. A voice model that hears you instead of reading you. And three pieces of plumbing that decide what the next year of AI costs.


> **译文：** 机器人会先行走再抓取物品。语音模型能够听懂你的声音，而不是读出你的话。还有三件决定人工智能未来一年成本的管道设备。

PRESENTED BY MONGODB — Event Venue Operator: an agentic demo with three-layer memory on Atlas. Open the repo →


> **译文：** 由 MongoDB 呈现 — 活动场地运维工具：基于 Atlas 的三层内存智能体演示。打开代码库 →

01 · GOOGLE DEEPMIND · ROBOTICS

Google DeepMind Ships Three Physical AI Models For Whole Body Control, Dexterity And Multi Robot Collaboration


> **译文：** 谷歌DeepMind发布三款用于全身控制、灵巧性和多机器人协作的物理人工智能模型

A robot used to be a machine that repeated itself. Gemini Robotics 2 ships three models — a VLA, an embodied reasoning VLM, and an on-device VLA — and one checkpoint drives Apollo 2 with two different hands plus a Franka Duo gripper. Whole body control, not table-top. The robot walks to the shelf, then places the object.


> **译文：** 过去，机器人是重复执行动作的机器。Gemini Robotics 2 推出了三种型号——VLA、具身推理 VLM 和设备端 VLA——其中一个检查点驱动 Apollo 2 使用两只不同的机械手和一个 Franka Duo 机械臂。它采用全身控制，而非桌面式操作。机器人走到货架前，然后放置物品。

The honesty is the best part: multi-finger dexterity still runs 32% to 92% depending on the task. Unscrewing a bulb is solved. Tying a trash bag is not.


> **译文：** 最棒的是它的诚实性：多指灵巧度仍然只有32%到92%不等，具体取决于任务。拧灯泡的问题解决了，但扎垃圾袋的问题仍然存在。

02 · POLYAI · VOICE AI

PolyAI Releases Dialog-RSN-1: An Audio-Native Dialog Model That Fuses Turn-Taking, Speech Recognition, Function Calling, And Response


> **译文：** PolyAI发布Dialog-RSN-1：一种融合了轮流对话、语音识别、函数调用和响应功能的音频原生对话模型

Every voice stack throws away the thing that matters. The ASR hands over its best guess, and the tone, the hesitation, the doubt — all gone before the model reads a word. Dialog-RSN-1 listens to the audio itself.


> **译文：** 每个语音识别系统都会舍弃最重要的信息。自动语音识别（ASR）给出的是它的最佳猜测，而语气、犹豫、疑虑——所有这些都在模型读取一个字之前就消失了。Dialog-RSN-1 则直接聆听音频本身。

Turn-taking is the first output token: EMPTY, ONGOING or COMPLETE. TTS stays separate, so you still own the voice. Sub-300ms responses, +11% relative containment at a restaurant group, −37% latency at an insurer. English only, and only through PolyAI — no open weights, no public API.


> **译文：** 轮流发言是第一个输出标记：EMPTY（空）、ONGING（进行中）或COMPLETE（完成）。TTS（文本转语音）保持独立，因此您仍然拥有语音控制权。响应时间低于300毫秒，餐饮集团的相对控制率提升11%，保险公司的延迟降低37%。仅支持英语，且仅通过PolyAI提供——不开放权重，不提供公共API。

03 · TENCENT · INFERENCE

Tencent Open-Sources AngelSpec: A Unified Training Framework for MTP and Block-Parallel Speculative Decoding on Hy3 Models


> **译文：** 腾讯开源 AngelSpec：面向 Hy3 模型的 MTP 和块并行推测解码的统一训练框架

Everyone hunts for the one drafter that wins the average benchmark. Real traffic is not an average. Open-ended chat and code are different problems, so AngelSpec ships two drafters instead of one compromise — autoregressive MTP for conversation, block-parallel DFly for code and math.


> **译文：** 每个人都在寻找能够胜任平均基准测试的绘图工具。但实际流量并非平均值。开放式聊天和代码是不同的问题，因此 AngelSpec 提供了两种绘图工具，而不是一种折衷方案——用于对话的自回归 MTP 和用于代码及数学运算的块并行 DFly。

On Hy3-A21B, DFly reaches 4.79 mean accepted length against 3.69 for DFlash and 3.00 for MTP. On HY3-295B-A21B at TP=8, DFly-8 delivers a 1.98–2.40× speedup across concurrency 4 to 64. Seven checkpoints, one config-driven pipeline, six draft architectures.


> **译文：** 在 Hy3-A21B 上，DFly 的平均接受长度达到 4.79，而 DFlash 为 3.69，MTP 为 3.00。在 HY3-295B-A21B 上，当 TP=8 时，DFly-8 在并发数 4 到 64 之间实现了 1.98 到 2.40 倍的加速。七个检查点，一个配置驱动的流水线，六个草案架构。

04 · MOONSHOT AI · TRAINING INFRA

Moonshot AI Open-Sources MoonEP: A Perfectly Balanced Expert Parallelism Library for MoE Training


> **译文：** Moonshot AI 开源 MoonEP：一个用于 MoE 训练的完美平衡的专家并行库

A collective runs at the speed of its slowest rank. So the hottest expert sets the price of every training step, and the shapes change every step, and your memory fragments. MoonEP makes one hard promise instead: every EP rank receives exactly S × K tokens, no matter how skewed the router is.


> **译文：** 集体运行的速度取决于其中排名最低的专家。因此，最热门的专家决定了每个训练步骤的价格，而算法的形状每一步都在变化，你的记忆也会因此变得碎片化。MoonEP 则做出了一个明确的承诺：无论路由的偏差有多大，每个 EP 排名都会获得 S × K 个代币。

It gets there with redundant experts planned online on-GPU, then prefetched before expert compute. Static shapes kill the per-layer host sync. MIT licensed, shipped on Kimi K3 Open Day alongside FlashKDA and AgentEnv.


> **译文：** 它通过在 GPU 上在线预加载冗余专家来实现，然后在专家计算之前进行预取。静态形状会破坏逐层主机同步。该软件采用 MIT 许可，并在 Kimi K3 开放日与 FlashKDA 和 AgentEnv 一起发布。

05 · LIQUID AI · OPEN WEIGHTS

Liquid AI Releases LFM2.5-Encoder-230M and LFM2.5-Encoder-350M: Bidirectional Encoders That Stay Fast at 8K Context on CPU


> **译文：** Liquid AI 发布 LFM2.5-Encoder-230M 和 LFM2.5-Encoder-350M：在 CPU 上处理 8K 上下文时仍能保持快速响应的双向编码器

Nobody demos an encoder. Everybody runs one — under the classifier, the intent router, the safety filter, the PII detector. All day. Usually with no GPU. These two carry 8,192 tokens of context, which is roughly 13 to 15 pages: one contract, one patient record, one forward pass.


> **译文：** 没人演示编码器。但每个人都在运行它——在分类器、意图路由器、安全过滤器、PII检测器下面。整天都在运行。通常没有GPU。这两个组件承载了8192个上下文标记，大约相当于13到15页：一份合同、一份患者记录、一次前向传播。

The 350M posts an 81.02 mean across 17 tasks and ranks fourth of 14 — the three models above it are all larger, the top one nearly ten times its size. At 8K on CPU, the 230M runs a forward pass in about 28s against over 90s for ModernBERT-base. LFM Open License v1.0, 15 languages, evaluation harness open under Apache-2.0.


> **译文：** 350M 模型在 17 项任务中平均得分 81.02，在 14 个模型中排名第四——排在它前面的三个模型都比它大，其中排名第一的模型规模几乎是它的十倍。在 CPU 上以 8K 分辨率运行前向传播，230M 模型耗时约 28 秒，而 ModernBERT-base 模型则耗时超过 90 秒。该模型采用 LFM 开源许可证 v1.0，支持 15 种语言，评估框架基于 Apache-2.0 开源。

ONE MORE THING…

MARKTECHPOST · OPEN SOURCE

Meet Token Saver: An Open-Source MCP Extension Using Local Hybrid RAG to Cut Claude PDF Token Costs 90-99%


> **译文：** Token Saver 简介：一款开源 MCP 扩展，使用本地混合 RAG 算法，可将 Claude PDF Token 成本降低 90-99%。

Drop a 200-page PDF into a chat and you do not pay once. You pay again on every follow-up, forever, because the history gets re-sent. Token Saver ends that. The PDF never leaves your machine.


> **译文：** 把一份 200 页的 PDF 文件扔进聊天窗口，你虽然不用付一次钱，但每次后续都要重新付费，因为聊天记录会被重新发送。Token Saver 可以解决这个问题。PDF 文件永远不会离开你的电脑。

A local MCP server runs hybrid retrieval — BM25 over SQLite FTS5 weighted 0.4, plus a local all-MiniLM-L6-v2 embedding at 0.6 — and hands Claude only the passages that answer the question, with page numbers attached. On a 233-page filing: 133,349 tokens down to 740. That is 99.4%. No Python, no terminal. One .mcpb file, MIT licensed. Built at Marktechpost.


> **译文：** 本地 MCP 服务器运行混合检索——基于 SQLite FTS5 的 BM25 加权 0.4，加上本地全 MiniLM-L6-v2 嵌入（加权 0.6）——并仅向 Claude 提供回答问题的段落，并附上页码。在一份 233 页的文件中，从 133,349 个词元中筛选出 740 个词元，收敛效率高达 99.4%。无需 Python，无需终端。仅使用一个 .mcpb 文件，采用 MIT 许可。由 Marktechpost 开发。