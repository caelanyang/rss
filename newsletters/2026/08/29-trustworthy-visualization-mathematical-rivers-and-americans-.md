# Trustworthy visualization, mathematical rivers, and Americans not working

**来源：** Nathan Yau / FlowingData (newsletter@flowingdata.com)  
**日期：** 2026-08-29  
**查看原邮件：** <https://mail.google.com/mail/u/1/#search/subject%3A%22Trustworthy%20visualization%2C%20mathematical%20rivers%2C%20and%20Americans%20not%20working%22>

---

Hi, FlowingData readers. This week, I made a bunch of charts to see why different groups are not in the labor force. There’s also a fun talk about visualization and a turn against data centers, which everyone definitely loves.

> **译文：** 嗨，FlowingData的读者们。本周，我制作了一系列图表，探究不同群体为何未进入劳动力市场。此外，还有一场关于可视化的趣味演讲，以及一篇关于数据中心遭遇反对的讨论——这个话题大家肯定都爱看。

## Why Americans are not working

About 62% of civilians in the United States, 16 years and older, said they either had a job or were looking in July 2026. Curious about the 38% who are not working, <a href="https://flowingdata.com/2026/08/25/who-is-not-working-and-why/" rel="noopener noreferrer nofollow" target="_blank"><span style="color: rgb(17, 17, 17);">I made a lot of line charts</span></a> .

> **译文：** 2026年7月，约62%的16岁及以上美国平民表示自己有工作或在找工作。对于那38%未工作的人群，我产生了好奇，<a href="https://flowingdata.com/2026/08/25/who-is-not-working-and-why/" rel="noopener noreferrer nofollow" target="_blank"><span style="color: rgb(17, 17, 17);">于是制作了大量折线图</span></a>。

Make it to the end, and there’s an interactive chart to see the numbers for your cohort.

> **译文：** 看到最后，还有一个交互式图表，可以查看你所在群体的数据。

**Trustworthy data visualization** — Kieran Healy, a professor of sociology at Duke University, gives an enjoyable lecture on the limits of trust in data visualization.

> **译文：** **可信的数据可视化**——杜克大学社会学教授Kieran Healy带来了一场关于数据可视化信任限度的精彩讲座。

**Mathematical rivers** — There is a simple law from John Hack that says the length of a river is proportional to its drainage area. For Quanta Magazine, Natalie Wolchover describes how this law applies everywhere.

> **译文：** **数学之河**——John Hack提出了一条简单定律：河流的长度与其流域面积成正比。在《Quanta Magazine》上，Natalie Wolchover描述了这一定律如何普遍适用。

In 1957, a U.S. Geological Survey scientist named John Hack discovered the most important law of river networks. In rivers and streams in Virginia and Maryland, Hack measured the length of each stream and the area of the land that slopes toward that stream and therefore drains into it, called its basin or drainage area. What he discovered is now known as Hack’s law: Any stream, from the littlest brook to the mightiest river, has a length that’s proportional to its drainage area raised to the power of 0.6. (In symbolic form: L ~ A^0.6.) There’s a bit of variance around that 0.6 value — Earth is, after all, a complicated place — but “the general regularity of the relation is nevertheless remarkable,” Hack wrote. “Stream lengths tend to increase proportionally to the 0.6 power of the drainage area, regardless of the geological or structural characteristics of the area.”

> **译文：** 1957年，美国地质调查局的科学家John Hack发现了河流网络最重要的定律。在弗吉尼亚州和马里兰州的河流与溪流中，Hack测量了每条水流的长度，以及向该水流倾斜并最终汇入其中的陆地面积，即其流域或排水面积。他的发现如今被称为Hack定律：任何一条水流，从最小的溪流到最宏伟的河流，其长度与其排水面积的0.6次方成正比。（用符号表示：L ~ A^0.6。）0.6这个值周围存在一些偏差——毕竟地球是一个复杂的地方——但“这种关系的普遍规律性仍然令人瞩目，”Hack写道。“水流长度往往随排水面积的0.6次方成比例增加，无论该地区的地质或结构特征如何。”

**When politicians turned against data centers** — For the Washington Post, Jeremy B. Merrill analyzed newsletters and social media posts from politicians to estimate messaging around data centers .

> **译文：** **当政客们转向反对数据中心**——在《华盛顿邮报》上，Jeremy B. Merrill分析了政客们的新闻通讯和社交媒体帖子，以估算围绕数据中心的言论动向。

**Amazon shutting down Mechanical Turk** — Described by Jeff Bezos as the “artificial artificial intelligence”, the crowdsourcing platform was a great way for visualization folks to gather data for specific tasks from real people . Kind of sad to see it shutdown, but so it goes on the internet.

> **译文：** **亚马逊关闭Mechanical Turk**——被Jeff Bezos称为“人工人工智能”的这个众包平台，曾是可视化从业者从真实人群那里收集特定任务数据的绝佳途径。看到它关闭有点遗憾，但互联网上就是这样。

**A third of new webpages written with AI** — It is trivial to generate bodies of text on infinite topics, so of course the web is filled with the stuff. Pew Research tried to estimate how much.

> **译文：** **三分之一的新网页由AI撰写**——生成无限主题的文本轻而易举，所以网络自然充斥着这类内容。Pew Research试图估算其规模。

To explore this question, we used the Common Crawl web archive to collect almost half a million English-language webpages from the past five years – starting a couple of years before the release of ChatGPT. We then ran the text of those pages through an AI detection tool called Open Pangram to see how many of them were likely written or substantially edited by AI.

> **译文：** 为了探究这个问题，我们使用Common Crawl网络档案，收集了过去五年中近50万个英语网页——时间起点比ChatGPT发布早几年。然后，我们通过一个名为Open Pangram的AI检测工具运行这些页面的文本，看看其中有多少可能由AI撰写或大幅编辑。

In a random sample, 9% of English language webpages were marked as having signs AI authorship. When looking at only pages that went live after the release of ChatGPT, they found a much a higher rate of 1 in 3.

> **译文：** 在随机样本中，9%的英语网页被标记为具有AI创作迹象。而仅看ChatGPT发布后上线的页面时，他们发现这一比例要高得多，达到三分之一。

Caveats considered, such as the accuracy and false positives with Open Pangram, the upward trends are clear. I am not sure how I feel about this, but I do not like that the em dash and Oxford comma are now a mark of AI usage.

> **译文：** 尽管存在诸如Open Pangram准确性和误报率等注意事项，但上升趋势是明确的。我不确定对此作何感想，但我不喜欢破折号和牛津逗号如今成了AI使用的标志。

## Visualization tools, datasets, and resources — August 2026 roundup

> **译文：** ## 可视化工具、数据集和资源——2026年8月汇总

Yesterday morning, FlowingData members received issue No. 403 of The Process. This week is a roundup of visualization tools, datasets, and resources from August. To succeed in the future, we must know how things work and how to make.

> **译文：** 昨天早上，FlowingData会员收到了第403期《The Process》。本周是8月份可视化工具、数据集和资源的汇总。要在未来取得成功，我们必须了解事物如何运作以及如何创造。

Become a FlowingData member to access this week’s issue and access the archive of 402 other guides and musings from visualization land.

> **译文：** 成为FlowingData会员，即可阅读本周内容，并访问可视化领域其他402篇指南和思考的存档。

–––

This was issue #3 of Weekly Flow.

You can subscribe or unsubscribe.

–––

Powered by Buttondown, the easiest way to start and grow your newsletter: https://buttondown.com

> **译文：** 由Buttondown提供支持，这是启动和发展你的新闻通讯最简单的方式：https://buttondown.com
