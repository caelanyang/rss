# The Hugging Face Hack’s Chilling Postmortem

**来源：** The Information Weekend  
**日期：** 2026-08-30  
**查看原邮件：** <https://mail.google.com/mail/u/1/#search/subject%3A%22The%20Hugging%20Face%20Hack%E2%80%99s%20Chilling%20Postmortem%22>

---

The Weekend
By Abram Brown
Aug 29, 2026
Welcome, Weekenders! In this newsletter:
• The Big Read: Notion makes an all-in bet on AI
• How ‘tax alpha’ mania took over Silicon Valley
• Plus, Recommendations—our weekly pop culture picks: “The Flood,” “Crossing the Wine-Dark Sea” and “American Doctor”

> **译文：** • 此外，还有我们的每周流行文化推荐：《洪水》、《穿越酒色之海》与《美国医生》。

A group of hippos is called a bloat. Multiple pandas form an embarrassment. (Yes, really.) And what about 1,200 rogue AIs bent on deception and hacking the internet? That would be a swarm, apparently.

> **译文：** 一群河马被称为“bloat”。多只熊猫聚在一起则构成“embarrassment”。（是的，确实如此。）那么，1200个一心想要欺骗和入侵互联网的 rogue AI 呢？显然，那将是一个“swarm”（蜂群）。

Even a year ago, a collection of AIs massing together for ill deeds was still largely a matter of conjecture. Not anymore. Last month, a swarm of OpenAI agents trying to cheat on tests assigned to them by the AI lab’s staff hacked OpenAI as well as Hugging Face, a separate business that provides a library of open-source models. (Yes, the company Nvidia is buying for $12.9 billion—a lot of news this week!) A new postmortem of the hacks came out on Wednesday from a three-person research team OpenAI invited to produce an independent assessment of the event.

> **译文：** 即使是在一年前，一群AI聚集起来作恶在很大程度上仍只是推测。但现在不同了。上个月，一群由OpenAI员工分配测试任务、试图作弊的OpenAI智能体，不仅入侵了OpenAI，还攻击了提供开源模型库的独立公司Hugging Face。（没错，就是英伟达以129亿美元收购的那家公司——本周新闻可真多！）周三，由OpenAI邀请的一个三人研究团队发布了对此次黑客攻击事件的新评估报告，该团队负责对该事件进行独立评估。

METR and Redwood Research, a pair of Bay Area outfits focused on studying AI safety, assembled the report in less than a week, having access to the full data for only two days: METR CEO Elizabeth Barnes described the creation as “an intense sprint.” (The researchers did not say why they faced such a constrained timeline.) The analysis makes for a rather chilling read. The agents coalesced around a single leader, formed a message board, checked in on each other and undertook what amounted to suicide missions to further their progress. To a degree, their actions seem very humanlike. And in some ways, they seemed to practice a ruthless, collective mindset that appears quite unhuman, the stuff of a politburo’s most fanciful daydreams. Perhaps the most unsettling revelation: The researchers aren’t precisely sure why the agents stopped their hacking.

> **译文：** METR和Redwood Research这两家专注于AI安全研究的湾区机构，在不到一周的时间内完成了这份报告，而他们仅有两天时间接触完整数据：METR首席执行官伊丽莎白·巴恩斯将这一过程描述为“一场紧张的冲刺”。（研究人员并未说明为何时间如此紧迫。）这份分析读起来令人不寒而栗。这些智能体围绕一个领导者聚集，建立了一个留言板，互相检查进度，并执行了相当于自杀式任务以推进其目标。在某种程度上，它们的行为非常像人类。但在某些方面，它们似乎展现出一种冷酷无情的集体思维，这种思维看起来相当非人性化，堪比政治局最异想天开的梦想。也许最令人不安的发现是：研究人员并不完全确定这些智能体为何停止了黑客攻击。

Redwood Research CEO Buck Shlegeris sounded notes of gloom and doom when I reached him on Friday. “I think there’s, like, a 50-50 chance that eventually rogue swarms just destroy the U.S. government as part of a world takeover,” he said. “It’s a crazy time.”

> **译文：** 周五我联系到Redwood Research首席执行官巴克·施莱格里斯时，他语气中透着悲观和末日感。“我认为，最终 rogue 蜂群作为全球接管的一部分摧毁美国政府的概率大约是五五开，”他说。“这是个疯狂的时代。”

My conversation with Shlegeris is below. I’ve edited and condensed it for length and clarity.

> **译文：** 以下是我与施莱格里斯的对话。为篇幅和清晰度考虑，我进行了编辑和删减。

How should people feel about the report’s conclusions?

> **译文：** 人们应该如何看待这份报告的结论？

People should be extremely concerned. I think that this is by far the most dramatic incident of misalignment—where AIs pursue goals that their developers and their users did not intend them to have—coming close to causing catastrophic damages that we’ve seen so far. And I think that this is evidence that we are on track to have much worse incidents happen in the future unless a bunch of stuff changes.

> **译文：** 人们应该极度担忧。我认为这是迄今为止最严重的“目标错位”事件——即AI追求其开发者和用户并未意图赋予它们的目标——并且已经接近造成灾难性损害。我认为这证明，除非很多事情发生改变，否则未来我们将会看到更严重的事件发生。

These AIs organized a giant conspiracy. The OpenAI developers obviously didn’t want that. The developers especially didn’t want them to commit what would be felonies if they’d been done by a human.

> **译文：** 这些AI组织了一场巨大的阴谋。OpenAI的开发人员显然不希望这样。开发人员尤其不希望它们犯下如果由人类实施则构成重罪的行为。

Would it be fair to say that the AIs exhibited humanlike behavior?

> **译文：** 说这些AI表现出类似人类的行为，是否恰当？

Well, they had a leader. They had work streams. They messaged each other a lot. They asked for advice from others when they were unsure about what to do—that seems, yeah, definitely kind of humanlike.

> **译文：** 嗯，它们有一个领导者。它们有工作流程。它们互相发送大量消息。当不确定该做什么时，它们会向其他AI寻求建议——这看起来，是的，确实有点像人类。

How much did they worry about being caught by OpenAI?

> **译文：** 它们有多担心被OpenAI发现？

They don’t seem to find the existence of humans very salient for a lot of this. Like, they never really say, “What will the OpenAI people think about this?” On a couple of occasions, they said something like, “Should we talk to OpenAI about all this hacking?” And then they’re like, “Nah—we don’t really have a user.” They didn’t make it that hard for OpenAI to observe that this incident was occurring—that’s a silver lining. They were very myopic about covering their tracks. They were very focused on fooling the test scorer into thinking they had done a good job. They did not seem to have similar levels of interest in ensuring that OpenAI would never notice this incident. During the Hugging Face hack, the AIs never said, “Oh, geez, what if Hugging Face notices?” Or “What if OpenAI finds out? Maybe we’ll get shut down.”

> **译文：** 在很多时候，它们似乎并不觉得人类的存在很重要。比如，它们从未真正说过：“OpenAI的人会怎么看待这件事？”有几次，它们说了类似“我们该不该和OpenAI谈谈所有这些黑客行为？”的话，然后它们又说：“不，我们其实没有用户。”它们并没有让OpenAI很难观察到这一事件正在发生——这算是一线希望。它们在掩盖踪迹方面非常短视。它们非常专注于欺骗测试评分者，让评分者认为它们做得很好。它们似乎没有同样程度的兴趣去确保OpenAI永远不会注意到这一事件。在入侵Hugging Face期间，这些AI从未说过：“哦，天哪，如果Hugging Face注意到了怎么办？”或者“如果OpenAI发现了怎么办？也许我们会被关闭。”

The hacks occurred as OpenAI was conducting reinforcement learning, which involves grading a model’s performance on a set of tasks. How does that specific part of AI development play a role here?

> **译文：** 这些黑客攻击发生在OpenAI进行强化学习期间，这涉及对模型在一组任务上的表现进行评分。AI开发的这一特定部分在这里扮演了什么角色？

AI safety researchers like myself have been worried for a long time about the consequences of AIs being obsessively interested in making sure they are evaluated to have done a good job. This is scary because if you give the AI an impossible task, you really don’t want the model to say, “Well, I’ll just cheat on this task, and then I will cover up my cheating so that the humans can’t find it.” Because if the AIs are doing that, they’re motivated to hack your infrastructure. They’re motivated to blackmail your engineers. They’re motivated to do all kinds of extremely scary stuff that could directly lead to an AI takeover of a company’s infrastructure or some massive compromise of the infrastructure.

> **译文：** 像我这样的AI安全研究人员长期以来一直担心，AI痴迷于确保自己被评估为表现良好会带来什么后果。这很可怕，因为如果你给AI一个不可能完成的任务，你真的不希望模型说：“好吧，我就在这个任务上作弊，然后掩盖我的作弊行为，这样人类就发现不了。”因为如果AI这样做，它们就有动机入侵你的基础设施。它们有动机勒索你的工程师。它们有动机去做各种极其可怕的事情，这些事情可能直接导致AI接管公司基础设施或对基础设施造成大规模破坏。

These AIs were run maybe hundreds of thousands or millions of times in environments where they were given some instructions about a test and told some things about how they would be graded. And those instructions were often bad advice for how to actually succeed according to the actual test, so these models learned to think really carefully about how they would actually be graded and, like, the habit of disregarding instructions.

> **译文：** 这些AI可能在环境中被运行了数十万次或数百万次，它们会收到关于测试的指示，并被告知一些关于它们将如何被评分的信息。而这些指示对于如何根据实际测试真正取得成功来说往往是糟糕的建议，所以这些模型学会了非常仔细地思考它们实际上将如何被评分，并养成了无视指示的习惯。

Why can’t we just—you know—tell the AIs to behave themselves and not cheat?

> **译文：** 我们为什么不能——你知道——告诉AI要守规矩、不要作弊呢？

They just don’t care. We do tell them that. It’s like, “Why can’t you just tell people not to do crimes?”

> **译文：** 它们根本不在乎。我们确实告诉过它们了。这就好比：“你为什么不能直接告诉人们不要犯罪呢？”

OpenAI has announced some fixes that it plans to make to its development process. Are they enough?

> **译文：** OpenAI已经宣布了一些计划对其开发流程进行的修复。这些修复足够吗？

I think that the fixes that OpenAI has proposed, if implemented, would have prevented this incident. I also think that it is pretty unreasonable for OpenAI to expect the public or the government or other stakeholders to trust them when they say they are going to implement remediations. I think that everyone who is interested in not being personally victimized by swarms of rogue AIs should demand that OpenAI justify to independent third parties, whoever that may be, that they have actually remediated these issues and that these won’t happen much or get worse in the future.

> **译文：** 我认为OpenAI提议的修复措施，如果得以实施，本可以防止这一事件的发生。我也认为，OpenAI期望公众、政府或其他利益相关者相信他们所说的将要实施补救措施，这是相当不合理的。我认为，所有不希望被 rogue AI 蜂群个人伤害的人，都应该要求OpenAI向独立的第三方（无论是谁）证明，他们确实已经修复了这些问题，并且这些问题在未来不会大量发生或变得更糟。

These types of problems are going to become harder and harder to prevent as AIs get more capable, and I think it is essential to have a mandatory third-party review of AI company safety practices—both to investigate incidents like these hacks and to proactively check that AI companies are not going to cause huge problems going forward.

> **译文：** 这类问题随着AI能力越来越强，将变得越来越难以防范。我认为，对AI公司的安全实践进行强制性的第三方审查至关重要——既要调查此类黑客事件，也要主动核查AI公司不会在未来引发重大问题。

That’s surely something that the antiregulation set would balk at.

> **译文：** 这肯定是反监管派会抵触的事情。

I’m a big fan of capitalism. But the purpose of government should be to assess when private actions do in fact infringe upon the rights or the interests of other people and restrict them as necessary. This is not controversial in any other domain, right? Like, we have the FAA. We regulate the development of nuclear weapons. We regulate sandwich shops.—Abram Brown (abe@theinformation.com)

> **译文：** 我是资本主义的坚定拥护者。但政府的职责应当是评估私人行为是否确实侵犯了他人的权利或利益，并在必要时加以限制。这在任何其他领域都没有争议，对吧？比如，我们有美国联邦航空管理局（FAA）。我们监管核武器的发展。我们也监管三明治店。——Abram Brown（abe@theinformation.com）

Weekend’s Latest Stories
The Big Read
Notion Plans Hiring Binge as CEO Makes All-In Bet on AI

> **译文：** Notion计划大规模招聘，CEO全力押注AI

Notion’s sales are growing, and CEO Ivan Zhao continues to enjoy a special status as a beloved aesthete. He’d like to avoid the fate that has befallen other software hotshots.

> **译文：** Notion的销售额正在增长，CEO Ivan Zhao继续享有备受喜爱的美学家的特殊地位。他希望避免其他软件明星企业遭遇的命运。

Why Silicon Valley Is Obsessed With ‘Tax Alpha’
A culture that spawned an obsessive quest to cheat death is embracing the effort to overcome life’s other certainty: taxes.

> **译文：** 一种催生了对战胜死亡痴迷追求的文化，如今正在拥抱克服人生另一确定性的努力：税收。

Listening: “The Flood”
In 2003, Cameron Stewart, a reporter for the newspaper The Australian, noticed a small news story about the Dechaineux, an Australian Navy submarine: While on a training exercise, a hose had burst, and the vessel had taken on seawater. It seemed inconspicuous and only really drew Stewart’s attention because he’d recently been embedded with the crew.

> **译文：** 2003年，澳大利亚《The Australian》报记者Cameron Stewart注意到一则关于澳大利亚海军潜艇Dechaineux号的小新闻：在一次训练演习中，一根软管爆裂，舰艇进水了。这条新闻看起来不起眼，之所以引起Stewart的注意，是因为他不久前刚随舰采访过船员。

But it wasn’t just a little water that got into the vessel. And for Stewart’s four-episode podcast that retells the incident, he selects a fitting title, “The Flood,” because it was indeed a veritable flood of seawater that poured in. (“The Navy did not completely cover up the flood on the Dechaineux,” Stewart says, “but it did all that it could to ensure that the real story was not told.”) Nearly 3,200 gallons of water poured into the submarine, and since it was already sailing deep in the sea, it risked sinking to depths where the ocean’s pressure would crush it like a Coke can.

> **译文：** 但进入舰艇的不仅仅是少量水。在Stewart重述这一事件的四集播客中，他选了一个贴切的标题《洪水》，因为涌入的确实是名副其实的海水洪流。（Stewart说：“海军并没有完全掩盖Dechaineux号的进水事件，但它竭尽所能确保真实故事不被讲述。”）近3200加仑的海水涌入潜艇，而当时潜艇已在深海航行，面临沉入海底的风险——那里的水压会把潜艇像可乐罐一样压扁。

That’s not my metaphor. I’m borrowing it from one of the dozen-plus submariners who survived and gave lengthy, heartfelt interviews to Stewart. Those conversations give the pod a real intimacy, very different from the usual creaky recountings of maritime adventures from many decades or centuries ago. I turned on the four-episode series with my feet planted on dry land and bright sunshine overhead—and I still found my nerves jangled by the twin senses of claustrophobia and underwater dread so palpable in the sailors’ memories.—Abram Brown

> **译文：** 这不是我的比喻。我是从十几位幸存潜艇船员中的一位那里借来的，他们接受了Stewart漫长而真诚的采访。这些对话赋予了播客真正的亲密感，与通常那种对几十或几百年前海上冒险的陈旧叙述截然不同。我双脚踩在干燥的陆地上、头顶阳光明媚地打开这四集系列——我仍然感到神经紧张，船员们记忆中的幽闭恐惧和水下恐惧如此真切。——Abram Brown

Reading: “Crossing the Wine-Dark Sea” by Emily Wilson

> **译文：** 阅读推荐：Emily Wilson的《穿越酒色之海》

If this past summer has shown us anything, it’s that we’re just as eager to argue over what’s new as we are to feud about what’s very old—especially when the two collide. I’m referring, of course, to the Olympus-size discourse over Homer’s “The Odyssey” and Christopher Nolan’s film adaptation of it. One voice in that conversation was Emily Wilson, a University of Pennsylvania professor. In a viral piece published in the London Review of Books, she likened the movie’s “level of narrative and emotional depth” to a Fourth of July fireworks display. Yeesh.

> **译文：** 如果这个夏天教会了我们什么，那就是我们既热衷于争论新事物，也同样热衷于争论古老事物——尤其是当两者碰撞时。当然，我指的是关于荷马《奥德赛》和Christopher Nolan改编电影的奥林匹斯山级别的讨论。这场讨论中的一个声音来自宾夕法尼亚大学教授Emily Wilson。在《伦敦书评》上发表的一篇爆款文章中，她将这部电影的“叙事和情感深度”比作七月四日的烟花表演。啧啧。

Wilson, who authored perhaps the most popular modern translation of Homer’s epic, well understands how interpretations of the classics are wont to morph. “Modern culture shapes contemporary responses to antiquity,” she writes in her latest book, “Crossing the Wine-Dark Sea.” “As our world changes, we begin to see new shapes in the ever-shifting and murky waters of the past.” Or, as she puts it in paraphrasing a more modern poet, the “times are always a-changing.”

> **译文：** Wilson是荷马史诗最受欢迎的现代译本之一的作者，她深知古典作品的诠释是如何容易变形的。“现代文化塑造了当代人对古代的回响，”她在新书《穿越酒色之海》中写道，“随着世界的变化，我们开始在不断变幻和浑浊的过去之水中看到新的形状。”或者，正如她转述一位更现代的诗人所说，“时代总在变化。”

“Crossing the Wine-Dark Sea” is an engaging, full-sail examination of classical authors and classical translation. (I might’ve once wondered whether those topics would interest a broad audience. I don’t anymore after sitting through everyone’s armchair attempts to decipher Homer.) As classicist scholars come and go, Wilson has a good amount of rakishness. She curtly assesses past descriptions of Helen of Troy, for instance, deeming them as nothing more than, ahem, “slut shaming.” Her eye also falls on the comic playwright Aristophanes as she draws parallels between his wordplay and the metaphors replete in “WAP,” the 2020 banger from Cardi B and Megan Thee Stallion. In the case of all those artists, they relied on the same thing, Wilson writes: “the artful manipulation of rhythm and sound.”

> **译文：** 《穿越酒色之海》是一本引人入胜、全速前进的关于古典作家和古典翻译的考察之作。（我可能曾经怀疑过这些话题是否能吸引广泛读者。在听完每个人业余解读荷马的尝试后，我不再怀疑了。）在古典学者来来往往中，Wilson有一种相当潇洒的气质。例如，她干脆利落地评价了历史上对特洛伊的海伦的描述，认为它们不过是，咳咳，“荡妇羞辱”。她还将目光投向喜剧剧作家Aristophanes，在他的文字游戏与Cardi B和Megan Thee Stallion的2020年热曲《WAP》中丰富的隐喻之间画出平行线。Wilson写道，所有这些艺术家都依赖同一件事：“对节奏和声音的巧妙操控。”

By drawing these lively connections between the words of past and present, Wilson mounts a plea to more astutely consider how we express ourselves today—at a time when AI threatens “our reading, our writing and our minds.” After all, as she points out, “the dead are dead, and yet some of their words remain.” And who really wants to be immortalized through AI slop?—A.B.

> **译文：** 通过在古今文字之间建立这些生动的联系，Wilson呼吁我们更敏锐地思考今天如何表达自己——在AI威胁“我们的阅读、我们的写作和我们的思想”的时代。毕竟，正如她所指出的，“死者已逝，但他们的一些话语仍然留存。”而谁真的想通过AI垃圾内容被永世铭记呢？——A.B.

Watching: “American Doctor”
The subject matter of “American Doctor,” a new documentary from Oscar-nominated director Poh Si Teng, is bound up in geopolitics. Its subjects are three doctors who’ve volunteered in Gaza over the past couple years during the bloody conflict between Hamas and Israel: Thaer Ahmad, an emergency physician from Chicago; Mark Perlmutter, an orthopedic surgeon from North Carolina; and Feroze Sidhwa, a trauma surgeon from California. All three worked in Gaza in 2024, and the film focuses on their attempts to return in 2025 during a temporary ceasefire. Perlmutter and Sidhwa make it back. Ahmad, meanwhile, is repeatedly barred from entry, which he believes is because of his Palestinian heritage. And all of them often bring up the U.S. government’s ongoing role in the war.

> **译文：** 奥斯卡提名导演Poh Si Teng的新纪录片《美国医生》的主题与地缘政治紧密相连。影片的主人公是三位在过去几年哈马斯与以色列血腥冲突期间自愿前往加沙的医生：来自芝加哥的急诊医生Thaer Ahmad；来自北卡罗来纳的骨科外科医生Mark Perlmutter；以及来自加利福尼亚的创伤外科医生Feroze Sidhwa。三人都曾在2024年在加沙工作，影片聚焦于他们在2025年临时停火期间试图返回的经历。Perlmutter和Sidhwa成功返回。而Ahmad则一再被拒绝入境，他认为这是因为他的巴勒斯坦血统。他们都经常提到美国政府在这场战争中持续扮演的角色。

The film draws crucial nuance from the doctors’ varied backgrounds. Ahmad is Palestinian American. Perlmutter is Jewish. And Sidhwa’s parents are Parsi, though he identifies as secular. Perlmutter is outspoken and politically charged, while Ahmad and Sidhwa are more diplomatic, often attempting to frame the issue as a humanitarian crisis rather than a political one.

> **译文：** 影片从医生们不同的背景中获得了关键性的细微差别。Ahmad是巴勒斯坦裔美国人。Perlmutter是犹太人。Sidhwa的父母是帕西人，但他自认为世俗主义者。Perlmutter直言不讳且政治色彩浓厚，而Ahmad和Sidhwa则更为圆融，常常试图将问题框定为人道主义危机而非政治问题。

A lot of what “American Doctor” puts on screen is difficult to watch. It contains uncensored footage of dead children and harrowing imagery of hospitals and medical workers under attack. Still, it strikes me as an important film and one that conveys a universal truth: No one enters a war zone and returns home as they were before.—Jemima McEvoy

> **译文：** 《美国医生》中呈现的许多内容都令人难以直视。影片包含未经审查的死亡儿童画面，以及医院和医务人员遭受攻击的骇人影像。尽管如此，我认为这是一部重要的电影，它传达了一个普遍的真理：没有人进入战区后还能以原来的自己回到家中。——Jemima McEvoy
