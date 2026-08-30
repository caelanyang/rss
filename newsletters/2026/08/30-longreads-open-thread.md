# Longreads + Open Thread

**来源：** Byrne @ The Diff  
**日期：** 2026-08-30  
**查看原邮件：** <https://mail.google.com/mail/u/1/#search/subject%3A%22Longreads%20%2B%20Open%20Thread%22>

---

Longreads + Open Thread
By Byrne Hobart • 29 Aug 2026
Longreads
* A while ago, The Diff wrote about the Strategic Petroleum Reserve as a way for the US to write synthetic options on oil, hedged by its ability to allow more oil production and print more dollars ($). Turns out, it's also a physical place, and Brian Potter has written about how it works .

> **译文：** * 不久前，The Diff 曾撰文讨论战略石油储备（Strategic Petroleum Reserve），将其视为美国书写石油合成期权的一种方式，并以允许更多石油生产和印发更多美元（$）作为对冲。事实证明，它也是一个实体场所，Brian Potter 撰文介绍了其运作方式。

It's kind of a nice callback that oil is an incredibly convenient energy source we extract from the ground, and it's so useful that it would be a catastrophe if we lost access, but we use it in such volumes that it's expensive to store, but thanks to another geological feature, we can actually carve out big storage containers from salt domes. (The way to hollow them out is, basically, pump in freshwater, wait, pump out saltwater, repeat.) This turns out to be a great hack for storing oil for one big emergency, but a bit worse as a way to constantly tweak the supply.

> **译文：** 这算是一个不错的呼应：石油是我们从地下提取的极其便捷的能源，它如此有用，以至于一旦失去获取途径将是一场灾难，但我们的使用量之大使得储存成本高昂。然而，得益于另一种地质特征，我们实际上可以从盐丘中开凿出大型储存容器。（将其掏空的方法基本上是：注入淡水，等待，抽出盐水，重复进行。）事实证明，这是为一次重大紧急情况储存石油的绝妙技巧，但作为持续微调供应的手段则稍显逊色。

Interestingly enough, there's a kind of options contract called a swing option that maps to these physical limitations, so you can still think of the SPR as an option-writing strategy, just one that's a little more complicated to price.

> **译文：** 有趣的是，有一种名为摆动期权（swing option）的期权合约恰好对应这些物理限制，因此你仍然可以将战略石油储备视为一种期权写入策略，只是其定价稍微复杂一些。

* Dan Luu argues that slow software is now a choice : you can keep throwing inference at the problem of making something faster, including a mix of small improvements that a human programmer wouldn't think were worth the time and big but uncertain ones that a human might think weren't worth the risk that they'd take too long. The most interesting bit is the tradeoff between more compute and domain expertise. Luu built a game AI using LLMs, and found that his was better than the state of the art.

> **译文：** * Dan Luu 认为，软件运行缓慢如今是一种选择：你可以不断将推理能力投入到让某物更快的问题上，包括混合使用人类程序员认为不值得花时间的小改进，以及人类可能认为风险太大、耗时过长而不愿尝试的大而不确定的改进。最有趣的部分在于更多算力与领域专业知识之间的权衡。Luu 使用大语言模型构建了一个游戏 AI，并发现他的 AI 优于现有最先进水平。

But that was mostly because it could brute-force more effectively; the best competitors were cleverer, but too slow. He claims that every doubling of speed adds 100 to the Elo, which is a convenient rule of thumb to keep in mind if it generalizes.

> **译文：** 但这主要是因为他的 AI 能更有效地进行暴力计算；最佳竞争对手更聪明，但速度太慢。他声称，速度每翻一倍，Elo 评分就增加 100 点，如果这一规律具有普适性，倒是一个方便的经验法则。

There seems to be a general correlation between corporate success and caring a little more about latency than seems reasonable, at scales that range from how fast clicking a button does something to how long it takes to answer an email to how long it takes to negotiate an acquisition. Speed matters!

> **译文：** 企业成功与对延迟（latency）比看似合理程度更在意之间似乎存在普遍相关性，其范围从点击按钮后响应多快，到回复电子邮件需要多长时间，再到完成一项收购谈判需要多久。速度很重要！

* When people talk about the environmental impact of AI, they tend to use the broadest measure they can. Which is fair! If a datacenter is the reason a coal power plant didn't get shut down, it's a contribution to emissions. But doing this right means looking at cases where the emissions impact is negative, like rerouting drivers so their trip time is imperceptibly longer in order to make the average driver's trip faster, alongside a slight decrease in emissions . As with the piece above, there are many domains that weren't worth optimizing because collecting the data would be such a schlep. Now that's less true.

> **译文：** * 当人们谈论 AI 对环境的影响时，他们往往倾向于使用最宽泛的衡量标准。这很公平！如果一座数据中心是燃煤电厂未被关停的原因，那它就对排放有所贡献。但要做到准确评估，就需要考察排放影响为负面的案例，比如重新规划司机路线，使他们的行程时间几乎察觉不到地延长，从而让平均司机的行程更快，同时排放略有下降。与上文一样，许多领域此前因收集数据过于繁琐而不值得优化。如今情况已不再如此。

* Jack Despain Zhou on how learning with AI can make you feel like you're learning, at the expense of actually learning . In one sense, this is entirely possible. On the other hand, one of the studies cited compares students who did and didn't use AI; the AI users finished their homework much faster and got better scores, but did worse on their exams. However!

> **译文：** * Jack Despain Zhou 探讨了使用 AI 学习如何让你感觉自己在学习，却以真正学习为代价。从某种意义上说，这完全有可能。另一方面，其中引用的一项研究比较了使用和未使用 AI 的学生；使用 AI 的学生完成作业的速度快得多，成绩也更好，但考试表现更差。然而！

The magnitude of the homework time saving was bigger than the magnitude of the average test score gap; eyeballing the charts, the modal exam scores aren't that far apart, but there's a long tail of AI users who, to varying degrees, absolutely bombed the exam. Meanwhile, the right tails fo the distribution aren't as skewed.

> **译文：** 作业时间节省的幅度大于平均考试成绩差距的幅度；粗略观察图表，众数（modal）考试成绩相差不大，但有一长尾的 AI 使用者以不同程度彻底考砸了考试。与此同时，分布的右尾并不那么偏斜。

So, using AI to learn is kind of a Ring of Power: do it responsibly, and you will speed through the boring stuff and be able get hard concepts paraphrased over and over again until you've brute-forced your way into understanding them. There was certainly a point in the history of math education where calculators would have had this effect, but now we're in the era where teaching students how and when to use calculators is more effective than skipping this.

> **译文：** 因此，使用 AI 学习有点像一枚权力之戒（Ring of Power）：负责任地使用，你就能快速通过枯燥的内容，并能反复获得对困难概念的改写解释，直到你通过蛮力理解它们。在数学教育史上，确实曾有一个阶段计算器会产生这种效果，但如今我们正处于这样一个时代：教学生如何以及何时使用计算器，比跳过这一步更有效。

* Brad Burnham, Fred Wilson, Dayna Gant, and Lindel Eakman on how the first Union Square Ventures fund was raised . Interesting throughout, half because of what's changed, half because of what hasn't.

> **译文：** * Brad Burnham、Fred Wilson、Dayna Gant 和 Lindel Eakman 讲述了第一只 Union Square Ventures 基金是如何募集的。全文都很有趣，一半是因为变化之处，一半是因为未变之处。

One fun detail is that raising a new venture fund in the early 2000s was partly a form of regulatory arbitrage: public pension funds had recently been required to disclose more data about returns, and so the biggest venture funds stopped raising from them in order to keep their performance confidential. Which meant that those LPs were under-allocated to venture, and a new fund that put a lower value on secrecy could raise from them.

> **译文：** 一个有趣的细节是，在 2000 年代初募集新风险投资基金部分是一种监管套利：公共养老基金当时被要求披露更多回报数据，因此最大的风险基金停止向它们募资，以保持自身业绩的机密性。这意味着这些有限合伙人（LP）在风险投资上的配置不足，而一个对保密性重视程度较低的新基金可以从它们那里募资。

You could have looked at a new fund in this period as a quick money-grab, more focused on an opportunistic 2 than on an uncertain 20. But success tends to be correlated: someone who finds a good tactical way to raise money from investors they couldn't otherwise reach is probably better than average at strategically deploying what they raise. (Via Trevor Mckendrick .)

> **译文：** 你可以将这一时期的新基金视为一种快速捞钱之举，更关注机会主义的 2（管理费），而非不确定的 20（业绩报酬）。但成功往往具有相关性：一个能找到巧妙战术性方式从原本无法触及的投资者那里募资的人，在战略性部署所募资金方面可能也优于平均水平。（Via Trevor Mckendrick。）

* On Read.Haus, someone asks what to do if you're a founder who controls a company that's no longer growing , if you're worried that you may not be able to harvest the cash flows. In practice, there seem to be a few different answers.

> **译文：** * 在 Read.Haus 上，有人提问：如果你是一位创始人，控制着一家不再增长的公司，并且担心自己可能无法兑现现金流，该怎么办？在实践中，似乎有几种不同的答案。

One is that some companies try to maximize profits over some period, or hit some growth rate, but the most interesting thing to optimize for is maximizing your growth rate a few years out, i.e. making decisions today that give you the highest odds of being able to grow at a similar rate five years from now. That tends to involve solving some scaling problems that aren't problems yet, and sometimes reveals new kinds of growth.

> **译文：** 一种是，一些公司试图在某个时期内最大化利润，或达到某个增长率，但最值得优化的目标是最大化你几年后的增长率，也就是说，今天做出的决策能让你在五年后以类似速度增长的概率最高。这往往涉及解决一些尚未成为问题的扩展难题，有时还会揭示新的增长类型。

Another pretty conventional answer is that founders should diversify gradually: having most of your money in a mature business is a smaller problem than having most of your money in a high-growth and high-uncertainty one.

> **译文：** 另一个相当常规的答案是，创始人应该逐步分散投资：将大部分资金放在成熟业务中，比将大部分资金放在高增长、高不确定性的业务中问题更小。

The last answer is that PE firms are partly in the business of making this somebody else's problem: there is a level of leverage that allows a mature company's returns to equity holders to be closer to what people demand from venture, but running things that way is a different specialization from running a growth company or taking care of a stable one. Life is full of tradeoffs, and being undiversified has a cost in the form of volatility drag.

> **译文：** 最后一个答案是，私募股权（PE）公司在一定程度上就是在做把这个问题变成别人问题的事情：存在某种杠杆水平，能让成熟公司对股权持有者的回报更接近人们对风险投资的要求，但以这种方式运营是一种不同于经营成长型公司或照看稳定公司的专业分工。生活充满权衡，而缺乏分散化会以波动拖累（volatility drag）的形式付出代价。

So perhaps the best way to think about this is that maintaining control of a company and refusing to diversify is the world's most expensive luxury good.

> **译文：** 因此，也许最好的思考方式是：保持对公司的控制并拒绝分散化，是世界上最昂贵的奢侈品。

* In Capital Gains, a discussion of how a tech-driven equity bubble can turn into one based on financial engineering . This is, of course, all about how in the 1920s, corporate treasurers found that they could lend their cash to banks that made margin loans and earn more money than their earnings yield, creating a loop where investors paid high interest rates to invest in companies whose earnings were, increasingly, from lending to those same investors.

> **译文：** * 在 Capital Gains 中，有一篇讨论科技驱动的股票泡沫如何转变为基于金融工程的泡沫。这当然完全是关于 1920 年代企业财务主管发现他们可以将现金借给提供保证金贷款的银行，赚取高于其盈利收益率（earnings yield）的回报，从而形成一个循环：投资者支付高利率投资于那些收益越来越依赖于向这些同一批投资者放贷的公司。

You're on the free list for The Diff! This week, paying subscribers read about how non-AI companies want to get control of the flow of data, and to steer towards places that generate more training data ($); Meta's effort to rewrite the rules of teen social media use ($); and AI agents as eusocial organisms subject to evolutionary pressure ($), featuring an extended digression about whether or not evolution has risk premia. Upgrade today for full access.

> **译文：** 你正在阅读 The Diff 的免费列表！本周，付费订阅者阅读了关于非 AI 公司如何希望掌控数据流并引导向生成更多训练数据（$）的领域；Meta 改写青少年社交媒体使用规则的努力（$）；以及 AI 智能体作为受进化压力影响的真社会性生物（$），其中还包含一段关于进化是否存在风险溢价的长篇离题讨论。立即升级以获取完整访问权限。

Upgrade Today
Books
Rickover: The Struggle for Excellence : There are many modern jobs that make me wonder what the people who are good at them used to do before that job existed. Someone who's technically skilled and incredibly driven today is going to get a lot of social cues about how to turn those skills into an interesting and lucrative career. But a few generations ago, there was less of a script, so you have to look elsewhere for that archetype. Specifically, you can look at someone like Hyman Rickover. Rickover was born in Poland in 1900, grew up in Chicago, joined the Navy, and led the development of the nuclear submarine fleet and later the Shippingport reactor, which used a pressurize-water design that later became standard for most reactors in the US.

> **译文：** 里科弗：追求卓越：当今有许多职业让我好奇，那些擅长这些工作的人，在职业诞生之前从事什么。如今，一个技术娴熟且极具驱动力的人会接收到大量社会信号，指引他们如何将这些技能转化为有趣且高薪的职业。但在几代人之前，这样的路径并不明确，因此你只能从别处寻找这种原型。具体来说，你可以看看海曼·里科弗这样的人。里科弗1900年出生于波兰，在芝加哥长大，加入海军，领导了核潜艇舰队的发展，后来还负责了希平波特反应堆项目，该反应堆采用了压水式设计，后来成为美国大多数反应堆的标准。

Rickover is partly a story about extreme social mobility, with a fun early ingredient: one of his first jobs, during high school, was delivering telegraphs. It's an unskilled job—if you have a bicycle and can read a street address, you can do it. But it's also a job with extreme variation in individual performance, and one that introduces some scrappy young people to a completely different social class that they might set out to join. (Andrew Carnegie's career also accelerated when he started delivering messages like this; both he and Rickover found ways to get the highest-value messages, which meant both better tips and better connections.)

> **译文：** 里科弗的故事部分是关于极端的社会流动性，其中有一个有趣的早期细节：他高中时期的第一份工作之一是送电报。这是一份无需技能的活儿——如果你有自行车，能看懂街道地址，就能胜任。但这也是一份个人表现差异极大的工作，它让一些有闯劲的年轻人接触到他们可能立志加入的完全不同的社会阶层。（安德鲁·卡内基的职业生涯也是从这样送信开始加速的；他和里科弗都设法获取最有价值的电报，这意味着既能有更多小费，也能建立更好的人脉。）

Rickover, with a bit of political maneuvering, got admitted to the Naval Academy, and spent time in positions of increasing responsibility aboard battleships and submarines. He seems to have developed an early instinct for constant optimization. The fleet had an internal competition about engineering excellence, quantified on the basis of how little fuel and fresh water they needed to accomplish a mission. So Rickover would slow-walk repairs to heating equipment, mandated short showers, replaced lightbulbs with lower-watt ones, etc. He was very good at trading off anything and everything against numerical targets.

> **译文：** 里科弗通过一些政治手腕进入了海军学院，并在战列舰和潜艇上担任了责任越来越重的职务。他似乎很早就养成了不断优化的本能。舰队内部有一项关于工程卓越性的竞赛，以完成任务所需的燃料和淡水消耗量来衡量。因此，里科弗会拖延供暖设备的维修，规定缩短淋浴时间，更换低瓦数灯泡等。他非常擅长用一切东西去换取数字目标的达成。

The Rickover story is about politics and power, in a weird way. Rickover was extremely abrasive, and seemed to make lifelong enemies wherever he went. The general rule was that people loved his results but hated him, so he tended to get support that skipped a step or two in the org chart.

> **译文：** 里科弗的故事在某种程度上是关于政治和权力的。里科弗极其尖刻，似乎走到哪里都会树敌终身。普遍的规律是，人们喜欢他的成果但讨厌他本人，因此他往往能获得跳过组织架构中一两个层级的支持。

As he rose up the ranks, rising got harder because there was less room at the top, and at one point he was passed over for a promotion and could have been forced to retire, midway through the first nuclear submarine project.

> **译文：** 随着他职级上升，晋升变得越来越难，因为高层空间有限，有一次他在第一个核潜艇项目进行到一半时被跳过晋升，可能被迫退休。

His supporters were able to lobby for him, and made it a media project—it's hard to imagine it being a big news story today that the Navy failing to promote someone might delay a project, but it was big news, and led to lots of letters-to-Congressmen and other pressure until he got the promotion. Rickover was no one's ideal of a natural politician, but he had enough political sense to leave that job to other people.

> **译文：** 他的支持者设法为他游说，并将其变成了一个媒体事件——如今很难想象，海军未能晋升某人可能延误项目会成为大新闻，但当时这确实是重大新闻，引发了大量致国会议员的信件和其他压力，直到他获得晋升。里科弗绝非天生的政治家，但他有足够的政治敏感度，把这类事情交给别人去做。

One other thing that stands out about the book: he spends a surprising amount of time in the hospital for assorted illnesses. This is the kind of thing that I've paid more and more attention to in biographies as I've gotten older. Success usually involves some kind of compound interest, building up skills, connections, and different kinds of capital. So losing a year or two to illness is a pretty big deal, especially if there's some zero-sum aspect to the competition. The fact that Rickover didn't get derailed by his various medical problems means that, graded on a curve, he's even more impressive.

> **译文：** 这本书还有一个突出的特点：他因各种疾病住院的时间出奇地多。随着年龄增长，我在传记中越来越关注这类细节。成功通常涉及某种复利效应，积累技能、人脉和各种资本。因此，因病损失一两年时间是非常重大的事情，尤其是在竞争具有零和性质的情况下。里科弗没有被各种健康问题所击倒，这意味着，按曲线评分的话，他更加令人印象深刻。
