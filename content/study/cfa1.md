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
{{< hint info >}}{{< katex >}}FV = PVe^{r_s}N{{</ katex >}}{{</ hint >}}

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

- _Net Present Value_ calculated as:
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

- _Internal Rate of Return (IRR)_ is the rate of return where the NPV is 0:
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

- _money market_ is the market for short-term debt instruments (one-year maturity or less). eg. US Treasury bill (T-bill), commercial paper (corp bonds), negotiable certificates of deposits
- the _face value_ of a T-bill is the amount the US government promises to pay back to the investor at maturity. The investor doesn't pay the face value of the T-bill when they buy it, instead, they pay the face value minus _discount_
- the discount is effectively the interest rate
- T-bills are whats called _pure discount instruments_
- T-bills are quoted on a _bank discount basis_ (annualizes based on 360-day year):  
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
| [ ] | g. range, mean absolute deviation, variance and standard deviation of population of sample ||
| [ ] | h. _Chebyshev's_ inequality for proportion of observations falling within specified # of standard deviations |
| [ ] | i. coefficient of variation, _Sharpe_ ratio |
| [ ] | j. skewness, positive vs negative skewed distributions |

#### R/9 - Probability Concepts

### S/3 - Application

## Economics (4 - 5)

### S/4 - Micro / Macro Economics

### S/5 - Monetary & Fiscal Policy, International Trade and Currency Exchange Rates

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
