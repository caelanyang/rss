# Deep|Space: Orbital Data Centers - Lower Launch Costs Do Not Make GW-Scale Commercialization Viable

**来源：** FundaAI  
**日期：** 2026-06-23  
**查看原邮件：** <https://mail.google.com/mail/u/1/#search/subject%3A%22Deep%7CSpace%3A%20Orbital%20Data%20Centers%20-%20Lower%20Launch%20Costs%20Do%20Not%20Make%20GW-Scale%20Commercialization%20Viable%22>

---

View this post on the web at https://fundaai.substack.com/p/deepspace-orbital-data-centers-lower

> 在网页上查看此帖子：https://fundaai.substack.com/p/deepspace-orbital-data-centers-lower

Over the past six months, orbital data centers have moved from science-fiction framing into serious discussion among US equity investors. The reason is straightforward: terrestrial data centers are increasingly constrained by power interconnection, water, land permitting, noise, local opposition, and capex inflation, while Starship, reusable launch vehicles, and the LEO satellite supply chain have made large orbital infrastructure look less remote. The first layer of the bull case is valid. If launch cost and launch cadence continue to improve, many orbital infrastructure concepts that previously could not be financed will re-enter the investable discussion.
Why does the launch cost alone not price it
From an investment framework perspective, however, orbital data centers cannot be valued solely based on lower launch costs. The core of a data center is not where the servers sit; it is whether electricity can be converted into saleable compute at controllable cost while an almost equal amount of waste heat is reliably removed. Terrestrial data centers can scale to 100MW or GW class because the grid, water, air, land, maintenance workforce, and supply chain all exist outside the facility. In orbit, those external conditions become subsystems that the spacecraft itself must carry and manage. Starship lowers the transportation friction of reaching orbit. Still, it does not automatically solve continuous power, continuous heat rejection, closed-loop fluid circulation, in-orbit assembly, asset life, customer SLA, or depreciation recovery.
Based on our discussions with a launch and structural-systems expert, the long-term commercialization bottleneck for orbital data centers is not single-launch access to orbit. It is heat rejection, system life, replacement economics, and control over launch and platform infrastructure. A 1MW in-orbit thermal demo may not be physically out of reach, but as the system scales toward 100MW or GW-class, radiator area, pumped fluid loops, solar array area, in-orbit assembly, and micrometeoroid tolerance all scale up simultaneously. The broad concept of space compute should be split into three levels: whether a 1MW demo can operate, whether 10-100MW can become a repeatable deployment unit, and whether GW-class systems can become economically financeable infrastructure. The area most likely to be over-capitalized today is the distant GW vision; the area most in need of validation is the engineering chain between demo and repeatable deployment unit.
The ‘space is cold’ misconception
The first misconception in this chain is that space is cold, so cooling should be easier. That intuition is misleading for valuation. Terrestrial data-center cooling relies on air, water, gravity, and open external systems. Heat can be removed through cold plates, liquid cooling loops, cooling towers, evaporation, air convection, and external water systems. In orbit, the real change is not that the environment is colder; it is that there is no air. In a vacuum, there is no convection, traditional air cooling does not exist, and fluids cannot be consumed in an open loop because every gram of working fluid carries launch cost and resupply risk. The external heat-rejection mechanism that orbital systems can rely on over time is primarily radiation.
Based on our discussions with a thermal-management expert, the phrase “space is cold” is only half right. Deep space is cold, but in a vacuum, there is no air or other medium to carry heat away by convection. Compared with terrestrial conduction and convection, radiation is a much slower heat-transfer mechanism. The key variables in orbital thermal control are not a single ambient temperature, but operating temperature, radiator area, surface emissivity/absorptivity, and view factor. Large radiators not only see deep space; they are also affected by Earth’s infrared, albedo, solar exposure, and thermal radiation from nearby solar arrays. Electronics also cannot be run arbitrarily hot to improve radiative efficiency, because chips, packaging, board-level components, power modules, and long-term reliability all have temperature windows. This is the starting point for the engineering and valuation discussion: an orbital data center is not finished once the servers reach orbit; it must demonstrate that a closed-loop thermal management system can operate for years.
Radiator area: putting the problem in numbers

> 过去六个月，轨道数据中心已从科幻小说中的概念转变为美国股票投资者认真讨论的话题。原因很简单：地面数据中心日益受到电力互联、水资源、土地许可、噪音、当地反对和资本支出通胀等问题的制约，而星舰、可重复使用运载火箭和低地球轨道卫星供应链的出现，使得大型轨道基础设施不再遥不可及。看涨的第一层理由是成立的。如果发射成本和发射频率持续改善，许多以前无法融资的轨道基础设施项目将重新进入投资讨论的视野。

为什么单凭发射成本不足以评估其价值？

然而，从投资角度来看，轨道数据中心的价值不能仅仅基于较低的发射成本来衡量。数据中心的核心不在于服务器的放置位置，而在于能否以可控的成本将电力转化为可销售的计算能力，同时可靠地排出几乎等量的废热。地面数据中心可以扩展到 100MW 或 GW 级，因为电网、水、空气、土地、维护人员和供应链都位于设施外部。而在轨道上，这些外部条件变成了航天器自身必须携带和管理的子系统。星舰降低了进入轨道的运输阻力。然而，它并不能自动解决持续供电、持续散热、闭环流体循环、在轨组装、资产寿命、客户服务水平协议 (SLA) 或折旧回收等问题。

根据我们与一位发射和结构系统专家的讨论，轨道数据中心长期商业化的瓶颈并非单次发射即可进入轨道，而是散热、系统寿命、更换成本以及对发射和平台基础设施的控制。1MW 的在轨热演示或许并非遥不可及，但随着系统规模向 100MW 或 GW 级扩展，散热器面积、泵送流体循环、太阳能电池阵列面积、在轨组装以及微流星体耐受性等问题都将同步扩大。太空计算的总体概念应分为三个层面：1MW 的演示系统能否运行，10-100MW 能否成为可重复部署的单元，以及 GW 级系统能否成为经济上可行的基础设施。目前最有可能过度投资的是遥远的 GW 级愿景；最需要验证的是演示系统与可重复部署单元之间的工程链。

“太空寒冷”的误解

这条链中的第一个误解是太空寒冷，因此冷却应该更容易。这种直觉会误导估值。地面数据中心的冷却依赖于空气、水、重力和开放式外部系统。热量可以通过冷板、液冷回路、冷却塔、蒸发、空气对流和外部水系统排出。在轨道上，真正的变化不是环境更冷，而是没有空气。在真空中，不存在对流，传统的空气冷却方式也不可能存在，而且由于每一克工作流体都会增加发射成本和补给风险，因此不能在开式循环系统中消耗流体。轨道系统能够长期依赖的外部散热机制主要是辐射。

根据我们与一位热管理专家的讨论，“太空很冷”这种说法只对了一半。深空确实很冷，但在真空中，没有空气或其他介质可以通过对流带走热量。与地球上的传导和对流相比，辐射是一种慢得多的传热机制。轨道热控制的关键变量并非单一的环境温度，而是工作温度、散热器面积、表面发射率/吸收率以及视角因子。大型散热器不仅会受到深空的影响，还会受到地球红外线、反照率、太阳辐射以及附近太阳能电池阵列的热辐射的影响。电子元件也不能为了提高散热效率而随意提高工作温度，因为芯片、封装、板级元件、电源模块以及长期可靠性都存在温度范围。这正是工程和评估讨论的出发点：轨道数据中心并非在服务器进入轨道后就完成了；它必须证明闭环热管理系统能够持续运行数年。

散热器面积：用数字量化问题

Unsubscribe https://substack.com/redirect/2/eyJlIjoiaHR0cHM6Ly9mdW5kYWFpLnN1YnN0YWNrLmNvbS9hY3Rpb24vZGlzYWJsZV9lbWFpbD90b2tlbj1leUoxYzJWeVgybGtJam96T0RZNU9UY3lOaXdpY0c5emRGOXBaQ0k2TWpBek1EVTRPVFEwTENKcFlYUWlPakUzT0RJeE1qYzBOVElzSW1WNGNDSTZNVGd4TXpZMk16UTFNaXdpYVhOeklqb2ljSFZpTFRNeU9ERXdNVEVpTENKemRXSWlPaUprYVhOaFlteGxYMlZ0WVdsc0luMC56UU5SaTZWdV9XNDA1b1V3OTBOMUk1czZrUUZVOVdVcllycmRmNER0LWI4IiwicCI6MjAzMDU4OTQ0LCJzIjozMjgxMDExLCJmIjp0cnVlLCJ1IjozODY5OTcyNiwiaWF0IjoxNzgyMTI3NDUyLCJleHAiOjIwOTc3MDM0NTIsImlzcyI6InB1Yi0wIiwic3ViIjoibGluay1yZWRpcmVjdCJ9.ltbnghDkSgsHZ44SZQFB9gKpF4CnzE3NFXwL3RkJvKA?

> 取消订阅 https://substack.com/redirect/2/eyJlIjoiaHR0cHM6Ly9mdW5kYWFpLnN1YnN0YWNrLmNvbS9hY3Rpb24vZGlzYWJsZV9lbWFpbD90b2tlbj1leUoxYzJWeVgybGtJam96T0RZNU9UY3lOaXdpY0c5emRGOXBaQ0k2TWpBek1EVTRPVFEwTENKcFlYUWlPakUzT0RJeE1qYzBOVElzSW1WNGNDSTZNVGd4TXpZMk16UTFNaXdpYVhOeklqb2ljSFZpTFRNeU9ERXdNVEVpTENKemRXSWlP aUprYVhOaFlteGxYMlZ0WVdsc0luMC56UU5SaTZWdV9XNDA1b1V3OTBOMUk1czZrUUZVOVdVcllycmRmNER0LWI4IiwicCI6MjAzMDU4OTQ0LCJzIjozMjgxMDExLCJmIjp0cnVlLCJ1IjozODY5OTcyNiwiaWF0IjoxNzgyMTI3NDUyLCJleHAiOjIwOTc3MDM0NTIsImlzcyI6InB1Yi0wIiwic3ViIjoibGluay1yZWRpcmVjdCJ9.ltbnghDkSgsHZ44SZQFB9gKpF4CnzE3NFXwL3RkJvKA?