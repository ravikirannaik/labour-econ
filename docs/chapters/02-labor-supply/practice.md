---
title: "Practice — Labor Supply"
description: "Practice problems for Borjas Chapter 2 — budget constraints, income and substitution effects, reservation wages, EITC, and Indian LFPR data"
---

# Practice: Labor Supply

**Borjas Chapter 2 | 12 Questions**

These questions cover the neoclassical model of labour supply, from basic budget constraint calculations to policy applications. Click on any question to reveal the answer.

---

## Budget Constraint and Utility Maximization

??? question "Q1. A worker has 110 hours per week available for work and leisure. She earns a wage of Rs. 200 per hour and has non-labour income of Rs. 5,000 per week. (a) Write down her budget constraint. (b) What is her full income? (c) If she chooses to work 40 hours per week, what is her total consumption?"

    **(a) Budget constraint:**

    \[
    C = w(T - L) + V = 200(110 - L) + 5{,}000
    \]

    or equivalently:

    \[
    C = 200h + 5{,}000
    \]

    where \( h = 110 - L \) is hours of work.

    **(b) Full income:**

    \[
    \text{Full income} = wT + V = 200 \times 110 + 5{,}000 = 22{,}000 + 5{,}000 = \text{Rs. }27{,}000
    \]

    This is the maximum she could earn if she worked every available hour plus her non-labour income.

    **(c) Consumption at 40 hours of work:**

    \[
    C = 200 \times 40 + 5{,}000 = 8{,}000 + 5{,}000 = \text{Rs. }13{,}000
    \]

    She has 70 hours of leisure.

??? question "Q2. Using the setup from Q1, suppose the worker's non-labour income increases from Rs. 5,000 to Rs. 10,000 per week (e.g., her spouse gets a raise). Assuming leisure is a normal good, predict the effect on: (a) the budget constraint, (b) hours of work, (c) hours of leisure."

    **(a) Budget constraint:** The budget line shifts **upward (parallel shift)**. The slope remains \( -w = -200 \) (the wage has not changed), but the vertical intercept increases:

    - New intercept at \( L = 0 \): \( C = 200 \times 110 + 10{,}000 = 32{,}000 \) (was 27,000)
    - Intercept at \( L = 110 \): \( C = 10{,}000 \) (was 5,000)

    **(b) Hours of work decrease.** This is a pure income effect. The worker is richer (higher \( V \)) but the wage has not changed, so there is no substitution effect. Since leisure is a normal good, the worker "buys" more leisure.

    **(c) Hours of leisure increase** -- the mirror image of (b).

    This prediction is consistent with the empirical finding that lottery winners and inheritance recipients tend to reduce their labour supply.

??? question "Q3. Suppose the wage rate increases from Rs. 200 to Rs. 300 per hour, with non-labour income unchanged at Rs. 5,000. Decompose the effect on hours of work into the income effect and substitution effect. Under what conditions would hours of work fall?"

    **Substitution effect (SE):** The higher wage makes leisure more expensive (its opportunity cost has risen from 200 to 300). Holding utility constant, the worker substitutes away from leisure toward consumption/work. **SE always increases hours worked.**

    **Income effect (IE):** The higher wage makes the worker richer (full income rises from 27,000 to 38,000). Since leisure is a normal good, the worker wants more leisure. **IE always decreases hours worked** (when leisure is normal).

    **Graphically:** The budget line rotates outward around the point \( (L = 110, C = 5{,}000) \), becoming steeper.

    **Net effect:**

    - If \( |SE| > |IE| \): hours of work **increase** (the worker is on the upward-sloping portion of her supply curve)
    - If \( |IE| > |SE| \): hours of work **decrease** (backward-bending portion)

    **Hours would fall when the income effect dominates.** This is more likely when:

    - The worker is already working many hours (so \( h \) is large, amplifying the income effect term \( h \cdot \partial h / \partial V \))
    - The worker has a strong preference for leisure
    - The worker is already at a high income level

---

## Reservation Wage and Participation

??? question "Q4. A non-working individual has non-labour income of Rs. 15,000 per month. At the point where she consumes all her time as leisure (L = T), her MRS of leisure for consumption is Rs. 150 per hour. (a) What is her reservation wage? (b) Will she participate in the labour market if the market wage is Rs. 120/hour? (c) What if the market wage is Rs. 180/hour?"

    **(a) Reservation wage:**

    \[
    w^* = MRS_{L,C}\Big|_{L=T} = \text{Rs. }150 \text{ per hour}
    \]

    The reservation wage is the MRS evaluated at the endowment point -- it is the minimum wage at which this person would be willing to give up the first hour of leisure.

    **(b) At \( w = 120 < w^* = 150 \):** She does **not** participate. The market wage is below her reservation wage -- the market does not compensate her enough for the first hour of leisure she would give up.

    **(c) At \( w = 180 > w^* = 150 \):** She **does** participate. The market wage exceeds her reservation wage, so working positive hours makes her better off than the corner solution.

??? question "Q5. List three factors that would increase a person's reservation wage (making them less likely to participate in the labour market). For each, explain the mechanism using the work-leisure model."

    1. **Higher non-labour income (\( V \)).** A person with a wealthy spouse, large inheritance, or generous government transfer has higher consumption at the endowment point. If leisure is normal, the marginal utility of consumption \( MU_C \) is lower at the endowment point (diminishing marginal utility), so \( w^* = MU_L / MU_C \) rises. Intuitively, they have less "need" to work for income.

    2. **Presence of young children.** Children increase the value of time spent at home (higher \( MU_L \) at the endowment point), since the "leisure" time now includes childcare, which the parent values highly. This raises \( w^* = MU_L / MU_C \).

    3. **High costs of working** (commuting, childcare costs, uniforms, loss of home production). These costs effectively reduce the net wage the worker receives. If the net wage \( w - \text{costs per hour} \) falls below \( w^* \), the person does not participate. Equivalently, these costs raise the *effective* reservation wage in terms of the gross wage.

    Other valid factors: disability or health limitations (lower productivity of work hours), social norms discouraging work (especially for married women in some cultural contexts), availability of home production substitutes (subsistence farming).

---

## Income and Substitution Effects: Identification

??? question "Q6. For each of the following policy changes, identify the income effect, the substitution effect, and the predicted net effect on hours of work. (a) A proportional income tax is introduced (tax rate t on all earnings). (b) A lump-sum tax of Rs. 2,000 per month is imposed on all workers. (c) Overtime premium: the wage rate doubles for all hours worked beyond 40 per week."

    **(a) Proportional income tax (rate \( t \)):**

    - **Substitution effect:** The after-tax wage falls from \( w \) to \( w(1-t) \), making leisure cheaper. SE: work fewer hours.
    - **Income effect:** The worker is poorer (lower after-tax income for any given hours). Since leisure is a normal good, the worker "buys" less leisure. IE: work more hours.
    - **Net effect: ambiguous.** SE and IE work in opposite directions. Empirically, for most workers, the effects roughly cancel -- labour supply is relatively inelastic with respect to proportional tax changes.

    **(b) Lump-sum tax of Rs. 2,000:**

    - **Substitution effect: none.** The lump-sum tax does not change the wage rate, so the relative price of leisure is unchanged.
    - **Income effect:** The worker is poorer by Rs. 2,000 (non-labour income effectively falls by 2,000). Since leisure is normal, the worker consumes less leisure. IE: work more hours.
    - **Net effect: hours increase** (unambiguously, since only the income effect operates).

    This is why economists generally favour lump-sum taxes over income taxes for efficiency -- lump-sum taxes do not distort the work-leisure choice.

    **(c) Overtime premium (wage doubles beyond 40 hours):**

    This creates a **kinked budget constraint**. For hours 0-40, the wage is \( w \). Beyond 40 hours, the wage is \( 2w \).

    For a worker already working more than 40 hours:

    - **Substitution effect:** The higher marginal wage beyond 40 hours makes leisure more expensive at the margin. SE: work more hours.
    - **Income effect:** The worker is richer (earns more for the same hours). IE: work fewer hours.
    - **Net effect: ambiguous** for hours beyond 40, but the kink makes it likely that some workers cluster at exactly 40 hours.

    For a worker currently working fewer than 40 hours, the overtime premium has no direct effect on their marginal decision (their relevant wage hasn't changed), though the income effect from potentially higher future earnings could matter.

??? question "Q7. 'If leisure is an inferior good, the labour supply curve must be upward-sloping.' Is this statement true or false? Explain."

    **True.** Here is the reasoning:

    If leisure is an inferior good, then an increase in income (holding prices constant) leads the worker to consume *less* leisure -- i.e., work *more* hours. This means the income effect of a wage increase *reinforces* the substitution effect rather than opposing it:

    - **Substitution effect of a wage increase:** always reduces leisure (increases work)
    - **Income effect of a wage increase with inferior leisure:** *also* reduces leisure (increases work)

    Since both effects push in the same direction, a wage increase unambiguously increases hours of work. The supply curve is upward-sloping everywhere -- there is no backward-bending segment.

    However, the empirical evidence strongly suggests that leisure is a **normal** good for most people (hours of work decline when non-labour income increases), so the inferior-leisure case is theoretically possible but empirically unlikely for the general population.

---

## Policy Applications

??? question "Q8. Consider a negative income tax (NIT) with a guaranteed income of Rs. 8,000 per month and a benefit reduction rate of 50%. (a) Write the formula for the NIT transfer. (b) What is the break-even income? (c) For a worker earning Rs. 12,000 per month, what is the transfer? (d) Why does the NIT unambiguously reduce labour supply for workers below the break-even point?"

    **(a) NIT transfer formula:**

    \[
    \text{Transfer} = 8{,}000 - 0.50 \times \text{Earnings}
    \]

    (The transfer equals zero or is positive only when earnings are below the break-even point.)

    **(b) Break-even income:**

    Set Transfer = 0:

    \[
    0 = 8{,}000 - 0.50 \times E^* \implies E^* = \frac{8{,}000}{0.50} = \text{Rs. }16{,}000
    \]

    Workers earning above Rs. 16,000 receive no transfer.

    **(c) Transfer at Rs. 12,000 earnings:**

    \[
    \text{Transfer} = 8{,}000 - 0.50 \times 12{,}000 = 8{,}000 - 6{,}000 = \text{Rs. }2{,}000
    \]

    **(d) Why the NIT unambiguously reduces labour supply:**

    The NIT affects the budget constraint in two ways:

    - **The guaranteed income** \( g = 8{,}000 \) raises non-labour income, generating a pure **income effect** that reduces hours (leisure is normal).
    - **The benefit reduction rate** of 50% reduces the effective wage from \( w \) to \( w(1 - 0.50) = 0.5w \), generating a **substitution effect** that also reduces hours (leisure is now cheaper relative to consumption).

    Since **both** effects reduce hours of work, the NIT unambiguously reduces labour supply for workers below the break-even point. This is a fundamental design problem: any program that provides income to non-workers and phases out benefits as earnings rise will discourage work at the margin.

??? question "Q9. Explain how the Earned Income Tax Credit (EITC) differs from the NIT in its effect on labour supply. Why is the EITC generally considered more effective at encouraging work?"

    The EITC differs from the NIT because it **subsidises earnings** rather than guaranteeing income to non-workers. The EITC has three ranges:

    | Range | Effective wage | Income effect | Substitution effect | Net effect on hours |
    |-------|---------------|---------------|--------------------|--------------------|
    | **Phase-in** | \( w(1+s) > w \) | Richer -- work less | Higher effective wage -- work more | Ambiguous (but strong participation effect) |
    | **Flat** (max credit) | \( w \) (unchanged) | Richer -- work less | None | Work less |
    | **Phase-out** | \( w(1-t) < w \) | Richer -- work less | Lower effective wage -- work less | Unambiguously work less |

    **Key difference from NIT:** The EITC provides **no transfer to non-workers** (you must earn income to get the credit). The phase-in range creates a strong incentive at the **extensive margin** -- it makes the first dollar of earnings worth more than a dollar, pulling non-participants into the labour force.

    **Empirical evidence:** Eissa and Liebman (1996) found that the 1986 EITC expansion increased labour force participation among single mothers by 2.8 percentage points -- a substantial extensive margin response. However, for workers already in the phase-out range, the EITC discourages additional hours, similar to the NIT.

    The EITC is considered more effective at encouraging work because: (1) it targets the subsidy to earners, not non-earners; (2) the extensive margin response (participation) is typically much larger than the intensive margin response (hours); and (3) it avoids the large income effect at zero earnings that the NIT creates.

---

## Indian Context

??? question "Q10. The table below shows female LFPR (usual principal status, age 15+) from the PLFS. Interpret the trend using the income and substitution effects from the work-leisure model."

    | Year | Rural Female LFPR | Urban Female LFPR |
    |------|:-----------------:|:-----------------:|
    | 2017-18 | 24.6% | 20.4% |
    | 2018-19 | 26.4% | 20.4% |
    | 2019-20 | 32.2% | 22.3% |
    | 2020-21 | 35.8% | 23.2% |
    | 2022-23 | 41.5% | 25.4% |

    *Source: PLFS Annual Reports, NSO.*

    **Interpretation using the work-leisure model:**

    **The long decline (pre-2017-18):** India's female LFPR fell from the early 2000s through 2017-18. The work-leisure model suggests this was driven by the **income effect** dominating: as male earnings and household incomes rose, women could "afford" to withdraw from (often arduous, low-paid) work. Social norms reinforced this -- families viewed women's withdrawal from manual labour as a sign of improved status.

    **The recent recovery (2017-18 onwards):** The sharp increase in rural female LFPR may reflect several factors:

    - **Measurement change:** The PLFS switched from the older NSS methodology, and expanded the definition of economic activity to better capture women's unpaid work in household enterprises and agriculture. Part of the "increase" may be statistical.
    - **Economic distress / income effect reversal:** Stagnant or falling rural household incomes (particularly after demonetisation and COVID-19) may have pushed women back into the labour force -- an "added worker" effect at the household level.
    - **Substitution effect from rising education:** As more women complete secondary and higher education, their market wage rises, making the substitution effect stronger and tipping the participation decision.
    - **NREGA and self-employment:** Government programs and the expansion of self-help groups may have lowered entry barriers.

    The urban-rural gap is consistent with the model: rural women face lower wages and fewer job opportunities (weaker substitution effect), but also face greater economic distress during downturns (stronger income effect pushing them into work).

??? question "Q11. A rural Indian household has one adult male member who works as a farm labourer earning Rs. 250/day and one adult female member who does not participate in the labour market. NREGA is introduced, offering Rs. 300/day for 100 days/year. Using the concepts of reservation wage and the budget constraint, explain how NREGA might affect the female member's participation decision."

    **Before NREGA:**

    The female member's reservation wage \( w^*_f \) exceeds the market wage available to her (say Rs. 150-200/day for casual agricultural work). She remains out of the labour force.

    **After NREGA:**

    NREGA affects her participation through two channels:

    **1. Direct effect (if she can access NREGA work):** NREGA offers Rs. 300/day, which may exceed her reservation wage. If \( 300 > w^*_f \), she enters the labour force. NREGA effectively shifts the **available market wage** above her reservation wage.

    **2. Indirect effect through the husband's wage:** NREGA pushes up private-sector rural wages (empirically, by about 4-5%). If the husband's wage rises from Rs. 250 to, say, Rs. 270/day, the household's non-labour income (from the wife's perspective) rises. This is an **income effect** that raises her reservation wage, potentially keeping her out. However, if NREGA work is directly available to her and the NREGA wage exceeds her (now slightly higher) reservation wage, the direct effect dominates.

    **Empirically:** Azam (2012) and others find that NREGA **increased** female LFPR, particularly in states with strong implementation. This suggests the direct wage effect (making market wages exceed reservation wages for many women) dominated the indirect income effect through the husband's higher earnings.

    The key insight is that NREGA changed the **constraint set** -- it offered a new employment option that many women had not previously had access to. In terms of the budget constraint, it created a new segment at \( w = 300 \) for up to 100 days, which the woman could now optimise over.

---

## Stata Application

??? question "Q12. Using a hypothetical PLFS-like dataset, write Stata commands to: (a) compute the LFPR by gender for the working-age population (age 15+), and (b) tabulate LFPR by education level for women. Explain what patterns you would expect to find."

    !!! stata "Stata Commands"

        ```stata
        * Load the PLFS person-level dataset
        use plfs_person_2024.dta, clear

        * (a) LFPR by gender
        * Assume: age = age in years
        *         sex = 1 (male), 2 (female)
        *         usual_status = usual principal activity status
        *         (codes 11-51 = employed, 81 = unemployed seeking,
        *          91-97 = not in labour force)

        * Generate working-age indicator
        gen working_age = (age >= 15)

        * Generate labour force indicator
        gen in_lf = inrange(usual_status, 11, 81) if working_age == 1

        * Tabulate LFPR by gender (using survey weights)
        tab sex in_lf [aw=weight] if working_age == 1, row nofreq

        * (b) LFPR by education for women
        * Assume: education = 1 (illiterate), 2 (primary), 3 (middle),
        *         4 (secondary), 5 (higher secondary), 6 (graduate+)

        tab education in_lf [aw=weight] if sex == 2 & working_age == 1, row nofreq
        ```

    **Expected patterns:**

    **(a) LFPR by gender:** Male LFPR should be around 75-78%, female LFPR around 35-40% (usual principal status, PLFS 2023-24). The gender gap of ~40 percentage points is one of the largest in the world.

    **(b) Female LFPR by education:** We expect a **U-shaped or J-shaped pattern**:

    | Education level | Expected female LFPR | Reasoning |
    |----------------|---------------------|-----------|
    | Illiterate | High (~40-50%) | Economic necessity; agricultural/manual work |
    | Primary/Middle | Lower (~25-35%) | Income effect from household's rising income; few suitable jobs |
    | Secondary | Lowest (~20-25%) | Income effect dominates; social norms against women's work |
    | Higher secondary | Slightly higher (~25-30%) | Beginning of substitution effect |
    | Graduate+ | Highest (~50-60%) | Strong substitution effect; white-collar opportunities; changed norms |

    This U-shape in education mirrors the cross-country U-shape in development: at low and high education levels, women participate; at intermediate levels, the income effect (and social norms) dominate.

---

*These practice problems cover the main concepts from Borjas Chapter 2. For additional resources, see the [Resources](resources.md) page.*
