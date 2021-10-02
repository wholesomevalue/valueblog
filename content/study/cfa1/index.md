---
title: "CFA Level I"
---

## Overview
- 18 study sessions (S/1 - S/18); 1wk per study session; _15-20hrs per study session (per week)_; therefore curriculum should be finished in 18 weeks;
- everything is required / examined, except when marked as optional
- each session is divided into many readings (R/1 - R/x)
- each reading is preceded by _LOS_ = learning outcome statements (checklists)
- attempt all problems at end of readings

## Ethical & Professional Standards

skip  

## Quantitative Methods (2 - 3)

### S/2 - Basic Concepts

#### R/6 - Time Value of Money  

| [x] | Topic |
| ----|-------|
| [ ] | a. interest rate can also be though of as:  _rates of return_, _discount rates_, _opportunity costs_|
| [ ] | b. interest rate is sum of _real risk-free rate_ and _premium_ for risk |
| [ ] | c. _effective_ vs _stated_ annual interest rate, _frequency of compounding_ |
| [ ] | d. solve time value of money problems for different frequencies of compounding |
| [ ] | e. calculate _future value (FV)_, _present value (PV)_ for: single sum of money, ordinary annuity, annuity due, perpetuity (PV only), and unequal cash flows |
| [ ] | f. use time line to model / solve time value of money problems |

##### Interest Rate: Interpretations

- when we value a security, we attempt to determine worth of stream of future cash flows.
- a future cashflow is _discounted_ to compensate for 'nowness' (money today is worth more than money in the future).
- _interest rate_ is the rate of return / compensation applied to a future value - e.g. if $9,500 received today = $10,000 in 1yr, then interest rate _r_ is $500 / $9,500 = 0.0526 or 5.26%
- interest rate (_r_) = _discount rate_ = _opportunity cost_
{{< hint info >}}
r = _real risk-free interest rate_ + (_inflation_ + _default_ + _liquidity_ + _maturity_) premiums
{{</ hint >}}
- where:
  - _real risk-free i/r_ is completely risk-free rate sans inflation - i.e. given no inflation and no other risks, how much discount would you be willing to take to receive it now?
  - _inflation premium_ - compensation for inflation; real risk-free i/r + inflation premium = _nominal risk-free interest rate_ - e.g. 90-day US Treasury bill (_T-bill_)
  - _default risk premium_ - compensates for default possibilities
  - _liquidity premium_ - compensates for lack of liquidity, e.g. many corp bonds
  - _maturity premium_ - compensates for risks associated with 'longer' time to maturity

##### The _Future Values_ of a Single Cash Flow

- consists of a initial investment, or _present value (PV)_, and earns rate of return (interest per period, _r_) to arrive at its _future value (FV)_, which will be received _N_ years or periods from today
{{< hint info >}}{{< katex >}}FV_N = PV(1 + r)^N{{</ katex >}}{{</ hint >}}
- important that N and r are expressed in the same time unit (e.g. if r is annually, then N must be multiples of years)
- e.g:
  calculate future value of $5M invested at 7% per annum, compouding yearly for five years:  
  > PV = $5,000,000  
  > r = 7% = 0.07  
  > N = 5  
  > {{< katex >}}FV_N = PV(1+r)^N = \$5,000,000 (1.07)^5 = \$7,012,758.65{{</ katex >}}

- _frequency of compounding_ - when compounded multiple times per year (_discrete compounding_):
{{< hint info >}}{{< katex >}}FV_N = PV(1 + \frac{r_s}{m})^{mN}{{</ katex >}}{{</ hint >}}
- e.g: 
  > calculate future value of $10,000 invested with 8% annual interest, compounded quarterly for 2 years.  
  > PV = $10,000  
  > {{< katex >}}r_s{{</ katex >}} = 8% = 0.08 (annually)  
  > m = 4 (quarterly)  
  > {{< katex >}}r_s/m = 0.08 / 4 = 0.02{{</ katex >}}
  > N = 2
  > mN = 4(2) = 8 interest periods  
  > {{< katex >}}FV_N = \$10,000(1.02)^8 = \$10,000(1.171659) = \$11,716.59{{</ katex >}}  
- where:
  - {{< katex >}}r_s{{</ katex >}} is the interest rate per year
  - _m_ is the number of compounding periods per year
  - _N_ is the number of years
{{< rawhtml >}}<a name="s2_EAR"></a>{{</ rawhtml >}}
- the _stated annual rate_ vs _effective annual rate_ (EAR)
{{< hint info>}}{{< katex >}}EAR = (1 + r_p)^m - 1{{</ katex >}}{{</ hint >}}
  where {{< katex >}}r_p{{</ katex >}} is the period rate, and _m_ is the number of periods per annum  
  e.g. 8% per annum, but paid & compounded semiannually, the stated rate is 8%, while the effective rate is 8.16% = `EAR = (1 + periodic rate)^m - 1` = (1 + 0.04)^2 - 1 = 0.0816 or 8.16%
- for _continuous_ compounding (as opposed to discrete compounding):  
{{< hint info >}}{{< katex >}}EAR = e^{r_s} - 1{{</ katex >}}{{</ hint >}}
  where {{< katex >}}r_s{{</ katex >}} is the stated annual rate, e.g. 8% per annum, compounded continuosly, is {{< katex >}}e^{0.08} - 1 \approx 0.0833 \approx 8.33\%{{</ katex >}}
- the future value of a continuously compounding is:   
{{< hint info >}}{{< katex >}}FV = PVe^{r_s N}{{</ katex >}}{{</ hint >}}

##### The _Future Values_ of a Series of Cash Flow

- _annuity_ - finite set of level sequential cash flows
  - _ordinary_ annuity - t = 1
  - annuity _due_ - t = 0 (i.e. first payment is immediate)
- _perpetuity_ - never ending annuity (t = 1)

- An ordinary annuity with equal cashflow is calculated as follows:
{{< hint info >}}{{< katex >}}FV_N = A[\frac{(1 + r)^N - 1}{r}]{{</ katex >}}{{</ hint >}}
  where
  > _A_ is the annuity amount received per period
  > _N_ is the number of periods
  > _r_ is the interest rate per period

##### The _Present Values_ of a Single Cash Flow

- present value of a single cashflow, with discrete, annual compounding
{{< hint info >}}{{< katex >}}PV = FV_N(1 + r)^{-N}{{</ katex >}}{{</ hint >}}
  because: {{< katex >}}FV_N = PV(1 + r)^N{{</ katex >}}, so {{< katex >}}PV = \frac{FV_N}{(1 + r)^N} = FV_N[\frac{1}{(1 + r)^N}]{{</ katex >}}

- present value of a single cashflow, with discrete, multiple (m) periodic compounding per annum
{{< hint info >}}{{< katex >}}PV = FV_N(1 + \frac{r_s}{m})^{-mN}{{</ katex >}}{{</ hint >}}

- present value of a _perpetuity_:
{{< hint info >}}{{< katex >}}PV = A\sum_{t=1}^{\infty}[\frac{1}{(1 + r)^t}]{{</ katex >}}, which simplies to (as long as r is positive): {{< katex >}}PV = \frac{A}{r}{{< /katex >}}{{</ hint >}}
  where _A_ is the annuity received per year

#### R/7 - Discounted Cash Flow Applications

| [x] | Topic |
| ----|-------|
| [ ] | a. calc _NPV_ (net present value) and _IRR_ (internal rate of return) |
| [ ] | b. contrast NPV rule vs IRR rule, problems with IRR rule |
| [ ] | c. calculate _total return_ |
| [ ] | d. calculate _money-weighted_ vs _time-weighted_ rates of return; evaluate portfolios performance using such measures |
| [ ] | e. calculate different types of yields: _bank discount yield_, _holding period yield_, _effective annual yield_, and _market yield_ for US T-Bills |
| [ ] | f. convert between different yields |

##### Net Present Value (NPV) and Internal Rate of Return (IRR)

- _capital budgeting_ - the allocation of funds to long-range projects / investments
- _capital structure_ - the choice of long-term financing for the investments the company wants to make
- _working capital management_ - management of the company's short term assets (e.g. inventory), and short-term liabilities (e.g. payables to suppliers)
- the concept of NPV and IRR applies in both capital budgeting and security analysis contexts

- ***Net Present Value*** calculated as:
{{< hint info >}}{{< katex >}}NPV = \sum_{t=0}^{N} \frac{CF_t}{(1 + r)^t} {{</ katex >}}{{</ hint >}}
  where:  
  {{< katex >}}CF_t{{</ katex >}} = the expected cash flow at time t  
  _N_ = the investment's projected life, and  
  _r_ = the discount rate aka rate of return aka opportunity cost of capital  

- negative NPV projects should be rejected, and competing positive NPV projects selected by greater NPV
- inputs must be in compatible time units - e.g. N is years, and r is annual rate
  > example, review project that requires initial outlay of $2M ({{< katex >}}CF_0{{</ katex >}} = -$2M). The project expected to generate {{< katex >}}CF_1 {{</ katex >}} = $500K (at year 1), {{< katex >}}CF_2{{</ katex >}} = $750K, {{< katex >}}CF_3{{</ katex >}} = $1.35M. using r = 10% per annum (discount rate):  
  > {{< katex block >}}NPV = -\$2 + \$0.50/(1.10)^1 + \$0.75/(1.10)^2 + \$1.35/(1.10)^3 = \$0.088655M{{</ katex >}}  
  > since NPV > $0, project accepted; note that the discount rate chosen plays a big part in making NPV + vs -; justification required

- ***Internal Rate of Return (IRR)*** is the rate of return where the NPV is 0:
{{< hint info >}}{{< katex >}}NPV = 0 = CF_0 + \frac{CF_1}{(1 + IRR)^1} + \frac{CF_2}{(1 + IRR)^2} + ... + \frac{CF_N}{(1 + IRR)^N}{{</ katex >}}{{</ hint >}}
  Where, {{< katex >}}CF_N{{</ katex >}} is the cash flow at Nth year  
- IRR is known as the _hurdle rate_ where the projected cash outflow = inflow, i.e. the rate of return that needs to be achieve breakeven; therefore, the cost of capital must be <= hurdle rate  
  > e.g. a R&D project is projected to return $150K in perpetuity, with the the initial outlay of $1M, calculate the IRR  
  > {{< katex >}}NPV = -\$1,000,000 + \frac{\$150,000}{IRR}{{</ katex >}} (PV of perpetuity = {{< katex >}}\frac{A}{r}{{< /katex >}})  
  > {{< katex >}}NPV = 0 = -\$1,000,000 + \frac{\$150,000}{IRR}{{</ katex >}}  
  > {{< katex >}}\$1,000,000 = \frac{\$150,000}{IRR}{{</ katex >}}  
  > {{< katex >}}\therefore IRR = \frac{\$150,000}{\$1,000,000} = 15\%{{</ katex >}}  
  > so if the cost of capital is < 15% then the project would have a positive cashflow

- when IRR and NPV are conflicting, select using NPV - e.g. when IRR for project A > B, but NPV for B > A, then select project B; remember that we want to maximize $ returns, a greater IRR (percentage return) doesn't neccessarily mean greater return in $ terms

##### Portfolio Return Measurement

- _holding period return_ 
- _money-weighted rate of return_ is essentially IRR in investment management speak, ie we solve for _r_
  > e.g. I invested $200 for 1 share (t=0), and another share @ $225 (t=1), at t=2 (holding for 2 years), I liquidate the shares for $235 each ($470 total), and during the hold, I received $5 dividend from the 1st share (not reinvested) and at the end of 2nd year, I received $10 (2 x $5) in dividends, calculate the money-weighted rate of return (r):  
  > {{< katex >}}\$200 + \frac{\$225}{(1 + r)} = \frac{\$5}{(1 + r)} + \frac{\$480}{(1 + r) ^ 2}{{</ katex >}} ($480 because we received $10 in dividend in the final year)  
  > on the left, is our money outflows (invested), on the right is our money inflows (dividend + cash received when shares sold)  
  > so essentially, our equation is: _PV(outflows) = PV(inflows)_  
  > we apply discounting on both side of the equation: on the left side, we arrive at PV of $225 with: {{< katex >}}\frac{\$225}{(1+r)^1}{{</ katex >}} and on the right side, we arrive at PV of the dividends and liquidation with: {{< katex >}}\frac{\$5}{(1+r)^1}{{</ katex >}} and {{< katex >}}\frac{\$480}{(1+r)^2}{{</ katex >}}  
- money-weighted rate of return _IS_ affected by addition/withdrawals of funds

- _time-weighted rate of return_ _IS NOT_ affected by the addition/withdrawals of funds. Is preferred measurement.
- in time-weighted rate of return, we solve for the rate of return r, for $1 invested, taking into account the return for each period, compounded, arriving at r by finding the [geometric mean](https://en.wikipedia.org/wiki/Geometric_mean) of the periodic returns :
  > e.g. In the money-weighted rate of return example from above, if we take a closer look at each period (year 1 & 2), we have:  
  > year 1 = 15% return: ($5 + $225 - $200) / $200 = 15%  
  > year 2 = 6.67% return: ($10 + $470 - $450)/ $450 = 6.67%  
  > so: {{< katex >}}(1 + r_{tw}) = (1.15)(1.0667){{</ katex >}}  
  > {{< katex >}}r_{tw} = \sqrt{(1.15)(1.0667)} - 1 = 10.76%{{</ katex >}}  
  > where {{< katex >}}r_{tw}{{</ katex >}} is the time-weighted rate of return  

- daily evaluation of the portfolio is accepted in the industry as sufficient valuation frequency for time-weighted rate of return. The daily return is calculated as follows:  
  {{< hint info >}}{{< katex >}}r_t = \frac{\text{MVE}_t - \text{MVB}_t}{\text{MVB}_t}{{</ katex >}}{{</ hint >}}  
  where:  
  {{< katex >}}r_t{{</ katex >}} = the rate of return at day _t_,  
  {{< katex >}}\text{MVB}_t{{</ katex >}} = the market value at beginning of day _t_  
  {{< katex >}}\text{MVE}_t{{</ katex >}} = the market value at end of day _t_  

  the time-weighted return {{< katex >}}r_{tw}{{</ katex >}} would be:  
  {{< hint info >}}{{< katex >}}r_{tw} = [(1 + r_1) \times (1 + r_2) \times ... \times (1 + r_N)]^{\frac{1}{N}} - 1 {{</ katex >}}{{</ hint >}}

##### Money Market Yields

- ***money market*** is the market for short-term debt instruments (one-year maturity or less). eg. US Treasury bill (T-bill), commercial paper (corp bonds), negotiable certificates of deposits
- the ***face value*** of a T-bill is the amount the US government promises to pay back to the investor at maturity. The investor doesn't pay the face value of the T-bill when they buy it, instead, they pay the face value minus _discount_
- the discount is effectively the interest rate
- T-bills are whats called _pure discount instruments_
- T-bills are quoted on a ***bank discount basis*** (annualizes based on 360-day year):  
  {{< hint info >}}{{< katex >}}r_{bd} = \frac{D}{F} \times \frac{360}{t}{{</ katex >}}{{</ hint >}}
  where:  
  {{< katex >}}r_{bd}{{</ katex >}} = the annualized yield on a bank discount basis  
  {{< katex >}}D{{</ katex >}} = the dollar discount on the face value  
  {{< katex >}}F{{</ katex >}} = the face value  
  {{< katex >}}t{{</ katex >}} = the amount of days left to maturity  
  360 = number of days in a year (bank convention)  
  > e.g. Suppose a T-bill with a face value (aka par value) of $100,000 and 150 days until maturity is selling for $98,000. What is the bank discount yield?  
  > in this case, the dollar discount D is $2,000. The yield would be:  
  > {{< katex >}}r_{bd} = \frac{\$2,000}{\$100,000} \times \frac{360}{150} = 4.8\%{{</ katex >}}  

  > when the bond was originally issued, the investor would have purchased it for:  
  > {{< katex >}}r_{bd} = 4.8\% = \frac{D}{\$100,000} \times \frac{360}{360}{{</ katex >}}  
  > {{< katex >}}\therefore D = 4.8\% \times \$100,000 = \$4,800{{</ katex >}}  
  > and so the investor paid: $100,000 - $4,800 = $95,200

- bank discount rate does not show the actual return on the investment, 3 additional yields are listed in table below:  

| Holding Period Yield (HPY) | Effective Annual Yield (EAY) | Money Market Yield |
| ------------- |:-------------| -----|
| {{< hint info >}}{{< katex >}}\text{HPY} = \frac{P_1 - P_0 + D_1}{P_0}{{</ katex >}}{{</ hint >}} | {{< hint info >}}{{< katex >}}\text{EAY} = (1 + \text{HPY})^{\frac{365}{t}} - 1{{</ katex >}}{{</ hint >}} | {{< hint info >}}{{< katex >}}r_{mm} = \frac{360r_{bd}}{360 - (t)(r_{bd})}{{</ katex >}}{{</ hint >}} |
| yield for duration of hold | yield annualized (365 days) | {{< katex >}}r_{bd}{{</ katex >}} annualized (360 days) |

#### R/8 - Statistical Concepts and Market Returns

| [x] | Topic |
| ----|-------|
| [ ] | a. compare descriptive statistics vs inferential statistics; population vs sample; measurement scales |
| [ ] | b. define parameter, sample statistic, frequency distribution |
| [ ] | c. given frequency distribution, calculate relative frequencies, cumulative relative frequencies |
| [ ] | d. properties of dataset presented as histogram / frequency polygon |
| [ ] | e. central tendency - calculate mean, sample mean, arithmetic mean, geometric mean, weighted average/mean, harmonic mean, median, mode |
| [ ] | f. quartiles, quintiles, deciles, percentiles |
| [ ] | g. range, mean absolute deviation, variance and standard deviation of population of sample |
| [ ] | h. _Chebyshev's_ inequality for proportion of observations falling within specified # of standard deviations |
| [ ] | i. coefficient of variation, _Sharpe_ ratio |
| [ ] | j. skewness, positive vs negative skewed distributions |

#### R/9 - Probability Concepts

### S/3 - Application

## Economics (4 - 5)

### S/4 - Micro / Macro Economics

### S/5 - Monetary & Fiscal Policy, International Trade and Currency Exchange Rates

#### R/18 Monetary and Fiscal Policy

| [x] | Topic |
| ----|-------|
| [ ] | a. monetary vs fiscal policy |
| [ ] | b. functions & definitions of money |
| [ ] | c. money creation process |
| [ ] | d. theories of demand / supply of money |
| [ ] | e. _Fisher_ effect |
| [ ] | f. roles & objectives of central banks |
| [ ] | g. contrast costs of expected and unexpected inflation |
| [ ] | h. tools used to implement monetary policy |
| [ ] | i. monetary transmission mechanism |
| [ ] | j. qualities of effective central banks |
| [ ] | k. explain relationships between monetary policy <-> economic growth <-> inflation <-> interest <-> exchange rates |
| [ ] | l. contrast use of inflation, interest rate, exchange rate targeting by central banks |
| [ ] | m. expansionary policy vs contractionary monetary policy |
| [ ] | n. limitations of monetary policy |
| [ ] | o. roles & objectives of monetary policy |
| [ ] | p. tools of fiscal policy, advantages and disadvantages |
| [ ] | q. arguments for/against whether size of national debt relative to GDP matters? |
| [ ] | r. how is fiscal policy implemented, any difficulties? |
| [ ] | s. determine if fiscal policy is expansionary or contractionary |
| [ ] | t. interactions between monetary and fiscal policy |

- ***monetary policy*** - central bank activities to influence _quantity_ of money and credit in the economy (federal reserve)
- ***fiscal policy*** - government's decision about taxation and spending (treasury?)
- goal of monetary + fiscal policies is to control inflation, and bring stable growth to economy

##### Monetary Policy

###### Money

- _monetary policy_ (central bank) seeks to influence the macro economy by influecing the quantity of money and credit in the economy  
- _barter economy_ & the _double coincidence of wants_ - in order for a barter exchange to occurr, an exchange can only happen if both parties wants the other's good (e.g. a camel for a pig)
- _medium of exchange_ - is anything that can be used to purchase goods/services or repay debt
- money is an instance of medium of exchange; it:
  - readily acceptable
  - have a known value
  - easily divisible
  - high value relative to weight
  - difficult to counterfeit
- _promissory note_ - precedes paper money; was a note given by a goldsmith that noted how much gold the person holds with the goldsmith;
- ***fractional reserve banking*** - banks take deposits, and make loans. bank only needs to keep % of the deposits, and lend out the rest. the % is called the _reserve requirement_. This is called _fractional reserve banking_
  > e.g. reserve requirement is 10%; person A deposits $1,000 into FirstBank; FirstBank lends 90% ($900) to person B, who then buys goods from merchant person C; Person C deposits $900 into SecondBank, who then lends out $810 and so on  
  > FirstBank's balance sheet would be: Asset=($100 cash + $900 loan to B) & Liability = $1,000 to A, etc  
  > the total money created would be $1,000 / 0.1 = $10,000  
- the amount of money the fractional reserve banking system creates is:
  {{< hint info >}}{{< katex >}}M = \frac{1}{R}{{</ katex >}}{{</ hint >}} 
  where _R_ is the reserve requirement. _M_ is called the ***money multiplier***  
  > e.g. if the reserve requirement is 10%, then M = 1 / 0.1 = 10

- _Definitions of Money_: ***narrow money(M1)*** in US is comprised of essentially cash/cash equivalents: notes, coins in cirulation + travellers cheques of non-bank issuers, demand deposits at commercial banks + other deposits where cheques an be written; ***broad money(M2)*** in US is comprised of M1 + 'near money' (money that can be easily converted into cash): savings and money market deposits, time deposit acounts < $100K + other balances in retail money markets & mutual funds

- ***quantity theory of money*** expresses the relationship between money and price, and asserts: total spending is proportional to quantity of money  

- ***quantity equation***:    
  {{< hint info >}}{{< katex >}}M \times V = P \times Y{{</ katex >}}{{</ hint >}}  
  where  
  _M_ = the quantity of money  
        _V_ = the velocity of exchange of money (avg number of times in a period a unit of currency changes hands ??? how is this calculated ???)  
        _P_ = average price level  
        _Y_ = real output (GDP?)  
  _M x V_ is the _total spending (monetary value)_  
  _P x Y_ is the _total output (monteray value)_
- when the quantity of money increases, it does not effect neither real output _Y_ nor velocity of exchange _V_, instead, it will have a direct proportional effect on price _P_ - ***money neutrality*** - 
- if goods/services aka output is constant, there is no need for exchange to increase

- _Demand for Money_: ***transaction money balances*** vs ***precautionary money balances*** vs ***speculative money balances***

###### Role of Central Banks

- roles: lender of last resort, supplier of currency, banker's bank/to the government, regulator/supervisor of payments system, conductor of monetary policy, supervisor of banking system

###### Objectives of Monetary Policy

- monetary policy maintains ***price stability***; expected inflation vs unexpected inflation (prefer expected b/c can plan/predict)
- central banks have 3 main policy tools: ***open market operations***, ***refinancing rate (policy rate)*** (aka _official policy rate_, _official interest rate_, _fed discount rate_), ***reserve requirement***
- _open market operations_: 
  - buying/selling of government bonds by the central bank
  - central bank buying bond = increasing the supply of money in circulation;
  - central bank selling bond = decreasing the supply of money in circulation;
  - so when CB wishes to decrease the money supply (e.g. when there is running inflation), they would offer to sell bonds at a bigger discount (higher interest rate), which would attract banks/investors, and thus withdrawing money from circulation (to the cb)
  - when CB wishes to increase the money supply, they would offer to buy bonds from banks/investors at a lower discount rate (meaning a higher bond $value) which would attract banks/investors to sell (since previously, the investors bought the bonds at a bigger discount)
- _policy rate_:
  - policy rate aka: _official policy rate_, _refinancing rate_, _official interest rate_, _fed discount rate_
  - policy rate expresses the CB's intentions, and it seeks to influence short/long-term interst rates, and ultimately economic activity
  - the policy rate the CB announces is the rate at which it is willing to lend to banks
  - when CB raises the rate, the bank would need to raise the rate also, since the CB has the ability to sell bonds, thus decreasing the supply of money in circulation, which would mean the banks would need to borrow to maintain their reserve requirements (likely borrowing from CB, if interbank borrowing drys up)
  - when CB lowers the rate, the bank would want to reduce the rate also to remain competitive among themselves
  - US: refinancing rate known as the ***discount rate***, however fed also specifies a ***fed funds rate*** (a set range of interest rate for interbank lending)
    - fed fund rate is a target for the FOMC members to target using open market operations; the rate is reviewed every 6 weeks
    - see [investopedia - how do central banks impact interest rates](https://www.investopedia.com/ask/answers/031115/how-do-central-banks-impact-interest-rates-economy.asp)
    - see [investopedia - open market operations](https://www.investopedia.com/terms/o/openmarketoperations.asp)
    - if a bank's cash reserve is below the reserve requirement at the end of the day (e.g. if customers withdrawals > deposits), then bank needs to top up reserves to meet reserve requirements
    - bank can either borrow cash from another bank or from the fed to maintain the reserve requirement. 
    - cost to borrow = either fed fund rate or discount rate; borrowing is usually just overnight
    - usually the discount rate > fed fund rate to discourage banks from borrowing from fed directly
    - if there are no excess liquidity from any other bank, then need to borrow from fed
  - UK: refinancing rate is know as: ***two-week repo rate***
  - ECB: ***refinancing rate***
  - when CB wishes to temporarily increase money supply, they would enter into a ***repurchase agreement*** in the overnight/short-term money market where they buy bonds from counterparties (e.g. banks), and sell it back to them later at a premium
  - when CB wishes to temporarily decrease money supply, they would enter into a ***reverse repo agreement*** in the overnight/short-term money market where they sell bonds to counterparties (e.g. banks), and buy them back later at a premium
  - [New York Fed Reverse Repo FAQ](https://www.newyorkfed.org/markets/rrp_faq.html)
  - [New York Fed Repo FAQ](https://www.newyorkfed.org/markets/repo-agreement-ops-faq.html)
- _reserve requirement_
  - third primary way CB can limit or expand supply of money
  - this tool is seldom used nowadays due to its disruptive effects on banks
  - Australia used this tool to cool down the mortgage bubble during the 2008 financial crisis?

- official interest rate should directly affect: _Market Rates_, _Asset Prices_ (e.g. bond/stock prices), _Expectations/Confidence_, _Exchange Rate_; these then flow on through multiple layers to affect _Inflation_
- ***inflation targeting*** by CBs attempts to use transparent reporting, monetary policy tools to pin inflation within a certain range.
- credibility of the CB is important in inflation targeting, this is achieved through:
  - CB being a separate entity to the government
  - CB having power to set interest rate, 
  - CB continuosly/transparently report/communicate its views/goals to the public
- CB's transparent communications may itself be enough to set inflation expectations and effect inflation to its desired levels
- Current belief is that:
  - 0% inflation target would lead to deflation (bad)
  - > 3% inflation target would lead to unstable growth
- NZ was the first to introduce inflation targeting
- US and Japan does not use inflation targeting

##### Fiscal Policy

- involves directing government spending / tax revenue to effect: distribution of wealth, aggregate demand (e.g. spending in infrastructure), sector resource allocation
- essentially primarily manage economy by influencing aggregate national output (_real GDP_)
- gov ***bugdet surplus / deficit*** is the difference between gov revenue and expenditure
- when gov spending > gov income, the budget will be in deficit; spending < income, budget is in surplus
- when gov spending and revenue is equal, its called a ***balanced budget***
- ***expansionary*** (raising spending) vs ***contractionary*** (reducing spending) fiscal policy
- gov spending is viewed as a % of GDP, e.g. Australia in 2019, expenditure is [38.29% of GDP](https://www.statista.com/statistics/260547/australias-ratio-of-government-expenditure-to-gross-domestic-product/)
- while surplus/deficit is for a specific period, ***national debt*** is the accumulation of the difference over time
- national debt rises/falls: e.g. world war II, UK national debt was 250% of GDP
- Australian national debt to GDP seems to be [rising steadily](https://www.statista.com/statistics/271843/public-debt-of-australia-in-relation-to-gross-domestic-product-gdp/), currently at 72.11%
- who owns the government debt? usually the public (e.g. through the purchase of gov bonds)
- for UK 2010-11, 6.3% of the gov expenditure was to cover the government debt interest

###### Fiscal Policy Tools

- ***Transfer payments*** - redistribution of income; welfare payments e.g. pension, low income support, unemployment benefits etc; not counted towards GDP
- ***Current government spending*** - regular/recurring basis; e.g. health, education, defense
- ***Capital expenditure*** - e.g. infrastructure spending on roads, hospitals, schools etc;



## Financial Reporting & Analysis (6 - 9)

### S/6 - Intro

### S/7 - Income Statements, Balance Sheets & Cash Flow Statements

### S/8 - Inventories, Long-lived Assets, Income Taxes and Non-current Liabilities

### S/9 - Reporting Quality & Analysis

## Corporate Finance and Portfolio Management (10 - 12)

### S/10 - Corporate Governance, Capital Budgeting & Cost of Capital

### S/11 - Leverage and Working Capital Management

### S/12 - Portfolio Management

## Equity and Fixed Income (13 - 16)

### S/13 - Organization, Indices and Efficiency

### S/14 - Equity Analysis and Valuation

### S/15 - Fixed Income - Basic Concepts

#### R/50 Fixed-Income Securities: Defining Elements

- fixed income issued by company is relatively lower risk compared to common share holders of company b/c fixed income investor has first claim to company asset vs common share holder
- bond features - issuer, maturity, par value (face value), coupon rate & frequency, currency denomination - determines a bond's expected and actual return
- "traditional" bonds vs ***Asset Backed Securities (ABS)***
- ABS invovles securitization of assets from original owner to new special holding entity; holding entity issues the bond
- _issuer_ - categorizations: government, government-related, corporate, structure finance sector (ABS)
- investment grade vs non-investment grade (speculative) bond issues
- _maturity_: how long before issuer need to pay all outstanding principal to bond holder; ***tenor*** is the time remaining to bond's maturity date; maturities range from overnight to 30yrs or longer; < 1yr = ***money market securities***, > 1yr = ***capital market securities***
- ***par value***: aka ***principal*** is amount issuer will repay to holder at maturity date; bond prices are quoted as % of par value; e.g. par value $1000, a 95 par bond is 95% of $1000 = $950; if bond is trading at 100% of its par value, its trading at premium, otherwise its trading at discount
- ***coupon rate*** / frequency: {{< katex >}}coupon = couponrate \times par value{{</ katex >}}; i.e. _coupon_ is the interest the bond issuer pays to the bond holder; e.g. coupon rate 6% of $1000 par value, paid annually: 6% x $1000 = $60 of coupon (interest) yearly; payment frequency e.g. yearly, semi-annually, quarterly, monthly;
- ***basis point*** is equal to 0.01%, so 1% = 100 basis points
- ***bond identure*** is the ***trust deed*** (legal contract) that specifies e.g. _collaterals_, _credit enhancements_, _covenants_ related to the bond issued.
- ***covenants*** are clauses specifying rights of bond holders and actions the issuer is obligated to perform or prohibited from performing (e.g. in the case of the outstanding bond paid off by GME, which had covenants prohibiting GME from taking on further debt)
- ***collateral*** is the assets/financial guarantee underlying the bond issue
- ***credit enhancements*** are provisions reducing risk for the holders
- _seniority_ ranking of bond determines who gets repaid first in case of default; e.g. senior debt > junior debt, secured bond > unsecured bond
- 

#### R/51 Fixed-Income Markets: Issuance, Trading and Funding

#### R/52 Introduction to Fixed-Income Valuation

#### R/53 Introduction to Asset-Backed Securities

### S/16 - Fixed Income - Analysis of Risk

## Derivatives and Alternative Investments (17 - 18)

### S/17 - Derivatives

### S/18 - Alternative Investments

## Glossary

- `continuous compounding`
- `discrete compounding`
- `EAR` - Effective Annual Rate, is the actual annual rate being applied to the investment rather than the _stated annual rate_,
  > e.g. 8% per annum, but paid & compounded semiannually, the state rate is 8%, but the effective rate is [8.16%](#s2_EAR)
- `geometric mean` is the mean (average) of the _product_ of a set of numbers (as opposed to arithmetic mean, which is the mean of the sum of a set of numbers):  
  {{< katex >}}\left(\prod _{i=1}^{n}x_{i}\right)^{\frac {1}{n}}={\sqrt[{n}]{x_{1}x_{2}\cdots x_{n}}}{{</ katex >}}
- `nominal risk-free interest rate` - is the _risk-free rate_ + _inflation rate_; e.g. US Treasury Bill (T-Bill)
- `refinancing rate` is 1 of 3 monetary policy tools the central bank has (the other 2 being _open market operations_ and _reserve requirements_)
  - in Australia, its called the _official interest rate_
  - in US, its called the _fed discount rate_, however there is another rate called the _fed funds rate_, which is usually lower than the fed discount rate, and is the rate for interbank borrowings
  - 
