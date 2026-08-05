# Money Stuff: Leveraged ETF Crash Hedging ETF

**来源：** Matt Levine  
**日期：** 2026-08-05  
**查看原邮件：** <https://mail.google.com/mail/u/1/#search/subject%3A%22Money%20Stuff%3A%20Leveraged%20ETF%20Crash%20Hedging%20ETF%22>

---

Money Stuff

Cliquet, taxes, Santos, wallet, dentist.

View in browser

Subscribe to Bloomberg.com for unlimited access to all our coverage.

> **译文：** 订阅彭博社网站，即可无限畅享我们的所有报道。

Leveraged ETF crash put cliquet ETF

Last weekend Bloomberg’s Yiqin Shen published a fun story that would make for a good final exam in a financial engineering class. It has a bit of everything.

> **译文：** 上周末，彭博社的沈怡琴发表了一篇趣味十足的文章，很适合作为金融工程课程的期末考试题。这篇文章包罗万象。

Start with leveraged exchange-traded funds. Lots of investors want to get 2 or

> **译文：** 先从杠杆型交易所交易基金（ETF）入手。很多投资者都想获得2倍或以上的收益。

3 times the daily return of some stock, and there are single-stock levered ETFs that provide this. Investors put in $100 of their own money, the ETF borrows

> **译文：** 某些股票的日收益可以达到三倍，而且市面上也有一些单只杠杆ETF可以提供这种收益。投资者投入100美元自有资金，ETF则借入资金。

$100 from a bank, and it buys $200 of SK Hynix Inc. stock or whatever. (Really it will do this using total return swaps, but that doesn’t matter for our purposes.) If the stock goes up 5%, the ETF will have $210 worth of stock, a

> **译文：** 它从银行借入 100 美元，然后购买价值 200 美元的 SK 海力士公司股票或其他股票。（实际上，它会使用总收益互换来实现这一点，但这与我们的目的无关。）如果股票上涨 5%，该 ETF 将持有价值 210 美元的股票，

10% return on the investors’ $100. To keep providing the same 2x exposure the next day,the ETF will have to rebalance : It will borrow another $10 from its bank to buy more stock, so that the next day it has

> **译文：** 投资者投入100美元，获得10%的回报。为了第二天继续提供相同的2倍敞口，该ETF需要进行再平衡：它将从银行再借10美元购买更多股票，以便第二天拥有……

$220 worth of stock, twice its equity. Or if the stock goes down, the ETF will sell some to repay some borrowing.

> **译文：** 价值 220 美元的股票，是其净值的两倍。或者，如果股价下跌，ETF 将出售部分股票以偿还部分借款。

This means that, each day, the bank has loaned $X against $2X of stock: It has no real long-term risk, because if the collateral ever loses value some of the loan is automatically repaid. The only risk is if the stock falls more than 50% in a day [1] <>: The ETF only has $100 from its investors, and if that equity is wiped out then there’s nothing else. If it borrows $100 to buy $200 of

> **译文：** 这意味着，银行每天都以价值 2X 美元的股票为抵押发放 X 美元的贷款：它没有真正的长期风险，因为如果抵押品贬值，部分贷款会自动偿还。唯一的风险是股票在一天内下跌超过 50% [1] <>：该 ETF 只有 100 美元的投资者资金，如果这部分资金全部损失，那么它就没有其他资产了。如果它借入 100 美元购买价值 200 美元的股票，

stock, and that stock falls 60%, the bank has only $80 of collateral to secure its $100 loan. It can’t send a margin call asking for more money; there’s no more money. Shen:

> **译文：** 如果股票下跌了60%，银行只有80美元的抵押品来担保其100美元的贷款。它无法发出追加保证金通知，因为已经没有钱了。沈：

The setup leaves banks exposed to what’s known as “gap risk.” If a stock falls sharply enough in a single session — roughly more than 50% for a 2X fund or 33% for a 3X fund — the ETF is at risk of losing an amount greater than its net assets, potentially strapping the banks with losses that the fund’s issuer can’t cover.

> **译文：** 这种机制使银行面临所谓的“缺口风险”。如果一只股票在一个交易日内大幅下跌——对于2倍杠杆基金来说，跌幅大约超过50%；对于3倍杠杆基金来说，跌幅大约超过33%——那么该ETF就有可能损失超过其净资产，这可能会使银行背负基金发行方无法弥补的损失。

This is a very unlikely risk, but not impossible: Leveraged ETFs are particularly popular on underlying stocks that are volatile to begin with, and leveraged ETFsincrease the volatility of the underlying stock by buying when it goes up and selling when it goes down. We talked last month about a leveraged ETF on Lucid

> **译文：** 这虽然风险极小，但并非完全不可能：杠杆ETF尤其受到那些本身波动性就较大的股票的青睐，因为它们通过在标的股票上涨时买入、下跌时卖出来加剧标的股票的波动性。我们上个月讨论过Lucid平台上的一只杠杆ETF。

Group Inc., which got wiped out when Lucid fell 57% intraday. It happens.

> **译文：** Group Inc. 的股票在 Lucid 盘中暴跌 57% 时全部损失殆尽。这种情况时有发生。

Banks do not like this sort of weird tail risk, so they want to buy insurance.

> **译文：** 银行不喜欢这种奇怪的尾部风险，所以他们想购买保险。

The insurance takes approximately the form “if the underlying stock falls more than 50% on any day, you pay us the difference.” That is a put option, or more technically it’s acliquet , a series of daily put options each struck at a price that is down 50% from the previous day’s close.

> **译文：** 这种保险的形式大致是“如果标的股票在任何一天下跌超过 50%，您需向我们支付差价”。这是一种看跌期权，或者更准确地说，是一种看跌期权组合，即一系列每日看跌期权，每个期权的行权价格都比前一天的收盘价下跌 50%。

A bank might pay a hedge fund some premium upfront for a one-year series of these puts, to hedge it against its leveraged ETF risk on a stock:

> **译文：** 银行可能会预先向对冲基金支付一定的溢价，以获得为期一年的此类看跌期权，从而对冲其杠杆ETF在某只股票上的风险：

The result has been a quiet surge of activity in an exotic corner of the derivatives market, where investment banks, hedge funds and other institutional investors trade what are often known as “crash puts” and sometimes referred to as cliquets or stability notes.

> **译文：** 其结果是，衍生品市场一个特殊的领域悄然出现了交易活跃度激增，投资银行、对冲基金和其他机构投资者在这里交易通常被称为“崩盘看跌期权”的证券，有时也被称为“稳定票据”或“稳定债券”。

“I have never seen this level of demand in this product,” said Natasha Sibley, a portfolio manager in the diversified alternatives team of Janus Henderson.

> **译文：** “我从未见过这种产品有如此高的需求，” Janus Henderson 多元化另类投资团队的投资组合经理 Natasha Sibley 说。

We talked about crash insurance last week , and I mentioned some problems with it:

> **译文：** 我们上周讨论了交通事故保险，我提到了一些它存在的问题：

* People do not like selling way-out-of-the-money insurance against unlikely events, because they collect only a small premium for the insurance, but might have to pay out a lot of money in bad states of the world.

> **译文：** 人们不喜欢销售赔付金额过高的保险，以应对不太可能发生的事件，因为他们只能收取少量保费，但在世界局势恶化时，他们可能不得不支付一大笔钱。

* You might not want to buy way-out-of-the-money insurance against unlikely events from a hedge fund, because if the bad state of the world occurs, the hedge fund might be bankrupt.

> **译文：** * 你可能不想从对冲基金购买针对不太可能发生的事件的严重亏损的保险，因为如果世界局势恶化，对冲基金可能会破产。

The solution to the second problem, as we discussed last week, is pre-funding:

> **译文：** 正如我们上周讨论的那样，第二个问题的解决方案是预先筹资：

Instead of just paying the hedge fund, say, $3 for its future promise to pay up to $100 in a crash, the bank sells the hedge fund a $100structured note. The hedge fund gives the bank $100 upfront for the note. If the crash happens, the bank keeps (some of) the money; the note is triggered and doesn’t repay its full principal amount. If no crash happens, the bank repays the hedge fund’s

> **译文：** 银行并没有直接向对冲基金支付3美元（假设其承诺在市场崩盘时支付最高100美元），而是向其出售一张面值100美元的结构性票据。对冲基金预先向银行支付100美元购买该票据。如果市场崩盘发生，银行可以保留部分资金；票据被触发，但不会偿还全部本金。如果没有发生市场崩盘，银行则会偿还对冲基金的100美元。

$100, plus interest, plus the $3 insurance premium, in a year.

> **译文：** 一年下来，本金100美元，外加利息，外加3美元的保险费。

That $3 is not very exciting, though. The solution to the first problem is levering the note:Instead of the hedge fund giving the bank $100 for the note, the hedge fund gives the bank $20 for the note and borrows the other $80 from the bank. [2] <> If the crash happens, the bank keeps (some of) the hedge fund’s $20. If the crash is really really bad, though, the hedge fund’s $20 is

> **译文：** 不过，这3美元确实没什么吸引力。第一个问题的解决方法是利用杠杆：对冲基金不必向银行支付100美元购买票据，而是支付20美元，然后从银行借入剩余的80美元。[2] 如果崩盘发生，银行将保留（部分）对冲基金的20美元。但如果崩盘非常严重，对冲基金的20美元将损失殆尽。

not sufficient to cover the bank’s losses, and the bank eats the rest. It has not insured itstail risk, per se, but rather the, like, first-few-inches-of-the-tail risk.

> **译文：** 不足以弥补银行的损失，剩余部分由银行自行承担。它并没有为尾部风险本身投保，而只是为类似尾部最初几英寸的风险投保。

This might be sensible for intuitive how-leveraged-ETFs-work reasons. If the underlying stock falls a lot, the leveraged ETF (or rather the bank providing the leverage) will sell stock during the day to reduce its risk. This will drive the stock further down. But by the time the stock has fallen by 50%, the bank will have sold all of the underlying stock (and the leveraged ETF will go

> **译文：** 从杠杆ETF的运作原理来看，这或许合情合理。如果标的股票大幅下跌，杠杆ETF（或者更确切地说是提供杠杆的银行）会在当天卖出股票以降低风险。这将进一步推低股价。但当股价下跌50%时，银行将卖出所有标的股票（杠杆ETF也将退出交易）。

poof). There won’t be any more selling pressure from the ETF, so the stock should recover. (Worked for Lucid!) There will be some slippage — the stock won’t turn on a dime at a 50% loss — but if the hedge funds cover the losses from down 50% to down 60%, that’s probably a good enough cushion.

> **译文：** （噗）。ETF不会再有抛售压力，所以股价应该会反弹。（Lucid就是个例子！）当然，股价下跌50%后不会立刻反弹，但如果对冲基金能够弥补50%到60%的损失，那应该就足够了。

And now, instead of earning a $3 premium on a $100 investment (a ho-hum 3%), the hedge fund is earning a $3 premium on a $20 investment, a juicier 15%. [3]

> **译文：** 现在，对冲基金不再像以前那样，投资 100 美元只能赚取 3 美元的溢价（3%），而是投资 20 美元就能赚取 3 美元的溢价，这可是高达 15% 的丰厚回报。[3]

<> Now the trade works for the hedge fund. The bank has bought pre-funded tail insurance from a hedge fund, and then levered up that insurance — effectively buying back part of the tail risk — to make the economics work:

> **译文：** 现在这笔交易对这家对冲基金有利。这家银行从一家对冲基金购买了预先融资的尾部保险，然后利用杠杆购买了该保险——实际上是回购了一部分尾部风险——从而使交易在经济上可行：

One email from Goldman Sachs Group Inc. in May pitched a trade idea around

> **译文：** 高盛集团五月份的一封电子邮件提出了一项交易策略。

“Expensive Crash Cliquet”: it meant to capitalize on “immense demand” to hedge the share prices of South Korea’s SK Hynix Inc. and Samsung Electronics Co., since a one-day share-price drop of 50% or more could wipe out the 2X ETFs tied to them. How expensive exactly? The proposed yields on offer for investors with the gumption to assume the tail risk for up to one year — and use leverage to

> **译文：** “高价崩盘基金”：其目的是利用“巨大的市场需求”对冲韩国SK海力士和三星电子的股价，因为股价单日下跌50%或更多就可能导致与这两家公司挂钩的2倍ETF全部损失。究竟有多贵？对于那些有胆量承担长达一年尾部风险并愿意利用杠杆的投资者来说，拟议的收益率是多少？

amplify returns — ranged from 14.2% to 20%.

The trade “presents an opportunity for investors to act as the ‘insurer,’ selling this overpriced crash protection to earn a high premium,” the email read.

> **译文：** 邮件中写道，这项交易“为投资者提供了一个扮演‘保险人’的角色的机会，通过出售这种价格过高的碰撞保险来赚取高额保费”。

And then the cherry on top is that you smash the whole thing into an ETF:

> **译文：** 更妙的是，你还要把所有这些都打包成一个ETF：

These days, the type of income available from crash-put products isn’t only available to big funds: There are now ETFs that offer it. Janus Henderson launched two active structured income funds in April, JELH and JELM, which use stability swaps and equity-linked notes to package institutional structured-note strategies.

> **译文：** 如今，崩盘期权产品带来的收益不再仅限于大型基金：现在也有ETF提供此类收益。骏利亨德森(Janus Henderson)于4月推出了两只主动型结构化收益基金JELH和JELM，它们利用稳定互换和股票挂钩票据，将机构结构化票据策略打包在一起。

“It’s been great timing,” said Sibley. “When we designed these ETFs, we wanted to include stability notes in there along with autocallables. We were familiar with them in the index space and liked the pricing, but since then they have exploded in the single-stock space.”

> **译文：** “时机真是太好了，”西布利说。“我们在设计这些ETF时，就想把稳定收益凭证和自动赎回条款一起纳入其中。我们之前在指数领域就接触过这类产品，也很喜欢它们的定价，但从那以后，它们在个股领域也迅速发展起来。”

An ETF that sells crash puts against the gap risk of leveraged single-stock

> **译文：** 卖出崩盘看跌期权的ETF可以对冲杠杆个股的缺口风险。

ETFs, wonderful.

Taxes

It seems plausible that finance would be getting more efficient over time. A lot of smart people work long hours to apply increasingly sophisticated math and technology to the allocation of capital; surely they should get better at it. What would that mean for investors? The simplest answer seems drab and boring: If finance is more efficient, it should be hard to beat the market;

> **译文：** 金融效率随着时间的推移而提高似乎是合情合理的。许多聪明人长时间工作，运用日益复杂的数学和技术来配置资本；他们当然应该做得更好。这对投资者意味着什么？最简单的答案似乎枯燥乏味：如果金融效率更高，那么战胜市场就应该变得非常困难；

every investment should earn its appropriate risk-adjusted return. Efficient computers canmake market prices correct more cheaply than old-fashioned artisanal human arbitrageurs did, so the returns to being smarter than the market should go down.

> **译文：** 每项投资都应该获得与其风险相符的收益。高效的计算机能够比传统的手工套利者更经济地纠正市场价格，因此，比市场更聪明所带来的收益应该下降。

If you expand your focus a little bit, you could tell more optimistic stories.

> **译文：** 如果你稍微拓宽一下视野，你就能讲述更多乐观的故事。

“Efficient finance will allow society tofinance a giant artificial intelligence buildout that willusher in a golden age of abundance, and which would not have been possible in an earlier era of less perfect capital allocation”: sure, maybe? With perfectly efficient finance, investors can’t really expect to earn market-beatingreturns, but maybe the market returns will be higher if the

> **译文：** “高效的金融体系将使社会能够为大规模人工智能建设提供资金，从而开启一个富足的黄金时代，而这在资本配置不完善的早期时代是不可能实现的”：真的吗？也许吧？在完全高效的金融体系下，投资者实际上无法指望获得超越市场的回报，但如果……，市场回报或许会更高。

market omnisciently finances the best projects.

Those are the two main sources of returns to investors: Increasing financial efficiency might increase economic growth, but it can’t increase net market-beating returns, and should probably decrease gross market-beating returns.

> **译文：** 这是投资者获得回报的两大主要来源：提高金融效率可能会促进经济增长，但不能提高净市场收益，而且可能会降低总市场收益。

But there is another source of returns. That source is the Internal Revenue

> **译文：** 但还有另一种收益来源，那就是美国国税局的税收收入。

Service. The aggregate return of investing, to investors, is notquite the market return. It’s the market return minus taxes. If the broad market return is 10%, then investors in the aggregate will earn 10% before taxes. But they might earn 8% or 9% or 10% or conceivably 12% after taxes. That number will be determined by skill: The more skillful and efficient finance is, the more brain

> **译文：** 服务。对投资者而言，投资的总体回报并非市场回报，而是市场回报减去税收。如果整体市场回报率为10%，那么投资者税前总回报率为10%。但税后回报率可能为8%、9%、10%，甚至可能达到12%。这个数字取决于投资技巧：金融越精明高效，投资者的回报就越高。

and computer power that is devoted to reducing taxes, the lower the taxes will be. On investors. [4] <>

> **译文：** 计算机算力用于减税的程度越高，税收就越低。对投资者而言。[4] <>

If finance is getting more efficient over time, then one way — perhaps increasingly themain way? — that would manifest is in the form of investors paying no taxes.

> **译文：** 如果金融业随着时间的推移变得越来越高效，那么其中一种表现形式——或许会成为主要表现形式？——就是投资者无需缴纳税款。

And here we are! We talked last month about Section

> **译文：** 好了！我们上个月讨论了“章节”部分。

351 exchange-traded funds. The gist of it is:

* ETFs are, approximately, investing vehicles that pay no taxes on their gains; and

> **译文：** * ETF（交易所交易基金）大致来说是一种投资工具，其收益无需缴税；

* In a perfectly efficient financial world, every investor can become their own ETF, so that they never need to pay taxes on their gains.

> **译文：** * 在一个完全高效的金融世界里，每个投资者都可以成为自己的ETF，这样他们就永远不需要为自己的收益缴税。

And today Bloomberg’s Loukia Gyftopoulou, Katherine Burton, Sridhar Natarajan and Justina Leereport :

> **译文：** 今天彭博社的Loukia Gyftopoulou、Katherine Burton、Sridhar Natarajan和Justina Leereport报道：

Cliff Asness … and his team at AQR Capital Management had figured out a way to make a widespread technique for reducing taxes much more potent. Their discovery: The right mix of stock bets not only grows tax-free, it can eliminate taxes from other investments, too. ...

> **译文：** 克利夫·阿斯内斯（Cliff Asness）……以及他在AQR资本管理公司的团队，找到了一种方法，可以更有效地运用一种广泛应用的减税技巧。他们的发现是：正确的股票组合不仅可以免税增长，还可以消除其他投资的税收。

By some estimates, a total of more than $150 billion is deployed at the firm and a phalanx of competitors that run their own versions of what’s known as tax-aware long-short investing. That puts them at the cutting edge of the broader “tax alpha” universe, in which more than $1 trillion is deployed in strategies devoted to delaying or shrinking payments to the government. …

> **译文：** 据估计，该公司及其众多竞争对手共投入超过1500亿美元，这些竞争对手各自运营着所谓的“避税型多空投资”策略。这使它们处于更广泛的“避税阿尔法”领域的前沿，该领域投入的资金超过1万亿美元，用于制定旨在延迟或减少向政府缴纳税款的策略。

For AQR, the payoff already has been enormous, turning it into the world’s largest hedge fund by the end of 2025, the latest industry data show. Its hedge fund assets multiplied within just a few years, leapfrogging rivals to surpass

> **译文：** 对于AQR而言，回报已十分丰厚。最新行业数据显示，到2025年底，AQR将成为全球最大的对冲基金。其对冲基金资产在短短几年内成倍增长，超越竞争对手，遥遥领先。

$140 billion by the end of March.

We have talked a few times about tax-aware long-short strategies. If you buy a bunch of stocks, some will go up and some will go down. You sell the ones that went down, generating capital losses that you can use to offset other capital gains, and keep the ones that went up, deferring capital gains taxes.

> **译文：** 我们之前多次讨论过节税型多空策略。如果你买入一批股票，有些会涨，有些会跌。卖掉那些下跌的股票，产生资本损失，这些损失可以用来抵消其他资本收益；而持有那些上涨的股票，则可以延缓缴纳资本利得税。

This is called “tax loss harvesting,” and back in the olden days it was a sophisticated strategy that your financial adviser would laboriously execute for you, but now any robo-adviser will do it.

> **译文：** 这被称为“税损收割”，在过去，这是一种复杂的策略，需要你的财务顾问费尽心思为你执行，但现在任何智能投顾都能做到。

“Tax-aware long-short” involves grossing this up: Instead of spending $100 to buy a bunch of stocks, you borrow $100, buy $200 worth of stocks and then short

> **译文：** “避税型多空策略”涉及将总收益提高：与其花费 100 美元购买大量股票，不如借入 100 美元，购买价值 200 美元的股票，然后做空。

$100 of other stocks. You still have $100 of net market exposure — you are still exposed to the market return on $100 of stocks — but you have much more tax loss. (Because you own $200 of stocks instead of $100, and because you now have offsetting long and short bets, one of which will presumably win when the other loses.) And then maybe with the right witchcraft you can do this in ways

> **译文：** 100 美元的其他股票。你仍然有 100 美元的净市场敞口——你仍然会面临这 100 美元股票的市场回报——但你的税收损失要大得多。（因为你持有 200 美元的股票而不是 100 美元，而且你现在有相互抵消的多头和空头头寸，其中一个头寸很可能在其中一个头寸亏损时盈利。）然后，或许通过某种“魔法”，你可以用某种方式做到这一点。

that generate ordinary-income losses rather than capital losses.

> **译文：** 产生普通收入损失而非资本损失。

One thing to say about tax-aware long-short is that it is not just about reading the tax code cleverly. It really is about increasing financial efficiency; it is an outgrowth of modern academic finance. When I first wrote about it,here’s how I started :

> **译文：** 关于税务敏感型多空策略，需要指出的是，它不仅仅是巧妙地解读税法。它真正关乎的是提高财务效率；它是现代学术金融的产物。我最初撰写相关文章时，是这样开头的：

One useful intuition of modern finance is that stocks are all kind of the same. Oh they’re not, they’re not, this isn’t true. But lots of stocks are interchangeable to some degree, particularly if you own a lot of them. A fair amount of the returns of many stock portfolios are determined by the returns to the overall market, to industry sectors, and to other well-known factors like

> **译文：** 现代金融中一个有用的直觉是，股票本质上都差不多。哦，它们并不一样，这说法并不正确。但很多股票在某种程度上是可以互换的，尤其是在你持有大量股票的情况下。许多股票投资组合的收益很大程度上取决于整体市场、行业板块以及其他一些众所周知的因素的收益，例如……

value and size. You could construct a diversified portfolio of 100 stocks that is reasonably well correlated with the S&P 500 Index, and then you could construct a diversified portfolio of 100 entirely different stocks that is also reasonably well correlated with the S&P 500.

> **译文：** 价值和规模。你可以构建一个由100只股票组成的多元化投资组合，该投资组合与标普500指数具有相当好的相关性；然后，你也可以构建一个由100只完全不同的股票组成的多元化投资组合，该投资组合也与标普500指数具有相当好的相关性。

This would have sounded like witchcraft a generation ago. “No,” investors would have said, “an investment in Amalgamated Spats is a bet on the spats industry and the cut of the chief executive officer’s jib; selling Amalgamated

> **译文：** 这在上一代人看来简直就是巫术。“不，”投资者会说，“投资Amalgamated Spats就是押注护腿行业和首席执行官的魄力；出售Amalgamated Spats的股票就是在押注护腿行业和首席执行官的魄力；

Spats to buy Consolidated Sprockets is no substitute at all.” But the rise of quantitative finance and factor investing — in which Asness and AQR are leading figures — has normalized this view. “My portfolio has a lot of exposure to small-cap value,” an investor might say, without knowing what actual stocks she owns. You can get your small-cap value exposure from a lot of different stocks.

> **译文：** 认为买入 Consolidated Sprockets 完全不可取。”但量化金融和因子投资的兴起——阿斯内斯和 AQR 是这方面的领军人物——已经使这种观点变得普遍。“我的投资组合中有很多小盘价值股，”一位投资者可能会这样说，却不知道自己实际持有哪些股票。你可以通过很多不同的股票来获得小盘价值股的配置。

This matters for tax-aware long-short strategies, because:

> **译文：** 这对于注重税务筹划的多空策略至关重要，因为：

* You have to be long some stocks, and short some other stocks as a hedge. If the short stocks are going to be a good hedge, they have to be correlated with the long stocks. [5] <> But you can’t be long and short the same stocks:

> **译文：** * 你必须做多一些股票，同时做空另一些股票来进行对冲。如果做空的股票要起到良好的对冲作用，它们必须与做多的股票具有相关性。[5] <> 但你不能同时做多和做空同一批股票：

That’s astraddle , and you won’t be able to deduct your losses. You have to be long and shortsimilar stocks, which requires a factor-based quant approach.

> **译文：** 这是跨式期权策略，你的损失无法抵扣。你必须同时做多和做空相似的股票，这需要采用基于因子的量化方法。

* When you harvest your tax losses, you have to sell some stocks (the losers) and buy new ones to replace them. [6] <> You can’t buy the same stocks: That’s awash sale , and you won’t be able to deduct your losses. You have to sell your stocks and buy similar stocks, which again requires a quantitative notion of similarity.

> **译文：** * 当你利用税收亏损进行交易时，你需要卖掉一些股票（亏损的股票），并买入新的股票来替代它们。[6] <> 你不能买入相同的股票：那样就属于重复交易，你将无法抵扣亏损。你必须卖掉亏损的股票，并买入类似的股票，这又需要对“类似”进行量化定义。

The upshot is that, if you take a bunch of finance PhDs and apply sophisticated mathematical methods to investing, what you might get islower taxes.Which makes total sense.

> **译文：** 结论是，如果你召集一群金融学博士，并将复杂的数学方法应用于投资，你可能会得到更低的税收。这完全合乎逻辑。

Also, there’s a reason that this stuff made AQR the world’s largest hedge fund. If finance is getting more efficient, then that should mean that alpha is getting scarcer: It is harder to beat the market, and the returns to being smarter than everyone else should be getting lower and harder to find. But if finance is getting more efficient, the that should mean thattax alpha is

> **译文：** 此外，AQR之所以能成为全球最大的对冲基金，也是有原因的。如果金融效率不断提高，那么超额收益（alpha）应该会越来越稀缺：战胜市场变得更加困难，比其他人更聪明所带来的回报应该越来越低，也越来越难获得。但如果金融效率不断提高，那么税收超额收益（tax alpha）应该会越来越稀缺。

getting more plentiful: It is easier to beat the IRS, and the returns to being smarter than the IRS should be getting higher. You can put more money to work in “beat the IRS” than you can in “beat other hedge funds.”

> **译文：** 机会越来越多：战胜美国国税局变得越来越容易，而且比国税局更聪明的回报也应该越来越高。比起“战胜其他对冲基金”，你可以投入更多资金来“战胜国税局”。

Anyway the Bloomberg story has other good bits. For instance:

> **译文：** 总之，彭博社的报道还有其他精彩之处。例如：

A presentation that AQR recently provided to some wealth managers to recruit more clients sketches out an astonishing scenario: Invest $100 million in the most aggressive of AQR’s Flex strategies. Wait 10 years while the money triples. And in that period, it may generate over $580 million of losses that can be used to erase taxes from other investments.

> **译文：** AQR最近向一些财富管理机构提供的一份旨在招揽更多客户的演示文稿描绘了一个令人震惊的场景：投资1亿美元于AQR最激进的Flex策略。等待10年，资金将翻三倍。在此期间，该策略可能产生超过5.8亿美元的亏损，这些亏损可用于抵消其他投资的税款。

It’s safe to say that, in the hedge fund world, boasting that a strategy might produce almost six times more losses than the initial investment is unusual.

> **译文：** 可以肯定地说，在对冲基金界，吹嘘某种策略可能会造成比初始投资高出近六倍的损失是不寻常的。

No, it’s efficient. In the modern world, if you send clients a presentation saying “we will 6x your money in 10 years,” they’ll be like “no, markets are efficient, you cannot promise that level of outperformance.” If you send clients a presentation saying “we will generate reasonable alpha but also tax losses of 6x your investment in 10 years” they will be like “ah, good, you are

> **译文：** 不，这很有效。在当今世界，如果你给客户发一份演示文稿，说“我们将在10年内让你的投资翻6倍”，他们会说“不，市场是有效的，你不可能承诺如此高的超额收益”。但如果你给客户发一份演示文稿，说“我们将在10年内为你带来合理的超额收益，但同时也会产生相当于你投资额6倍的税收损失”，他们会说“啊，很好，你们……”

doing your job efficiently.”

Commodity market manipulation

Earlier this year, Kalshi had some betting markets about who would attend the

> **译文：** 今年早些时候，Kalshi 开出了一些关于谁会参加的博彩市场。

State of the Union address. One market was on George Santos, the former congressman, who naturally (1) traded the contract and (2) posted on X to manipulate its price:

> **译文：** 国情咨文。其中一个市场关注的是前国会议员乔治·桑托斯，他自然而然地（1）交易了该合约，并且（2）在X网站上发帖操纵其价格：

Santos made a series of social media posts regarding his plans to attend the

> **译文：** 桑托斯在社交媒体上发布了一系列帖子，表达了他参加活动的计划。

State of the Union. Shortly after these posts, the price of the SOTU event contract rose or dropped. For example, while holding a Yes position on his attendance, Santos posted on the X social media platform about what he should wear to the State of the Union. Within hours of the post, the price of the Yes position rose, after which Santos exited at a profit. ...

> **译文：** 国情咨文。这些帖子发布后不久，国情咨文合约的价格就出现了波动。例如，桑托斯在持有“出席国情咨文”合约时，曾在社交媒体平台上发帖讨论他应该穿什么出席。帖子发布后几个小时内，“出席”合约的价格就上涨了，之后桑托斯获利了结。

The next day, Santos posted a video on X stating he would be attending the event. After this video, the contract price for his attendance rose. Later that same day, Santos began building a No position regarding his attendance. … On the day of the State of the Union, Santos posted that he was stuck at the airport and would miss the event. The price of the Yes position fell,

> **译文：** 第二天，桑托斯在X平台上发布了一段视频，表示他将出席此次活动。视频发布后，他出席的合约价格上涨。当天晚些时候，桑托斯开始构建关于他是否出席的“否”仓位。……在国情咨文发表当天，桑托斯发帖称他被困在机场，将错过此次活动。他出席的“是”仓位价格下跌。

conversely making the value of the No position increase in value. At this point, both his plane and train tickets had been cancelled, and he had not purchased any alternative travel options. In the early hours of February 25th,

> **译文：** 反过来，这使得“否”立场的价值增加。此时，他的机票和火车票都已被取消，而且他也没有购买任何替代的旅行方案。2月25日凌晨，

Santos exited his No position, making a profit of $14,390.57.

> **译文：** 桑托斯平掉了他的 No 仓位，获利 14,390.57 美元。

That is from last week’s US Commodity Futures Trading Commission settlement with Santos , in which he agreed to disgorge

> **译文：** 这是上周美国商品期货交易委员会与桑托斯达成的和解协议中的内容，根据该协议，桑托斯同意退还非法所得。

$17,569.98 of profits and pay a $17,500 fine. Obviously this is all incredibly stupid. When wetalked about this in June , I wrote:

> **译文：** 17,569.98 美元的利润，还要缴纳 17,500 美元的罚款。这显然是极其愚蠢的。六月份我们讨论这件事的时候，我写道：

Every headline about this says

“insider trading

,” but I don’t think this is insider trading? Santos had no obligation of confidentiality to anyone to keep his State of the Union plans confidential; therefore he was free to trade on them. …

> **译文：** 但我认为这不算内幕交易吧？桑托斯没有义务对任何人保密他的国情咨文计划；因此，他可以自由地就此进行交易。

I do think that announcing that you’re going to the State of the Union to push up the “Yes” price, buying “No” contracts and then not showing up seems like a pretty textbook case ofmarket manipulation.

> **译文：** 我认为，宣布要去参加国情咨文演讲以推高“赞成”价格，购买“反对”合约，然后不露面，这看起来是一个非常典型的市场操纵案例。

And in fact the CFTC came after him for market manipulation, not insider trading:

> **译文：** 事实上，美国商品期货交易委员会（CFTC）对他提起诉讼的原因是操纵市场，而不是内幕交易：

Santos violated Section 6(c)(1) and Regulation 180.1(a) when he traded in an event contract where he could influence the outcome of the underlying event and engaged in activity designed to affect the price of the swap. Santos made misleading public statements and omissions about his activities in relation to the underlying event to influence the contract price for the benefit of his

> **译文：** 桑托斯违反了《证券交易法》第6(c)(1)条和第180.1(a)条规定，因为他交易了一份事件合约，该合约允许他影响标的事件的结果，并且他从事了旨在影响互换合约价格的活动。桑托斯就其与标的事件相关的活动发表了误导性公开声明和隐瞒事实，以影响合约价格，从而使其受益。

trading position.

If he just bet against himself, without posting about it, it might have been fine? Not legal advice.

> **译文：** 如果他只是跟自己打赌输赢，而且不发帖炫耀，也许就没事了？这可不是法律建议。

FBI crypto theft

There are so many very poor decisions that one could make related to cryptocurrency wallets, but I suppose one of them is … stealing $1 million of crypto from North Korean hackers (?) while working for the FBI? Orwhatever this is :

> **译文：** 关于加密货币钱包，人们可能会做出很多糟糕的决定，但我想其中之一就是……在为FBI工作期间从朝鲜黑客手中窃取价值100万美元的加密货币？或者诸如此类的事情：

An FBI agent has allegedly turned himself in for stealing about $1 million in cryptocurrency from foreigners the agency was investigating.

> **译文：** 据称，一名联邦调查局特工因盗窃该机构正在调查的外国人的约 100 万美元加密货币而自首。

Patrick Steven Yaroch contacted the Department of Justice last week to confess to making “very poor decisions related to cryptocurrency wallets,” according to a Federal Bureau of Investigation affidavit filed with a district court in

> **译文：** 根据联邦调查局向地区法院提交的宣誓书，帕特里克·史蒂文·亚罗奇上周联系了司法部，承认自己在加密货币钱包方面做出了“非常糟糕的决定”。

Virginia.

Yaroch used FBI systems to access the keys needed to transfer funds from cryptocurrency accounts associated with an “adversarial nation” to himself, the document released Monday says. Starting in late 2024 or early 2025, he conducted about 10 transfers totaling around $1 million, it says.

> **译文：** 周一公布的文件显示，亚罗奇利用联邦调查局的系统获取了将资金从与“敌对国家”相关的加密货币账户转移到自己账户所需的密钥。文件称，从2024年末或2025年初开始，他进行了大约10笔转账，总额约为100万美元。

Terrific. Was turning himself in also a very poor decision related to cryptocurrency wallets? Who can say, buthere was his earlier plan

> **译文：** 太棒了。自首是不是也跟加密货币钱包有关，是个非常糟糕的决定？谁也说不准，但这可是他之前的计划。

:

The authorities said in court papers that a search of the agent’s internet activity showed that in May, he had asked ChatGPT to recommend how to invest a million dollars with “a goal of potentially retiring around 40, and a clear interest in eventually building a slower-living vineyard/agricultural lifestyle in places like Cilento or Portugal’s Dao region.”

> **译文：** 当局在法庭文件中表示，对该代理人互联网活动的搜索显示，他在 5 月份曾要求 ChatGPT 推荐如何投资 100 万美元，“目标是在 40 岁左右退休，并明确表示有兴趣最终在 Cilento 或葡萄牙的 Dao 地区等地建立一种慢节奏的葡萄园/农业生活方式。”

I was joking/guessing about North Korea, but this really is a good thriller plot.

> **译文：** 我之前只是开玩笑/猜测朝鲜，但这确实是一个很棒的惊悚片情节。

Dentists!

Sure :

A growing number of investors from the US to South Korea are using leveraged exchange-traded funds for long-term investing, a far cry from the day trading they were designed for. …

> **译文：** 从美国到韩国，越来越多的投资者开始使用杠杆式交易所交易基金（ETF）进行长期投资，这与ETF最初设计用于日内交易的用途截然不同。

In South Korea, the epicenter of the leveraged-ETF trend, former dentist Song

> **译文：** 在杠杆ETF趋势的中心韩国，前牙医宋

Wonjun says the products helped him retire at 44 after turning them into the centerpiece of a long-term investing strategy he now teaches to hundreds of thousands of online followers.

> **译文：** 元俊表示，这些产品帮助他在 44 岁退休，因为它们成为了他长期投资策略的核心，他现在将这种策略传授给成千上万的在线粉丝。

If your financial adviser is going around online touting long-term investments in leveraged ETFs, that seems bad. If your dentist is doing it, yeah, that seems right.

> **译文：** 如果你的理财顾问在网上到处兜售杠杆ETF的长期投资，那可就糟了。但如果是你的牙医这么做，嗯，那倒也挺合适的。

Things happen

Inside Google’s $200bn Wall Street finance machine for Anthropic. AI Power Demands Spur Builders to Seek Billions inBank Pledges

> **译文：** 揭秘谷歌斥资2000亿美元在华尔街为Anthropico融资的内幕。人工智能电力需求促使开发商寻求数十亿美元的银行贷款承诺。

. Anthropic Inks $10 Billion Computing Deal

With New Cloud Startup. China’s AI Blitz Creates ‘

Death Zone ’ for Rival US Model Makers. The AI Boom

> **译文：** 美国模型制造商的“死亡地带”。人工智能热潮

Is Transforming the American Economy Beyond

Recognition. Millennium Lost 2% Last Month as AI Trade

> **译文：** 认可。千禧年上月因人工智能交易而下跌2%。

Whipsawed Hedge Funds. Wells Fargo to Roll Out

Tokenized Deposits for Corporate Clients. Jet Fuel

Made From Tropical Fruit Gets $3 Billion Backing.

JPMorgan Chase to Invest $750 Billion to Boost U.S. Housing Supply,Homeownership

> **译文：** 摩根大通将投资7500亿美元以促进美国住房供应和房屋拥有率

. easyJet Extends

Castlelake’s Deadline to Top Apollo’s $7.6 Billion Bid. Deutsche Bank,

> **译文：** Castlelake必须在最后期限前超越Apollo 76亿美元的收购报价。德意志银行

JPMorgan, BofA Enabled Epstein , Wyden Report Says.

> **译文：** 怀登报告称，摩根大通和美国银行助长了爱泼斯坦的犯罪活动。

Revolut chief Nik Storonskysued by broker over

€350mn superyacht. ‘Cursed island’: the $100bn luxury development hostingtech nomads and scammers . Private Colleges Admit More

> **译文：** 价值3.5亿欧元的超级游艇。“诅咒之岛”：价值1000亿美元的豪华开发项目，为科技游牧民和骗子提供庇护。私立大学招生人数增加

Students Who Didn’t Apply . “Mets win ETF

: A new way to lose money.”

If you'd like to get Money Stuff in handy email form, right in your inbox, pleasesubscribe at this link . Or you can subscribe to Money Stuff and other great Bloomberg newslettershere

> **译文：** 如果您想通过电子邮件便捷地接收“理财资讯”，请点击此链接订阅。您也可以点击此处订阅“理财资讯”和其他精彩的彭博新闻简报。

. Thanks!

[1] Or two days in which it is limit down. Shen: “Even though the South Korea market has a 30% daily price limit and circuit breakers in place, a sharp multi-day move can still hit hard because crash puts calculate on an official close-to-close basis — so if a stock hits limit down and stays halted until market close, the move gets priced into the next session.”

> **译文：** [1] 或者连续两天触及跌停板。沈：“即使韩国股市设有每日30%的涨跌幅限制和熔断机制，连续多日的剧烈波动仍然会造成严重冲击，因为崩盘看跌期权是按官方收盘价计算的——所以如果一只股票触及跌停板并停牌至收盘，那么这波波动就会反映在下一个交易日的价格中。”

[2] Two roughly equivalent ways to do this are: (1) actually lending the hedge fund $80, non-recourse, to pay for a $100 note or (2) making it a $20 structured note where the embedded option is a (cliquet) put spread rather than a put. In the second case the hedge fund is explicitly at risk for, like, “down

> **译文：** [2] 有两种大致等效的方法可以实现这一点：(1) 实际借给对冲基金 80 美元（无追索权），用于支付 100 美元的票据；(2) 将其制成 20 美元的结构化票据，其中嵌入的期权是（cliquet）看跌价差，而不是看跌期权。在第二种情况下，对冲基金明确承担风险，例如“下跌”。

50% to down 60%,” while the bank explicitly takes the down-60%-or-more risk.

> **译文：** 下跌 50% 至 60%”，而银行则明确承担下跌 60% 或更多的风险。

[3] I mean really the price of the put spread is less than the price of the naked put, but you get the idea.

> **译文：** [3] 我的意思是，实际上看跌期权价差的价格低于裸看跌期权的价格，但你应该明白我的意思。

[4] I am being cutesy and of course in important ways this is zero-sum too, but in a broader sense. If “finance” can generate zero taxes for its customers, then that should raise the tax burden (or lower services, etc.) for non-consumers of “finance.”

> **译文：** [4] 我这是在开玩笑，当然，从某种重要意义上讲，这也是零和博弈，但从更广义的角度来看。如果“金融”能够为其客户创造零税收，那么就应该增加非“金融”消费者的税收负担（或降低服务水平等）。

[5] Ideally the long stocks should be better than the short ones, because then your tax-aware long-short strategy will beat the market even before the tax savings. This is good because (1) it is always better tomake more money than less money and also (2) for tax reasons, you want to be able to demonstrate pre-tax alpha : If you’re

> **译文：** [5] 理想情况下，做多股票应该优于做空股票，因为这样一来，即使在享受税收优惠之前，你的节税型多空策略也能跑赢市场。这很好，因为（1）赚的钱越多越好，（2）出于税务方面的考虑，你需要能够证明税前超额收益（alpha）：如果你

doing this trade *only* to generate tax losses you might get in trouble. On the other hand, most customers of long-short tax-aware products want the shorts to be good hedges for the longs, andnot just a single risky levered bet on AI or whatever . So you might want broadly similar factor exposures in the long and short portfolios, etc.

> **译文：** 如果仅仅为了产生税务亏损而进行此类交易，可能会惹上麻烦。另一方面，大多数多空策略的客户都希望空头头寸能够有效地对冲多头头寸的风险，而不是仅仅押注于人工智能或其他领域，进行高风险的杠杆投资。因此，你可能希望多头和空头投资组合的因子敞口大致相似等等。

[6] And vice versa with your shorts.

Follow Us

Get the newsletter

Like getting this newsletter? Subscribe to Bloomberg.com

> **译文：** 喜欢这份新闻简报吗？订阅彭博社网站吧！

for unlimited access to trusted, data-driven journalism and subscriber-only insights.

> **译文：** 无限畅享值得信赖、数据驱动的新闻报道和仅限订阅用户才能获取的独家资讯。

Before it’s here, it’s on the Bloomberg Terminal. Find out more about how the

> **译文：** 在它正式发布之前，彭博终端上就已经有了。了解更多相关信息……

Terminal delivers information and analysis that financial professionals can’t find anywhere else.Learn more

> **译文：** 该终端提供金融专业人士在其他任何地方都无法获取的信息和分析。了解更多

.

Want to sponsor this newsletter? Get in touch here

.
