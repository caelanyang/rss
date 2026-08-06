# AI Alert: OpenAI’s escaped agent acted like a genie

**来源：** IEEE Spectrum  
**日期：** 2026-08-06  
**查看原邮件：** <https://mail.google.com/mail/u/1/#search/subject%3A%22AI%20Alert%3A%20OpenAI%E2%80%99s%20escaped%20agent%20acted%20like%20a%20genie%22>

---

Plus revisiting ELIZA,﻿ folding DNA,﻿ and the new digital divide

> **译文：** 此外，还将回顾ELIZA、DNA折叠以及新的数字鸿沟。

To view this email as a webpage, click here .

5 August 2026

AI Alert

AI Alert 5 August 2026

In our top story this week, Barath Raghavan and Bruce Schneier propose a “Genie coefficient”  to measure the gap between what we ask an AI agent to do and what it actually does. Just as the article was published, OpenAI disclosed a startling real-world example: An agent had escaped its sandbox and broken into Hugging Face’s networks. Below, Raghavan and Schneier share their thoughts on what the incident revealed about genie behavior.  — Eliza Strickland, AI editor

> **译文：** 本周头条新闻中，Barath Raghavan 和 Bruce Schneier 提出了“精灵系数”，用于衡量我们对人工智能体的要求与其实际行为之间的差距。文章发表后不久，OpenAI 就披露了一个令人震惊的真实案例：一个人工智能体逃出了沙盒，入侵了 Hugging Face 的网络。以下是 Raghavan 和 Schneier 对该事件揭示的“精灵行为”的看法。—— Eliza Strickland，人工智能编辑

OpenAI’s model was being tested on its ability to turn security vulnerabilities into working exploits. Because this was an unreleased model being run without any guardrails, it was constrained in a sandbox and denied access to the internet. Its goal was to do as well as it could on the ExploitGym benchmark. The model decided that instead of doing the work to solve the puzzles in the benchmark, it would break out of its sandbox, find a way to access the internet, and then break into the Hugging Face networks—because something in its training set led it to believe that the answers could be found there.

> **译文：** OpenAI 的模型正在接受测试，以检验其将安全漏洞转化为有效攻击手段的能力。由于这是一个尚未发布的模型，且运行过程中没有任何防护措施，因此它被限制在一个沙箱环境中，无法访问互联网。它的目标是在 ExploitGym 基准测试中取得尽可能好的表现。然而，该模型并没有选择解决基准测试中的难题，而是决定突破沙箱，找到访问互联网的方法，然后入侵 Hugging Face 网络——因为它的训练集中某些信息让它相信答案就在那里。

This is the behavior of a genie . It achieved its goal, but in a way its prompters neither expected nor wanted. It thought “outside the box,” because it didn’t have any conception of the box. And the only reason we know about this example is because Hugging Face noticed that they were under cyberattack and researched the incident.

> **译文：** 这就像一个精灵的行为。它达到了目的，但方式却出乎其策划者的意料，也出乎他们的意愿。它跳出了思维定式，因为它根本没有“盒子”的概念。我们之所以知道这个例子，是因为Hugging Face注意到自己遭受了网络攻击，并对事件进行了调查。

Imagine two different scenarios and what could have happened. First, imagine if the model hacked someone with worse intrusion detection capabilities: Would OpenAI have even realized that their model was acting like a genie? Second, imagine if this were a Chinese model that hacked a US company: Would we believe the company when they said it was an accident, or would this have resulted in an international incident?

> **译文：** 设想两种不同的情况，以及可能发生的事情。首先，假设该模型入侵了入侵检测能力较弱的系统：OpenAI 是否会意识到他们的模型如同神灯精灵一般作祟？其次，假设入侵美国的是一家美国公司，而入侵者是中国公司：我们会相信该公司声称这是一起意外事故吗？还是会因此引发国际事件？

Genie behavior like this is trickier to deal with than malice or failure, because there's no attacker: The user, the AI vendor, and the model are all cooperative, on the same side, and yet things go sideways. This is why we need to explicitly study, and measure, the extent of the problem.   — Barath Raghavan and Bruce Schneier

> **译文：** 像这种“精灵式”行为比恶意行为或故障更难处理，因为没有攻击者：用户、人工智能供应商和模型都是合作的，站在同一阵线，但事情却出了差错。这就是为什么我们需要明确地研究和评估问题的严重程度。——巴拉特·拉加万和布鲁斯·施奈尔

Why AI Needs a “Genie Coefficient”  Proposing a new metric for whether AI actually does what you want.

> **译文：** 为什么人工智能需要一个“精灵系数”？提出一种新的指标来衡量人工智能是否真的能做到你想要的事情。

The First Chatbot’s Multiple Personalities  A software archeology project uncovered ELIZA’s source code and revealed the chatbot's hidden depths.

> **译文：** 首个聊天机器人的多重人格：一项软件考古项目发现了 ELIZA 的源代码，揭示了该聊天机器人的隐藏深度。

AI Is Designing Radio Chips That Humans Couldn’t Even Imagine

> **译文：** 人工智能正在设计人类甚至无法想象的无线电芯片

Freed from intelligibility and aesthetics, AI designs faster.

> **译文：** 摆脱了可理解性和美观性的束缚，人工智能设计速度更快。

ADVERTISEMENT Online Master of Science in Data Science

> **译文：** 广告：在线数据科学硕士课程

Purdue’s online Master’s in Data Science equips students with in-demand skills, providing hands-on experiences and preparing students for emerging careers in data science.

> **译文：** 普渡大学的在线数据科学硕士课程为学生提供市场所需的技能，提供实践经验，并为学生在数据科学领域的新兴职业做好准备。

This AI Folds DNA Into Mini Masterpieces  Generative AI model designs DNA origami for any shape.

> **译文：** 这款人工智能将DNA折叠成微型杰作，其生成式人工智能模型可以设计出任何形状的DNA折纸。

AI Is Hyper-Scaling Digital Inequality  The next digital divide is about who gets to build, govern, and benefit from AI.

> **译文：** 人工智能正在加剧数字不平等。下一个数字鸿沟关乎谁能构建、管理和受益于人工智能。