# BestBlogs.dev Issue #99: Fable and Mythos

**来源：** BestBlogs  
**日期：** 2026-06-13  
**查看原邮件：** <https://mail.google.com/mail/u/1/#search/subject%3A%22BestBlogs.dev%20Issue%20%2399%3A%20Fable%20and%20Mythos%22>

---

BestBlogs.dev Issue #99: Fable and Mythos

 20 picks   

Hey there! Welcome to BestBlogs.dev Issue #99. 

This week, AI had one keyword: Claude Fable 5. Anthropic released two models at once: Fable 5 for everyone, and Mythos 5 for trusted security partners only. Fable 5 sets state-of-the-art results across nearly every benchmark at less than half the price of Mythos Preview. In a real deployment at Stripe, it completed a codebase-wide migration of 50 million lines of Ruby in a single day, work that would have taken a whole team over two months. When the strongest model gets dramatically cheaper while an even stronger one goes behind a trusted-access gate, we may be watching the distribution model of AI capability change in real time. 

本周，人工智能领域只有一个关键词：Claude Fable 5。Anthropic 同时发布了两款模型：面向所有人的 Fable 5 和仅供受信任的安全合作伙伴使用的 Mythos 5。Fable 5 在几乎所有基准测试中都取得了最先进的结果，而价格却不到 Mythos Preview 的一半。在 Stripe 的实际部署中，它仅用一天时间就完成了 5000 万行 Ruby 代码的全库迁移，这项工作如果由一个团队完成，则需要两个多月的时间。当最强大的模型价格大幅下降，而更强大的模型却被置于受信任访问的门槛之后时，我们或许正在见证人工智能能力分布模式的实时变革。

On the BestBlogs side, there is a fun easter egg that echoes this issue's theme: we shipped v2.5.0 with a brand-new World Cup special page at bestblogs.dev/worldcup, designed and built entirely by Claude Fable 5. If you are watching the World Cup this month, come take a look. 

BestBlogs这边有一个有趣的彩蛋，与本期主题相呼应：我们在v2.5.0版本中加入了一个全新的世界杯特辑页面，网址是bestblogs.dev/worldcup，该页面完全由Claude Fable 5设计和构建。如果你本月正在观看世界杯，不妨来看看。

Here are 10 highlights worth your attention this week: 

以下是本周值得您关注的10个亮点：

🧠 Claude Fable 5 and Mythos 5 are here. Fable 5 achieves state-of-the-art results across software engineering, knowledge work, and visual understanding, while Mythos 5 is deployed only to trusted security researchers through Project Glasswing. Simon Willison's verdict after 5.5 hours of testing: slow and expensive, but it handles every complex task delightfully and is worth every dollar. 

🧠 Claude 的 Fable 5 和 Mythos 5 现已发布。Fable 5 在软件工程、知识工作和视觉理解方面均取得了顶尖水平的成果，而 Mythos 5 仅通过 Project Glasswing 部署给受信任的安全研究人员。Simon Willison 在经过 5.5 小时的测试后得出结论：速度慢且价格昂贵，但它能出色地处理所有复杂任务，物有所值。

🛡️ Anthropic CEO Dario Amodei published a policy essay arguing that AI's exponential progress and slow policymaking have formed a dangerous mismatch. He lays out a five-part agenda, from FAA-style mandatory third-party testing to wage insurance for labor displacement and biomedical regulatory reform, and warns that the window for effective action is closing. 

🛡️ Anthropic 首席执行官 Dario Amodei 发表了一篇政策文章，指出人工智能的指数级发展与缓慢的政策制定形成了危险的错配。他提出了五项议程，从类似美国联邦航空管理局 (FAA) 的强制性第三方测试，到针对失业的工资保险和生物医学监管改革，并警告说，采取有效行动的窗口期正在关闭。

⚡ Inference speed is the new battleground. DiffusionGemma generates 256-token blocks in parallel with a diffusion head, passing 1,000 tokens per second on a single H100; Xiaomi MiMo and TileRT use model-system co-design to push a 1T-parameter model past 1,000 tokens per second on a standard 8-GPU cluster. One changes the architecture, the other squeezes the system — and they arrive at the same place. 

⚡推理速度是新的竞争焦点。DiffusionGemma 利用扩散头并行生成 256 个 token 的区块，在单个 H100 上每秒可处理 1000 个 token；小米 MiMo 和 TileRT 则采用模型系统协同设计，在标准的 8 GPU 集群上，将 1T 参数模型的推理速度提升至每秒 1000 个 token 以上。一个改变了架构，另一个则压缩了系统——最终它们殊途同归。

🔄 The Claude Code one-year retrospective traces the evolution from coding assistant to autonomous agent workflows: verification loops, Auto Mode, and routines entering real work. The "Loop Engineering" essay pushes the direction to its logical end, designing unattended autonomous loops from automation, worktrees, skills, subagents, and external memory. 

🔄 Claude Code 一周年回顾文章追溯了其从编码助手到自主代理工作流程的演变历程：验证循环、自动模式以及应用于实际工作的例程。“循环工程”一文将这一方向推向了逻辑的极致，从自动化、工作树、技能、子代理和外部存储器等方面设计了无人值守的自主循环。

📚 Skills are becoming engineering assets. Tencent's "How to Write a Good Skill" manual covers the full chain from Description writing to prompt injection defenses; Alibaba Cloud compares Trace2Skill, EvoSkill, and SkillOpt as routes to making skills evolve themselves in a controlled, measurable way. 

📚 技能正逐渐成为工程资产。腾讯的《如何编写好技能》手册涵盖了从技能描述编写到提示注入防御的完整流程；阿里云则比较了 Trace2Skill、EvoSkill 和 SkillOpt，认为它们是使技能以可控、可衡量的方式自我演进的途径。

🏗️ "AI doesn't lack IQ, it lacks discipline." An Alibaba engineer's two-month Harness practice argues the bottleneck in AI coding is shifting from model capability to process engineering, with a three-layer loading architecture keeping resident context under 8K. InfoQ's Coding Agent landscape and Tencent's teardown of context compression strategies across six agents confirm the same judgment from different angles: context and process are today's main battlefield. 

🏗️ “人工智能并非缺乏智商，而是缺乏自律。”一位阿里巴巴工程师历时两个月的Harness实践表明，人工智能编码的瓶颈正从模型能力转向流程工程，而三层加载架构可以将驻留上下文控制在8K以内。InfoQ的编码代理概览以及腾讯对六个代理的上下文压缩策略的拆解分析，从不同角度印证了这一观点：上下文和流程是当今的主要战场。

🏢 The truth about enterprise agents: Salesforce distilled 20,000 deployments into a counterintuitive lesson — 90% of the work comes after launch. Anthropic's Claude Managed Agents answers from the infrastructure side: decouple the brain from the hands, and let the platform handle hosting, scaling, and credential isolation. 

🏢 关于企业代理的真相：Salesforce 从 20,000 次部署中提炼出一个反直觉的教训——90% 的工作都在上线之后。Anthropic 的 Claude Managed Agents 从基础设施层面解决了这个问题：将大脑与操作分离，让平台负责托管、扩展和凭证隔离。

🔭 Two takes on the future of engineers. Google DeepMind's Logan Kilpatrick argues that models will swallow the agent scaffolding, as external tooling migrates into native model systems; another essay counters the job-loss narrative with data: code written grew 8x while releases grew only 30%, so writing code was never the bottleneck. 

🔭 关于工程师的未来，有两种观点。谷歌DeepMind的Logan Kilpatrick认为，随着外部工具迁移到原生模型系统中，模型将吞噬智能体框架；另一篇文章则用数据反驳了失业论调：代码编写量增长了8倍，而版本发布量仅增长了30%，因此代码编写从来都不是瓶颈。

🍎 AI's consumer moments: at WWDC26, Siri got its biggest upgrade yet with a standalone app, and Apple is co-building next-generation foundation models with Google, though mainland China users miss the launch; Kimi announced that 300 sub-agents will publicly predict all 104 World Cup matches, finding Germany's championship odds underpriced by the market. 

🍎 AI 的消费时刻：在 WWDC26 上，Siri 迎来了迄今为止最大的升级，推出了独立应用程序；苹果正在与谷歌共同构建下一代基础模型，尽管中国大陆用户错过了发布；Kimi 宣布 300 个子代理将公开预测全部 104 场世界杯比赛，并发现德国夺冠的赔率被市场低估了。

🎙️ Two interviews worth a long sit: Anker founder Yang Meng spends 4 hours reviewing 15 years of company history and the strategic shift from shallow-water categories to deep-water systems; iPod father Tony Fadell reminds us that in the age of AI-accelerated prototyping, what is scarce is not execution speed but taste and judgment. 

🎙️ 两篇值得长时间观看的采访：Anker 创始人杨猛花了 4 个小时回顾了公司 15 年的历史以及从浅水产品类别到深水系统的战略转变；iPod 之父 Tony Fadell 提醒我们，在人工智能加速原型设计的时代，稀缺的不是执行速度，而是品味和判断力。

Hope this issue sparks some new ideas. Stay curious, and see you next week!   Curated picks  1. The evolution of agentic surfaces: building with Claude Managed Agents | Claude    2. Why AI hasn’t replaced software engineers， and won’t    3. Claude Fable 5 and Claude Mythos 5    4. Initial impressions of Claude Fable 5    5. Loop Engineering    6. 如何写好 Skill：一份终极实战经验手册    7. 如何更科学、方向可控的实现 Skill 的“自进化”?    8. Coding Agent 技术全景图：Context Engineering、Subagents 与 Harness，一年范式转移全解析    9. 横向拆解 Claude Code、Codex 等六大 Agent 上下文压缩策略后，我们做了第 7 个    10. What Salesforce Learned from 20，000 Enterprise Agent Deployments    11. Dario Amodei — Policy on the AI Exponential    12. DiffusionGemma: 4x faster text generation    13. Xiaomi MiMo 携手 TileRT｜1T 模型首次突破 1000 tokens/s 输出速度    14. Reflecting on a year of Claude Code    15. Kimi 将公开预测 104 场世界杯赛事：德国队或爆冷夺冠    16. Father of the iPod and iPhone on building taste， judgment， and creativity in the AI era    17. 144. 对阳萌的 4 小时访谈：消费电子死与生、第三类公司、AI 变量、产品方法、打游戏的模式选择    18. Google DeepMind's Logan Kilpatrick: Why the Model Eats the Harness    19. iPhone 终于支持 Siri AI！但国行无缘首发，闹钟成为最大惊喜    20. AI 不缺智商缺纪律：一场 Harness 工程化实践        About BestBlogs 

希望这个问题能够引发一些新的想法。保持好奇心，下周见！   精选精选 1. 代理表面的演变：使用 Claude Managed Agents 进行构建 |克劳德 2. 为什么人工智能没有取代软件工程师，将来也不会 3. 克劳德寓言 5 和克劳德神话 5 4. 克劳德寓言 5 的初步印象 5. 循环工程 6. 如何写好技能：一份终极实战经验手册 7. 如何更科学、方向可控的实现技能的“自进化”？    8. Coding Agent 技术全景图：Context Engineering、Subagents 与 Harness，一年范式转移全解析 9. 横向拆解 Claude Code、Codex 等六大 Agent 上下文压缩策略后，我们做了第 7 个 10. Salesforce 从 20,000 个企业代理部署中学到了什么 11. Dario Amodei — 关于 AI 指数的策略 12. DiffusionGemma：文本生成速度提高 4 倍13. 小米 MiMo 数据 TileRT｜1T 模型突破 1000 tokens/s 输出速度 14. 回顾克劳德代码的一年 15. Kimi 将公开预测 104 现场世界杯首次赛事：德国队或爆冷公告 16. iPod 和 iPhone 之父，打造 AI 时代的品味、判断力和创造力 17. 144. 对阳对萌的 4小时访谈：消费电子死与生、第三类公司、AI指标、产品方法、打游戏的模式选择    18. Google DeepMind 的 Logan Kilpatrick: Why the Model Eats the Harness 19. iPhone 终于支持 Siri AI！国行无缘主板，闹钟成为最大惊喜 20. AI 不缺智商缺纪律：正在进行 Harness 工程化实践 About BestBlogs

BestBlogs.dev curates the best technical writing from across the web. Subscribe for editor-picked stories every Friday.   You're receiving this because you subscribed to BestBlogs weekly.
  ·

BestBlogs.dev 精选全网最佳技术文章。每周五订阅即可阅读编辑精选文章。您收到此邮件是因为您已订阅 BestBlogs 周刊。

·