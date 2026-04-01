---
title: "Labor Supply"
description: "The neoclassical model of labour supply — work-leisure choice, income and substitution effects, and applications — Borjas Chapter 2"
---

# 2. Labor Supply

**Borjas Chapter 2 | 5 lecture hours**

> *"How many hours are you willing to work? The answer to that question depends on how much you are getting paid."* -- George J. Borjas, *Labor Economics*, 8th ed.

Labour supply is about the decisions workers make: whether to participate in the labour market at all, and if so, how many hours to work. These are among the most consequential decisions a person makes, shaping income, consumption, leisure, health, and family life. This chapter develops the neoclassical model of labour supply -- a framework built on utility maximization that generates surprisingly rich predictions about how wages, taxes, and government programs affect work behaviour.

---

## The Work-Leisure Framework

The starting point is a simple but powerful idea: workers have a fixed amount of time and must choose how to allocate it between **work** (which generates income) and **leisure** (which generates direct utility).

!!! model "Setup of the Model"

    A worker has:

    - \( T \) = total hours available (e.g., 168 hours per week, or a normalised "time endowment")
    - \( L \) = hours of leisure consumed
    - \( h = T - L \) = hours of work
    - \( w \) = the hourly wage rate
    - \( V \) = non-labour income (dividends, transfers, spouse's income, etc.)

    The worker chooses \( L \) (or equivalently \( h \)) to maximise utility \( U(C, L) \), where \( C \) is a composite consumption good, subject to a budget constraint.

---

## The Budget Constraint

The worker's budget constraint states that consumption spending equals labour income plus non-labour income:

\[
C = w(T - L) + V = wh + V
\]

This can be rearranged as:

\[
C + wL = wT + V
\]

!!! model "Interpreting the Budget Constraint"

    The right-hand side, \( wT + V \), is called **full income** -- the maximum income the worker could earn if they worked every available hour, plus non-labour income. The left-hand side shows how full income is "spent": on consumption goods (\( C \)) and on leisure, where the **price of leisure is the wage rate** \( w \).

    This is a key insight: **the wage rate is simultaneously the reward for working and the opportunity cost of not working.** An hour of leisure "costs" \( w \) in foregone earnings.

**Graphically,** the budget constraint is a straight line in \( (L, C) \) space:

- **Horizontal intercept:** \( L = T \), \( C = V \) (the worker consumes all time as leisure and lives on non-labour income)
- **Vertical intercept:** \( L = 0 \), \( C = wT + V \) (the worker works every available hour)
- **Slope:** \( -w \) (the wage rate determines the trade-off between leisure and consumption)

An increase in \( w \) **rotates the budget line outward** around the point \( (T, V) \), making it steeper. An increase in \( V \) **shifts the budget line upward** in a parallel fashion.

---

## Indifference Curves and Preferences

The worker has preferences over consumption and leisure, represented by indifference curves. We assume:

- **More is better:** workers prefer more consumption and more leisure (both are "goods").
- **Diminishing marginal rate of substitution:** indifference curves are convex to the origin. As a worker gets more leisure, the amount of consumption they are willing to give up for one more hour of leisure declines.
- **Different workers have different preferences:** some are "workaholics" (steep indifference curves -- they need a lot of consumption to compensate for lost leisure); others are "leisure lovers" (flat indifference curves).

!!! model "The Marginal Rate of Substitution (MRS)"

    The **marginal rate of substitution** of leisure for consumption is:

    \[
    MRS_{L,C} = \frac{MU_L}{MU_C}
    \]

    where \( MU_L \) is the marginal utility of leisure and \( MU_C \) is the marginal utility of consumption. The MRS measures how much consumption the worker is willing to sacrifice for one more hour of leisure while remaining equally well off. Graphically, it is the (absolute) slope of the indifference curve.

---

## The Optimal Labour Supply Decision

The worker maximises utility by choosing the point on the budget constraint that lies on the highest attainable indifference curve.

!!! model "Interior Solution: The Tangency Condition"

    At an **interior optimum** (where the worker works positive hours), the indifference curve is tangent to the budget line:

    \[
    MRS_{L,C} = w
    \]

    In words: **the marginal value of leisure (in terms of consumption) equals the wage rate.** The worker works up to the point where the subjective value of one more hour of leisure exactly equals the market price of that hour.

    Equivalently, the worker works until the marginal benefit of working one more hour (earning \( w \) more in consumption) equals the marginal cost (giving up one more hour of leisure, valued at \( MRS \) units of consumption).

---

## The Reservation Wage

Not everyone works. Some individuals are at a **corner solution** where \( L = T \) and \( h = 0 \) -- they choose not to participate in the labour market.

!!! model "The Reservation Wage"

    The **reservation wage** \( w^* \) is the minimum wage that would induce a non-participant to enter the labour force. Formally, it is the MRS evaluated at the point \( (L = T, C = V) \) -- the endowment point where the worker consumes all their time as leisure:

    \[
    w^* = MRS_{L,C} \Big|_{L=T, C=V} = \frac{MU_L(T, V)}{MU_C(T, V)}
    \]

    **Decision rule:**

    - If the market wage \( w > w^* \): the person enters the labour force (works positive hours).
    - If the market wage \( w \leq w^* \): the person does not participate.

    The reservation wage is higher for persons who value leisure more (e.g., those with young children), who have more non-labour income (e.g., a wealthy spouse), or who face high costs of working (e.g., commuting, childcare).

---

## Income Effect and Substitution Effect

The most important analytical tool in this chapter is the decomposition of the response to a wage change into two components.

!!! model "Decomposing a Wage Increase"

    When the wage rises from \( w_0 \) to \( w_1 \):

    **1. Substitution effect:** Holding utility constant, a higher wage makes leisure more expensive relative to consumption. The worker substitutes away from leisure toward work. **The substitution effect always increases hours of work** (reduces leisure) when the wage rises.

    **2. Income effect:** A higher wage makes the worker richer (they can afford more of everything). Since leisure is a normal good, the worker "buys" more leisure -- i.e., works fewer hours. **The income effect always reduces hours of work** (increases leisure) when the wage rises, provided leisure is a normal good.

    The **net effect** depends on which force dominates:

    | Condition | Net effect of wage increase on hours |
    |-----------|--------------------------------------|
    | Substitution effect > Income effect | Hours of work **increase** |
    | Income effect > Substitution effect | Hours of work **decrease** |
    | Effects exactly offset | Hours unchanged |

    Formally, using the Slutsky equation:

    \[
    \frac{\partial h}{\partial w} = \underbrace{\frac{\partial h}{\partial w}\bigg|_{U=\bar{U}}}_{\text{Substitution effect } (> 0)} + \underbrace{h \cdot \frac{\partial h}{\partial V}}_{\text{Income effect } (< 0 \text{ if leisure is normal})}
    \]

This decomposition is not merely theoretical -- it is the key to understanding why labour supply elasticities differ across groups and why certain policies have counterintuitive effects.

---

## The Backward-Bending Labour Supply Curve

The income-substitution decomposition implies that the individual labour supply curve need not be upward-sloping everywhere.

- At **low wages**, the substitution effect tends to dominate: a wage increase raises hours supplied. The supply curve slopes upward.
- At **high wages**, the income effect may dominate: the worker is already earning well and values additional leisure more than additional income. A wage increase reduces hours supplied. The supply curve bends backward.

!!! empirical "Is the Labour Supply Curve Really Backward-Bending?"

    The backward-bending supply curve is not just a theoretical curiosity. There is considerable evidence that:

    - **For prime-age men,** labour supply is quite inelastic -- wage changes have small effects on hours. The income and substitution effects roughly cancel out. Estimated elasticities are close to zero or slightly negative.

    - **For married women,** labour supply is more elastic, particularly at the extensive margin (whether to participate at all). This is because many married women are near the participation margin, so wage changes can tip the decision.

    - **Over the long run,** the backward-bending curve is evident in historical data: as real wages rose over the 20th century, the average workweek fell from ~60 hours to ~34 hours, consistent with the income effect dominating at the economy-wide level.

---

## The Added Worker Effect and the Discouraged Worker Effect

Two phenomena link individual labour supply decisions to the business cycle.

!!! model "Cyclical Effects on Labour Force Participation"

    **Added worker effect:** When one household member (typically the primary earner) loses their job during a recession, other household members (typically the spouse) may enter the labour force to compensate for the lost income. This is an income effect: the fall in household non-labour income (from the spouse's perspective, \( V \) has fallen) increases the incentive to work.

    **Discouraged worker effect:** During a recession, market wages fall and job-finding probabilities decline. Some workers, concluding that no suitable job is available, **drop out of the labour force entirely**. The market wage has effectively fallen below their reservation wage.

    **Which dominates?** Empirically, the discouraged worker effect typically dominates, so the labour force tends to *shrink* during recessions. However, the added worker effect is important for understanding within-household dynamics and is particularly relevant in developing economies where formal safety nets are weak.

---

## Elasticity of Labour Supply

The responsiveness of labour supply to wage changes is measured by the **wage elasticity of labour supply**:

!!! model "Labour Supply Elasticity"

    \[
    \varepsilon = \frac{\% \Delta h}{\% \Delta w} = \frac{\partial h}{\partial w} \cdot \frac{w}{h}
    \]

    - \( \varepsilon > 0 \): substitution effect dominates (upward-sloping portion of supply curve)
    - \( \varepsilon < 0 \): income effect dominates (backward-bending portion)
    - \( \varepsilon = 0 \): perfectly inelastic (vertical supply curve)

    Two distinctions matter:

    - **Extensive margin elasticity:** responsiveness of the *participation decision* (whether to work at all)
    - **Intensive margin elasticity:** responsiveness of *hours worked* conditional on participation

!!! empirical "Estimated Labour Supply Elasticities"

    The empirical literature, surveyed by Blundell and MaCurdy (1999) and Chetty et al. (2011), finds:

    | Group | Intensive margin | Extensive margin |
    |-------|-----------------|-----------------|
    | Prime-age men | ~0.1 (very inelastic) | ~0.0 (almost all participate) |
    | Married women | ~0.2 | ~0.5-0.8 (more elastic) |
    | Single mothers | ~0.1-0.3 | ~0.5-1.0 (most elastic) |
    | Elderly workers | -- | High (retirement margin) |

    The key insight is that **the groups most affected by tax and transfer policies are those with the largest extensive margin elasticities** -- typically married women and single mothers.

---

## Application: Income Maintenance Programs

The work-leisure model provides a unified framework for analysing how government transfer programs affect labour supply.

### The Negative Income Tax (NIT)

!!! policy "The Negative Income Tax"

    A negative income tax provides a **guaranteed income** \( g \) to those with no earnings, and reduces the transfer at a **benefit reduction rate** (or "tax rate") \( t \) as earnings rise:

    \[
    \text{Transfer} = g - t \cdot (wh)
    \]

    The transfer reaches zero when earnings equal \( g/t \), the **break-even point.**

    **Effects on labour supply:**

    1. **Income effect of the guarantee:** The guaranteed income \( g \) raises non-labour income \( V \), which reduces labour supply (leisure is a normal good).

    2. **Substitution effect of the tax rate:** The benefit reduction rate \( t \) reduces the effective wage from \( w \) to \( w(1-t) \), making work less attractive at the margin. This also reduces labour supply.

    **Both effects work in the same direction: the NIT unambiguously reduces labour supply** (on the working side of the break-even point). This was confirmed by the US income maintenance experiments of the 1970s (SIME-DIME), which found significant reductions in hours worked.

### The Earned Income Tax Credit (EITC)

!!! policy "The Earned Income Tax Credit"

    The EITC is designed to "make work pay." Unlike the NIT, it *subsidises* earnings over a range:

    - **Phase-in range:** Earnings are subsidised at rate \( s \). Effective wage = \( w(1+s) \). Both income and substitution effects encourage work.
    - **Flat range:** The maximum credit is received regardless of additional earnings. Only an income effect (discouraging work at the margin) operates.
    - **Phase-out range:** The credit is gradually withdrawn at rate \( t \). Effective wage = \( w(1-t) \). Both income and substitution effects discourage hours.

    The EITC has a strong effect on the **extensive margin** -- drawing non-participants into the labour force -- because the phase-in subsidises the first dollar earned. Eissa and Liebman (1996) found that the 1986 EITC expansion significantly increased labour force participation among single mothers.

    But the effects on the **intensive margin** (hours for those already working) are ambiguous and depend on where the worker is located in the schedule. Workers in the phase-out range face both a higher income (reducing hours) and a lower effective wage (also reducing hours).

---

## India's Labour Supply: Gender and Participation

!!! indian "Female Labour Force Participation in India: The U-Shaped Hypothesis"

    One of the most debated questions in Indian labour economics is why female LFPR is so low and whether it follows a U-shape with respect to economic development.

    **The U-shaped hypothesis** (Goldin, 1995; Klasen and Pieters, 2015) suggests that as countries develop:

    1. **At low income levels,** women participate heavily in agriculture and household enterprises out of economic necessity. LFPR is high.
    2. **At middle income levels,** rising household incomes allow families to withdraw women from the labour force (income effect), social norms about women working outside the home become binding, and the decline of home-based production reduces female employment opportunities. LFPR falls.
    3. **At high income levels,** rising female education shifts preferences and social norms, expanding white-collar job opportunities pull women back in, and declining fertility rates reduce the time cost of childcare. LFPR rises again.

    **Where is India on the U?** India appears to be near the bottom of the U. PLFS data show that:

    - Rural female LFPR has shown some recovery in recent years (from a low of ~18% in 2017-18 in current weekly status to about 28-30% by 2023-24), though measurement and definitional changes complicate trend analysis.
    - Urban female LFPR has been more stable at around 20-25%.
    - Education has a non-monotonic effect: LFPR falls with education up to the secondary level (as the income effect pulls women out), then rises sharply for women with graduate and above education (as labour market opportunities improve).

    The work-leisure framework helps organise these facts: rising household income (from male earnings growth) generates an income effect reducing female LFPR, while rising female education and wages generate substitution effects that eventually pull LFPR back up.

!!! policy "NREGA as a Labour Supply Shifter"

    The Mahatma Gandhi National Rural Employment Guarantee Act (NREGA), introduced in 2006, provides a guarantee of 100 days of unskilled manual work per year to every rural household at the statutory minimum wage.

    From a labour supply perspective, NREGA operates through multiple channels:

    - **Reservation wage effect:** NREGA effectively raises the reservation wage in rural areas. Workers who might have accepted private employment at very low wages during the lean season can now fall back on NREGA, which puts upward pressure on private-sector wages.

    - **Participation effect:** NREGA draws marginal workers (especially women) into the labour force. Female participation in NREGA has been substantial -- about 50-60% of person-days in some states.

    - **Seasonal smoothing:** By providing work during agricultural lean seasons, NREGA reduces the seasonal fluctuation of labour supply and earnings. This is an important departure from the static model -- in practice, labour supply decisions are dynamic and seasonal.

    Empirical evidence supports these channels. Imbert and Papp (2015) find that NREGA raised private-sector wages by 4-5% in early-implementation districts. Azam (2012) finds significant increases in female LFPR in districts with high NREGA exposure.

---

## Key Takeaways

1. The neoclassical labour supply model frames the work decision as a **utility-maximizing choice between consumption and leisure**, subject to a budget constraint \( C = w(T-L) + V \).

2. The **price of leisure is the wage rate** -- an hour of leisure costs \( w \) in foregone earnings.

3. At an interior optimum, the worker equates the **MRS of leisure for consumption to the wage rate**: \( MRS = w \).

4. The **reservation wage** is the minimum wage that induces participation. Persons with high reservation wages (e.g., due to high non-labour income or strong preference for leisure) may choose not to work.

5. A wage increase has two opposing effects: a **substitution effect** (leisure is more expensive, so work more) and an **income effect** (richer, so consume more leisure). The net effect is ambiguous, producing the **backward-bending supply curve**.

6. Labour supply elasticities are **small for prime-age men** but **substantial for married women and single mothers**, especially at the extensive margin.

7. Transfer programs like the **NIT unambiguously reduce labour supply** (both income and substitution effects discourage work), while the **EITC has mixed effects** but is effective at increasing participation at the extensive margin.

8. In India, female LFPR is shaped by the tension between **income effects** (rising household income pulling women out) and **substitution effects** (rising education and wages pulling them in), consistent with the **U-shaped hypothesis**. NREGA acts as a **reservation wage floor** in rural labour markets.

---

[:octicons-arrow-left-24: Previous: Introduction](../01-introduction/index.md){ .md-button } [:octicons-arrow-right-24: Next: Labor Demand](../03-labor-demand/index.md){ .md-button }
