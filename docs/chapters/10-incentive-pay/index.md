---
title: "Incentive Pay"
---

# 10. Incentive Pay

Why do some workers earn a fixed salary while others are paid by the piece? How do firms motivate effort when they cannot perfectly observe what workers do? This chapter analyses the design of compensation contracts, focusing on the principal-agent problem and its solutions: piece rates, efficiency wages, tournaments, and deferred compensation.

---

## The Principal-Agent Problem

The employment relationship is fundamentally a **principal-agent** problem. The employer (principal) wants the worker (agent) to exert effort, but effort is costly to the worker and difficult for the employer to observe. If the employer pays a fixed wage regardless of output, the worker has an incentive to shirk.

!!! model "The Core Trade-Off"
    The principal-agent problem arises when:

    1. **Hidden action:** The employer cannot perfectly observe the worker's effort \( e \).
    2. **Divergent interests:** The worker prefers less effort; the employer prefers more.
    3. **Output is stochastic:** Output \( q = f(e, \varepsilon) \) depends on both effort and a random component \( \varepsilon \), so the employer cannot infer effort perfectly from output.

    The employer must design a compensation contract that **aligns incentives** --- making it in the worker's self-interest to exert the desired level of effort.

---

## Time Rates vs. Piece Rates

The simplest distinction in compensation is between **time rates** (payment per hour or month) and **piece rates** (payment per unit of output).

### Piece Rates

Under a piece rate system, the worker earns \( w = r \times q \), where \( r \) is the rate per unit and \( q \) is output. This directly ties compensation to performance.

!!! model "Optimal Effort Under Piece Rates"
    A worker chooses effort to maximise:

    \[
    U = r \cdot q(e) - C(e)
    \]

    where \( C(e) \) is the cost of effort with \( C'(e) > 0 \) and \( C''(e) > 0 \). The first-order condition is:

    \[
    r \cdot q'(e) = C'(e)
    \]

    The worker exerts effort until the marginal revenue from an additional unit of effort equals the marginal cost. A higher piece rate \( r \) increases effort.

### Advantages and Disadvantages

| Piece Rates | Time Rates |
|------------|------------|
| Strong effort incentives | Weak effort incentives (requires monitoring) |
| Self-selection: attracts high-ability workers | No adverse selection by risk tolerance |
| Risk imposed on worker (income varies) | Risk borne by employer (wage is fixed) |
| May encourage quantity over quality | Easier to maintain quality standards |
| Difficult when output is hard to measure | Works when output is difficult to quantify |

!!! empirical "Lazear (2000): The Safelite Study"
    Edward Lazear studied the Safelite Glass Corporation's switch from hourly wages to piece rates for auto-glass installers. Key findings:

    - **Productivity increased by 44%** after the switch to piece rates.
    - About half the increase came from the **incentive effect** (existing workers worked harder) and half from the **sorting effect** (more productive workers were attracted to the firm, and less productive workers left).
    - This study provides clean evidence that incentive pay matters both for motivation and selection.

---

## Efficiency Wages

An alternative approach to the monitoring problem is to pay workers **above** the market-clearing wage, making the job valuable enough that workers do not want to risk losing it by shirking.

### The Shapiro-Stiglitz (1984) Model

!!! model "Efficiency Wages and the No-Shirking Condition"
    Consider a worker who can either work (effort \( e \)) or shirk (effort 0). The employer detects shirking with probability \( d \) per period and fires the worker if caught.

    **The worker's calculus:**

    - **Value of employed-and-working:** \( V_E^W = w - e + \beta V_E^W \)
    - **Value of employed-and-shirking:** \( V_E^S = w + \beta[(1-d)V_E^S + d \cdot V_U] \)

    where \( V_U \) is the value of being unemployed and \( \beta \) is the discount factor.

    The **no-shirking condition (NSC)** requires that the worker prefers working to shirking:

    \[
    V_E^W \geq V_E^S
    \]

    Solving, the efficiency wage must satisfy:

    \[
    w \geq \bar{w} + e + \frac{e}{d} \cdot \left(\frac{r + b + d}{d}\right)
    \]

    where \( \bar{w} \) is the alternative wage and \( r \) is the interest rate. The efficiency wage **exceeds** the market-clearing wage, and the excess is larger when:

    - Effort cost \( e \) is high
    - Detection probability \( d \) is low (monitoring is difficult)
    - The unemployment rate is low (the cost of losing the job is small)

### Implications

Efficiency wages create **involuntary unemployment**: at the above-market wage, there are more workers who want jobs than there are jobs available. This unemployment is not a market failure but an equilibrium feature --- it serves as the **discipline device** that prevents shirking.

!!! empirical "Other Efficiency Wage Theories"
    The Shapiro-Stiglitz shirking model is one of several efficiency wage theories:

    - **Turnover reduction:** Above-market wages reduce costly employee turnover (Salop, 1979).
    - **Adverse selection:** Higher wages attract more productive applicants (Weiss, 1980).
    - **Gift exchange:** Workers reciprocate generous wages with higher effort out of fairness norms (Akerlof, 1982).
    - **Nutritional efficiency wages:** In developing countries, higher wages improve nutrition and physical productivity (Leibenstein, 1957).

---

## Tournaments

In many organisations, workers compete against each other for promotion. The prize is not directly tied to absolute performance but to **relative** performance. Lazear and Rosen (1981) formalised this as a **tournament model**.

!!! model "Tournament Theory (Lazear & Rosen, 1981)"
    Two workers compete for a promotion. The winner receives wage \( W_H \) and the loser receives \( W_L \). Each worker's output is:

    \[
    q_i = e_i + \varepsilon_i
    \]

    where \( e_i \) is effort and \( \varepsilon_i \) is a random shock. The worker with higher output wins.

    The worker chooses effort to maximise:

    \[
    E[U_i] = P(\text{win}) \cdot W_H + [1 - P(\text{win})] \cdot W_L - C(e_i)
    \]

    The **optimal effort** depends on the **prize spread** \( \Delta W = W_H - W_L \):

    \[
    C'(e^*) = \Delta W \cdot g(0)
    \]

    where \( g(0) \) is the density of the difference in luck at zero. Key predictions:

    1. **Larger prize spreads elicit more effort.** This explains why CEO pay is so much higher than that of vice-presidents --- the gap motivates all those competing for the top job.
    2. **Effort depends on the spread, not the level.** Raising both \( W_H \) and \( W_L \) by the same amount does not change incentives.
    3. **More randomness (larger variance of \( \varepsilon \)) reduces effort** for a given prize spread.

### Applications

- **Corporate hierarchies:** The large gap between CEO and senior VP compensation serves as a tournament prize, motivating effort throughout the organisation.
- **Sports:** Prize structures in professional tennis and golf are explicitly tournament-based, and empirical evidence shows that larger prizes generate better performance.
- **Academic tenure:** The tenure system can be viewed as a tournament where assistant professors compete for a limited number of permanent positions.

---

## Deferred Compensation

Many firms pay workers less than their marginal product when young and more than their marginal product when old, creating an **upward-sloping age-earnings profile** that exceeds the productivity profile.

!!! model "Lazear's Deferred Compensation Model"
    A worker's marginal product (VMP) is constant over the career at \( VMP^* \). Instead of paying \( w = VMP^* \) in every period, the firm offers:

    - \( w_{\text{young}} < VMP^* \) early in the career
    - \( w_{\text{old}} > VMP^* \) late in the career

    Subject to the constraint that the present value of wages equals the present value of productivity:

    \[
    \sum_{t=0}^{T} \frac{w_t}{(1+r)^t} = \sum_{t=0}^{T} \frac{VMP^*}{(1+r)^t}
    \]

    **Why defer?** The worker has a stake in the job: if caught shirking and fired, the worker loses the deferred premium \( (w_{\text{old}} - VMP^*) \). This creates incentives without direct monitoring. The worker effectively posts a "bond" through the low early wage and collects the return through the high late wage.

    **Mandatory retirement** is a natural feature of this system: the firm must terminate the relationship at a predetermined date because the worker is being paid more than their productivity in the later years.

---

## Team Production and Free-Riding

When output is jointly produced by a team and individual contributions are not separately observable, a new incentive problem arises: **free-riding**.

!!! model "The Free-Rider Problem in Teams"
    Suppose \( n \) workers in a team produce total output \( Q = \sum_{i=1}^n q_i \) and share revenue equally. Worker \( i \) receives:

    \[
    \text{Pay}_i = \frac{1}{n} \cdot R(Q)
    \]

    Worker \( i \)'s marginal benefit of effort is only \( \frac{1}{n} \) of the marginal revenue product, while bearing the full marginal cost. Each worker under-provides effort relative to the social optimum.

    **Solutions:**

    - **Monitoring by a residual claimant:** One team member (the "manager") monitors others and claims the residual profit (Alchian & Demsetz, 1972).
    - **Peer pressure and social norms:** Repeated interactions and small team sizes enable mutual monitoring.
    - **Profit-sharing with budget-breaking:** Holmstrom (1982) shows that if the employer can impose a penalty when total output falls below a threshold, efficient effort can be sustained.

---

## Executive Compensation

CEO compensation has grown dramatically: the ratio of CEO-to-median-worker pay in the US rose from about 20:1 in 1965 to over 300:1 by the 2020s. Several theories explain this pattern:

1. **Tournament theory:** Extreme pay gaps are the prize that motivates effort in the corporate hierarchy.
2. **Superstar markets:** A small difference in CEO talent generates large differences in firm value when firms are very large, justifying high pay (Gabaix & Landier, 2008).
3. **Rent extraction:** Weak corporate governance allows CEOs to set their own pay (Bebchuk & Fried, 2004). Stock options and golden parachutes may reflect managerial power rather than optimal incentive design.

!!! empirical "Stock Options and Risk-Taking"
    Stock options give executives the right to buy shares at a fixed "strike" price. If the stock price rises above the strike price, the option is valuable; if it falls below, the option is worthless. This **convex payoff structure** encourages risk-taking: the executive captures upside gains but bears no downside cost. This contributed to excessive risk-taking in the financial sector before the 2008 crisis.

---

## Incentive Structures in India

!!! indian "Piece Rates and the Informal Sector"
    India's large informal sector relies heavily on piece-rate compensation. Home-based workers in garment production, bidi rolling, and agarbatti (incense) making are typically paid per piece. While piece rates align incentives, they often result in exploitative outcomes when workers have no bargaining power:

    - **Bidi workers** earn as little as Rs. 150--200 per 1,000 bidis, working 10--12 hour days.
    - **Piece rates in agriculture:** Sugarcane cutting, tea plucking, and cotton picking are paid by weight or quantity.
    - Workers bear all the production risk (defective pieces are rejected without pay) but have no access to insurance or benefits.

    The informal sector illustrates that piece rates can coexist with extremely low earnings when markets are monopsonistic and workers lack alternatives.

!!! indian "NREGA Wage Structure"
    The Mahatma Gandhi National Rural Employment Guarantee Act (NREGA) provides an interesting case study in incentive design:

    - NREGA mandates a **minimum wage** for unskilled manual labour, with wages varying by state.
    - The original design included both **time rates** and **piece rates** (task-based wages). Piece rates were intended to improve productivity on public works.
    - In practice, many states shifted to time-rate payment due to difficulties in measurement and disputes over piece-rate norms.
    - Imbert and Papp (2015) show that NREGA increased private-sector wages by 4.7%, demonstrating how a public employment programme can alter the wage structure for the entire rural labour market.

---

## Key Takeaways

1. **The principal-agent problem** is central to compensation design: when effort is unobservable, firms must design contracts that align worker and employer incentives.
2. **Piece rates** provide strong incentives and attract high-ability workers, but impose risk on workers and may encourage quantity over quality.
3. **Efficiency wages** above the market-clearing rate prevent shirking by making job loss costly; the resulting unemployment acts as a discipline device.
4. **Tournaments** explain large pay gaps in corporate hierarchies: effort depends on the prize spread, not the level of pay.
5. **Deferred compensation** (low early wages, high late wages) creates incentives through a worker's accumulated stake in the job.
6. **Team production** creates free-rider problems that require monitoring, peer pressure, or budget-breaking schemes.
7. **Executive compensation** can be explained by tournament theory and superstar effects, but governance failures may lead to excessive pay.

---

<div style="display: flex; justify-content: space-between; margin-top: 2rem;">
<a href="../09-discrimination/index.md">&larr; Chapter 9: Labor Market Discrimination</a>
<a href="../11-unemployment/index.md">Chapter 11: Unemployment &rarr;</a>
</div>
