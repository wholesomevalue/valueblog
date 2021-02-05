
# BLAH BLAH

# Selling Shorts Naked - AKA Naked Short Selling

{{< rawhtml >}}<span style="background-color: red; color: white; padding: 0.5em; font-weight: bold;">UPDATE</span>{{< /rawhtml >}}: Link to [theintercept.com article](https://theintercept.com/2016/09/24/naked-shorts-cant-stay-naked-forever/) that explores the same issue. The article also goes on to discuss something called [Reverse Stock Split](https://www.reddit.com/r/wallstreetbets/comments/lcpwh0/how_gme_can_still_be_a_great_play/) - basicall where (unscrupulous) naked short sellers go to die.  

_Original Post:_  

I think you came here to learn why someone would sell their shorts naked. I can explain, because I read a bunch of papers [link], which helped me recreate the *totally accurate* events between Point72, Citadel and Melvin that led to the greatest Short Squeeze (that is yet to happen) on GameStop (G or R18+ versions available). 

I hope to enlighten you, so please read the entire thing - you won't be disappointed. But if you're busy, or autistic but brilliant, and just want the bullet points, here it is:

### The Bullets

- Naked Short Selling (`NSS`) is bascially creating shares out of thin air
- Can be useful for making markets, but can also be abused (think the current GameStop saga)
- Basically only Market Makers (MMs) - think [prime brokerages](https://en.wikipedia.org/wiki/Prime_brokerage) ie. elites such as JP Morgan, _Point72_, _Citadel_ etc - can execute Naked Short Selling 
- There is no easy way to detect `altruistic NSS` (making a market, encourage) vs `abusive NSS` (predatory short selling, discourage)
- The public can only go by [DTSS/NSCC FTDs (Failed-to-Deliver) reports](https://www.sec.gov/data/foiadocsfailsdatahtm) which are published once a month (face palm)
- Even with FTD reports, you simply can't tell who the abusive NSS participants are (because the report only has aggregate data on each stock - no details on who owes what stock, when and why)
- Given this, if you're a `crook` (think [$1B fine for insider trading](https://en.wikipedia.org/wiki/Steve_Cohen_(businessman)#Racketeering_and_insider_trading_charges)) that owns one of the larger prime brokers around, why wouldn't you exploit it for your / your friend's benefit? - the formula is fairly easy, NSS the stock to obvlivion, stock = $0, then there is no stock to return - easy peasy [lemon squeezy]()? - or so they thought - until they encountered `GameStop` and a bunch of 'retarded degenerates' from `WSB`.

{{< rawhtml >}} <h1 style="color: red">The Big Picture: The Short Squeeze hasn't even started yet</h1> {{< /rawhtml >}}
- Somebody(s) going to pay for this, and its not going to be the WSB degenerates.  
  
Alright, here goes the longer version:  

### Long live GME

Normal short selling - you know what it is right? ok skip to the next paragraph - is (`with pants on`), you borrow a share (that you don't own) from your friend who owns the stock (the broker), and sell it to someone else. You then wait a while, buy the share back and return it to your friend (broker). all is well if the price went down and conversely all is bad if the price went up - YOU win or lose, bit deal... NOTE: the broker actually _OWNS_ {{< rawhtml >}}<sup>2</sup> {{< /rawhtml >}} the share.

Naked Short Selling - AKA `Selling Shorts (Pants) Naked`, on the other hand, is a much more extreme version of selling - I think the person who coined the term _Naked_ short selling had some very deep intiuitions about what it is...

![](/img/expose.jpg)

First of all, you and I can't sell shorts naked - I can't simply tell my broker, nor would my broker believe me, that I have 70M shares of GameStop (GME) stock to sell. The conversation would go something like this:

for reference see [Ortex](https://www.ortex.com/symbol/NYSE/GME/short_interest)

`ME` (15th Oct 2020): hey bro, I have 70M of GME stock I want you to sell for me  

`IBKR`: You do? congratulations, hold on one sec, let me do some DD (due dilligence), 

`IBKR`: Sorry, [reddit](https://www.reddit.com/r/wallstreetbets/comments/kz7ygv/gme_dd_one_dd_to_rule_them_one_dd_to_find_them/) says there is only 46M shares floating <sup>3</sup> around, of which we know that [Ryan Cohen](https://www.newsweek.com/who-ryan-cohen-gamestop-investor-3-billion-overnight-1565095) of Chewy fame, who also happens to be on the board of GME, [owns 13%](https://www.cnbc.com/2021/01/27/gamestops-surge-has-made-its-3-largest-shareholders-billions-overnight.html#:~:text=The%20chief%20beneficiary%20of%20the,owns%2013%25%20stake%20in%20GameStop.&text=GameStop%20CEO%20George%20Sherman%20has,value%20of%20about%20%24350%20million). Therefore you can't possibly have 150% of the floating shares in the company! if that was the case, you would have more shares than there are shares outstanding<sup>4 outstanding vs floating</sup> (69M) of the company!  

`ME` (15th Jan 2020) : Would you believe I have 30M ?  

`IBKR`: Let me check with reddit again, nope, sorry reddit says they're holding their shares, either you identify your self as a prime broker (e.g. Steven Cohen, or Kenny G), or we have to end this call now.  

[End of phone call]

# Identify as Steven Cohen or Kenny G???

Thats right, IBKR is correct, you need to be a prime broker, ie. any one of the [participants in DTCC](https://www.dtcc.com/client-center/dtc-directories), in order to bullshit about how much shares you have in a company.

These elite of the elites are called `Market Makers` (`MM`s) because they are meant to make (create) a market when there isn't one (think spread between bid and ask being too large), and <u>ONLY MMs are allowed to go naked and sell shorts</u> (we simply can't trust anyone else to do so).  

So imagine a hypothetical situation, in which the difference (the `spread`) between the bids and asks for GameStop were so wide that no body wanted to buy nor sell

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

Market makers will come in and use their special powers to facilitate / get trades going between buyers and sellers, by taking both sides (keypoint here is take *BOTH* sides)

So the MM would, e.g. sell 5 shares it doesn't own, at the bid price, and buy 5 shares at the ask price, to hopefully kick things off...

What the MM did (in the case of selling a share it doesn't own), is `execute a naked short sell (NSS)`. This is perfectly normal (not the picture, but the act), and often needed - all fine and altruistic:

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

At the end of the day, however, the MM needs to put pants back on, because its cold, and they don't want anyone to see them like this:

![](/img/shrink.png)

If the MM did its job of making the market correctly, it should have no risk - i.e. neutral, and make money by playing with the spread...


# The Risk

The risk with selling shorts while naked is that your junk is exposed, actually its not really (which I'll get to in a second), but you are exposed:

The exposure is VERY REAL if, instead of taking both sides, you (the MM) only takes one side (in relevance to what we're discussing here - taking the short side only).  

The exposure is that you eventually have to deliver the *REAL* share to the person you sold it to, if you don't then it just becomes a joke right? I mean [nothing like this has ever happened!](https://www.amazon.com.au/I-U-John-Lanchester/dp/1439169861) (I havn't read the book btw, I just like the cover).  

So in order to deliver the *REAL* share to the buyer (you don't have it because you were naked), you have to buy it - *AT ANY COST* - on the market <- big risk if you ask me.

{{< rawhtml >}}<h3 style="color:red">Important Point 1: Big Risk - Buy AT ANY COST</h3>{{< /rawhtml >}}

Anyways, back to the narrative that MMs are 'altruistic', which they're not, and only want to fuck *ahem*, help the market trade by adding liquidity...

So MMs are *NOT* altruistic, because its called capitalism - and they're in it for the money, which is fair enough - you take the risk to allow the market to trade - you should be compensated for it. 

Problem is, some MMs don't think their trillion dollar fortune is large enough, and so don't just want to play the spread game to earn $dough, they get creative and participate in a much more risky / predatory game, and this is when shit hits the fan/ceiling (and it will this time):  

<h3 style="color:red">A 100% accurate phone messages I intercepted, and conversations between different parties of the GME saga:</h3>

### Feb 15, 2019

`Melvin`: Hey pappa, we have a bit of a problem here, this guy called [Andrew Left](https://en.wikipedia.org/wiki/Andrew_Left), from some wanna be Hedge Fund called "ShitTron" or something, is copying our trade, with him and all his extended family of idiots copying our TOP SECRET trade on GME. They've now bought the remaing shares we could have used. I think we need to work some magic. I know what I'll have to do (love emoji, xxx,), I hope to see you at 10? K...  

[explainer: the magic refered to here is creating a small amount of shares, out of thin air, to use for shorting GME]  

[checkout this opinion piece by Bloomberge LMFAO](https://www.bloomberg.com/opinion/articles/2021-01-29/gamestop-gme-trading-short-sellers-like-citron-aren-t-the-enemy) - yep, [Lefty](https://en.wikipedia.org/wiki/Andrew_Left#Citron's_reports_on_Chinese_companies) is one of the good guys because he shits on China...

`SugarDaddy`: You'll have to work very hard for this one *wink* *wink*, ok see you at 10. Come to my office and be discete.  

[GME price goes further south, `note`: the game now is not simply to profit from short selling, the game is now to completely `KILL off GME`, otherwise they have to deliver some *REAL* shares to the 'idiots' who bought shares...]

### Jan 11, 2020

`Melvin`: Alright, more problems, this time theres a guy called `Ryan Cohen` who just joined GME's board, is he related to you?  

`SugarDaddy`: No, but see you at 10, same place, same shit (*wink* xxx)  

### Jan 22, 2021

[More and more WSB Retards find out about the position]  

`Melvin`: More?  

`SugarDaddy`: Sure  

[Shit explodes]

### Jan 27, 2021

`Melvin` to the public: We think you guys are stupid, therefore, we announce that we have exited the trade, taken a big hit. Calm down will ya, simply just trying to survive, making some money to feed my family, geez...  

[The whole world finds out about the position]  

`WSB` retards: Nah, Melvin no exit, Citadel and Point72 simply bought the short positions, called it a 'cash injection', so that Melvin can say they 'lost', we're not as retarded as you think.  

`CNBC`: these `WSB` guys are so stupid, of course Melvin is out, because they told us so... and we're smart, you guys don't know anything... 

`WSB` retards: "We don't like CNBC", in the most PG language ever

### Jan 28, 2021 (WSB Day)

`SugarDaddy`: hey DTCC, just wanted to let you know that somebody created a humongous short position on GME, not me, but somebody. If you don't raise your collateral requirements, then the entire stock market will be history. Get it?  

`DTCC`: sure we will raise the collateral by 500%. Btw, you know about our [Stock Borrow Programme](https://www.researchgate.net/publication/228260887_Naked_Short_Sales_and_Fails_to_Deliver_An_Overview_of_Clearing_and_Settlement_Procedures_for_Stock_Trades_in_the_US) (which [everyone thinks is awesome](https://www.sec.gov/rules/proposed/s72404/s72404-14.pdf)) right? You can borrow whatever how much you need (of GME), {{< rawhtml >}}<span style="background-color:red; color:white; font-weight: bold; padding: 0.5em;">AT 0% INTEREST</span>{{< /rawhtml >}} to cover your tracks. and after 3 days, Just "roll" your FTDs over to the idiot broker who's naked...

[All brockerages shut buying of GME, int the hope of locating *REAL* shares to reduce the number of synthetic shares]  

`Brokers`: Dear retail traders, we're doing this for you, to protect you from harm...  

`The world`: Fuck you, we're not dumb, if this is not collusion, then what the fuck is?  


Meanwhile, on twitter, our friend [Steven Cohen](https://en.wikipedia.org/wiki/Steve_Cohen_(businessman)#Racketeering_and_insider_trading_charges), who is [*totally unrelated to Melvin*](https://www.prnewswire.com/news-releases/melvin-announces-2-75-billion-investment-from-citadel-and-point72--301214477.html#:~:text=%22I%20am%20incredibly%20proud%20to,these%20two%20great%20investment%20icons.%22) says:  

![](/img/steven.jpg)

I think he is telling Melvin (stock jocks?) to bring the *REAL* shares back to the rightful owners. He is a good guy yep.  

{{< rawhtml >}} <h3 style="color:red">Important Point #2: Someone is still exposed</h3> {{< / rawhtml >}}

Because someone created a shit tonne of shares, out of thin air, to try to drive a company to the ground in order to hide the fact that the fake shares were created... Keyword here is _tried_, and failed, because they were stupid enough to fight with idiots, and as we all know you shouldn't fight with idiots, because if you do, then they'll drag you down to their level, and beat you fair and square with experience (of being stupid)...

_Disclosure: I am one of them (idiot), WSB variety._

# Why is My Junk Not Exposed (Not because I don't have one)

(explainer: not my junk)

So I hypothesis that someone (or group of people) is still exposed, and they tried to hide it (by trying to bankrupt GME), but failed (thanks to retards).  

And Janet Yellen also knows this, because apparently she wants to [understand fully what happened](https://www.investing.com/news/economy/yellen-says-wants-to-understand-deeply-gamestop-frenzy-before-taking-action-2409327) before taking action...

Anyways this someone/group can only really be exposed by Yellen, because the public has no way of knowing. To understand why that is so, we have to understand how clearing and settlement works (in the US):

go read [this](https://www.researchgate.net/publication/228260887_Naked_Short_Sales_and_Fails_to_Deliver_An_Overview_of_Clearing_and_Settlement_Procedures_for_Stock_Trades_in_the_US). I know you probably didn't read it so I'll summarize:

- `Depository Trust and Clearing Corporation (DTCC)` provides clearing & settlement services. DTCC has 2 subsidiaries: NSCC and DTC
- Clearing is done by the `National Securities Clearing Corporation (NSCC)`, while settlement is handled by the `Depository Trust Company (DTC)`
- Clearing is required to 'simplify' the settelment, e.g. since most shares are held in [Street Name](), we don't need to make transfers for each individual owner, simply aggregate transfers per participant (e.g. broker) will do.
- The clearing is done by NSCC taking both sides of every trade, to produce a _NET_ settlement file. Something like:

[TODO: pic of clearing]

- The settlement file is then fed into DTC, to effect settlement. This is where things get interesting (for GME at least)...
- Anyways, the key thing here to note is something called `Failed-To-Delivers (FTDs)`, for which a report is provided by the SEC [every month?](https://www.sec.gov/data/foiadocsfailsdatahtm).
- So the DTC, while effecting the settlement by going over each line in the settlement file, would mark any shares that could not be located (`Failed-to-Deliver`) by the participant.
- For GME, for a fairly long time, it has always been in the hundreds of thousands, sometimes even millions of shares -  day after day, week after week!

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
- This is got to be fishy right? But heres the catch, people can argue that because the numbers are aggregate, its just the way a hotly traded stock is...
- But it is not (hint: 140% short interest, the ability to naked short selling by MMs without any checks and balances), and we will soon see, because there is no way GME is going to $0...

{{< rawhtml >}} <h3 style="color:red">Important Point #3 - Failed-To-Delivers</h3> {{< /rawhtml >}}

<h1 style="color:green">Because you can't simply continue to write IOUs... just like in the GFC, the house of cards will come down.</h1>


Disclosure: I'm an idiot.

Ok, finally I hope you enjoyed this hyperbole bullshit, or is it???, that I just wrote 

My advice would be to <h1>HODL</h1> your GME stock, because if you NEVER SELL, YOU NEVER LOSE right? *GME is not Enron guys and girls, GME has value. I like the stock*

Alright I think I have to spell it out for you retards to understand, since somebody said that if you keep reducing a number by 50% of it self, you will end up with 0. Which totally makes sense to Melvin I'm sure, and Andrew... but not someone like Steven, so here goes:

{{< rawhtml >}}<h1 style="color: green">HODL GME until you either die or a big payout is given to you, they will cave eventually, or Yellen will be yelling</h1>{{< /rawhtml>}}

BTW if you can spare a few change, do send send a small donation Paypal Address here:  

### [paypal.me/wholesomevalue](paypal.me/wholesomevalue)

because I would like to buy more of GME, but I can't afford to because I'm broke now (down 70%)...

Alternatively my Bitcoin Address is:

![](/img/btc_address.png)

3Hia9udRvDb1R7Ljt85EdJJUR5xfhRrtHL

Note only send BTC to this address, everything else will get rejected.


Cheers!

WholesomeValue (an idiot)

![](/img/lemon.png)

