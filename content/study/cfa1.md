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
  - e.g. 8% per annum, but paid & compounded semiannually, the stated rate is 8%, while the effective rate is 8.16% = `EAR = (1 + periodic rate)^m - 1` = (1 + 0.04)^2 - 1 = 0.0816 or 8.16%
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


#### R/7 - Discounted Cash Flow Applications

| [x] | Topic |
| ----|-------|
| [ ] | a. calc _NPV_ (net present value) and _IRR_ (internal rate of return) |
| [ ] | b. contrast NPV rule vs IRR rule, problems with IRR rule |
| [ ] | c. calculate _total return_ |
| [ ] | d. calculate _money-weighted_ vs _time-weighted_ rates of return; evaluate portfolios performance using such measures |
| [ ] | e. calculate _bank discount yield_, _holding period yield_, _effective annual yield_, and _market yield_ for US T-Bills |
| [ ] | f. convert between different yields |


{{< katex >}}
f(x) = \int_{-\infty}^\infty\hat f(\xi)\,e^{2 \pi i \xi x}\,d\xi
{{</ katex >}}

### S/3 - Application

## Economics (4 - 5)

### S/4 - Micro / Macro Economics

### S/5 - Monetary & Fiscal Policy, International Trade and Currency Exchange Rates

## Financial Reporting & Analysis (6 - 9)

### S/6 - Financial Reporting and Analysis - Intro

### S/7 - Income Statements, Balance Sheets & Cash Flow Statements

### S/8 - Inventories, Long-lived Assets, Income Taxes and Non-current Liabilities

### S/9 - Financial Reporting Quality & Financial Statement Analysis

## Corporate Finance and Portfolio Management (10 - 12)

### S/10 - Corporate Governance, Capital Budgeting & Cost of Capital

### S/11 - Leverage and Working Capital Management

### S/12 - Portfolio Management

## Equity and Fixed Income (13 - 16)

### S/13 - Market Organization, Market Indexes and Market Efficiency

### S/14 - Equity Analysis and Valuation

### S/15 - Fixed Income - Basic Concepts

### S/16 - Fixed Income - Analysis of Risk

## Derivatives and Alternative Investments (17 - 18)

### S/17 - Derivatives

### S/18 - Alternative Investments

## Glossary

- `EAR` - Effective Annual Rate, is the actual annual rate being applied to the investment rather than the _stated annual rate_,
  > e.g. 8% per annum, but paid & compounded semiannually, the state rate is 8%, but the effective rate is [8.16%](#s2_EAR)
- `discrete compounding`
- `continuous compounding`
