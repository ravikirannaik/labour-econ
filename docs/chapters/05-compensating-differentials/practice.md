---
title: "Practice — Compensating Wage Differentials"
---

# Practice: Compensating Wage Differentials

Test your understanding of hedonic wage theory, the value of a statistical life, and the economics of job amenities. Click on a question to reveal the answer.

---

??? question "Q1. What is a compensating wage differential, and what assumption about labour markets is necessary for it to arise?"

    A **compensating wage differential** is a wage premium (or penalty) that arises to compensate workers for undesirable (or desirable) non-wage characteristics of a job. For example, a dangerous job pays more than an otherwise identical safe job.

    The key assumptions are:

    1. **Workers have full information** about job characteristics (including risks).
    2. **Workers are mobile** --- they can freely move between jobs.
    3. **The labour market is competitive** --- neither firms nor workers have market power.

    Under these conditions, utility-maximising workers sort across jobs, and the wage differential adjusts until the marginal worker is indifferent between the two jobs.

??? question "Q2. Draw and explain the hedonic wage function. Why is it generally upward-sloping in wage-risk space?"

    The hedonic wage function \(w(\rho)\) plots the equilibrium wage against the probability of injury \(\rho\) across all jobs in the market.

    It is **upward-sloping** because workers dislike risk. To attract workers to riskier jobs, firms must offer higher wages. Formally, since \(\partial U / \partial \rho < 0\), workers require \(dw/d\rho > 0\) to maintain the same utility level.

    The function is the **envelope** of tangency points between worker indifference curves and firm isoprofit curves. Each point on the function represents a different worker-firm match. It does not trace out any single worker's preferences or any single firm's cost structure.

??? question "Q3. Worker A is highly risk-averse and Worker B is relatively risk-tolerant. Both face the same hedonic wage function. Who ends up in the riskier job, and who earns the higher wage?"

    **Worker B** (risk-tolerant) ends up in the riskier job and earns a higher wage. Worker B has a relatively flat indifference curve --- she does not require a large wage increase per unit of additional risk. She is therefore matched with a firm offering a risky, high-wage job.

    **Worker A** (risk-averse) has a steep indifference curve and matches with a safer, lower-wage job. Worker A accepts the lower wage because she places a high value on safety.

    Both workers are on the same hedonic wage function \(w(\rho)\), but at different points. The key insight is that **sorting** by risk preferences determines the allocation of workers to jobs.

??? question "Q4. A firm can make its workplace safer by investing in safety equipment. Explain how this investment affects the firm's isoprofit curve in wage-risk space."

    A firm's isoprofit curve shows combinations of \((w, \rho)\) that yield the same profit. If the firm invests in safety (reducing \(\rho\)), it incurs additional costs, so it must reduce the wage it offers to maintain the same profit. The isoprofit curve therefore slopes **upward**: higher \(\rho\) allows higher \(w\).

    The curve is typically **concave** because: the first units of risk reduction are cheap (easy safety measures), but further reductions become increasingly expensive. This means the firm must cut wages by larger amounts for each additional unit of safety.

    Firms with **low-cost safety technology** have flatter isoprofit curves (they can cheaply provide safe workplaces). Firms where safety is inherently expensive have steeper curves. In equilibrium, low-cost safety firms match with risk-averse workers.

??? question "Q5. Workers at a chemical plant earn Rs 5,000 per month more than similar workers at a nearby textile mill. The chemical plant has an annual fatality risk of 3 per 10,000 workers, while the textile mill has a risk of 1 per 10,000. Calculate the implied VSL."

    The wage differential is Rs 5,000/month = Rs 60,000/year.

    The risk differential is \(\Delta \rho = (3 - 1) / 10{,}000 = 2 / 10{,}000 = 0.0002\).

    \[
    \text{VSL} = \frac{\Delta w}{\Delta \rho} = \frac{60{,}000}{0.0002} = \text{Rs } 30{,}00{,}00{,}000 = \text{Rs 30 crore}
    \]

    This means that workers collectively value the prevention of one statistical death at Rs 30 crore. Note: this is the implied VSL from the revealed preferences of workers at the margin of switching between these two jobs.

??? question "Q6. A government safety regulation reduces the annual fatality risk at factories from 5/10,000 to 2/10,000. The regulation costs Rs 100 crore per year and affects 1 million workers. Using a VSL of Rs 20 crore, should the regulation be implemented?"

    **Step 1: Calculate lives saved.**

    Risk reduction per worker: \(\Delta \rho = (5 - 2) / 10{,}000 = 0.0003\)

    Expected lives saved: \(1{,}000{,}000 \times 0.0003 = 300\) statistical lives per year.

    **Step 2: Calculate benefits.**

    Benefits = Lives saved \(\times\) VSL = \(300 \times \text{Rs 20 crore} = \text{Rs 6,000 crore}\)

    **Step 3: Compare costs and benefits.**

    Benefits (Rs 6,000 crore) \(>\) Costs (Rs 100 crore).

    **Yes**, the regulation should be implemented. The benefit-cost ratio is 60:1, indicating a highly cost-effective intervention.

    **Caveat:** This analysis assumes the VSL estimate is appropriate for this population and that the risk reduction is correctly estimated. It also assumes the regulation is effectively enforced.

??? question "Q7. Explain why the hedonic wage function does not trace out any single worker's indifference curve. What identification problem does this create for empirical researchers?"

    The hedonic wage function is the **market envelope** --- the locus of tangency points between different workers' indifference curves and different firms' isoprofit curves. Each point on the function corresponds to a **different** worker-firm match.

    This creates the **Rosen identification problem**: observing the hedonic wage function tells us the equilibrium wage-risk tradeoff, but it does not directly reveal the structural demand (worker preferences) or structural supply (firm cost) functions.

    To identify the slope of the hedonic wage function (and thus the VSL), researchers regress wages on risk and controls:

    \[
    w_i = \alpha + \beta \rho_i + \mathbf{X}_i \gamma + \varepsilon_i
    \]

    The coefficient \(\beta\) estimates the compensating differential per unit of risk. But this is the slope of the **market equilibrium** locus, not the worker's willingness to pay for risk. To recover structural preferences, one would need to observe the same worker choosing between different risk levels at different wages, or use an instrumental variables strategy.

??? question "Q8. List three reasons why compensating differentials may fail to emerge in practice, even in a developed-country labour market."

    1. **Imperfect information:** Workers may not know the true risks of their jobs. If workers underestimate the probability of injury, they will not demand adequate compensation. Studies show that workers' perceptions of risk often differ substantially from objective data.

    2. **Barriers to mobility:** If workers cannot easily switch jobs (due to geographic immobility, firm-specific human capital, search costs, or non-compete agreements), they cannot "vote with their feet." Firms then face less competitive pressure to pay risk premiums.

    3. **Omitted variable bias:** If dangerous jobs are systematically held by low-skill or disadvantaged workers (who have fewer outside options), the observed wage-risk relationship may be confounded. The regression may attribute a low compensating differential to the risk variable when in fact the low wage reflects the workers' low bargaining power.

    Additional reasons include: monopsony power (firms setting wages below competitive levels), collective bargaining that compresses wage differentials, and compensating variation occurring through non-wage benefits (health insurance, pensions) rather than through wages.

??? question "Q9. Explain why manual scavenging in India contradicts the predictions of compensating wage differential theory. What labour market features account for this?"

    The theory predicts that extremely hazardous jobs --- like manual scavenging, which involves cleaning sewers and septic tanks and carries a high risk of death from toxic gas inhalation --- should pay a **large compensating premium** to attract workers.

    In reality, manual scavengers earn very low wages, often less than the minimum wage. This contradicts the theory because several key assumptions are violated:

    1. **Occupational segregation by caste:** Manual scavenging is performed almost exclusively by Dalits (Scheduled Castes). Caste norms and social exclusion restrict their access to alternative employment, so they cannot "choose" a safer job.

    2. **Labour market segmentation:** The informal sector in which these workers operate is disconnected from the formal labour market. Workers cannot freely sort across the entire job distribution.

    3. **Information asymmetry:** Workers may lack full awareness of the specific health risks (long-term effects of hydrogen sulphide exposure) even if they recognise the immediate danger.

    4. **Monopsony/exploitation:** With limited outside options, workers have no bargaining power. Municipal contractors can offer subsistence wages for highly dangerous work.

    This case illustrates a fundamental limitation of the hedonic model: it assumes competitive markets with free mobility, but discrimination and social stratification can create profound market failures.

??? question "Q10. A company offers two compensation packages: (A) Rs 50,000/month with a 50-hour work week, no flexibility; (B) Rs 42,000/month with a 40-hour work week and work-from-home option. Use the compensating differentials framework to explain this wage gap."

    The Rs 8,000/month difference is a **compensating differential** for job amenities. Package A requires longer hours and no flexibility (an undesirable characteristic), so it must offer higher wages to attract workers. Package B offers desirable amenities --- shorter hours and work-from-home flexibility --- and workers are willing to accept a lower wage for these benefits.

    In the hedonic framework, the amenity (flexibility) is a job characteristic that enters workers' utility functions positively. Along the hedonic wage function, jobs with better amenities offer lower wages:

    \[
    \frac{\partial w}{\partial (\text{flexibility})} < 0
    \]

    The observed wage gap of Rs 8,000 reflects the **market's implicit price of flexibility**. Workers who value flexibility highly will choose Package B (accepting the wage cut). Workers who prioritise income will choose Package A.

    **Important nuance:** The Rs 8,000 gap is the equilibrium price of flexibility, which depends on both the supply of flexible jobs (how costly it is for firms to offer flexibility) and the demand for flexibility (how much workers value it). If remote work becomes easier to provide (lower cost to firms), we would expect the compensating differential to shrink.

---

<div style="display: flex; justify-content: space-between; margin-top: 2rem;">
<a href="../05-compensating-differentials/">:material-arrow-left: Chapter Content</a>
<a href="../05-compensating-differentials/resources/">Resources :material-arrow-right:</a>
</div>
