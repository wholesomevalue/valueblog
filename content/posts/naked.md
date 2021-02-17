# Selling Shorts Naked - AKA Naked Short Selling

*TL;DR* A deep dive into The DTCC Settlement & Clearing Process; why it is a joke - allowing shady operatives to use illegal Naked Short Selling to bully, defecate and prey on smallcap companies without ANY consequence - and [how to throw it back at them](#guerrilla-warfare)

{{< rawhtml >}}<span style="background-color: red; color: white; padding: 0.3em; font-weight: bold;">NOTE</span>{{< /rawhtml >}} This post was written after alot of research and digging around. It contains mostly facts (e.g. what illegal Naked Short Selling is, how the DTC/NCSS clearing & settlement of securities works, and why it doesn't work - allowing illegal naked short selling), and some relatable fiction for entertainment purposes only. Therefore, before going any further, you should [read the disclaimer](#disclaimer) first.  

Are you laughing? If not I know you havn't read the [disclaimer](#disclaimer). If so, please continue...  

I think you came here to learn why someone would sell their shorts naked. I can explain, not because I do so, but because I read a bunch of [papers and articles](#references), which helped me understand the situation alot better.  

After receiving englightenment, I was able to recreate a [*99.99% accurate* reenactment of the events](#reenactment) that led to the greatest Short Squeeze (that could have been / yet to happen) in history (the cast includes SugarDaddy, his boy RobinYou, sugar babies Melvin, Shittron and their dog CNBC).

I hope to make you laugh, but more importantly also to enlighten you, so please read the entire thing - you won't be disappointed. 

However, if you're busy, or autistic but brilliant, and just want the bullet points, here it is:

## Bullet Points

- Naked Short Selling (`NSS`) = creating shares out of thin air
- It can be useful for [making markets](#makingmarket), but also be abused (e.g. the current GameStop saga)
- Basically only [Market Makers (MMs)](#two-types-of-market-makers) - [prime brokerages](https://en.wikipedia.org/wiki/Prime_brokerage) ie. elites such as JP Morgan, _Point72_, _Citadel_ etc - are able to execute Naked Short Selling (_NOTE_: I'm using the terms "Market Makers" and "Broker-Dealers" interchangeably, the distinction isn't really important here)
- The DTCC (whose system is at the end of [infinite stupdity](#dtcc)), is being gamed by these MMs due to:
  - The lack of public information & transparency + infrequent & dumbed down reporting
  - Unwillingness of participants to invoke [Buy-Ins](#elusive-buy-ins) to force delivery of FTDs
  - The [Stock Borrowing Programme](#failed-to-receives-ftrs) artificially reducing [FTRs](#failed-to-receives-ftrs) at _0% interest_,
  - Which allows [FTDs](#failed-to-delivers-ftds) to remain in perpetuity without consequence (neither financial nor regulartory)
  - Not to mention allowing antique [Ex-Clearing](#ex-clearing) to occur
  - And finally, the _Lack of oversight_ by the SEC
- MMs who are meant to be staying neutral, making markets and maintaining liquidity, instead use their special market making previleges to play risqué  games with their shorts down - using Naked Short Selling to take on risky single sided positions for predatory means
- E.g.  if you've made mistakes before (think {{< rawhtml >}}<a href="https://en.wikipedia.org/wiki/Steve_Cohen_(businessman)#Racketeering_and_insider_trading_charges" target="_blank" class="ext">$1B fine for insider trading</a>{{</ rawhtml >}}) and owns one of the larger prime brokers around, why wouldn't you (at least consider) exploit it for your / your friend's benefit? - the formula is fairly easy: step (1). _NSS the stock to obvlivion_, step (2). _rinse & repeat NSS, wait till stock = $0_, culminating in step (3): _no stock to return - easy peasy lemon squeezy_? - except they encountered a [cat](https://www.youtube.com/channel/UC0patpmwYbhcEUap0bTX3JQ) called [DFV](https://www.reddit.com/user/DeepFuckingValue/) and bunch of die-hard 'retarded degenerates' from [WSB](https://www.reddit.com/r/wallstreetbets/)  
- Finally, I propose that the short squeeze hasn't happened yet, because the MM(s) are still holding onto the bags (of FTDs) without much cost/consequences (so far)
- However, what the MMs have been (wrongfully) discounting is how strongly willed some of these GME investors are at holding the stock till they die
- So sooner rather than later, the game will stop, with a liquidity crunch coming after them faster than they could ever hope to cover - they'll have no choice but to make deals or get annihilated (taking others down with them as collateral damage)
- How? I present the {{< rawhtml >}}<span class="red-hl" style="padding:0.5em;"><a href="#guerrilla-warfare">GME Guerrilla Warfare Operations Manual</a></span>{{</ rawhtml >}} that walks you through each of the _3 steps_, understanding the _why_, _what_ and _how_ the war will be won.
- Is this ^ financial terrorism? nope, its called financial _counter-terrorism_


{{< rawhtml >}} <h1 style="color: red"><span style="color:white; background-color: red; padding: 0.3em; line-height: 2.5em;">The Big Picture</span><br/>The system is BROKEN, and the Short Squeeze hasn't even started yet (or may never happen)</h1> {{< /rawhtml >}}

Alright, here goes the longer version:  

## Two types of Market Makers

Normal short selling - refresher - is when you borrow a share from your friend who owns it (the broker), and sell it to someone else. You then wait a while, buy the share back to return to your friend (broker). all is well if the price went down and conversely all is bad if the price went up - YOU win or lose.

The key thing to note about (normal) short selling, is that _no shares are created_ - its only borrowed and eventually returned. The share that was borrowed from the broker is a real share issued by the underlying company (e.g. with its initial public offering) 

`Naked Short Selling` - AKA Selling Shorts Naked, on the other hand, is a much more extreme version of selling - The person who coined the term _Naked_ short selling must have had some very deep intiuitions about what it is...

![](/img/expose.jpg)

First of all, you and I can't sell shorts naked - I can't simply tell my broker, nor would my broker believe me, that I have [70M shares of GameStop (GME) stock to sell](#ortex_gme_si). The conversation would go something like this:

`ME` (15th Oct 2019): hey bro, I have 70M of GME stock I want you to sell for me  

`IBKR (Interactive Brokers)`: You do? congratulations, hold on one sec, let me do some DD (due dilligence), 

`IBKR`: Sorry, [reddit](https://www.reddit.com/r/wallstreetbets/comments/kz7ygv/gme_dd_one_dd_to_rule_them_one_dd_to_find_them/) says there is only 46M shares floating {{< rawhtml >}}<sup><a href="#outstanding_floating">3 - outstanding vs floating</a></sup>{{</ rawhtml >}} around, of which we know that [Ryan Cohen](https://www.newsweek.com/who-ryan-cohen-gamestop-investor-3-billion-overnight-1565095) of Chewy fame, who also happens to be on the board of GME, [owns 13%](https://www.cnbc.com/2021/01/27/gamestops-surge-has-made-its-3-largest-shareholders-billions-overnight.html#:~:text=The%20chief%20beneficiary%20of%20the,owns%2013%25%20stake%20in%20GameStop.&text=GameStop%20CEO%20George%20Sherman%20has,value%20of%20about%20%24350%20million). Therefore you can't possibly have [150%](#ortex_gme_si) of the floating shares in the company! if that was the case, you would have more shares than there are shares outstanding (69M) of the company!  

`ME` (15th Jan 2020) : Would you believe I have 30M ?  

`IBKR`: Let me check with reddit again, nope, sorry still not possible, either you identify your self as a prime broker (e.g. Steven Cohen, or Kenny G), or we have to end this call now.  

[End of phone call]

Identify as Steven Cohen or Kenny G? Thats right, you need to be a prime broker, ie. any one of the [participants in DTCC](https://www.dtcc.com/client-center/dtc-directories), in order to bullshit about how much shares you have in a company.

These elites are called `Market Makers` (`MM`s) because they are meant to make (create) a market when there isn't one (think spread between bid and ask being too large), and <u>ONLY MMs are allowed to go naked and sell shorts</u> (we simply can't trust anyone else to do so, and must make this process as opaque as possible in order to be 'transparent').  

There are 2 types of MMs:  

### Type 1: George Constanza (Mostly PBTR, Risk Adverse)

PBTR = play by the rules  

{{< rawhtml >}}<a name="makingmarket"></a>{{< /rawhtml >}}
So imagine a hypothetical situation, in which the difference (the [spread](https://www.investopedia.com/spread-4184182)) between the bids and asks for GameStop were so wide that no body wanted to buy nor sell

```
 BID                ASK
       1000.00 3000000     <- What WSB is selling the shares at
          ....
          4.20 
          4.10
1000000   4.00             <- The price at which Ryan Cohen purchased at
          0.01             <- What GME board (before Ryan came in) believed the value is at
          0.00             <- Where Melvin wants the price to be

```

In this situation, the market is dead - no one is trading - so we can't allow that, because if that was the case, e.g. how could brokers make any commission? So [Market Makers](https://www.investopedia.com/terms/m/marketmaker.asp) will come in and use their special powers to facilitate / get trades going between buyers and sellers, by taking both sides (`NOTE`: keypoint here is taking *BOTH* sides)

So the MM would, e.g. sell 5 shares it doesn't own, at the bid price, then buy 5 shares at the ask price, to hopefully kick things off...  

```
 BID                ASK
 [5]MM 1000.00 3000000     <- also, MM takes the opposite side of the short trade, by buying 5 shares @ $1000.00. This is to hedge the risk of the 5 (synthetic) shares sold @ $4.00
          ....
          4.20 
          4.10
1000000   4.00 [5] MM      <- first the MM will sell 5 shares here to the bidder, note MM doesn't have any shares (i.e. the share is synthetic)
          0.01                     
          0.00                     

```

What the MM did (in the case of selling the 5 shares of GME at bid price, which it doesn't own yet because it hasn't bought the 5 shares of GME at ask price), is `execute a naked short sell (NSS)`. This is perfectly normal (not the the guy with the coat open, but the MM making the market), and often needed in the name of making markets

Note that the MM in the example also acquired 5 shares of GME, so the MM has a balanced book, i.e. the net effect is the MM has 0 shares of GME, effectively meaning it hasn't created 5 shares of GME out of thin air.  

In practice, of course, the MM may not have a balanced book during the day, but by the end of the day, the risk adverse MM needs to put pants back on (i.e. get to neutral) because they don't want anyone to see them like this:

![](/img/shrink.png)

Anyways, back to the narrative that MMs are 'altruistic', which they're not, and only want to fuck *ahem*, help the market trade by adding liquidity... So MMs are *NOT* altruistic? yep they are not - its called capitalism - they're in it for the money, which is fair enough - you take the risk to allow the market to trade - you should be compensated for it. The type of MM we just talked about (taking both sides of the trade, making markets, staying neutral, and making $dough by playing the spread game) have small balls - they're very risk adverse - think _George Costanza_ (well meaning to an extent, but mostly selfish and hyperactive)

There exists another type of MM that both loves risk, wants more money, and likes to prey on...  

### Type 2: Theodore Edgar McCarrick (Predatory, Abusive, and  Risk Loving)

![](/img/pedo.jpg)

This type of MM just don't give a shit about risk (they're too big to fail), and don't think their trillion dollar fortune is large enough, and so don't just want to play the [spread game](https://www.youtube.com/watch?v=-zTHKcJEGe8) to earn a decent living - they abuse, groom and play dirty...

Now the risk with selling shorts while naked is that your junk is exposed, actually its not really (due to the way the DTCC/NCSS `Continuous Net Settlement (CNS)` system works, which I'll get into [later](#dtcc)), but you are exposed:

The exposure is VERY REAL if, instead of taking both sides, you (the abusive MM) only takes one side (in relevance to what we're discussing here - taking the short side only).  

The exposure is that you eventually have to deliver the *REAL* share to the person you sold it to, if you don't then it just becomes a joke right? I mean [nothing like this has ever happened!](https://www.amazon.com.au/I-U-John-Lanchester/dp/1439169861) (I havn't read the book btw, I just like the cover):  

![](/img/iou.jpg)

So in order to deliver the *REAL* share to the buyer (you don't have it because you, the abusive MM is still naked), you have to buy it - *AT ANY COST* - on the market <- big risk if you ask me.

{{< rawhtml >}}<h1 style="padding: 0.2em"><span style="color: white; background-color:red; padding: 0.3em">Important Point #1</span> Big Risk - Buy AT ANY COST</h1><br/>{{< /rawhtml >}}  
  
## Reenactment

Lets watch an reenactment of a recent event, to illustrate how Predatory Naked Short Selling works:

_The following reenactment is for entertainment purposes only, the characters described within are not real, for example, Melvin is the incestual brother of Elmer J. Fudd, CNBC is the name of my black english staffy, who shits 3 times a day, RobinYou is a young priest, and SugarDaddy is a pedophile that lives in the higher echalons of the church of market makers. The church is called the DTCC_

{{< rawhtml >}}<h1><span style="color:white; background-color: red; padding: 0.3em;">Reenactment</span> (99.99% accurate)</h1><a href="#disclaimer">Disclaimer</a><br/>{{< /rawhtml >}}
  
### _Feb 15, 2019_ - Sexting transcript between Melvin and Sugardaddy

`Melvin`: Hey pappa, we have a bit of a problem here, this guy called [Andrew Left](https://en.wikipedia.org/wiki/Andrew_Left), from some wanna be Hedge Fund called "ShitTron" or something, is copying our trade, with him and all his extended family of idiots copying our TOP SECRET trade on GME. They've now bought the remaing shares we could have used. I think we need to work some magic. I know what I'll have to do (love emoji, xxx,), I hope to see you at 10? K...  

Btw, [checkout this opinion piece by Bloomberge LMFAO](https://www.bloomberg.com/opinion/articles/2021-01-29/gamestop-gme-trading-short-sellers-like-citron-aren-t-the-enemy) - yep, [Lefty](https://en.wikipedia.org/wiki/Andrew_Left#Citron's_reports_on_Chinese_companies) is one of the good guys because he shits on China... LMFAO

[Dick pics omitted]

{{< rawhtml >}}
<div class="explainer">
<b>Explainer</b>
<p>1. The "magic" refered to here is creating a "small" (e.g. 150% of float) amount of shares through Naked Short Selling (using SugarDaddy's special MM privileges), for Melvin to use to short GME to the ground. While Melvin shorts GME to obvlivion, they need to find people 'dumb' enough to take the other side (i.e. buy GME), so they ask <b>RobinYou</b>'s help...</p>
<p>2. RobinYou have a massive following of retail retards who buys everything RobinYou tells them to, on margin, which is just perfect, because these margin accounts easily blows up, adding downward pressure to lower the price of GME</p>
<p>3. How Hedge Funds (HFs) work:<br/><b>Due Dilligence (DD)</b> = "Whats the big boys (e.g. Melvin) doing? Lets copy them".<br/><b>Playbook</b> = "Throw some bullshit news against the company (e.g. company is fraud), with history lesson about Enron, throw some bones at dogs like CNBC; borrow from SugarDaddy; rinse & repeat until company bankrupt. Profit + collect commission; (then buy hookers and cocaine)"<br/><b>Risk Management</b> = "WTF is that?"</p> 
</div>
{{< /rawhtml >}}

`SugarDaddy`: You'll have to work very hard for this one *wink* *wink*, ok see you at 10. Come to my office and be discete. Btw, you also need make our young priest `RobinYou` happy...

_[ GME price goes further south... but people who actually did DD, and have real conviction (e.g. [1](https://www.reddit.com/user/DeepFuckingValue/), [2](https://twitter.com/ryancohen?lang=en), [3](https://twitter.com/RodAlzmann)) hold on tight ]_

### _Jan 11, 2020_ - Sexting transcript Melvin and Sugardaddy

`Melvin`: Alright, more problems, this time theres a guy called `Ryan Cohen` who just joined GME's board, is he related to you?  

`SugarDaddy`: No, but see you at 10, same place, same shit (*wink* xxx) 

[Pegging pics ommitted]

_[ More and more WSB Retards find out about the position ]_

### _Jan 22, 2021_ - Transcript of phone call Melvin and Sugardaddy

`Melvin`: More?  

`SugarDaddy`: Sure  

_[ Shit explodes ]_

{{< rawhtml >}}
<div class="explainer">
<b>Explainer</b>: The game is to completely <b>KILL off GME</b>, because everything is on the line
<p>Why? Because SugarDaddy created shares of GME out of thin air (illegal because its not "bona-fide market making"), and need to eventually deliver it. If GME = $0, whats there to deliver? Also profit + no capital gains tax (i think, disclaimer: not a tax agent)</p>
<p>SugarDaddy gets really dirty and opens up  bag of tricks including but not limited to:</p>
<p><b>1</b>. Short Ladder Attacks</p>
<p><b>2</b>. Misinformation through CNBC</p>
<p><b>3</b>. Run bots against r/wallstreetbets</p>
<p><b>4</b>. [Pay for Yellen to talk](https://slate.com/news-and-politics/2021/01/janet-yellen-paid-speeches-citadel-gamestop.html)</p>
<p><b>5</b>. Too much to list</p>
</div>
{{< /rawhtml >}}
…

### _Jan 27, 2021_ - Transcript of public announcements etc

`Melvin` to the public: We think you guys are stupid, therefore, we announce that we have exited the trade, taken a big hit. Calm down will ya, simply just trying to survive, making some money to feed my family, geez...  

_[ The whole world finds out about the position ]_

`WSB` retards: Nah, Melvin no exit, Citadel and Point72 simply bought the short positions, called it a 'cash injection', so that Melvin can say they 'lost', we're not as retarded as you think.  

`CNBC (dog)`: these `WSB` guys are so stupid, of course Melvin is out, because they told us so... and we're smart, you guys don't know anything... 

`WSB` retards: "We don't like CNBC", in the most PG language ever

### _Jan 28, 2021 (WSB Day)_, Transcript of phone call between SugarDaddy and DTCC

`SugarDaddy`: hey DTCC, just wanted to let you know that somebody created a humongous short position on GME, not me, but somebody. If you don't raise your collateral requirements, then the entire stock market will be history. Get it?  

`DTCC`: sure we will [raise the collateral](https://blog.robinhood.com/news/2021/1/29/what-happened-this-week) by 5000%. Btw, you know about our [Stock Borrow Programme](https://www.researchgate.net/publication/228260887_Naked_Short_Sales_and_Fails_to_Deliver_An_Overview_of_Clearing_and_Settlement_Procedures_for_Stock_Trades_in_the_US) (which [everyone thinks is awesome](https://www.sec.gov/rules/proposed/s72404/s72404-14.pdf)) right? You can borrow whatever how much you need (of GME or anything), {{< rawhtml >}}<span style="background-color:red; color:white; font-weight: bold; padding: 0.5em;">AT 0% INTEREST</span>{{< /rawhtml >}} to cover your tracks. and after 3 days or something, Just "roll" your [FTDs](https://www.sec.gov/data/foiadocsfailsdatahtm) over to the idiot broker who's naked, anyways you know the drill, you've done it before... Also remind your boy to spin it like its a clearing/settlement problem...

_[ All brockerages shut buying of GME, int the hope of locating *REAL* shares to reduce the number of synthetic shares ]_

### _Jan 28, 2021 (WSB Day)_, Brokers to the world

`RobinYou / Brokers`: Dear retail traders, we're doing this for you, to protect _you_ from harm...  

`The world`: Fuck you, we're not dumb, if this is not collusion, then what the fuck is?  

Meanwhile, on twitter, our friend [Steven Cohen](https://en.wikipedia.org/wiki/Steve_Cohen_(businessman)#Racketeering_and_insider_trading_charges), who is [*totally unrelated to Melvin*](https://www.prnewswire.com/news-releases/melvin-announces-2-75-billion-investment-from-citadel-and-point72--301214477.html#:~:text=%22I%20am%20incredibly%20proud%20to,these%20two%20great%20investment%20icons.%22) says:  

![](/img/steven.jpg)

I think he is telling Melvin (stock jocks?) to bring the *REAL* shares back to the rightful owners. He is a good guy yep.  

{{< rawhtml >}} <h1 style="padding: 0.3em;"><span style="color: white; background-color: red; padding: 0.3em;">Important Point #2</span> Someone is still exposed</h1>{{< / rawhtml >}}

Someone created a alot of fake shares of GME, and tried to drive the company to the ground in order to hide the act. The deed is done, the company is still around, and so somebody is still very much exposed.

Lets continue our journey into _infinite stupidity_...

## Why is My Junk Not Exposed (Not because I don't have one)

(explainer: not my junk)

So by now you should understand what my hypothesis is:  

{{< rawhtml >}}
<div style="padding: 1em; background-color: #f0f0f0;">
Someone (or group of people), and by someone I mean a prime broker/mm, created alot of fake shares of GameStop using Naked Short Selling,  attempted to bury the evidence by bankrupting GME - after which no one would care / ask.
</div>
{{< /rawhtml >}}

Still not convinced? Ask yourself: _why was the Short Volume @ 150% of GME's float???_  

You might say, well its not anymore, because now, the short interest as a percentage of the float is down to something like 38%...  

But, do you know what a [FTD (Fail-to-Deliver)](#ftd) is? Do you think the FTD count is/should be added to the numerator of the SI% formula (short volume / float)? i.e. for the various SI% reported publicly (I think they all differ a bit), do they take FTD into account?

Some data aggregators now reports SI% to be only 38%, but if the FTD was e.g. 50M, and if we also take FTD into account, then what does that make the SI%? 150%??? 200%??? 300%???

Anyways, the point is - don't use short interest alone to evaluate the situation, try and understand how things work underneath:  
{{< rawhtml >}}<a name="dtcc"></a>{{< /rawhtml >}}

## The Dark Side of the `DTCC` Settlements and Clearing Process

All on board the train to _infinite stupidity_, aka the DTCC...

Please watch this introductory video first:

{{< rawhtml >}}
<iframe width="560" height="315" src="https://www.youtube.com/embed/I0WXg5T3cBE" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
{{</ rawhtml >}}
  

Now continue reading to understand in detail the stupidity:  

### Clearing & Settlement - Happy Days

This is the Happy days scenario, where SugarDaddy, Melvin and Shittron & Co isn't around and it goes like this:  

![](/img/dtcc_normal.png)

- Assume `GME's float is 4 shares` (3 held in the "Pool of lendable shares", and 1 held by the Cash Account Seller)
- `Short seller` and `Seller (with cash account)`, both clients of `Broker A`, instructs Broker A to sell 2x GME shares in aggregate.
- The responsible broker then tries to `locate` 1x GME share (because the Short Seller doesn't own any) from the pool of lendable GME shares.
- This pool is created from shares of [hypothecable](#hypo) (i.e. margin accounts), institutional lending programs (i.e. institutional investors who are LONG GME, holding unencumbered? shares) and other brokers.
- Note the 2 located shares are marked {{< rawhtml >}}<span style="color:red">red</span>{{< /rawhtml >}}, to denote they are being sold, to be delivered to the counterparty during settlement.
- Broker A sends sell instructions to the `Stock Exchange`
- `Broker B` who is also under instruction from its `Cash Investor`, sends instruction to buy 2 x share of GME for $500 to the exchange
- Stock Exchange records the trade happening, and at the end of day (EOD), sends the trade information to NSCC (a [subsidiary of DTCC](https://www.dtcc.com/about/businesses-and-subsidiaries/nscc))
- `NSCC` does the job of clearing by placing itself as the central counter party to ALL trades.
- So in this case, the NSCC is both the buyer of 2x shares of GME from Broker A, and also the seller of 2x shares of GME to Broker B
- NSCC produces net positions (what stock a participant owes NSCC, and what stock NSCC owes a particpant) for each participant / stock
- In this simple case, there will be 2 positions: `Broker A: -2 GME`, `Broker B: +2 GME`
- This net position is passed onto `DTC` as instructions to effect settlement
- The DTC would record -2 GME from Broker A's stock account, and +2 GME to Broker B's stock account
- Settling Banks are then sent instructions accordingly (for Broker A, +$1000, and for Broker B, -$1000)
- Notice the FTD/FTR register is empty - nice and simple...

_Note that in practice a small amount of FTD/FTRs is common, due to various reasons such as physical certificates, human error etc_

### Clearing & Settlement - Sad Days

When SugarDaddy and Melvin enters the arena, things gets complicated:  

![](/img/dtcc_sugar.png)

- Before digging into FTD this and FTR that, lets pause for a moment, and consider the float...
- It might seem like there is now 5 shares of GME floating around! - Did the process of the normal short selling create 1 share out of thin air?
- The Answer is _NO_, the float is still _4_, as explained below:
  - The Original Owner (`OO`) of the the share sold short (now {{< rawhtml >}}<span style="color: lightgrey">greyed out</span>{{< /rawhtml >}}) is now simply holding a claim to it (e.g. claim to the fluctuating price, and dividends), but no voting rights anymore - i.e. as far as GME is concerned, the OO is not their share holder anymore - the owner's equity now belongs to Broker B's investor ({{< rawhtml >}}<span style="color: green">in green</span>{{< /rawhtml >}}).
  - The claims are satisfied by the Short Seller's collateral ($500, ignoring daily mark-to-market adjustments), interest paid etc.
  - So what happens when the OO wants to SELL?
  - Simple - Broker A first locates another share in its `Pool of lendable GME shares`, sell it on the market (key point is that the share being sold is located), with the proceeds going to `OO`.
  - Broker A also marks the newly sold share as being lent to the Short Seller, effecting the same claim and accounting as for `OO` to the new lender (new OO).
- _ALL IS GOOD_ so far... but now lets enter the _twilight zone_, where Melvin and the SugarDaddy resides, a dark place full of `FTDs`, `FTRs`, `SBP`, `IOUs`, and the elusive `Buy-Ins`...

{{< rawhtml >}}<a name="ftd"></a>{{< /rawhtml >}}
### Failed-to-Delivers (FTDs)

- So after receiving favours from Melvin, SugarDaddy sells 4x GME shares for him, and says WTF, i'll sell 2x GME for ShitTron and Co just for shits and giggles...
- `IMPORTANT` - note that SugarDaddy `DOES NOT LOCATE THE SHARES, AND DOES NOT TAKE ON THE OTHER SIDE` (risks means nothing to him)- So SugarDaddy executes `Naked Short Sell of 6x GME` on the Exchange.
- Because in the real world you can't just create shares out of thin air, `GME's float is still at 4 shares`
- Anyways the trade is made on the exchange because some lucky dude saw that the GME shares are being sold at _way below intrinsic value_, so quickly instructs Broker A to "buy this for me NOW" using `Market Order` (at Ask)
- Now the `Short Interest` (Short Volume / Float) is `150%` of GME's float! (6/4 = 1.5 or 150%)...
- At the EOD, as usual, the trades are transmitted to NSCC via the Exchange
- NSCC, when doing the netting (clearing) notices something odd -> that SugarDaddy's stock account doesn't have the 6 GME shares sold to Broker A. so records a `Failed-to-Deliver` (`FTD`) against SugarDaddy...
- At the same time, NSCC will record `Failed-to-Receive` (FTR) against Broker A (like an `IOU`).

### Failed-to-Receives (FTRs)

- You might have noticed that only `2x FTRs for GME` were recorded against Broker A (meaning Broker A is owed 2 shares of GME), Why is that???
- This is due to a very well known trick (for insiders at least) called `Stock Borrow Programme`, which apparently is so well conceived and _"NOT AT ALL"_ abused that DTCC had to write a [letter to the sec of SEC](https://www.sec.gov/rules/proposed/s72404/s72404-14.pdf),  _Jonathan G. Katz_,  proclaiming how perfect it is - and don't listen to people who complain about it being abused because it is perfect...
- So notice how Broker B, has access to Cash Account Investor's 2x GME shares (assume agreed to let broker lend its shares out) - the Cash Investor obtained the 2x GME shares fair and square previously in the [Happy Days Scenario](#simple-overview)
- Broker B is a participant of the DTCC, and also in its `Stock Borrowing Programme`.
- Note that very little information is available on the internet (except for the letter to the SEC dated 2004) about DTCC's `Stock Borrow Programme`, I learnt about it, and the inner workings of the DTC/NCSS through the [Research Paper](https://www.researchgate.net/publication/228260887_Naked_Short_Sales_and_Fails_to_Deliver_An_Overview_of_Clearing_and_Settlement_Procedures_for_Stock_Trades_in_the_US) (see [reference](#reference)) by _Talis. J. Putnins_ (University of Sydney, NSW, Australia). The paper was released in October 2009, so be aware some info in there might be out of date (e.g. `T+3` it mentions is now `T+2` i believe).
- There is some info about this new system called [SFT](https://www.dtcc.com/clearing-services/equities-clearing-services/sft), due to be rolled out in 2021 (pending regulatory approval?), so I'm reading this as, the `Stock Borrow Programme` is still in use (_and still being abused_ for predatory naked short selling)
- Loving how _OPAQUE_ this whole thing is?
- Moving on, because NSCC is the central counterparty to all trades, NSCC borrows (not SugarDaddy) from the Stock Borrow Programme, effectively at 0% interest rate, in order to deliver the missing shares, and thereby reducing the Broker A's `FTR` from 6 to just 2.

{{< rawhtml >}}<h1 style="padding: 0.2em; line-height: 1.5em;"><span style="color: white; background-color:red; padding: 0.3em">Important Point #3</span> BROKEN - The <b>Stock Borrow Programme</b> (SBP) effectively allows SugarDaddy to game the system and borrow at 0% interest to make up for shares it can't deliver</h1>{{< /rawhtml >}}

### Elusive Buy-ins

- Are we approaching _infinite stupidity_ yet? Yes, we are, let me introduce to you the _elusive Buy-In_:
- `Buy-Ins` - are what MMs who received `FTRs` (Failed-to-Receives, aka IOUs) instead of real shares invoke when the they *REALLY* wants the real shares owed to them...
- This however, is rarely invoked in practice - in the same way why states don't assasinate each other's head of states, MMs don't invoke Buy-Ins for fear of retribution, and:
  - MM's clients doesn't know that they're actually holding `IOU`s
  - The `Continuous Net Settlement` Service, in an ingenious way (whether intentionally designed or not), assigns highest priority to FTRs, therefore people with FTRs actually get delivery of real shares the next EOD or 2 arrives (e.g. via other brokers or SBP) - whats the point of upsetting SugarDaddy when we just wait a few days before actual delivery?
  - What happens to the FTD? it doesn't expire, but remember, SBP = 0% interest, so SugarDaddy can sit on it forever, or orchestrate Brokerage shutdowns (28th of Jan, 2021)...
  - And so in effect, the FTR has been rolled to the next unlucky participant, again and again, in perpetuity

Let me just quote the exact texts from the [Talis. J. Putnins research paper](#references):  

`Page 11` - _"Buy-ins are rare. Evans et al. (2009) find that out of a total of 69,063 failed transactions of a market maker in 1998-1999 only 86 were bought-in. Boni (2006) argues that one reason why buy-ins are rare is that firms are unwilling to earn a reputation for forcing delivery in the hope that other firms will be equally lenient towards them when they fail to deliver"_ (Commentary: is this the catholic church we're talking about or DTCC???)

`Page 12` - _"Because the incidence of buy-ins is low and penalties for failing are small, naked short selling effectively is a way of short selling difficult or impossible to borrow stocks"_ (Commentary: GME???)

`Page 13` - _"Only in rare circumstances or in very infrequently traded stocks would a participant have an FTR for long enough to initiate the Buy-in process, let alone complete it."_

`Page 13` - _"Finally, the US clearing and settlement system does not provide any significant disincentives for naked short selling. The Buy-in procedure, on the rare occasions that it is used, is unlikely to force a naked short seller to close out the FTD; the Stock Borrow Program effectively facilitates a zero-fee zero-rebate loan to the naked short seller; and the fees for failing are insignificant."_


{{< rawhtml >}}<h1 style="padding: 0.2em; line-height: 1.5em;"><span style="color: white; background-color:red; padding: 0.3em">Important Point #4</span> BROKEN - The Elusiveness of the <b>Buy-In</b>, together with the <b>SBP</b> gives an infinite number of 'get-out-of-jail-free' cards to the predatory MM, allowing its FTDs to exist in perpetuity, without interest/consequence</h1>{{< /rawhtml >}}


### Ex-Clearing

{{< rawhtml >}}<h1 style="padding: 0.2em; line-height: 1.5em;"><span style="color: white; background-color:red; padding: 0.3em">Important Point #5</span> BROKEN - Do Not blindly trust the FTD, FTR numbers</h1>{{< /rawhtml >}}
I had to rewrite this section since the new FTD numbers came out - I was already suspicious of The January 14th FTD number (621,483 FTDs), now the January 29th figure (138,179 FTDs) makes me even more suspicious... we know:   

- Short sellers had borrowed 150% of floating shares of GME
- Lets assume they were some how (highly unlikely) able to borrow 100% of the float, the other 50% must be made up (i.e. through naked short selling by their MM/broker-dealer).
- 50% of 46.89M (according to yahoo) = `23M (23,445,000) fake shares` that should fail to deliver.
- Nowhere in any of the previous and current FTD reports did we see anything close to 23M FTDs reported...  
- Is there another loop hole somewhere being exploited to under report FTD (or even to not report FTDs at all)???
- _YES OF COURSE THERE IS_: its called [Ex-Clearing](http://brokerage101.com/comparison.html)
- Ex-clearing basically allows any two broker-dealers to do clearing between themselves, and then report any FTDs to the NSCC/DTCC
- So e.g. if we had 2 broker-dealers who are in collusion: 
  - broker-dealer #1 (RobinYou) 'helps' retail trader to buy GME,
  - broker-dealer #2 (SugarDaddy) naked short sells GME for Melvin, ShitTron and Co
  - #1 and #2 decides to do clearing outside of the DTCC/NSCC electronic system, between themselves (golden shower)
  - #1 and #2 reports to DTCC/NSCC that there is no FTDs, all shares were delivered (bullshit).
  - DTCC/NSCC believes them and reports +0 FTDs for GME

Alright so, I know its speculation, but the system does actually allow this to happen...


## Guerrilla Warfare

NOT INVESTMENT ADVICE - see [disclaimer](#disclaimer)  

{{< rawhtml >}}

<p style="padding: 0.5em; background-color: red; color: white;"><b>TL;DR</b>: Move everything off RobinHood into reputable broker with CASH ACCOUNT (no margin!); Hold + continue accumulating <i>unencumbered</i> GME shares, because:
<ul>
  <li>GME is a valuable company (currently undervalued @ $50)</li>
  <li>More unencumbered GME holdings = less GME shares available for short selling = more cost to hold existing short positions = <i>Real Short Squeeze</i></li>
  <li>More unencumbered GME shares we hold = <i>Nuclear Arsenal</i> = We fire as last resort to force delivery (force invoke <a href="#elusive-buy-ins">Buy-In</a>) of real GME shares from whoever created the fake shares.</li>
</ul>
</p>

<div class="explainer che">
<h3><span>Guerrilla Warfare</span><br/><div class="cols"><span class="col gme">GME</span><img class="col" src="/img/grenade_2.png"/></div><span>Operations Handbook</span><br/><span class="sign">WholesomeValue</span></h3>
<a name="gmewar1"></a>
<h4>1. Pre-requisites - Setup your Base</h4>
<ul>
<li><b>Understand</b> the game completely by reading <a href="https://blog.wholesomevalue.com/posts/naked">Naked Short Selling</a> from start to finish, pay particular attention to the section <a href="https://blog.wholesomevalue.com/posts/naked/#the-dark-side-of-the-dtcc-settlements-and-clearing-process">Dark Side of DTCC</a>, and enjoy a laugh or two reading the <a href="https://blog.wholesomevalue.com/posts/naked/#the-dark-side-of-the-dtcc-settlements-and-clearing-process">Re-enactment</a> and <a target="_blank" href="https://blog.wholesomevalue.com/posts/naked/#disclaimer">Disclaimer</a>.</li>
<li>Setup a <b>CASH</b> account with a reputable broker (i.e. not RobinHood)</li>
</ul>
<p>
Be <i>100% certain</i> the account you setup is a <i>CASH account</i> - some brokerages by default signs you up for margin account (e.g. RobinHood).
</p>
<p>
You don't want to be buying under a margin account because the shares you buy with it are lendable by the broker - which will increase availability of the shares to short sellers. Something this volatile, on margin, will also ensure your margin account explodes leaving you knee deep in debt.
</p>
<h4>2. Propaganda, Ammunition & Intelligence</h4>
<h5>2.1. Prepare for Battle</h5>
<p>
Campesinos! To prepare yourself for battle, you need to understand <i>why</i> you've bought GME, <i>what</i> we're fighting for, and <i>how</i> the war will be won:
</p>

<div id="wwh-tabs" class="tabs-container">
  <div class="tabs">
    <a data-tab-why onclick="selectTab(event.target, event);" class="active">Why</a>
    <a data-tab-what onclick="selectTab(event.target, event);">What</a>
    <a data-tab-how onclick="selectTab(event.target, event)">How</a>
  </div>
  <div data-tab-why class="tab-content active">
    <p>Simply put, GME represents <i>value</i>, and more:</p>
    <ul>
      <li><b>Brand Recognition</b> - <i>Everybody</i> now knows about GameStop. The brand stands for so much more than just a meme stock company</li>
      <li><b>Leadership</b> - To name a few of the leadership team on board now: <i>Ryan Cohen (Chewy)</i> - Brings proven ability for online execution and operational know how. Best of all he is 34 years old, just the right age to understand what gaming is all about; <i>Matt Francis</i> (formerly Amazon AWS) recently joined as CTO of GameStop (why would a AWS executive join GameStop if he didn't believe?); <i>Alan Attal</i> and <i>Jim Grube</i> of Chewy pedigree with long history of successful achievements; these leaders and more are executing the "Pursuit of Growth and Market Leadership" for GME.</li>
      <li><b>Macro Bullishness, Untapped Potential</b> - Ages 35-44 (+disposable income); Console/PC gaming +6.8% YOY (2020); Next-gen platform/games driving uplift; You can count on GME tapping into: <i>e-sports</i> - worth <i>$950M</i> in 2020, projected market value <i>$1.6B</i> in 2023; <i>online games distribution</i>: both physical media and electronic DL (think Steam @ $4B), <i>Gaming Experience Centers</i> - remember the good old <i>LAN parties</i>? what made it fun? playing together with your friends in the <i>same</i> room!; gaming by yourself just doens't compete with gaming with your friends; Synergy anyone?</li>
    </ul>
    <p>
    Remember value isn't just a brain dead calculation derived from formulas such as <i>discounted cash flow</i>. Even the greatest value investors such as <a class="ext" target="_blank" href="https://www.oaktreecapital.com/docs/default-source/memos/something-of-value.pdf">Howard Marks</a> acknowledge that <i>value</i> is reflexive, and it consitutes not only of the tangibles, but also the intangiles such as potential "<i>growth in the distant future</i>".
    </p>
    <p>Whats more, have a read of <a class="ext" target="_blank" href="https://www.gmedd.com/wp-content/uploads/2021/01/GMEdd-GameStopValuation-20Jan21.pdf">GMEDD.com's bull case for GameStop</a>: <i>$169</i> - and thats was early January! What should it be now? One thing is for sure, <i>$50</i> is a <i>STEAL</i>! Not to mension that we're at the end-of-life of <a class="ext" target="_blank" href="https://en.wikipedia.org/wiki/Eighth_generation_of_video_game_consoles">8th generation consoles</a>!</p>
    <p>Let it sink in that GameStop is <i>NOT</i> Enron.</p>
  </div>
  <div data-tab-what class="tab-content">
    <p>GameStop is a reputable company. Its starting to turn a profit for its loyal investors, and at the same time providing much needed job security to everyday people, not just in the USA, but around the world (e.g. EBGames in Australia) - <i>jobs that put food on the table and roof over their heads</i> - during what surely must be one of the most difficult times in our lives.</p>
    <p>Now ask yourself: What has SugarDaddy, Melvin and ShitTron ever done for everyday people?...</p>
    <p>Campesinos, what we're fighting for is this:</p>
    <ul>
      <li><b>Vengence</b> - It isn't right what SugarDaddy, Melvin and ShitTron did, and they need to be held accountable - they need to bleed, <i>MASSIVELY</i>. GameStop isn't the first, neither will it be the last if these people are not made examples of. Vengence, not just for GameStop, but for <i>ALL</i> past fallen companies and their employees at their hands. These people need <i>ETHICS</i> tatooed onto their foreheads to remind them every single morning, day, and night.</li>
      <li><b>Change</b> - The system is broken, and it allows SugarDaddy and its babies to amass billions in personal wealth, while millions lose their livelihoods. This system simply can't continue in its current form - This fight is to <i>FORCE</i> the hand of the SEC to take action one way or another.</li>
      <li>and finally, <b>Tendies</b> - For all of you who held and stayed strong. <i>YOU DESERVE IT</i>.</li>
    </ul>
  </div>
  <div data-tab-how class="tab-content" >
    <p>What SugarDaddy has done (the illegal naked shorting) is similar to a bank that has issued <i>IOUs</i>(FTRs), but holds <i>NO RESERVES</i>(real GME shares) - an over simplication (see <a href="#the-dark-side-of-the-dtcc-settlements-and-clearing-process">Dark Side of DTCC</a> for complete picture) - but useful to make a point: <i>What happens when IOUs holders requests underlying real shares at the same time?</i> - This is our <i>Nuclear</i> option, aka the "Bank Run"...</p> 
    <p>However, we prefer not to press the nuclear button and cause a nuclear fallout, our go to option would still be the short squeeze aka <i>liquidity crunch</i> (sorry shorties, you play the role of the <a class="ext" target="_blank" href="/img/lamb.jpg">sacrificial lamb</a>):</p>
    <p>A <i>liquidity crunch</i> happens when there is a simultaneous increase in demand for and  decrease in the availability of a security - GME in this case, and it has the following  negative effect on the short sellers:</p>
    <ul>
      <li><b>Borrowing Cost Increase</b> - Because their brokers needs to compete with buyers to locate shares of GME, so interest rate% rises (as we've seen recently as high as 20%+)</li>
      <li><b>Mark-to-market Losses</b> - They need to either provide more collateral for the shares borrowed, or cover some of their positions to reduce collateral requirements</li>
      <li><b>Upward Spiral</b> - The continuing demand (from both longs and shorts covering) produces an upward spiral of GME price, thus continuing to take out short positions at higher price entry levels, leading to more and more to capitulate and the spiral to continue)</li>
    </ul>
    <p>The 3 keys to effecting the short squeeze are:</p>
    <ul>
      <li><b>Popular Support</b> - Lets admit it, currently the popular sentiment is against us, people think that we are bag holders. Your job is to educate them, shine the light, give this operations manual to them and educate them the "what", "why", and "how". To do this, you better make sure you have <a href="#gmewar1">established your base</a> (step 1).</li>
      <li><b>Continued Demand</b> - You've setup a <i>CASH ACCOUNT</i> with your broker right? Are you sure? Ok, now build your <i>ammunition</i> by making recuring purchase (CASH only) of GME weekly/fortnightly/monthly, whatever your budget allows - whether its 1 x GME per month or 100 x GME per week - just <b>BUY + HODL</b>. ONLY USE MONEY YOU CAN AFFORD TO LOSE. If you can't afford to, just HODL and / or give emotional support to the troops. Enough of this ammunition is needed to keep the fight going.</li>
      <li><b>Intelligence</b> - Keep an eye out for trustworthy information, don't just regurgitate, evaluate yourself and then disseminate. At the same time, brush up on topics that you are not familiar with, ask questions on forums. Don't worry about the trolls, ignore them. Just maintain an inquisitive mindset. Don't be so closed minded because things change on a day-to-day basis. You need to be one with change, not against it.</li>
    </ul>
    <p>Before moving onto step 3, remember what <b>Mark Cuban</b> said:</p>
    <p>"<i>I know you are going to hate to hear this, but the lower it goes, the more powerful WSB can be stepping up to buy the stock again. The only question is what broker do you use . Do you stay with RH , who is going to have the same liquidity problems over and over again, or do you as a group find a broker with a far, far, far better balance sheet that wont cut you off and then go ham on Wall Street.</i>"</p>
  </div>
</div>

</p>
<h4>3. Bay of Pigs, and the Missile Crisis</h4>
<p>
The battles have already started, the war is yet to be won...
</p>
<p>We're fighting for 3 things: <b>Vengence</b>, <b>Change</b>(fairness), and <b>Tendies</b>. All of these could go pear shaped against us - e.g. The SEC could just pay lip service and play theatrics without doing anything concrete, letting SugarDaddy to keep its license with just a slap on the wrist (meaningless fine). Sure the lambs have been sacrificed, we get our tendies, but so what? Nothing meaningfull has happened - SugarDaddy hasn't learnt its lesson, and it can always find new lambs....</p>
<img src="/img/sec_ed.png"/>
<p>^ Maybe this should be "<i>Don't understand (trust) the System? Don't invest in anything based on the system</i>".</p>

<p>The above tweet illustrates how stupidly out of touch the SEC is and blind to whats happening. I really hope that we don't have to press the nuclear buttons, but just in case we had to, lets discuss if briefly here:</p>

<p>(If we don't already have enough) After accumulating the neccessary stockpile of GME shares, we have several nuclear warheads, and I don't think we need to go into specifics at this point in time. However they all work by detonating the <a href="#elusive-buy-ins">Elusive Buy-Ins</a>. How? I give you a hint: understand that you don't have to hold the securities with your broker, <a class="ext" target="_blank" href="https://www.sec.gov/reportspubs/investor-publications/investorpubsholdsechtm.html">you have other options</a>. e.g. I could just say "fuck it, I want a genuine GME share certificate to frame and put on my wall"... You get my drift now?
</p>
<p>
So lets examine what happens when we force the invocation of the <a href="#elusive-buy-ins">Buy-Ins</a>, forcing SugarDaddy (or whoever the bag holders of the FTDs are) to buy real GME shares on the market, competing with other market participants such as:</p>
<ul>
  <li>Gay Bear short sellers buying at market to cover (exit) their short positions</li>
  <li>Momentum (Day/Swing traders) Shorts covering their positions</li>
  <li>Momentum Longs looking for quick upside profit</li>
  <li>Long term investors & GME Campesinos</li>
  <li>Many others e.g. MMs hedging etc</li>
</ul>

<p>The result is a much more violent upward price explosion, and potentially a chain reaction that widens to the entire market. SEC intern I hope you're reading this...</p>
<p>At this point (and probably with the short squeeze also), you would expect someone to step in to contain the situation, we've got 2 likely candidates:</p>
<ul>
  <li><b>SEC</b> - Can't do much here?</li>
  <li><b>GameStop</b> - Can step in, issue new shares (equal to # of fake shares created), and sell it to the FTD bag holders @ market? above market?</li>
</ul>
<p>Btw, if you didn't understand, GameStop issuing / selling new shares to FTD bagholder = + cash to company treasury, and obviously gains for its shareholders...</p>
<p>Look the point is this, we have nuclear arsenal and we're not afraid to press the buttons. We're looking forward to your move SEC, starting with <a class="ext" href="https://www.washingtonpost.com/business/2021/02/14/sec-gamestop/" target="_blank">February 18</a>.</p>

</div>
{{</ rawhtml >}}

Here is some motivation: The [VW infinity squeeze](https://outline.com/E6XJsF) happened with only 12% short interest. The reason it happened is because there was just no one selling (and therefore short borrowing costs through the roof) - with VW/Porshe holding 70%+ of the stock in VW, and nobody else selling due to news of take over, the shorts were literally stuck between a rock and a hard place, either pay huge premium to cover, or pay huge borrowing costs to maintain the short positions + upsize collateral... clearly the better option was to exit by paying $1000 per share LMFAO.

{{< rawhtml >}}<h1 style="padding: 0.2em; line-height: 1.5em;"><span style="color: white; background-color:red; padding: 0.3em">Important Point #6</span> ULTIMATE ENDGAME - Lack of Liquidity is the Kryptonite</h1>{{< /rawhtml >}}


## Conclusion

Understand the 6 important points, and these 3:  

{{< rawhtml >}}<h1 style="background-color: green; color: white; padding: 0.6em">HODL GME until you either die or a big payout is given to you, Someone will cave eventually</h1>{{< /rawhtml>}}

{{< rawhtml >}}<h1 style="background-color: green; color: white; padding: 0.6em">GameStop is NOT ENRON, and now has a VERY BRIGHT future, thanks SugarDaddy</h1>{{< /rawhtml>}}

{{< rawhtml >}}<h1 style="background-color: green; color: white; padding: 0.6em">If Yellen don't start yelling at SugarDaddy and make an example of him, shall we all say hello to GFC 2.0</h1>{{< /rawhtml>}}

No more, no less.

_Disclaimer: I'm an idiot, so NOT INVESTMENT ADICE_, but:

- No Margin, Cash Only, Never Sell (for less than $1000)

![](/img/lemon.png)

Cheers

WholesomeValue

{{< rawhtml >}}<hr/>{{< /rawhtml >}}

## Appendices (organ)


### Extract of FTD report

See [source](https://www.sec.gov/files/data/fails-deliver-data/cnsfails202101a.zip)

The following have been massaged (GME only, latest few days only), with annotations (e.g. date=, entry=, etc)

```
# This is extracted from the SEC report
                              date       cusip         ftds         stock                 price
date=2021-01-05, entry=Entry(2021-01-05,36467W109,GME,490723,GAMESTOP CORP (HLDG CO) CL A,17.25)
date=2021-01-06, entry=Entry(2021-01-06,36467W109,GME,772112,GAMESTOP CORP (HLDG CO) CL A,17.37)
date=2021-01-07, entry=Entry(2021-01-07,36467W109,GME,799328,GAMESTOP CORP (HLDG CO) CL A,18.36)
date=2021-01-08, entry=Entry(2021-01-08,36467W109,GME,555658,GAMESTOP CORP (HLDG CO) CL A,18.08)
date=2021-01-11, entry=Entry(2021-01-11,36467W109,GME,703110,GAMESTOP CORP (HLDG CO) CL A,17.69)
date=2021-01-12, entry=Entry(2021-01-12,36467W109,GME,287730,GAMESTOP CORP (HLDG CO) CL A,19.94)
date=2021-01-13, entry=Entry(2021-01-13,36467W109,GME,662524,GAMESTOP CORP (HLDG CO) CL A,19.95)
date=2021-01-14, entry=Entry(2021-01-14,36467W109,GME,621483,GAMESTOP CORP (HLDG CO) CL A,31.40)

# Note the latest is first half of January 2021 (ending Jan 14)

# Who knows what the number might be for Jan 15 - Feb 14??? ftds = 50M???

```

{{< rawhtml >}}<a name="ortex_gme_si"></a>{{< /rawhtml >}}
### Ortex (ortex.com) GME Short Interest

Source: https://www.ortex.com/symbol/NYSE/GME/short_interest  

![](/img/ortex_gme_si.png)

{{< rawhtml >}}<a name="references"></a>{{< /rawhtml >}}

## References

- Putnins, Talis J. (2009) [_Naked Short Sales and Fails to Deliver: An Overview of Clearing and Settlement Procedures for Stock Trades in the US_](https://www.researchgate.net/publication/228260887_Naked_Short_Sales_and_Fails_to_Deliver_An_Overview_of_Clearing_and_Settlement_Procedures_for_Stock_Trades_in_the_US) Faculty of Economics and Business, University of Sydney 

- Dayen, David (2016) [_Naked Shorts Can't Stay Naked Forever_](https://theintercept.com/2016/09/24/naked-shorts-cant-stay-naked-forever/) The Intercept
{{< rawhtml >}}<a name="disclaimer"></a>{{< /rawhtml >}}

- Smith, Larry (2019) [_Part 7: Illegal Naked Shorting: DTCC Continuous Net Settlement and Stock Borrowing Programs Have Loopholes That Facilitate Illegal Naked Shorting_](https://smithonstocks.com/part-7-illegal-naked-shorting-dtcc-continuous-net-settlement-and-stock-borrowing-programs-have-loopholes-that-facilitate-illegal-naked-shorting/) smithonstocks.com

- No Auther [_Execution, Clearing and Settlement_](https://thismatter.com/money/stocks/settlement-and-clearing.htm) Internet Article

- Investopedia Staff / Anderson, Somer [Who Benefits From Lending Shares in a Short Sale?](https://www.investopedia.com/ask/answers/05/shortsalebenefit.asp) Investopedia.com

{{< rawhtml >}}<a name="hypo"></a>{{< /rawhtml >}}

- [SEC Fails-to-Deliver Data](https://www.sec.gov/data/foiadocsfailsdatahtm)

- [Hypothecation](https://www.investopedia.com/terms/h/hypothecation.asp) - bascially broker speak for, if you have margin account with us, then we have the right to lend out whatever you buy.

- [r/wallstreetbets Subreddit Stats](https://subredditstats.com/r/Wallstreetbets)

- [Naked Short Selling - Wikipedia](https://en.wikipedia.org/wiki/Naked_short_selling)

- [Ex-clearing](http://brokerage101.com/comparison.html)

- [Wall St Oasis Forum - Ex Clearing](https://www.wallstreetoasis.com/forums/ex-clearing)

- [SEC 6350A - Clearance / Settlement](https://www.finra.org/rules-guidance/rulebooks/finra-rules/6350a)

- [SEC Active Broker-Dealers List](https://www.sec.gov/help/foiadocsbdfoiahtm.html)

- [DTCC Obligation Warehouse](https://www.dtcc.com/clearing-services/equities-clearing-services/ow)

- [DTCC Article - Managing Risks with Ex-Clearing](https://www.dtcc.com/news/2011/april/01/managing-the-risks-of-ex-clearing-trades)

- [Investor.gov Ed - Order Execution](https://www.investor.gov/introduction-investing/investing-basics/how-stock-markets-work/executing-order) - this talks about how orders are routed (to exchange, to market makers etc), what "payment for orderflow" is

{{< rawhtml >}}<span style="background-color: red; color: white; padding: 0.3em; font-weight: bold;">UPDATE</span>{{< /rawhtml >}} Link to [theintercept.com article](https://theintercept.com/2016/09/24/naked-shorts-cant-stay-naked-forever/) that explores the same issue. The article also goes on to discuss something called [Reverse Stock Split](https://www.reddit.com/r/wallstreetbets/comments/lcpwh0/how_gme_can_still_be_a_great_play/) - basically how to nuke naked short sellers

## Disclaimer

(Read out loud at 100x the normal speed)  

{{< rawhtml >}}
<p style="font-size: 0.6em">
Peter Piper picked a peck of pickled peppers;
A peck of pickled peppers Peter Piper picked;
If Peter Piper picked a peck of pickled peppers,
Where’s the peck of pickled peppers Peter Piper picked

Betty Botter bought some butter but, said she, the butter’s bitter.
If I put it in my batter, it will make my batter bitter.
But a bit of better butter will make my bitter batter better.
So she bought some better butter, better than the bitter butter,
put it in her bitter batter, made her bitter batter better.
So ‘t was better Betty Botter bought some better butter.  

I invoke the Tucker Carlson disclaimer which basically says that no person of reasonable intelligence should mistake this hyperbole bullshit to be of any factual substance. Therefore you can't sue me unless you admit you are an idiot of super low intelligence on national TV. Even if you did, you still can't sue me. Regarding the reenactment, while it might be 99.99% accurate, there is a 100% margin of error. She sells seashells on the seashore.
The reenactment is for entertainment purposes only, the characters described within are not real, for example, Melvin is the incestual brother of Elmer J. Fudd, CNBC is the name of my black english staffy, who shits 3 times a day, RobinYou is new priest, and SugarDaddy is a pedophile that lives in the higher echalons of the church of market makers. The church is called the DTCC. Nothing on this page should be mistaken for investment advice - although full of facts, this was written by an idiot intended for idiots. So if you're smart like Andrew Left, please stay away from this.
The shells she sells are seashells, I’m sure.
And if she sells seashells on the seashore,
Then I’m sure she sells seashore shells.
</p>
{{< /rawhtml >}}

