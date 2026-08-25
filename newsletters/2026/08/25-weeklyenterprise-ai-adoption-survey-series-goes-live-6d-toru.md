# Weekly|Enterprise AI Adoption Survey Series Goes Live, 6D Torus Points to 4x Optical Content per TPU, OCP APAC Tak…



**来源：** FUNDA  

**日期：** 2026-08-25  

**查看原邮件：** <https://mail.google.com/mail/u/1/#search/subject%3A%22Weekly%7CEnterprise%20AI%20Adoption%20Survey%20Series%20Goes%20Live%2C%206D%20Torus%20Points%20to%204x%20Optical%20Content%20per%20TPU%2C%20OCP%20APAC%20Tak%E2%80%A6%22>



---



The question we get asked more than any other right now is whether enterprise AI adoption can take the baton from coding. Coding agents did the heavy lifting at the start of the year, Tokenmaxxing carried the debate through May and June, and the recent open-source releases have made everyone re-underwrite the cost side. We believe a repeatable read is essential on what enterprises are actually spending, what they're spending it on, and whether the line is still going up. So we built one. This week we launched a standing enterprise AI adoption survey, running 10-20 expert interviews a week, publishing an updated cut every week rather than a one-off snapshot that goes stale in a month. Volume 1 this week covered thirteen calls.

> **译文：** 目前我们被问到最多的问题是：企业采用人工智能能否取代编码工作？年初，编码代理承担了大部分工作；五六月份，Tokenmaxxing 引发了热议；而最近开源软件的发布，又让所有人重新审视了成本问题。我们认为，要了解企业实际支出多少、支出用途以及成本是否仍在上涨，必须进行可重复的评估。因此，我们构建了这样一个评估体系。本周，我们启动了一项持续进行的企业人工智能采用情况调查，每周进行 10-20 次专家访谈，并每周发布更新版本，而不是像以往那样发布一个月后就过时的单次快照。本周发布的第一卷包含了 13 次访谈的内容。

The headline from those thirteen: spend is still growing, and the interesting part is where the increment lands and where the trajectories start to split. Seats are close to saturated at the companies already committed, so the growth is moving into API calls and production workflows. One large global bank has gone from roughly $150-160mn a year to $200-300mn.

> **译文：** 这十三份报告中最引人注目的是：支出仍在增长，而有趣的是，增长的重点在于哪些方面有所体现，以及增长轨迹从何处开始出现分歧。已签约公司的席位几乎饱和，因此增长正在转向 API 调用和生产工作流程。一家大型全球银行的年支出已从大约 1.5 亿至 1.6 亿美元增长到 2 亿至 3 亿美元。

A large European telecom operator is running $30-50k a month, up from $15k at the start of the year, and expects just under $100k within six months. A mid-to-large biopharma has moved from roughly 80/20 subscription-to-API at the start of the year to 70/30. Against that, a large European automaker is up only 10-15% year to date, guides to broadly flat in 2027, and a large global pharma expects to approach a plateau over the next 12-18 months.

> **译文：** 一家大型欧洲电信运营商的月收入已从年初的1.5万美元增至3万至5万美元，并预计六个月内将接近10万美元。一家中大型生物制药公司已将其API订阅比例从年初的约80/20调整为70/30。相比之下，一家大型欧洲汽车制造商今年迄今为止的收入仅增长了10%至15%，预计2027年将基本持平，而一家大型全球制药公司预计未来12至18个月内将趋于稳定。

Our read is that the seat line is maturing on schedule and the API line is the one that compounds, which makes production workflow deployment the focus, not headcount. This number decides whether model vendor ARR reaccelerates.

> **译文：** 我们认为，座位产品线正按计划走向成熟，而API产品线才是增长最快的部分，因此生产工作流程部署才是重点，而非人员规模。这一数字将决定模型供应商的年度经常性收入（ARR）能否再次加速增长。

The other thread this week was optics, and it keeps getting better. Supply-chain chatter has Google taking the training-side TPU 9t from a 3D torus to a 6D torus for 2027-2028 deployment, which sounds incremental but isn't: wrap-around optical ports per chip go from 1.5 to 6, because at edge length 2 every chip becomes a boundary node. That is a 4x lift in OCS ports and optical module content per TPU before the 800G-to-2.4 T Coherent Lite upgrade is layered on top. Our OCP APAC takeaways point the same way from the other end of the stack, with copper running out of road at 400 Gbps per lane and the whole power path being redesigned from grid to chip. Next week is NVDA, where the only question that matters is whether management puts more shape on the cumulative $1T Blackwell/Rubin revenue path.

> **译文：** 本周的另一个话题是光通信，而且情况越来越好。供应链方面的消息称，谷歌计划在2027-2028年部署时，将训练端的TPU 9t从3D环面升级到6D环面。这听起来像是小幅升级，但实际上并非如此：每个芯片的环绕式光端口数量将从1.5个增加到6个，因为在边缘长度为2时，每个芯片都成为了一个边界节点。这意味着在800G到2.4T相干Lite升级之前，每个TPU的OCS端口和光模块数量就增加了4倍。我们从OCP亚太地区得出的结论也指向了同样的方向，即铜缆在每通道400Gbps的传输速度下已经接近极限，整个供电路径（从电网到芯片）都在重新设计。下周是英伟达（NVDA）的会议，唯一重要的问题是管理层是否会进一步明确Blackwell/Rubin累计1万亿美元的营收目标。

This Week’s Reports

Optics — a 6D torus would quadruple optical content per TPU, and the derivation is simple enough to check. Wrap-around optical ports per chip rise from 1.5 to 6 because edge length falls from four to two and every chip becomes a boundary node, which fills in the 2:1 to 10:1 scale-up range Lumentum showed at OFC without spelling out the architecture behind it.

> **译文：** 光学方面——一个6D环面可以将每个TPU的光容量提升四倍，其推导过程也很简单，易于验证。每个芯片的环绕式光端口数量从1.5个增加到6个，因为边缘长度从4个减少到2个，并且每个芯片都成为一个边界节点，这满足了Lumentum在OFC上展示的2:1到10:1的扩展范围，尽管他们并未详细说明其背后的架构。

OCP APAC — copper keeps losing ground on reach, and the power path is being redesigned end to end. Nvidia and Broadcom both claim CPO in production, while ASE says the ecosystem isn't ready; on the power side, the industry is converging on 800VDC with solid-state transformers as the endgame, and vertical power delivery is reshaping MLCC, SPS, and inductor demand.

> **译文：** OCP亚太地区——铜箔在传输距离方面持续落后，供电路径正在进行端到端的重新设计。英伟达和博通都声称其铜箔已投入量产，而日月光则表示生态系统尚未准备就绪；在电源方面，业界正朝着800VDC的目标迈进，固态变压器将成为最终解决方案，而垂直供电正在重塑MLCC、SPS和电感器的需求。

Premium Report Snapshot

Below is a snapshot of what Premium subscribers received this week beyond the Substack feed.

> **译文：** 以下是本周高级订阅用户在 Substack 信息流之外收到的内容概览。
