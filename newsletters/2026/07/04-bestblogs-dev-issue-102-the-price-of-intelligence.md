# BestBlogs.dev Issue #102: The Price of Intelligence

**来源：** BestBlogs.dev  
**日期：** 2026-07-04  
**查看原邮件：** <https://mail.google.com/mail/u/1/#search/subject%3A%22BestBlogs.dev%20Issue%20%23102%3A%20The%20Price%20of%20Intelligence%22>

---

BestBlogs.dev Issue #102: The Price of Intelligence

BestBlogs.dev 第 102 期：智慧的代价

Hey there! Welcome to BestBlogs.dev Issue #102.

Claude Sonnet 5, GPT-5.6, LongCat-2.0, and a new wave of multimodal models all pushed capability forward this week. Yet after reading these 20 pieces, the more interesting question is not how much smarter the models became. It is who ultimately pays for that intelligence. APIs have prices, inference has latency, agents consume context and verification, and organizations absorb the cost of learning, reviewing, and redesigning work.

本周，Claude Sonnet 5、GPT-5.6、LongCat-2.0 以及新一波多模态模型都推动了智能能力的提升。然而，读完这 20 篇文章后，更值得探讨的问题并非模型究竟变得多么智能，而是谁最终为这种智能买单。API 需要付费，推理需要延迟，智能体需要消耗上下文信息和进行验证，而组织机构则要承担学习、审查和重新设计工作流程的成本。

That is the idea behind this issue's theme, The Price of Intelligence. The point is not to dismiss AI as too expensive. It is to make the bill legible, so we can decide which capabilities are worth buying, which workflows are worth rebuilding, and what it takes to turn intelligence into durable value.

这就是本期主题“智能的代价”背后的理念。重点并非在于否定人工智能的昂贵，而是要清晰地列出其成本，以便我们能够决定哪些能力值得投入，哪些工作流程值得重建，以及如何将智能转化为持久的价值。

Here are 10 highlights worth your attention this week:

以下是本周值得您关注的10个亮点：

Claude Sonnet 5 brings Sonnet-class agent performance close to Opus 4.8 while launching at $2 per million input tokens and $10 per million output tokens. GPT-5.6 Sol scores 91.9% on Terminal-Bench 2.1, but remains limited to a small group of trusted partners. Simon Willison adds the developer's footnote: on one English sample, Sonnet 5's new tokenizer produced 1.42 times as many tokens. A lower list price does not always mean a smaller bill.

Claude Sonnet 5 将 Sonnet 级智能体的性能提升至接近 Opus 4.8 的水平，其定价为每百万输入代币 2 美元，每百万输出代币 10 美元。GPT-5.6 Sol 在 Terminal-Bench 2.1 测试中得分 91.9%，但目前仍仅限于少数受信任的合作伙伴。Simon Willison 补充道：在某个英文样本中，Sonnet 5 的新分词器生成的代币数量是之前的 1.42 倍。较低的定价并不总是意味着更少的费用。

DeepSeek's DSpark combines semi-autoregressive drafting with confidence-scheduled verification. On live traffic, it raises single-user generation speed for V4-Flash by 60% to 85%. LongCat-2.0 takes a different route, bringing 1.6T parameters, a 1M-token context window, and agentic coding to a 50,000-accelerator cluster built on domestic hardware.

DeepSeek 的 DSpark 结合了半自回归草案生成和置信度调度验证。在实际流量下，它将 V4-Flash 的单用户生成速度提升了 60% 到 85%。LongCat-2.0 则另辟蹊径，将 1.6T 参数、100 万个令牌的上下文窗口以及代理编码引入到基于国产硬件构建的 5 万个加速器的集群中。

Nano Banana 2 Lite generates a 1K image for $0.034 in about four seconds, while Gemini Omni Flash offers video generation and conversational editing at $0.10 per second of output. Multimodal creation is moving beyond impressive demos toward production tools with budgets, latency targets, and scaling decisions.

Nano Banana 2 Lite 生成一张 1K 图像仅需 0.034 美元，耗时约 4 秒；而 Gemini Omni Flash 则提供视频生成和对话编辑功能，每秒输出成本为 0.10 美元。多模态创作正从令人印象深刻的演示走向生产级工具，并需考虑预算、延迟目标和扩展性等问题。

Spotify is running agents across a codebase with more than 20 million lines, supported by Honk, CI, cross-platform builds, component ownership, testing, and safe auto-merge. Block offers an equally useful warning: roughly 90% of engineers were already using AI tools, yet customer-facing delivery was not getting faster.

Spotify 正在一个拥有超过 2000 万行代码的代码库上运行代理，并由 Honk、持续集成 (CI)、跨平台构建、组件所有权、测试和安全自动合并等机制提供支持。Block 也提出了一个同样重要的警告：大约 90% 的工程师已经在使用 AI 工具，但面向客户的交付速度并没有提升。

Agent frameworks keep changing, but Thread, Run, Step, Event, Artifact, and Checkpoint keep returning as stable runtime abstractions. ADK 2.0 separates deterministic code from model judgment, cutting token use by about 50% and latency by about 20%.

代理框架不断变化，但线程、运行、步骤、事件、工件和检查点作为稳定的运行时抽象概念却始终存在。ADK 2.0 将确定性代码与模型判断分离，从而减少了约 50% 的令牌使用量和约 20% 的延迟。

Taobao's engineering team defines a skill as behavioral programming. A skill should trigger in the right situation, load context progressively, and tighten control as risk rises. Microsoft Research's SkillOpt goes further by treating a skill file as a trainable parameter outside the model — best or tied for best across 52 evaluation cells.

淘宝的工程团队将技能定义为行为编程。技能应在合适的场景下触发，逐步加载上下文，并随着风险的增加而加强控制。微软研究院的 SkillOpt 更进一步，将技能文件视为模型之外的可训练参数——在 52 个评估单元中表现最佳或并列最佳。

Local AI is catching up too. Ahmad Osman estimates that open models now trail closed frontier systems by only four to eight months.

本地人工智能也在迎头赶上。艾哈迈德·奥斯曼估计，开放模型现在只比封闭前沿系统落后四到八个月。

As implementation gets cheaper, taste, curation, and direction become scarce. Codex lead Andrew Ambrosino argues that prototypes are useful for testing interaction, while ambiguous product ideas may still need precise writing.

随着实施成本的降低，品味、策划和方向变得愈发稀缺。Codex 的负责人 Andrew Ambrosino 认为，原型对于测试交互非常有用，而模糊的产品构想仍然需要精确的文字描述。

Cloudflare CEO Matthew Prince says bot traffic on the company's network surpassed human traffic in the first half of 2026, and predicts it could reach 1,000 times the volume of human traffic within five years.

Cloudflare 首席执行官 Matthew Prince 表示，该公司网络上的机器人流量在 2026 年上半年超过了人类流量，并预测五年内机器人流量可能会达到人类流量的 1000 倍。

Tencent Research calls the problem token diseconomics. One cited study found that nearly 80% of open-source software-engineering skills did not improve pass rates, even as token use rose by as much as 451%. Eighteen interviews across two consulting firms found middle managers verifying AI output, coaching junior staff, and documenting reusable practices without being given more time.

腾讯研究院将这个问题称为“代币经济效益低下”。一项研究发现，尽管代币使用率增长了高达 451%，但近 80% 的开源软件工程技能并未提高考试通过率。对两家咨询公司的 18 位受访者进行的访谈发现，中层管理人员在缺乏更多时间的情况下，仍然需要验证人工智能的输出结果、指导初级员工并记录可复用的实践经验。