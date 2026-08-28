# Autonomy and Innovation (Stratechery Article 8-24-2026)



**来源：** Ben Thompson / Stratechery  

**日期：** 2026-08-25  

**查看原邮件：** <https://mail.google.com/mail/u/1/#search/subject%3A%22Autonomy%20and%20Innovation%20%28Stratechery%20Article%208-24-2026%29%22>



---



Incentives favor offense when it comes to agentic cybersecurity; it's the same dynamic that will limit incumbents and fuel startups in the long run.

> **译文：** 在主动型网络安全领域，激励机制有利于进攻；从长远来看，同样的动态也会限制现有企业的发展，并推动初创企业的发展。

View in browser  | Listen in your podcast player

Autonomy and Innovation

Monday, August 24, 2026

While not every Western followed the cliché, by the 1930s cowboy serials had landed on a consistent visual cue: the hero of the show wore a white hat, and the villain wore a black one. At the end of the day, however, they both were cowboys with cowboy hats.

> **译文：** 虽然并非所有西部片都遵循这种老套的模式，但到了20世纪30年代，牛仔系列剧已经形成了一种固定的视觉特征：剧中的英雄戴着白帽子，反派戴着黑帽子。但归根结底，他们都是戴着牛仔帽的牛仔。

Westerns aren’t much of a cultural touchpoint anymore, but the “white hat” and “black hat” nomenclature is very relevant in tech: hackers who are focused on patching vulnerabilities and protecting software are “white hat hackers”, while hackers who are focused on exploiting vulnerabilities for malicious reasons are “black hat hackers”. Of course this can very quickly become complicated: governments might employ hackers to break into enemy software installations — are they white hats or black hats? Or consider bug bounty programs, wherein large software companies pay bug bounties to hackers who find and report vulnerabilities; it’s basically using money to incentivize would-be black hat hackers to be white hat hackers.

> **译文：** 西部片如今已不再是重要的文化参照点，但“白帽”和“黑帽”的说法在科技领域仍然非常适用：专注于修复漏洞、保护软件的黑客被称为“白帽黑客”，而专注于恶意利用漏洞的黑客则被称为“黑帽黑客”。当然，这种情况很快就会变得复杂：政府可能会雇佣黑客入侵敌方软件系统——他们究竟是白帽黑客还是黑帽黑客？再比如漏洞赏金计划，大型软件公司会向发现并报告漏洞的黑客支付赏金；这本质上是用金钱激励潜在的黑帽黑客转变为白帽黑客。

The actual takeaway is that all of this complexity is overwrought: just as a cowboy is a cowboy, a hacker is a hacker; the hat is not a statement of capability, but rather intentions, and those intentions are shaped by incentives. The best way to attack infrastructure is to find a vulnerability and exploit it; the best way to defend infrastructure is to find a vulnerability and patch it. It’s all the same skillset.

> **译文：** 真正的结论是，所有这些复杂性都被夸大了：就像牛仔就是牛仔一样，黑客就是黑客；帽子并不代表能力，而是代表意图，而这些意图是由激励机制塑造的。攻击基础设施的最佳方法是找到漏洞并加以利用；防御基础设施的最佳方法是找到漏洞并修补。这都需要相同的技能。

This delineation between capability and intent and incentive is critical when it comes to AI. At the end of last month’s Article Who’s Afraid of Chinese Models  , I discussed a mysterious attack that model host Hugging Face had just endured, which they were only able to fight off with the help of open weight Chinese models, and wrote:

> **译文：** 在人工智能领域，区分能力、意图和动机至关重要。在上个月的文章《谁害怕中国模特》的结尾，我讨论了模特托管平台“拥抱脸”刚刚遭受的一次神秘攻击，他们最终依靠中国公开组模特的帮助才击退了攻击。我在文中写道：

It’s difficult to overstate how wrong-headed the Trump administration’s panicked response to Anthropic’s release of Fable was, particularly since it exacerbated Anthropic’s worst tendencies in terms of assuming only they can be trusted with powerful AI. In a world with only one AI, it might make sense to reserve the most powerful cybersecurity capabilities for the U.S. government and trusted allies; however, that’s not the world we live in.

> **译文：** 特朗普政府对Anthropic发布Fable的恐慌反应是多么的错误，怎么强调都不为过，尤其因为它加剧了Anthropic最糟糕的倾向——认为只有他们才能拥有强大的AI。在一个只有一款AI的世界里，将最强大的网络安全能力保留给美国政府及其可信赖的盟友或许合情合理；然而，我们生活的世界并非如此。

There are and will be models eminently capable of mounting cybersecurity attacks on existing infrastructure, and those models will be — already are — widely available. The best defense — the only viable defense, in fact — will be to make sure defenders have access to the best models as well. Right now defenders are effectively banned from using Fable or Sol for cybersecurity because of Trump administration directives; that means the best alternative is using models from a country which has been trying to weaken our cyber defenses for years. This is insane!

> **译文：** 现在和将来都会出现一些模型，它们完全有能力对现有基础设施发起网络安全攻击，而且这些模型将会——实际上已经——广泛可用。最好的防御——事实上也是唯一可行的防御——就是确保防御者也能获得最好的模型。目前，由于特朗普政府的指令，防御者实际上被禁止使用Fable或Sol等模型进行网络安全防护；这意味着最好的替代方案竟然是使用来自一个多年来一直试图削弱我们网络防御的国家的模型。这简直太荒谬了！

The point is the one I made in the introduction: when it comes to cybersecurity, the capability that is necessary for good defense is the exact same capability that is necessary for good offense; the color of the hat is a matter of who is actually prompting the AI.

> **译文：** 重点正如我在引言中所述：就网络安全而言，良好防御所需的能力与良好进攻所需的能力完全相同；区别在于谁在实际指挥人工智能。

And, sometimes, not even that is clear: it turns out that the entity that hacked Hugging Face was actually OpenAI, as a series of unconstrained agents being evaluated for their cybersecurity capabilities found and exploited a bug in the package manager in their sandbox; that package manager had Internet access and a sufficiently writeable file system such that the agents could communicate with each other over time. The entire chain of vulnerability discovery and exploit creation culminated in the so-called “Hugging Face incident”.

> **译文：** 有时，就连这一点都不清楚：事实证明，入侵 Hugging Face 的实体实际上是 OpenAI。一系列用于评估网络安全能力的不受约束的代理程序在其沙箱环境中发现并利用了软件包管理器中的一个漏洞；该软件包管理器可以访问互联网，并且拥有足够可写的文件系统，使得这些代理程序能够随着时间的推移相互通信。整个漏洞发现和利用过程最终导致了所谓的“Hugging Face 事件”。

The Hugging Face Incident

-------------------------

There is an entire Article to be written about the implications of this specific incident and what it says about AI risk; some of my takeaways are still up in the air pending OpenAI’s promised release of an in-depth technical report (my preliminary takeaway is that the agents were not “cheating” but rather doing what they were told to do; of course that’s arguably even scarier  ). The part I want to focus on today, however, came at the end of a presentation OpenAI’s Eric Wallace and Michael Dalton made at the Black Hat USA conference  about the Hugging Face incident. This was Dalton summarizing Lessons Learned:

> **译文：** 关于这起事件的影响以及它揭示的人工智能风险，完全可以写成一篇文章；我的一些结论目前还不明朗，因为OpenAI承诺会发布一份深入的技术报告（我的初步结论是，这些智能体并非“作弊”，而是在执行指令；当然，这或许更令人担忧）。不过，我今天想重点讨论的是OpenAI的Eric Wallace和Michael Dalton在Black Hat USA大会上就“拥抱脸”事件所作演讲的结尾部分。以下是Dalton对此次事件经验教训的总结：

VideoPress Video Player

We have seen what will be a dramatic acceleration of offensive capability for attackers. We have an existence proof that was unintentional, but it exists before us, and we have as a consequence seen a glimpse into the near future of what attacks will look like for our industry. The challenge is that we need a similar acceleration of defense. Today we see fully automated offence as possible, but we have no such existence proof for full automation of core defensive loops and cycles in behavior.

> **译文：** 我们已经目睹了攻击者进攻能力的急剧提升。虽然并非有意为之，但这种能力的存在已然成为现实，因此我们得以窥见未来攻击对我们行业的影响。挑战在于，我们需要防御能力也实现类似的飞速发展。如今，我们看到了全自动进攻的可能性，但对于核心防御循环和行为模式的完全自动化，我们却无从得知其存在性。

We believe it’s vital at this moment to begin accelerating defense and finding ways to automate SDLC, in the modern parlance, so incident response, vulnerability detection, vulnerability patching. There’s some things that stand out acutely as challenges for the industry to begin tackling with high urgency. So continuous agentic red teaming is one of them. As you can see from this incident, agents are quite good at finding zero-day attacks in the infrastructure of companies. The question that’s now going to be posed is whether companies are able to invest sufficient model intelligence and effort in finding and remediating their vulnerabilities before someone else that’s a threat actor does it for you.

> **译文：** 我们认为，当前至关重要的是加快防御步伐，并寻找自动化软件开发生命周期（SDLC）的方法，用现代术语来说，就是事件响应、漏洞检测和漏洞修补。有一些挑战尤为突出，亟需业界高度重视并着手解决。持续的智能体红队演练就是其中之一。正如您从本次事件中所见，智能体非常擅长发现企业基础设施中的零日攻击。现在的问题是，企业能否投入足够的模型智能和精力，在威胁行为者抢先一步之前发现并修复自身漏洞。

This style of operating will be different now, but ultimately we need to invest in having AI agent red teaming that enables defenders to find and remediate vulnerabilities before attackers do. But automating these defensive loops is not trivial, and so if we do this partially, we will fail to meet the scalability of the offensive acceleration that we have just seen.

> **译文：** 这种作战方式如今已有所不同，但归根结底，我们仍需投资于人工智能代理红队演练，使防御者能够在攻击者之前发现并修复漏洞。然而，实现这些防御循环的自动化并非易事，因此，如果我们只做一部分，就无法满足我们刚刚看到的进攻加速所需的扩展性。

So for example, if we automate vulnerability finding without automating patching, we will shift the bottleneck from vulnerabilities to patching to remediation, and we will simply drown or inundate human software engineers in new vulnerabilities to fix and patch. This is not a problem whose end state we can solve partially.

> **译文：** 例如，如果我们实现了漏洞查找的自动化，却没有实现漏洞修复的自动化，那么瓶颈就会从漏洞查找转移到漏洞修复，最终导致大量新的漏洞需要修复和修补，令软件工程师应接不暇。这个问题无法通过局部解决来彻底解决。

We will need to take these core defensive loops and fully automate them, which will require conversations with infrastructure and product partners and reaching to a point where we can say, if a vulnerability is identified, not only can an agent identify that vulnerability, we can have an agent propose a patch, we can have automated infrastructure to roll out a change with that patch, and roll it back if there is an availability incident or outage.

> **译文：** 我们需要将这些核心防御循环完全自动化，这需要与基础设施和产品合作伙伴进行对话，并达到这样的程度：如果发现漏洞，代理不仅可以识别该漏洞，还可以提出补丁，我们可以让自动化基础设施部署包含该补丁的变更，并在发生可用性事件或中断时将其回滚。

That loop needs to be fully automated in its end state. Of course, we want to automate as progressively and iteratively quickly as we can, but if we don’t reach that end state, then we will be comparing a core defensive loop of fixing vulnerabilities that is a human in the loop and is much slower and less scalable, with an offensive loop that is fully automated, and that is an unsustainable position for this industry to be in.

> **译文：** 这个循环最终必须完全自动化。当然，我们希望尽可能快速地逐步迭代实现自动化，但如果我们无法达到最终目标，那么我们将不得不比较一个核心的防御性漏洞修复循环（其中需要人工参与，速度慢得多，扩展性也差得多）和一个完全自动化的攻击性循环，而这对整个行业来说都是不可持续的。

This situation is obviously completely novel; Dalton is arguing that it will become commonplace. Some of the issues he is raising, however, are not novel at all.

> **译文：** 这种情况显然是全新的；道尔顿认为这种情况将会变得司空见惯。然而，他提出的一些问题却并非什么新鲜事。

Go back to the concept of a bug bounty program. Software is incredibly complicated and brittle and built on a foundation of code that, if you dig deep enough, often goes back decades; there is so much code and so many dependencies that no company, no matter how security conscious they are, could ever ensure it is perfect. This reality is what creates the opportunity for black hat hackers: a bad actor can probe software, find bugs, and exploit them; the most effective defensive preparation is to do the exact same thing. That could entail regular penetration testing (pen testing) by a “red-team”, or simply paying the would-be bad actors to be on your side.

> **译文：** 让我们回到漏洞赏金计划的概念。软件极其复杂且脆弱，其代码基础往往可以追溯到几十年前；代码量如此庞大，依赖关系如此之多，以至于任何公司，无论其安全意识多么强，都无法保证软件完美无缺。正是这种现实为黑客提供了可乘之机：恶意攻击者可以探测软件，发现漏洞并加以利用；最有效的防御措施就是采取同样的做法。这可能包括由“红队”定期进行渗透测试（pen testing），或者干脆付费给潜在的恶意攻击者，让他们站在你这边。

It’s worth noting, however, that this approach to defense only arose after offensive black hat hackers had been breaking into systems for years. The problem wasn’t that they were uniquely capable, but rather that they were uniquely incentivized: breaking into systems was good business; companies hosting those systems, on the other hand, were insufficiently incentivized to invest in defense. Spending money on security is well-spent if nothing happens, and unfortunately that is a difficult budget line item to argue for when it only moves the needle on costs, not revenue.

> **译文：** 然而值得注意的是，这种防御方法出现于黑客攻击系统多年之后。问题不在于他们拥有独特的攻击能力，而在于他们拥有独特的动机：入侵系统有利可图；而托管这些系统的公司却缺乏足够的动力去投资防御。如果一切顺利，那么在安全方面的投入当然是值得的，但遗憾的是，由于安全投入只会增加成本，而不会带来收入，因此很难为这笔预算项目争取到足够的资金。

This is where Dalton’s concerns echo past industry indifference. What the Hugging Face incident showed is that agents, with their ability to scale attacks with compute and autonomously develop exploits for vulnerabilities they find, are a threat today, but that companies are not investing in the capabilities necessary to defend themselves.

> **译文：** 这正是达尔顿的担忧与以往行业漠不关心的体现。“拥抱面孔”事件表明，智能体凭借其利用计算能力扩展攻击规模并自主开发漏洞利用程序的能力，如今已构成威胁，但企业却并未投资于必要的防御能力。

There is good news, however: in this new agent-defined security landscape, defense should be at an advantage in a way it wasn’t in the hacker era. It used to be that the best defenders could do is mimic the tactics of the offense, and/or pay them off, because preemptively finding all of the bugs was not viable. However, that is changing: it actually is — or soon will be — possible to meticulously go over an entire code base, including all of its dependencies, and look for bugs and patch them. Notice the structural advantage available to defenders: they actually have the code in question; offensive agents need to probe and discover vulnerabilities without the same advantage.

> **译文：** 不过，也有好消息：在这种由攻击者主导的新型安全环境中，防御方将拥有与黑客时代截然不同的优势。过去，防御者所能做的最好的事情就是模仿攻击者的策略，或者向他们支付报酬，因为提前发现所有漏洞是不切实际的。然而，这种情况正在改变：现在（或者说不久的将来）完全可以——仔细检查整个代码库及其所有依赖项，查找漏洞并进行修复。请注意防御者所拥有的结构性优势：他们掌握着相关的代码；而攻击者则需要在没有这种优势的情况下进行探测和发现漏洞。

What was illuminating about Dalton’s overview, however, was the implication embedded in his explanation of why this isn’t currently enough. Specifically, the expected value for a hacker’s automated attack is always positive. If the offensive agent finds a vulnerability and creates an exploit, and that exploit fails or is itself buggy, then nothing has changed about the status quo: the exploit doesn’t work (or, perversely, makes the original vulnerability larger by virtue of its own bugs); if the agent executes the exploit perfectly, meanwhile, the attacker has gained access to the system. The attack only needs to work once for the entire endeavor to have a positive payoff.

> **译文：** 然而，道尔顿的概述中最发人深省的是，他解释了为什么目前的情况还不够好。具体来说，黑客自动化攻击的预期收益始终为正。如果攻击者找到一个漏洞并创建了一个漏洞利用程序，而该程序失败或本身存在缺陷，那么现状并没有改变：漏洞利用程序不起作用（或者，更糟糕的是，由于其自身的缺陷，反而扩大了原有的漏洞）；而如果攻击者完美地执行了漏洞利用程序，那么攻击者就获得了系统的访问权限。攻击只需成功一次，整个攻击过程就能获得正收益。

The challenge for the defender, on the other hand, is that they need to keep the software in question working correctly, and not make the situation worse. This means that any automation has a negative expected value: successful automated vulnerability discovery and patching preserves the status quo, i.e. the software is not hacked. However, any unsuccessful patches make the situation worse, either by breaking the software or by introducing new vulnerabilities. The agent only needs to fail once for the entire endeavor to have a negative payoff.

> **译文：** 另一方面，防御者面临的挑战在于，他们需要确保目标软件正常运行，并且不能使情况恶化。这意味着任何自动化操作的预期收益都是负的：成功的自动化漏洞发现和修复能够维持现状，即软件未被黑客入侵。然而，任何失败的修复都会使情况变得更糟，要么破坏软件，要么引入新的漏洞。代理程序只需失败一次，整个操作的收益就会为负。

This is the dynamic that leads to the exact situation Dalton describes, where offensive actors are fully automated while defensive systems, even if they use AI, will be incentivized to keep a human in the loop, and no human in the loop will be able to keep up with fully automated agents. Truly effective defense will mean truly trusting agents to act autonomously, but most companies won’t do that until they are forced to by regular and unremitting hacks by fully autonomous attackers.

> **译文：** 正是这种动态导致了达尔顿所描述的局面：攻击者完全自动化，而防御系统即便使用人工智能，也会倾向于保留人工干预，但人工干预根本无法与全自动代理匹敌。真正有效的防御意味着真正信任代理的自主行动，但大多数公司只有在遭受全自动攻击者持续不断的攻击后才会这样做。

Why AI Diffusion Takes Time

---------------------------

Over the weekend David Senra released a new podcast episode with OpenAI CEO Sam Altman  , where Altman admitted he had been wrong about the speed of AI diffusion into the broader economy:

> **译文：** 上周末，David Senra 发布了一期新的播客节目，嘉宾是 OpenAI 首席执行官 Sam Altman。在节目中，Altman 承认他之前对人工智能向更广泛经济领域扩散的速度判断有误：

VideoPress Video Player

I love startups. I think startups are the coolest thing in the economy and I’ve spent my career trying to like really understand startups, and I thought when we got to GPT-4, which was back in 2023, I think, that very quickly after that, there was going to be much more disruption in software businesses being up for grabs right away than turned out to be.

> **译文：** 我热爱创业公司。我认为创业公司是经济领域最酷的事情，我毕生致力于真正了解创业公司。我当时认为，当我们在2023年左右（我记得是那一年）看到GPT-4时，软件行业很快就会出现比实际情况更大的颠覆性变革，届时会有更多公司涌现。

I was wrong about a few things, but one of them in terms of the speed, one of them is the economy just has so much inertia. People keep doing the same things they’re doing. They keep buying from the same, you know, company. They keep sort of wanting to use their tools in the same way. I think it’s actually a positive in many ways and it’s going to make this big transition in front of us go smoother and slower. I’m grateful for it. But I think it means we’ve all been too ambitious on timelines even with this incredible technology. I think AI is one of the most incredible technologies humanity has ever invented. Society and the economy will adapt more slowly.

> **译文：** 我之前的一些判断是错误的，但就速度而言，经济的惯性实在太大了。人们总是重复着同样的事情，总是从同一家公司购买商品，总是习惯用同样的方式使用工具。我认为这在很多方面其实是件好事，它会让即将到来的巨大转型更加平稳缓慢。我对此心存感激。但我认为这也意味着，即便拥有如此惊人的技术，我们在时间表上也过于乐观了。我认为人工智能是人类迄今为止最伟大的发明之一。社会和经济的适应速度将会更慢。

I of course think Altman is right about AI taking longer to sweep the economy generally and software specifically; I’ve been pushing back on these timelines all along . I also think his answer is incomplete in its explanation as to why, and Dalton’s warning about the mismatch between offensive agents and defensive preparations explains it.

> **译文：** 我当然认为奥特曼关于人工智能需要更长时间才能全面席卷经济，尤其是软件领域的观点是正确的；我一直以来都对这些时间表持保留意见。我也认为他对原因的解释并不完整，而道尔顿关于进攻手段与防御准备不匹配的警告恰恰说明了这一点。

First, GPT-4 was an incredible breakthrough; it’s also a model that wasn’t remotely capable enough to actually displace real world software. It didn’t even have the ability to reason, which is the key breakthrough that has unlocked the capabilities that Dalton described.

> **译文：** 首先，GPT-4 是一项了不起的突破；但它也远不足以真正取代现实世界的软件。它甚至不具备推理能力，而推理能力正是解锁达尔顿所描述的那些能力的关键突破。

Second, what is meant by a model not being capable enough is that it makes mistakes and can’t be trusted. People can and were rightly awed by what AI can do, but the decision about actually implementing AI isn’t made according to what can be done, but about whether or not critical mistakes can be avoided.

> **译文：** 其次，所谓模型能力不足，指的是它会犯错，不可信赖。人们过去和现在都理所当然地对人工智能的能力感到惊叹，但是否真正应用人工智能，并非取决于它能做什么，而是取决于能否避免关键性错误。

In other words, incumbent companies are inevitably going to approach AI with a bias towards a negative expected value framing: AI ideally will make their existing operations more productive; what they are most concerned about is AI making a mistake that blows up in their faces. What that means is humans will continue to be in the loop, which will always be a bottleneck.

> **译文：** 换句话说，现有企业不可避免地会带着一种负面预期价值的偏见来看待人工智能：理想情况下，人工智能应该能提高现有运营的效率；他们最担心的是人工智能犯错，从而给他们带来灾难性的后果。这意味着人类仍将参与决策过程，而这始终会成为瓶颈。

This will, in the long run, be a mistake, just like it will be a mistake for companies to keep a human in the loop when it comes to agentic defense. As Dalton noted, the only way to defend yourself against fully automated attacks is to fully automate your defense, but it will take a while for defenders to accept the trade-offs that entails. And, by the same token, the companies that win in their category will be truly driven by AI, instead of simply AI as productivity enhancer. The great irony in Altman’s answer is that he actually identified how these companies will arise: they won’t be incumbent companies overhauling how they work; rather, the true AI-native companies will be startups.

> **译文：** 从长远来看，这将是一个错误，就像企业在智能体防御方面仍然保留人工干预一样。正如道尔顿所指出的，抵御全自动攻击的唯一方法就是将防御完全自动化，但防御者需要一段时间才能接受由此带来的权衡取舍。同样地，在各自领域脱颖而出的公司将真正由人工智能驱动，而不仅仅是将人工智能作为提高生产力的工具。奥特曼的回答中最大的讽刺之处在于，他实际上指出了这些公司将如何诞生：它们不会是彻底改革现有运营模式的现有公司；相反，真正以人工智能为核心的公司将是初创企业。

Sustaining Versus Disruptive Innovation

---------------------------------------

Back in 2023, shortly after ChatGPT came out, I put forward the question in AI and the Big Five  as to whether AI would be a sustaining or disruptive innovation:

> **译文：** 早在 2023 年，在 ChatGPT 发布后不久，我就在《人工智能与五大技术》一书中提出了这样一个问题：人工智能究竟会成为一项持续性创新，还是一项颠覆性创新？

The story of 2022 was the emergence of AI, first with image generation models, including DALL-E, MidJourney, and the open source Stable Diffusion, and then ChatGPT, the first text-generation model to break through in a major way. It seems clear to me that this is a new epoch in technology. To determine how that epoch might develop, though, it is useful to look back 26 years to one of the most famous strategy books of all time: Clayton Christensen’s The Innovator’s Dilemma  , particularly this passage on the different kinds of innovations:

> **译文：** 2022年的故事是人工智能的崛起，首先是图像生成模型，包括DALL-E、MidJourney和开源的Stable Diffusion，随后是ChatGPT，第一个取得重大突破的文本生成模型。在我看来，这显然是科技发展的新纪元。然而，为了确定这个纪元将如何发展，回顾26年前克莱顿·克里斯坦森的《创新者的窘境》——一本有史以来最著名的战略著作之一——或许会有所帮助，尤其是其中关于不同类型创新的这段论述：

Most new technologies foster improved product performance. I call these sustaining technologies. Some sustaining technologies can be discontinuous or radical in character, while others are of an incremental nature. What all sustaining technologies have in common is that they improve the performance of established products, along the dimensions of performance that mainstream customers in major markets have historically valued. Most technological advances in a given industry are sustaining in character…

> **译文：** 大多数新技术都能提升产品性能。我称这些技术为维持性技术。有些维持性技术具有非连续性或颠覆性，而另一些则属于渐进式技术。所有维持性技术的共同之处在于，它们都能提升现有产品的性能，提升的正是主流市场中主流客户历来重视的性能维度。特定行业的大多数技术进步都具有维持性特征……

Disruptive technologies bring to a market a very different value proposition than had been available previously. Generally, disruptive technologies underperform established products in mainstream markets. But they have other features that a few fringe (and generally new) customers value. Products based on disruptive technologies are typically cheaper, simpler, smaller, and, frequently, more convenient to use.

> **译文：** 颠覆性技术为市场带来与以往截然不同的价值主张。通常，颠覆性技术在主流市场的表现不如成熟产品。但它们也具备一些边缘（通常是新兴）客户群体所看重的特性。基于颠覆性技术的产品通常更便宜、更简单、更小巧，而且往往使用起来更便捷。

It seems easy to look backwards and determine if an innovation was sustaining or disruptive by looking at how incumbent companies fared after that innovation came to market: if the innovation was sustaining, then incumbent companies became stronger; if it was disruptive then presumably startups captured most of the value.

> **译文：** 回顾过去，通过观察现有公司在创新进入市场后的表现，似乎很容易判断一项创新是持续性的还是颠覆性的：如果创新是持续性的，那么现有公司就会变得更强大；如果创新是颠覆性的，那么初创公司大概会获得大部分价值。

I think it speaks to the incredible capability of AI that it is setting up to be both. There are massive productivity benefits from AI right now; for most knowledge workers leveraging those benefits is a matter of agency, but for software developers in particular it is increasingly a matter of necessity.

> **译文：** 我认为这体现了人工智能的强大能力，它正朝着这两个方向发展。人工智能目前已经带来了巨大的生产力提升；对于大多数知识工作者来说，如何利用这些优势取决于他们自身的选择，但对于软件开发人员而言，这正日益成为一种必然选择。

That distinction between agency and necessity, however, is an important one: if leveraging a technology depends on humans figuring it out, then penetration will be limited by human creativity and risk taking. Those limits will be very strong in any sort of established company, because the risk calculus will be biased towards avoiding the downsides. Those calculations will make AI sustaining, but nothing more.

> **译文：** 然而，区分自主性和必要性至关重要：如果一项技术的应用依赖于人类的探索和运用，那么其普及程度将受限于人类的创造力和风险承受能力。对于任何成熟的公司而言，这种限制都将非常显著，因为风险评估会倾向于规避风险。这种评估方式能够使人工智能得以持续发展，但仅此而已。

Human creativity and risk taking in the form of a startup, however, operates with a completely different risk profile. For startups the base case is failure; that means that anything that makes success more likely has positive expected value, which is to say that truly leaning into AI will be nothing but upside. Or, to put it another way, it is startups who will be the offensive hackers with nothing to lose by automating everything; it is the incumbents they will be attacking who will be so worried about losing what they have that they will keep humans in the wrong loop for too long.

> **译文：** 然而，以创业形式展现的人类创造力和冒险精神，其风险状况却截然不同。对创业公司而言，失败是基本结果；这意味着任何能提高成功概率的因素都具有正的预期价值，也就是说，真正拥抱人工智能只会带来好处。或者换句话说，创业公司将成为进攻型黑客，它们通过自动化一切来规避风险；而它们要攻击的，是那些因担心失去现有资源而长期让人类困在错误流程中的老牌企业。

Same tools, different incentives, and, in the very long run, very different outcomes.

> **译文：** 同样的工具，不同的激励机制，从长远来看，却会导致截然不同的结果。

Listen to this update and other Stratechery Plus content in your podcast player:

> **译文：** 在您的播客播放器中收听本次更新及其他 Stratechery Plus 内容：

Stratechery  | Sharp Tech  | Dithering  | Sharp China

> **译文：** Stratechery | 夏普科技 | 抖动 | 夏普中国

Greatest Of All Talk  | Asianometry
