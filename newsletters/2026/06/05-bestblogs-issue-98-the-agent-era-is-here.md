# BestBlogs.dev Issue #98: The Agent Era Is Here

**来源：** BestBlogs  
**日期：** 2026-06-05  
**查看原邮件：** <https://mail.google.com/mail/u/1/#search/subject%3A%22BestBlogs.dev%20Issue%20%2398%3A%20The%20Agent%20Era%20Is%20Here%22>

---

/Users/caelanyang/Library/Python/3.9/lib/python/site-packages/urllib3/__init__.py:35: NotOpenSSLWarning: urllib3 v2 only supports OpenSSL 1.1.1+, currently the 'ssl' module is compiled with 'LibreSSL 2.8.3'. See: https://github.com/urllib3/urllib3/issues/3020
  warnings.warn(
  ✅ Google Translate 翻译 12 段
This week felt like a threshold moment for the Agent era. Kimi Work launched, Coze 3.0 shipped, Claude Code's dynamic workflows went live, and Microsoft's SkillOpt brought self-evolving Agent skills into the open — all in the same week. Engineers at Tencent, Alibaba, and Anthropic published thousands of words answering the same question: when Agents become first-class citizens, what needs to change in our code, architecture, teams, and thinking?

本周仿佛是智能体时代的一个转折点。Kimi Work 上线，Coze 3.0 发布，Claude Code 的动态工作流正式启用，微软的 SkillOpt 也开放了智能体自进化技能——所有这些都发生在同一周。腾讯、阿里巴巴和 Anthropic 的工程师们发表了数千字的文章，都在回答同一个问题：当智能体成为核心成员时，我们的代码、架构、团队和思维方式需要做出哪些改变？

Here are 10 highlights from this issue's 20 curated picks:

以下是本期精选的20篇文章中的10个亮点：

🧠 OpenAI upgraded ChatGPT memory to background dreaming synthesis. Instead of saving memories manually, the new system quietly consolidates conversational fragments over time, letting ChatGPT continuously learn user preferences and become more attuned with use. The post also reveals that falling costs make this newly scalable across the entire user base.

🧠 OpenAI 将 ChatGPT 的内存升级为后台梦境合成。新系统不再手动保存记忆，而是随着时间的推移悄然整合对话片段，使 ChatGPT 能够持续学习用户偏好，并更好地适应使用情况。该文章还指出，成本的降低使得这项技术能够扩展到所有用户。

🤖 Open-source models hit new capability milestones, edge AI accelerates. MiniMax M3 packs state-of-the-art coding, 1M-token long context, and native multimodality into a single open-weight model — its MSA sparse attention architecture cuts long-context compute costs significantly. Google Gemma 4 12B lands on a laptop and runs complete agentic workflows locally, making privacy-first, low-latency AI applications genuinely practical.

🤖 开源模型达到新的能力里程碑，边缘人工智能加速发展。MiniMax M3 将最先进的编码、百万级上下文信息和原生多模态信息集成到一个开放权重模型中——其 MSA 稀疏注意力架构显著降低了长上下文计算成本。Google Gemma 4 12B 可安装在笔记本电脑上，并在本地运行完整的智能体工作流程，使以隐私为先、低延迟的人工智能应用真正成为现实。

🛠️ Agent products are reaching knowledge workers beyond developers. Kimi Work brings long-horizon execution and multi-agent parallelism to a desktop GUI built for finance, research, and office work. Coze 3.0 organizes Agents into project spaces with a skill store and cross-device coordination, forming a schedulable AI team. The audience for Agent products is expanding fast.

🛠️ 智能体产品正在惠及开发者以外的知识工作者。Kimi Work 将长期执行和多智能体并行处理功能引入专为金融、研究和办公工作打造的桌面图形用户界面。Coze 3.0 将智能体组织到项目空间中，并配备技能库和跨设备协调功能，从而构建可调度的 AI 团队。智能体产品的用户群体正在迅速扩大。

🔄 Microsoft SkillOpt: training Agent skills like neural network weights. The framework treats Agent skill documents as external trainable weights and runs a Rollout-Reflect-Edit-Gate loop to improve them automatically, earning 3,300 GitHub stars in one week. This moves prompt and skill engineering from hand-tuning to systematic optimization, a potential cornerstone for Agent infrastructure.

🔄 Microsoft SkillOpt：像训练神经网络权重一样训练智能体技能。该框架将智能体技能文档视为外部可训练权重，并运行一个“发布-反馈-编辑-门控”循环来自动改进它们，一周内就获得了 3300 个 GitHub 星标。这使得提示和技能工程从手动调整转向系统化优化，这有望成为智能体基础架构的基石。

⚡ Claude Code dynamic workflows: sub-agent orchestration breaks the context ceiling. Anthropic's new harness lets the model build a custom workflow on the fly for each task, spinning up independent sub-agents to handle large-scale parallel work, structured pipelines, or adversarial challenges, effectively overcoming the laziness and goal drift that plagues long single-context runs.

⚡ Claude Code 动态工作流：子智能体编排突破了上下文限制。Anthropic 的全新工具让模型能够针对每个任务动态构建自定义工作流，启动独立的子智能体来处理大规模并行工作、结构化流水线或对抗性挑战，从而有效克服长时间单上下文运行中常见的惰性和目标漂移问题。

🏗️ Anthropic opened up its AI-native engineering playbook. The team has moved from six-month roadmaps to immediate planning, uses Claude for most context gathering and code review, and has humans focus on product judgment and deep systems work. Hiring criteria have shifted toward builders with product instincts and deep systems specialists rather than pure executors.

🏗️ Anthropic 公开了其人工智能原生工程的运作模式。团队已从六个月的路线图制定转向即时规划，主要使用 Claude 进行上下文信息收集和代码审查，并让人类专注于产品判断和深度系统开发。招聘标准也从纯粹的执行者转向具备产品直觉的构建者和深度系统专家。

📐 A wave of long-form essays maps the new coordinates of software engineering. Tencent Cloud's manifesto for an AI-centered paradigm, Alibaba's shift from People-Oriented to Agent-Oriented infrastructure, Alibaba Cloud's LLM-Wiki plus skill-package automation framework, and Alibaba's AI Friendly architecture with three evolutionary patterns — each from a different angle, all pointing at the same conclusion: software engineering is undergoing its most fundamental paradigm shift in fifty years.

📐 一系列长篇论文描绘了软件工程的新坐标。腾讯云提出的以人工智能为中心的范式宣言、阿里巴巴从以人为本的基础设施向以代理为本的基础设施的转变、阿里云的LLM-Wiki加技能包自动化框架，以及阿里巴巴的AI友好型架构及其三种演进模式——每篇文章都从不同的角度出发，但都指向同一个结论：软件工程正在经历五十年来最根本的范式转变。

🔍 Tencent's 55,000-word source-level Agent architecture teardown. OpenClaw's microkernel, Gateway routing, Channel contracts, and memory system are dissected alongside Hermes' monolithic design, covering tool orchestration, security boundaries, and multi-client Agent design. A rare engineering reference for teams building production Agent systems with long-term memory or cross-platform support.

🔍 腾讯长达 55,000 字的 Agent 架构源代码级拆解报告。报告深入剖析了 OpenClaw 的微内核、网关路由、通道合约和内存系统，并结合 Hermes 的单体架构，涵盖了工具编排、安全边界和多客户端 Agent 设计。对于构建具有长期记忆或跨平台支持的生产级 Agent 系统的团队而言，这是一份难得的工程参考资料。

🌐 Industry signals from three directions. Satya Nadella at Microsoft Build laid out the case for a frontier intelligence platform and the Work IQ context layer for enterprises. Jensen Huang at COMPUTEX 2026 previewed the Agent factory stack from Vera Rubin chips to humanoid robots. And Ruanyifeng translated a US delegation's firsthand observations from 14 Chinese AI firms: the compute gap is roughly 8x in favor of the US, but China achieves 4 to 7 times more intelligence per FLOP, driven by efficiency innovation under chip constraints.

🌐 行业信号来自三个方面。萨蒂亚·纳德拉在微软Build大会上阐述了面向企业的前沿智能平台和Work IQ情境层的重要性。黄仁勋在2026年台北国际电脑展上预览了从维拉·鲁宾芯片到人形机器人的智能体工厂堆栈。阮义峰则转述了美国代表团对14家中国人工智能企业的第一手观察：尽管美国在计算能力方面拥有大约8倍的优势，但中国在芯片限制下通过效率创新，实现了每浮点运算4到7倍的智能水平。

🧩 People and organizations in the Agent era: super-individuals, new roles, and cognitive sovereignty. Tencent Research's 30,000-word report examines how super-individuals aggregate into super-teams. A Crossing podcast episode unpacks FDE as a new organizational role born from AI deployment. Benedict Evans argues that AI automates tasks not jobs, and Jevons' paradox will increase overall demand. And a thoughtful essay warns that as AI provides ready answers, people quietly stop questioning — protecting that habit of independent thought may be the most important cognitive investment of our time.

🧩 智能体时代的人和组织：超级个体、新角色和认知主权。腾讯研究院发布的3万字报告探讨了超级个体如何聚合为超级团队。Crossing播客的一期节目深入剖析了人工智能部署催生出的新型组织角色——功能性决策执行者（FDE）。本尼迪克特·埃文斯认为，人工智能自动化的是任务而非工作，而杰文斯悖论将增加整体需求。一篇发人深省的文章警告说，随着人工智能提供现成的答案，人们会悄然停止质疑——保护独立思考的习惯或许是我们这个时代最重要的认知投资。

