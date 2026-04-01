---
title: "Practice — Incentive Pay"
---

# Practice: Incentive Pay

Test your understanding of compensation design, principal-agent problems, and incentive structures. Questions cover both theoretical analysis and real-world applications.

---

??? question "Q1. Identifying the Principal-Agent Problem"
    For each of the following situations, identify: (a) who is the principal, (b) who is the agent, (c) what is the hidden action, and (d) what incentive mechanism could address the problem.

    1. A homeowner hires a contractor to renovate a kitchen.
    2. A university employs a professor to teach and do research.
    3. Shareholders hire a CEO to manage a corporation.

    **Answer:**

    **1. Homeowner and contractor:**

    - (a) Principal: homeowner
    - (b) Agent: contractor
    - (c) Hidden action: quality of materials used, care in workmanship, actual hours worked
    - (d) Solutions: fixed-price contract (contractor bears cost risk), performance milestones with inspection, warranty clauses, reputation in local market

    **2. University and professor:**

    - (a) Principal: university (administration)
    - (b) Agent: professor
    - (c) Hidden action: effort devoted to teaching preparation vs. research vs. leisure; quality of mentoring
    - (d) Solutions: tenure system (tournament for promotion), teaching evaluations, publication requirements, peer review

    **3. Shareholders and CEO:**

    - (a) Principal: shareholders
    - (b) Agent: CEO
    - (c) Hidden action: effort, risk-taking, empire-building vs. profit maximisation
    - (d) Solutions: stock options and equity compensation (aligns CEO wealth with stock price), performance bonuses, board monitoring, threat of takeover

??? question "Q2. Piece Rate vs. Time Rate"
    A garment factory employs 100 workers. Under hourly wages of $15/hour, each worker produces an average of 10 shirts per hour. The factory considers switching to a piece rate of $1.80 per shirt.

    (a) If a worker maintains the same productivity (10 shirts/hour), how do their earnings compare under the two systems?
    (b) Based on the Safelite evidence, what would you predict happens to average productivity after the switch?
    (c) Why might some workers prefer the hourly wage even if they could earn more under piece rates?

    **Answer:**

    **(a)** Under time rates: $15/hour. Under piece rates at 10 shirts/hour: \( 10 \times \$1.80 = \$18 \)/hour. The worker earns **$3 more per hour** under piece rates if productivity stays constant.

    **(b)** Based on Lazear (2000), we would predict:

    - **Incentive effect:** Existing workers increase effort, producing more than 10 shirts/hour, because each additional shirt now earns $1.80.
    - **Sorting effect:** Higher-ability workers are attracted to the firm (they earn more under piece rates), while lower-ability workers may leave (they earn less). Average productivity should rise substantially --- Lazear found a 44% increase at Safelite.

    **(c)** Risk-averse workers may prefer hourly wages because:

    - Piece-rate earnings are **variable**: bad days (machine breakdowns, illness, difficult fabric) reduce income.
    - Hourly wages provide **income certainty** regardless of output fluctuations.
    - Workers may also fear that management will **lower the piece rate** if productivity rises ("ratchet effect"), eroding the benefit.

??? question "Q3. Efficiency Wage Analysis"
    In the Shapiro-Stiglitz model, suppose the market-clearing wage is $12/hour, the effort cost is $3/hour, and the probability of detecting a shirker is 0.20 per period.

    (a) Explain intuitively why the firm must pay more than $12/hour.
    (b) If the unemployment rate rises, what happens to the efficiency wage needed to prevent shirking? Why?
    (c) A firm installs cameras that increase the detection probability to 0.50. What happens to the efficiency wage?

    **Answer:**

    **(a)** At $12/hour, the worker is indifferent between this job and unemployment. If caught shirking, the worker simply finds another job at $12/hour --- there is no cost to shirking. The firm must pay a **premium above market-clearing** so that the worker has something to lose (a "rent") if fired.

    **(b)** When the unemployment rate rises, the **cost of job loss increases**: it takes longer to find a new job, and the worker may endure a spell of zero or low income. This makes the current job more valuable even without a large wage premium. The efficiency wage needed to prevent shirking **falls** --- unemployment itself acts as a discipline device. This is the key insight of the Shapiro-Stiglitz model: unemployment is the "worker discipline device."

    **(c)** When the detection probability rises from 0.20 to 0.50, shirkers are more likely to be caught. The expected cost of shirking increases, so the wage premium needed to deter shirking **decreases**. Better monitoring is a substitute for higher wages. The efficiency wage falls because:

    \[
    w^* \propto \frac{e}{d}
    \]

    A higher \( d \) reduces the wage premium needed, all else equal.

??? question "Q4. Tournament Prize Structure"
    A law firm has 10 associates competing for 2 partner positions. The associate salary is $200,000 and the partner salary is $600,000.

    (a) What is the prize spread in this tournament?
    (b) According to tournament theory, what happens to associate effort if the firm increases the partner salary to $800,000 while keeping the associate salary unchanged?
    (c) The firm considers promoting 5 out of 10 instead of 2 out of 10. How does this affect incentives?
    (d) Why might the firm prefer a tournament to individual performance bonuses?

    **Answer:**

    **(a)** The prize spread is:

    \[
    \Delta W = W_{\text{partner}} - W_{\text{associate}} = \$600{,}000 - \$200{,}000 = \$400{,}000
    \]

    **(b)** Increasing the partner salary to $800,000 raises the prize spread to $600,000. Tournament theory predicts that **effort increases**: associates work harder because the reward for winning the promotion tournament is larger. The optimal effort condition \( C'(e^*) = \Delta W \cdot g(0) \) implies higher effort when \( \Delta W \) rises.

    **(c)** Promoting 5 out of 10 instead of 2 out of 10 **reduces effort**. When the probability of promotion is higher, each associate needs less effort to have a reasonable chance of winning. The tournament becomes less competitive. This is analogous to reducing the difficulty of a race --- participants run slower.

    **(d)** Tournaments have advantages over individual bonuses:

    - **Relative performance** filters out common shocks (e.g., if all associates face a bad economy, the tournament still rewards the best performers).
    - **Measurement is simpler:** the firm only needs to rank associates, not measure absolute output precisely.
    - **Collusion is harder** in tournaments: associates cannot collectively agree to reduce effort because each individual benefits from deviating.

??? question "Q5. Deferred Compensation"
    A firm offers the following wage profile to a worker whose marginal product is constant at $50,000 per year:

    | Years | Wage |
    |-------|------|
    | 1--15 | $40,000 |
    | 16--30 | $62,000 |

    (a) In which years is the worker "overpaid" and "underpaid" relative to productivity?
    (b) Why does this wage structure reduce shirking?
    (c) Why is mandatory retirement at year 30 a necessary feature of this contract?
    (d) What happens to a worker who is fired at year 10?

    **Answer:**

    **(a)** The worker is **underpaid** in years 1--15 (wage $40,000 < VMP $50,000) and **overpaid** in years 16--30 (wage $62,000 > VMP $50,000).

    **(b)** During years 1--15, the worker accumulates a "bond" --- the difference between productivity and wage (\$10,000/year for 15 years = \$150,000 in undiscounted terms). The worker expects to collect this bond through above-productivity wages in years 16--30. If the worker shirks and is fired before year 16, the worker forfeits the deferred premium. This creates a powerful incentive to work hard without direct monitoring.

    **(c)** Mandatory retirement is necessary because after year 15, the worker is paid above marginal product. The firm loses money on the worker in every year from 16 to 30. If the worker could stay indefinitely, the firm would accumulate losses. Mandatory retirement ensures the firm does not overpay in total --- the present value of wages equals the present value of productivity over the 30-year career.

    **(d)** A worker fired at year 10 has been underpaid by \$10,000/year for 10 years. The worker has "invested" $100,000 (undiscounted) in the firm through below-productivity wages but has not yet begun to collect the above-productivity wages. The firing imposes a substantial **capital loss** on the worker --- this is precisely why deferred compensation deters shirking. However, this feature also means that firms may opportunistically fire senior workers to avoid paying the deferred premium, which is why employment protections and reputational concerns are important.

??? question "Q6. Free-Riding in Teams"
    A software development team of 5 engineers shares a $100,000 bonus equally if the project ships on time. Each engineer's effort costs $8,000.

    (a) If the project requires all 5 engineers to exert effort to succeed, what is each engineer's net payoff from contributing?
    (b) What if Engineer A believes the other 4 will contribute regardless? What is A's incentive?
    (c) Propose two mechanisms to solve the free-rider problem.

    **Answer:**

    **(a)** If all 5 contribute: each receives \( \$100{,}000 / 5 = \$20{,}000 \) and incurs a cost of $8,000. Net payoff = $12,000 per engineer.

    **(b)** If A believes the other 4 will contribute:

    - If A contributes: project succeeds, A earns $20,000 - $8,000 = **$12,000**.
    - If A shirks: if the project **still succeeds** (other 4 are enough), A earns $20,000 - $0 = **$20,000**.
    - If A shirks and the project **fails** (requires all 5), A earns $0 - $0 = **$0**.

    If A's effort is truly essential, A should contribute. But if there is any probability the project succeeds without A (even partially), A has an incentive to free-ride. The larger the team, the smaller each member's impact and the stronger the free-riding incentive.

    **(c)** Two mechanisms:

    1. **Individual performance monitoring:** Track individual contributions (code commits, code reviews, tasks completed) and tie bonuses to individual as well as team output. A residual claimant (project manager) monitors and enforces.
    2. **Peer evaluation with budget-breaking:** Each team member rates others. If the team misses the deadline, all members receive zero bonus (Holmstrom's budget-breaking). The threat of collective punishment creates incentives for mutual monitoring and peer pressure.

??? question "Q7. Executive Compensation and Stock Options"
    A CEO receives 100,000 stock options with a strike price of $50. The current stock price is $50.

    (a) What is the value of these options if the stock price rises to $80? To $30?
    (b) Explain how this payoff structure might encourage excessive risk-taking.
    (c) Suggest a modification to the compensation package that would reduce risk-taking incentives.

    **Answer:**

    **(a)**

    - If stock price = $80: Each option is worth \( \$80 - \$50 = \$30 \). Total value = \( 100{,}000 \times \$30 = \$3{,}000{,}000 \).
    - If stock price = $30: Options are "out of the money" (stock price < strike price). The CEO does not exercise them. Total value = **$0**.

    **(b)** The payoff is **asymmetric**: the CEO captures gains when the stock rises but loses nothing (beyond the options becoming worthless) when the stock falls. This is a convex payoff that rewards volatility. A CEO with stock options prefers a risky strategy (50% chance of $80, 50% chance of $30) over a safe strategy ($50 for certain):

    - Risky: Expected option value = \( 0.5 \times \$30 + 0.5 \times \$0 = \$15 \) per option
    - Safe: Option value = $0 (stock stays at strike price)

    The CEO always prefers risk because options have limited downside. This contributed to excessive risk-taking in the financial sector before 2008.

    **(c)** Modifications to reduce risk-taking:

    - **Restricted stock** instead of options: the CEO owns actual shares, so they lose value when the stock falls. This creates a symmetric payoff.
    - **Clawback provisions:** bonuses are returned if performance reverses within a specified period.
    - **Deferred vesting:** options vest over 3--5 years, preventing the CEO from cashing in after short-term gains.

??? question "Q8. Piece Rates in India's Informal Sector"
    Bidi workers in India are paid approximately Rs. 200 per 1,000 bidis rolled. A skilled worker can roll about 1,000 bidis in a 10-hour day.

    (a) What is the effective hourly wage?
    (b) Is this a "pure" piece-rate system as described in labour economics textbooks? What features are different?
    (c) Why don't competitive forces raise the piece rate, as standard theory would predict?

    **Answer:**

    **(a)** Effective hourly wage = \( \text{Rs. 200} / 10 = \text{Rs. 20/hour} \). This is well below the statutory minimum wage in most Indian states (typically Rs. 350--400/day for unskilled work).

    **(b)** This is **not** a pure piece-rate system as described in textbooks because:

    - Textbook piece rates assume workers can freely choose effort and that the piece rate reflects marginal productivity. Here, the rate is set by contractors/middlemen with monopsony power.
    - Workers bear **all production risk**: defective bidis are rejected without pay, raw materials may be of poor quality, and there is no base wage or safety net.
    - There are no alternative employers or outside options for many home-based bidi workers, violating the competitive labour market assumption.
    - Workers lack access to insurance, healthcare, or benefits --- the "total compensation" is just the piece rate.

    **(c)** Competitive forces fail to raise the piece rate because:

    - **Monopsony power:** Bidi manufacturers and contractors are often the only employers in rural areas. Workers have limited geographic mobility and few alternative skills.
    - **Surplus labour:** An abundance of unskilled workers willing to work at very low wages (Lewis-type unlimited supply of labour) keeps the piece rate at subsistence levels.
    - **Lack of collective bargaining:** Home-based workers are difficult to organise into unions, and existing labour laws often do not cover them.
    - **Tied relationships:** Workers may depend on the contractor for credit, raw materials, and social services, creating a dependency that reduces bargaining power.

??? question "Q9. NREGA and Incentive Design"
    (a) The original NREGA design included both time-rate and piece-rate (task-based) payment options. Why might piece rates be desirable for public works projects?
    (b) In practice, many states moved away from piece rates. What problems might arise with piece-rate payment in public works?
    (c) Imbert and Papp (2015) find that NREGA raised private-sector wages by about 4.7%. Use the efficiency wage framework to explain this spillover.

    **Answer:**

    **(a)** Piece rates are desirable in public works because:

    - They incentivise effort on tasks where output is measurable (metres of road built, cubic metres of earth moved).
    - They prevent shirking on projects where direct supervision is costly (remote rural locations, many dispersed worksites).
    - They tie government expenditure to actual output, improving cost-effectiveness.

    **(b)** Problems with piece rates in public works:

    - **Measurement disputes:** Workers and officials disagree on how much work was completed, leading to payment delays and corruption.
    - **Heterogeneous tasks:** Different soil types, terrain, and weather make it difficult to set fair task norms.
    - **Adverse effects on vulnerable workers:** Older workers, women, and disabled workers may produce less per hour and earn below the minimum wage under piece rates.
    - **Administrative burden:** Measuring and verifying output for thousands of worksites is logistically difficult.

    **(c)** NREGA acts as an **outside option** for rural workers. In the efficiency wage framework, the firm must pay above the worker's best alternative to prevent shirking. When NREGA raises the value of the outside option \( \bar{w} \) (from near-zero to the NREGA wage), private employers must raise wages to maintain the no-shirking condition:

    \[
    w^* = \bar{w} + \text{shirking premium}
    \]

    An increase in \( \bar{w} \) (through NREGA) raises \( w^* \) proportionally. This is the wage spillover: even workers not employed in NREGA benefit because private employers must compete with the NREGA wage floor.

??? question "Q10. Comparing Incentive Mechanisms"
    Complete the following table:

    | Mechanism | Best Suited When... | Key Risk |
    |-----------|-------------------|----------|
    | Piece rates | ? | ? |
    | Efficiency wages | ? | ? |
    | Tournaments | ? | ? |
    | Deferred compensation | ? | ? |

    **Answer:**

    | Mechanism | Best Suited When... | Key Risk |
    |-----------|-------------------|----------|
    | Piece rates | Individual output is easily measurable and quality can be verified | Workers bear income risk; may sacrifice quality for quantity |
    | Efficiency wages | Monitoring is costly and detecting shirking is difficult | Creates involuntary unemployment; above-market wages raise firm costs |
    | Tournaments | Relative performance is easier to measure than absolute; common shocks are large | Sabotage (workers undermine competitors); excessive risk-taking; collusion |
    | Deferred compensation | Long-term employment relationships; specific human capital | Firms may opportunistically fire workers before the "payback" period; requires trust and employment protection |
