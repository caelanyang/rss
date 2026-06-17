# Why Do (Some) Chinese AI Labs Distill?

**来源：** Interconnected (Kevin Xu)  
**日期：** 2026-06-17  
**查看原邮件：** <https://mail.google.com/mail/u/1/#search/subject%3A%22Why%20Do%20%28Some%29%20Chinese%20AI%20Labs%20Distill%3F%22>

---

Why Do (Some) Chinese AI Labs Distill?
And why the Mythos/Fable drama doesn't matter here
By Kevin Xu, Jun 16, 2026

为什么（部分）中国人工智能实验室会进行数据提炼？

以及为什么神话/寓言式的争论在这里并不重要

作者：徐凯文，2026年6月16日

Ever since Anthropic released its report in February on three Chinese AI labs distilling its advanced models to train their own, I have been thinking a lot about adversarial distillation.

自从 Anthropic 在 2 月份发布报告，指出三个中国人工智能实验室正在提炼其先进模型来训练自己的模型以来，我一直在思考对抗蒸馏的问题。

I carried my thoughts to China, when I recently visited most of the leading labs there, including the three being accused. I tracked how the issue has evolved quickly into action and legislative proposals in Washington. I have monitored a growing narrative that China, the entire country, distills (coded for steals) to make progress in AI, not three labs out of many from China who distills.

我带着这些想法去了中国，最近我走访了那里的大部分顶尖实验室，包括被指控的那三家。我追踪了这个问题如何迅速演变为华盛顿的行动和立法提案。我注意到一种日益盛行的说法，即整个中国都在进行技术提炼（实际上是窃取）以推动人工智能的发展，而不仅仅是中国众多实验室中的三家。

Distillation Is Data Strategy

There are many legitimate and proper reasons to use distillation in the broader AI landscape, from pure research, to reducing the size of a large model to a smaller one to be deployable on device, to refining a general purpose large model to a more specialized vertical model.

在更广泛的人工智能领域，从纯粹的研究到将大型模型缩小到可在设备上部署的较小模型，再到将通用大型模型提炼成更专业的垂直模型，使用蒸馏有很多正当合理的理由。

In the specific case of adversarial distillation, the primary reason why certain labs do it is data. As in to quickly fix a lack of data to improve model capabilities, either generally or for specific use cases.

就对抗性蒸馏而言，某些实验室进行对抗性蒸馏的主要原因是数据。也就是说，为了快速弥补数据不足，从而提升模型的整体性能或针对特定用例的性能。

If you grasp this dimension, then why those three labs — DeepSeek, Moonshot, and MiniMax — were called out by Anthropic, but not other Chinese labs, is not so mysterious. Their relevant commonality is not that they are all from China, but that they are all independent labs struggling to obtain quality data to fuel their progress.

如果你理解了这一点，那么Anthropic公司为何点名批评DeepSeek、Moonshot和MiniMax这三家实验室，而没有批评其他中国实验室，也就不那么令人费解了。它们之间的共同点并非都来自中国，而是它们都是独立实验室，都在努力获取高质量数据以推动研究进展。

Out of the universe of AI labs in China, it is helpful to think of them in two categories: independent labs, like DeepSeek, Moonshot, MiniMax, Z, Stepfun, etc. and labs that live inside a giant tech company, like Qwen in Alibaba, Mimo in Xiaomi, Seed in ByteDance, Hunyuan in Tencent, etc. The independent labs resort to distillation as a shortcut, because they are more desperate for quality data. The labs that live within a big tech umbrella and have access to real world usage data from other business units inside the corporate family can leverage those data sources.

在中国众多人工智能实验室中，我们可以将其分为两类：独立实验室，例如 DeepSeek、Moonshot、MiniMax、Z、Stepfun 等；以及隶属于大型科技公司的实验室，例如阿里巴巴旗下的智文科技、小米旗下的微墨科技、字节跳动旗下的 Seed 科技、腾讯旗下的混源科技等。独立实验室由于更迫切需要高质量数据，因此往往采用数据提炼作为捷径。而隶属于大型科技公司旗下的实验室，由于能够获取集团内其他业务部门提供的真实世界使用数据，则可以充分利用这些数据资源。

Does this mean big tech labs in China don't practice adversarial distillation? Not necessarily, but at least Anthropic has not caught their hands in the cookie jar. Any measure to shut off or deter adversarial distillation won't affect them as much.

这是否意味着中国的大型科技实验室不进行对抗性蒸馏？未必如此，但至少Anthropic公司还没有被牵连其中。任何旨在关闭或阻止对抗性蒸馏的措施对它们的影响都不会太大。

No Data Advantage in China

One myth I want to bust: China actually does not have a data advantage, when it comes to frontier AI model development.

我想打破的一个迷思是：在尖端人工智能模型开发方面，中国实际上并没有数据优势。

There is no full-fledged data industry in China to feed the AI labs. There is no Scale, Surge, Mercor, Handshake, or any number of data vendors, paying software engineers or management consultants to label and evaluate data, then selling that output to OpenAI or Anthropic for multiple millions of dollars.

中国没有成熟的数据产业来支撑人工智能实验室。没有像Scale、Surge、Mercor、Handshake或其他任何数据供应商那样，雇佣软件工程师或管理顾问来标注和评估数据，然后将评估结果以数百万美元的价格出售给OpenAI或Anthropic等公司。

All this flies in the face of a common view that China has a data advantage because it has a lot of people, they generate a lot of data, and there is no data privacy in China. For some verticals, like manufacturing and supply chain, this is true. But when it comes to general purpose knowledge or information that is useful to train large frontier models, China has no advantage whatsoever.

所有这些都与一种普遍观点相悖，即中国拥有数据优势，因为中国人口众多，数据量巨大，而且中国不存在数据隐私问题。对于某些垂直领域，例如制造业和供应链，这种说法是正确的。但就通用知识或可用于训练大型前沿模型的信息而言，中国没有任何优势。

A researcher shared that they've tried using some data vendors in China, but the quality was poor and couldn't be guaranteed. So for some labs, resorting to distillation is almost an act of desperation, even if unseemly. Adversarial distillation is a shortcut to harvesting useful data, specifically chain of thought reasoning traces for post-training certain capabilities.

一位研究人员表示，他们曾尝试使用一些中国的数据供应商，但数据质量差强人意，无法保证。因此，对于一些实验室来说，诉诸对抗蒸馏几乎是一种无奈之举，即便这种做法并不体面。对抗蒸馏是一种快速获取有用数据的捷径，特别是用于训练后特定能力的思维推理轨迹。

Anti-Distillation As Policy

Is it worth making such a big deal out of three independent labs' adversarial distillation?

三个独立实验室的对抗性蒸馏结果值得如此重视吗？

Anthropic has every right to deny behaviors that violate its terms of service. But if your entire professional identity rests on a hardcore commitment to keep China behind the US in the "race" to AGI, anti-distillation policy is not how you get there.

Anthropic公司完全有权拒绝违反其服务条款的行为。但是，如果你的整个职业认同都建立在坚定不移地致力于在通用人工智能（AGI）“竞赛”中将中国远远甩在美国之上，那么反蒸馏政策绝非实现这一目标的正确途径。

Lack of a robust data industry is a problem, but not a hard problem. It is not nearly as hard as building fully domestic EUV lithography machines at scale. This problem is mostly a market dynamic one, not a technical one.

缺乏强大的数据产业固然是个问题，但并非难事。它远没有大规模自主研发极紫外光刻机那么困难。这个问题主要是一个市场动态问题，而非技术问题。

Does a regulated, delayed, or gated release of Mythos, Fable or more advanced model change the dynamic? Not really. Because not every lab from China needs the distillation shortcut. If this shortcut is turned off for good, it will be a temporary setback for some labs who have come to rely on this tactic, then life moves on. It will hurt the independent labs the most, less so the big tech labs.

对 Mythos、Fable 或更先进的型号进行监管、延迟或限时发布，会改变现状吗？其实不会。因为并非所有中国实验室都需要这种提纯捷径。如果这种捷径被永久关闭，对于一些依赖此策略的实验室来说，这只是暂时的挫折，之后一切照旧。独立实验室受到的冲击最大，大型科技实验室受到的影响较小。

In fact, letting some distillation happen may not be a bad idea, if the goal is to keep a competitor behind. After all, contrary to the human experience, the student model (the distilled one) can never be more capable than the teacher model. But since humans are still the ones building AI, the smart, resourceful, and hardworking students do end up more capable than the teacher, whether the teacher keeps teaching or not.

事实上，如果目标是保持领先于竞争对手，那么允许一定程度的提炼或许并非坏事。毕竟，与人类经验相反，学生模型（提炼后的模型）的能力永远不可能超过教师模型。但由于人工智能仍然是由人类构建的，因此无论教师是否继续授课，聪明、足智多谋且勤奋的学生最终都会比教师更胜一筹。
