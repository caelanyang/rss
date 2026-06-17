# Why Do (Some) Chinese AI Labs Distill?

**来源：** Kevin Xu @ Interconnected  
**日期：** 2026-06-16  
**查看原邮件：** <https://mail.google.com/mail/u/1/#search/subject%3A%22Why%20Do%20%28Some%29%20Chinese%20AI%20Labs%20Distill%3F%22>

---

Interconnected [https://interconnected.blog/r/7e6a8c88?m=43f4d58a-3897-4544-a71f-6735dd312936]

互联 [https://interconnected.blog/r/7e6a8c88?m=43f4d58a-3897-4544-a71f-6735dd312936]

---

Why Do (Some) Chinese AI Labs Distill? [https://interconnected.blog/r/92754fed?m=43f4d58a-3897-4544-a71f-6735dd312936]

为什么（一些）中国人工智能实验室会进行蒸馏？[https://interconnected.blog/r/92754fed?m=43f4d58a-3897-4544-a71f-6735dd312936]

---

View in browser [https://interconnected.blog/r/e2b56c5c?m=43f4d58a-3897-4544-a71f-6735dd312936]

在浏览器中查看 [https://interconnected.blog/r/e2b56c5c?m=43f4d58a-3897-4544-a71f-6735dd312936]

---

View in browser [https://interconnected.blog/r/c3af58f0?m=43f4d58a-3897-4544-a71f-6735dd312936]

在浏览器中查看 [https://interconnected.blog/r/c3af58f0?m=43f4d58a-3897-4544-a71f-6735dd312936]

---

Ever since Anthropic released its report [https://interconnected.blog/r/de248bed?m=43f4d58a-3897-4544-a71f-6735dd312936] in February on three Chinese AI labs distilling its advanced models to train their own, I have been thinking a lot about adversarial distillation.

自从 Anthropic 在 2 月份发布了关于三个中国人工智能实验室提炼其先进模型来训练自己模型的报告 [https://interconnected.blog/r/de248bed?m=43f4d58a-3897-4544-a71f-6735dd312936] 以来，我一直在思考对抗蒸馏。

---

I carried my thoughts to China, when I recently visited [https://interconnected.blog/r/ef40d1e5?m=43f4d58a-3897-4544-a71f-6735dd312936] most of the leading labs there, including the three being accused. I tracked how the issue has evolved quickly into action [https://interconnected.blog/r/b3ca009f?m=43f4d58a-3897-4544-a71f-6735dd312936] and legislative proposals [https://interconnected.blog/r/d4f4fdd1?m=43f4d58a-3897-4544-a71f-6735dd312936] in Washington. I have monitored (the situation) of a growing narrative uttered by many that China, the entire country, distills (coded for steals) to make progress in AI, not three labs out of many from China who distills. And with Mythos and Fable coming under the crosshairs of government export control [https://interconnected.blog/r/50295ba0?m=43f4d58a-3897-4544-a71f-6735dd312936], I’m seeing many confidently predicting [https://interconnected.blog/r/33890aa8?m=43f4d58a-3897-4544-a71f-6735dd312936] that delayed or limited release of American frontier models mean the end of China’s industrial-scale stealing via distillation is near.

我带着这些想法去了中国，最近我访问了那里的大部分顶尖实验室，包括被指控的三家。我追踪了这个问题如何迅速演变为华盛顿的行动和立法提案。我一直关注着一种日益盛行的说法，即中国，整个国家，都在通过“提炼”（实际上是窃取）技术来推动人工智能的发展，而不仅仅是中国众多实验室中的三个。随着Mythos和Fable项目受到政府出口管制（https://interconnected.blog/r/50295ba0?m=43f4d58a-3897-4544-a71f-6735dd312936），我看到许多人自信地预测（https://interconnected.blog/r/33890aa8?m=43f4d58a-3897-4544-a71f-6735dd312936），美国前沿模型的延迟或有限发布意味着中国大规模“提炼”技术窃取的时代即将终结。

---

(You can say, I have been distilling about distillation, hey yo!!)

（你可以说，我一直在研究蒸馏，嘿哟！！）

---

After sitting on this issue for almost four months (I distill slow), here’s what I have learned and what I think is missing or misunderstood in the distillation debate.

在思考这个问题近四个月之后（我思考得很慢），以下是我学到的东西，以及我认为在蒸馏辩论中缺失或误解的东西。

---

There are many legitimate and proper reasons to use distillation in the broader AI landscape, from pure research [https://interconnected.blog/r/f4714b24?m=43f4d58a-3897-4544-a71f-6735dd312936], to reducing the size of a large model to a smaller one to be deployable on device, to refining a general purpose large model to a more specialized vertical model.

在更广泛的人工智能领域，有很多正当合理的理由可以使用蒸馏技术，从纯粹的研究[https://interconnected.blog/r/f4714b24?m=43f4d58a-3897-4544-a71f-6735dd312936]，到将大型模型缩小到可在设备上部署的较小模型，再到将通用的大型模型细化为更专业的垂直模型。

---

In the specific case of adversarial distillation, however, the primary reason why certain labs do it is data. As in to quickly fix a lack of data to improve model capabilities, either generally or for specific use cases, e.g. coding, computer use, etc.

然而，就对抗性蒸馏而言，某些实验室进行对抗性蒸馏的主要原因是数据。这是为了快速弥补数据不足，从而提升模型能力，无论是通用模型还是针对特定用例，例如编码、计算机使用等。

---

If you grasp this dimension, then why those three labs – DeepSeek, Moonshot, and MiniMax – were called out by Anthropic, but not other Chinese labs, is not so mysterious. Their relevant commonality is not that they are all from China, but that they are all independent labs struggling to obtain quality data to fuel their progress.

如果你理解了这一点，那么Anthropic公司为何点名批评DeepSeek、Moonshot和MiniMax这三家实验室，而没有批评其他中国实验室，也就不那么令人费解了。它们之间的共同点并非都来自中国，而是它们都是独立实验室，都在努力获取高质量数据以推动研究进展。

---

Out of the universe of AI labs in China, it is helpful to think of them in two categories: independent labs, like DeepSeek, Moonshot, MiniMax, Z, Stepfun, etc. and labs that live inside a giant tech company, like Qwen in Alibaba, Mimo in Xiaomi, Seed in ByteDance, Hunyuan in Tencent, etc. The independent labs resort to distillation as a shortcut, because they are more desperate for quality data. The labs that live within a big tech umbrella and have access to real world usage data from other business units inside the corporate family can (and do) leverage those data sources. This dynamic is the same as Google’s Gemini models leveraging YouTube data because they all live under the Alphabet umbrella.

在中国众多人工智能实验室中，我们可以将其分为两类：独立实验室，例如 DeepSeek、Moonshot、MiniMax、Z、Stepfun 等；以及隶属于大型科技公司的实验室，例如阿里巴巴旗下的智文科技、小米旗下的微模科技、字节跳动旗下的 Seed 科技、腾讯旗下的混源科技等。独立实验室由于更迫切需要高质量数据，因此往往采用数据提炼作为捷径。而隶属于大型科技公司旗下的实验室，由于能够获取集团内其他业务部门的真实用户数据，因此可以（也确实）利用这些数据资源。这种现象与谷歌的 Gemini 模型利用 YouTube 数据的情况类似，因为它们都隶属于 Alphabet 集团。

---

Does this mean big tech labs in China don’t practice adversarial distillation? Not necessarily, but at least the Almighty Anthropic has not caught their hands in the cookie jar, or they would have been called out publicly already. But if they do, they don't need to rely on distillation nearly as badly as the independent labs. Any measure to shut off or deter adversarial distillation won’t affect them as much.

这是否意味着中国的大型科技实验室不进行对抗性数据提炼？未必如此，但至少像安人智库这样的巨头还没有被抓到把柄，否则早就被公开谴责了。即便他们真的这么做了，他们对数据提炼的依赖程度也远不及独立实验室。任何旨在阻止或遏制对抗性数据提炼的措施对他们的影响都不会太大。

---

Thus, data or lack thereof is why some Chinese labs do adversarial distillation, but certainly not all. It is not an industrial-scale, country-wide, anti-imperial socialist undertaking.

因此，数据（或数据的缺乏）是部分中国实验室进行对抗性蒸馏的原因，但并非所有实验室都如此。这并非一项工业规模的、全国性的、反帝的社会主义行动。

---

One myth I want to bust here and now is that China actually does not have a data advantage, when it comes to frontier AI model development.

我想在这里破除一个迷思，那就是中国在尖端人工智能模型开发方面实际上并没有数据优势。

---

One thing I picked up on, which others in my group shared during our recent trip there, is that there is no full-fledged data industry in China to feed the AI labs. There is no Scale, Surge, Mercor, Handshake, or any number of data vendors, paying software engineers or management consultants to label and evaluate data, then selling that output to OpenAI or Anthropic for multiple millions of dollars.

我注意到一点，我们小组其他成员在最近的中国之行中也提到过，那就是中国还没有一个成熟的数据产业来支撑人工智能实验室。中国没有像Scale、Surge、Mercor、Handshake这样的公司，也没有其他任何数据供应商，他们雇佣软件工程师或管理顾问来标注和评估数据，然后将这些成果以数百万美元的价格卖给OpenAI或Anthropic。

---

All this flies in the face of a common view (and misconception) that China has a data advantage because it has a lot of people, they generate a lot of data, and there is no data privacy in China (another misconception), so China has a ton of data for AI. For some verticals, like manufacturing and supply chain, this is true, because there is just a lot of manufacturing and supply chain in China. But when it comes to general purpose knowledge or information that is useful to train large frontier models, much of which is derived from the Internet or structured knowledge work, China has no advantage whatsoever. (Let’s not forget, the Chinese internet also shrinks from time to time.)

所有这些都与一种普遍的观点（以及误解）相悖，即中国拥有数据优势，因为中国人口众多，产生大量数据，而且中国不存在数据隐私（这也是一种误解），所以中国拥有海量人工智能数据。对于某些垂直领域，例如制造业和供应链，这确实如此，因为中国的制造业和供应链规模庞大。但是，就通用知识或可用于训练大型前沿模型的信息而言，而这些信息大多来源于互联网或结构化知识库，中国在这方面没有任何优势。（别忘了，中国的互联网规模也会不时缩小。）

---

I distinctly remember a researcher we met telling us how much he loves CommonCrawl [https://interconnected.blog/r/63f75aad?m=43f4d58a-3897-4544-a71f-6735dd312936], the massive open dataset crawled from the web that every lab used to start their AGI journey. His team later shared that they’ve tried using some data vendors in China, but the quality was poor and couldn’t be guaranteed, so it was a waste of time and limited resources.

我清楚地记得，我们遇到的一位研究员告诉我们他有多么喜欢CommonCrawl [https://interconnected.blog/r/63f75aad?m=43f4d58a-3897-4544-a71f-6735dd312936]，这是一个从网络上抓取的庞大开放数据集，几乎每个实验室在开始通用人工智能（AGI）之旅时都会使用它。他的团队后来告诉我们，他们尝试过使用一些中国的数据供应商，但数据质量很差，而且无法保证，所以浪费了时间和有限的资源。

---

So for some labs, resorting to distillation is almost an act of desperation (and probably some laziness too), even if unseemly. Adversarial distillation is a shortcut to harvesting useful data, specifically chain of thought reasoning traces for post-training certain capabilities. Nothing more, nothing less.

因此，对某些实验室来说，诉诸数据蒸馏几乎是一种无奈之举（或许也带有一些懒惰的成分），即便这种做法并不体面。对抗性数据蒸馏是获取有用数据的捷径，具体来说，它能获取用于训练后特定能力的思维推理轨迹。仅此而已。

---

Join Interconnected Premium [https://interconnected.blog/r/cd1c20bb?m=43f4d58a-3897-4544-a71f-6735dd312936]

加入 Interconnected Premium [https://interconnected.blog/r/cd1c20bb?m=43f4d58a-3897-4544-a71f-6735dd312936]

---

Knowing all this, is it worth making such a big deal out of three (ok may four or five) independent labs’ adversarial distillation?

了解了所有这些之后，是否值得对三个（好吧，也许是四个或五个）独立实验室的对抗性蒸馏结果如此大惊小怪呢？

---

To be clear, Anthropic has every right to deny behaviors that violate its terms of service or simply does not like, much in the same way that my local restaurant can hang up a sign proclaiming its right to refuse service to anyone. As a supporter of free enterprises and free markets, I will always defend Anthropic or any private enterprise’s right to do so.

需要明确的是，Anthropic完全有权拒绝违反其服务条款或它不喜欢的行为，就像我常去的餐馆可以挂出告示，声明其有权拒绝为任何人提供服务一样。作为自由企业和自由市场的支持者，我将始终捍卫Anthropic或任何私营企业这样做的权利。

---

But if your entire professional and personal identity rests on a hardcore commitment to keep China behind the US in the “race [https://interconnected.blog/r/efd4d4ee?m=43f4d58a-3897-4544-a71f-6735dd312936]” to AGI, I don’t think anti-distillation policy is how you get there. At least, if you think what I shared in this post makes any sense, you should temper your expectations.

但是，如果你的整个职业和个人身份都建立在坚定不移地致力于让中国在通用人工智能（AGI）竞赛中落后于美国之上，那么我认为反蒸馏政策并不能让你达到目的。至少，如果你觉得我在这篇文章中分享的内容有任何道理，你应该降低你的期望值。

---

Lack of a robust data industry is a problem, but not a hard problem. It is not nearly as hard as building fully domestic EUV lithography machines at scale. This problem is also mostly a market dynamic one, not a technical one. If there is demand for a data industry, which is low-margin and low-barrier-to-entry, that demand will get met in China in the same way that American labs’ data hunger is fed.

缺乏强大的数据产业固然是个问题，但并非难事。它远没有大规模自主研发极紫外光刻机那么困难。这个问题主要是一个市场动态问题，而非技术问题。如果市场对利润微薄、准入门槛低的数据产业有需求，那么这种需求在中国就能得到满足，就像美国实验室的数据需求得到满足一样。

---

Does a regulated, delayed, or gated release of Mythos, Fable or more advanced model in the future change the dynamic?

未来对 Mythos、Fable 或更高级模型进行监管、延迟或限时发布是否会改变这种局面？

---

Not really. Because not every lab from China needs the distillation shortcut. If this shortcut is turned off for good, it will be a temporary setback for some labs who have come to rely on this tactic, then life moves on. It will hurt the independent labs the most, less so the big tech labs. Let’s be honest, the hardware usage data from Xiaomi or video data from ByteDance is at least as good as Apple’s or Google’s.

未必如此。因为并非所有中国实验室都需要这种数据提炼捷径。即便这种捷径被永久关闭，对于一些依赖此策略的实验室来说，也只是暂时的挫折，之后一切照旧。独立实验室受到的冲击最大，大型科技公司实验室受到的影响相对较小。说实话，小米的硬件使用数据或字节跳动的视频数据至少与苹果或谷歌的数据一样可靠。

---

In fact, I shared a thought [https://interconnected.blog/r/14c2397f?m=43f4d58a-3897-4544-a71f-6735dd312936] with Nathan Lambert a while back, when I was still distilling on this issue, that letting some distillation happen may not be a bad idea, if the goal is to keep a competitor behind. After all, contrary to the human experience, the student model (the distilled one) can never be more capable than the teacher model. But since humans are still the ones building AI (recursive self-improvement be damned), the smart, resourceful, and hardworking students do end up more capable than the teacher, whether the teacher keeps teaching or not.

事实上，我之前在思考这个问题时，曾和内森·兰伯特（Nathan Lambert）分享过一个想法[https://interconnected.blog/r/14c2397f?m=43f4d58a-3897-4544-a71f-6735dd312936]：如果目标是保持领先于竞争对手，那么允许一定程度的“提炼”或许并非坏事。毕竟，与人类经验相反，学生模型（提炼后的模型）的能力永远不可能超过教师模型。但由于人工智能仍然是由人类构建的（递归式自我改进什么的先放一边），聪明、足智多谋、勤奋努力的学生最终确实会比教师更胜一筹，无论教师是否继续授课。

---

Interconnected © 2026 – Unsubscribe [https://interconnected.blog/unsubscribe/?uuid=43f4d58a-3897-4544-a71f-6735dd312936&key=beb0aaab04ae9594cdc0219f6859dd5edeb7e152bd47367cb1078f953d064dce&newsletter=0d889f70-7c61-4386-827d-2e7cf02fa103]

Interconnected © 2026 – 取消订阅 [https://interconnected.blog/unsubscribe/?uuid=43f4d58a-3897-4544-a71f-6735dd312936&key=beb0aaab04ae9594cdc0219f6859dd5edeb7e152bd47367cb1078f953d064dce&newsletter=0d889f70-7c61-4386-827d-2e7cf02fa103]

---

