---
title: "Labor Demand"
---

# 3. Labor Demand

<span class="chapter-tag hours-tag">5 Hours</span> <span class="chapter-tag borjas-tag">Borjas Ch. 3</span>

In the previous chapter we asked: *How do workers decide whether and how much to work?* Now we flip the question: **How do firms decide how many workers to hire?** The theory of labour demand is, at its core, a theory of the firm. A profit-maximizing employer will keep hiring workers as long as each additional worker adds more to revenue than to cost. This simple insight---the marginal productivity condition---is the foundation of everything in this chapter.

---

## The Firm's Production Function

A **production function** describes the technological relationship between inputs and output. In the simplest case with two inputs---labour (\(L\)) and capital (\(K\))---we write:

\[
q = f(L, K)
\]

where \(q\) is output. The production function is assumed to exhibit:

- **Positive marginal products**: Adding more of either input increases output.
- **Diminishing marginal returns**: Holding one input fixed, the marginal product of the other input eventually declines.

!!! model "Key Concept: Marginal Product of Labour"
    The **marginal product of labour (MPL)** is the change in output resulting from hiring one additional worker, holding capital constant:

    \[
    MP_L = \frac{\partial f(L, K)}{\partial L}
    \]

    The law of diminishing returns implies that \(MP_L\) eventually decreases as \(L\) increases (holding \(K\) fixed). Intuitively, if a factory has 10 machines, the 5th worker adds more output than the 50th, because the later workers have fewer machines to work with.

The **average product of labour** is \(AP_L = q / L\). It is useful for comparing productivity across firms or over time, but the *marginal* product is what drives hiring decisions.

---

## Short-Run Labour Demand

In the short run, at least one factor of production is fixed---typically capital. The firm can adjust only how much labour it employs.

### Profit Maximization in the Short Run

A competitive firm takes both the output price (\(p\)) and the wage (\(w\)) as given. Its profit is:

\[
\pi = p \cdot q - w \cdot L - r \cdot K
\]

where \(r\) is the rental rate of capital. Since \(K\) is fixed in the short run, the firm chooses \(L\) to maximise profit. Taking the first-order condition:

\[
\frac{\partial \pi}{\partial L} = p \cdot MP_L - w = 0
\]

!!! model "The Marginal Productivity Condition"
    A profit-maximizing firm hires labour up to the point where the **value of the marginal product of labour (VMP\(_L\))** equals the wage:

    \[
    VMP_L = p \times MP_L = w
    \]

    This condition says: the revenue from the last worker hired must exactly equal the cost of hiring that worker. If \(VMP_L > w\), the firm can increase profit by hiring more. If \(VMP_L < w\), the firm is paying more for the last worker than that worker produces, and profit rises by hiring fewer.

### Deriving the Short-Run Demand Curve

Because of diminishing returns, \(MP_L\) (and therefore \(VMP_L\)) declines as employment increases. This means the \(VMP_L\) curve is **downward-sloping** in \((L, w)\) space. The firm's short-run labour demand curve *is* the downward-sloping portion of its \(VMP_L\) curve.

**Shifts in labour demand** occur when:

- **Output price rises**: \(VMP_L = p \times MP_L\) shifts up --- the firm demands more labour at every wage.
- **Technology improves**: Higher \(MP_L\) at each level of employment shifts demand outward.
- **Capital stock increases**: May raise \(MP_L\) (if capital and labour are complements), shifting demand outward.

---

## Long-Run Labour Demand

In the long run, the firm can adjust **both** labour and capital. The hiring decision now involves choosing the cost-minimizing combination of inputs to produce a given level of output.

### Isoquants and Isocosts

An **isoquant** shows all combinations of \(L\) and \(K\) that produce the same level of output \(\bar{q}\). It is analogous to an indifference curve in consumer theory. Isoquants are convex to the origin, reflecting diminishing marginal rates of technical substitution.

!!! model "Marginal Rate of Technical Substitution"
    The **MRTS** is the rate at which the firm can substitute labour for capital while keeping output constant:

    \[
    MRTS_{LK} = -\frac{dK}{dL}\bigg|_{q=\bar{q}} = \frac{MP_L}{MP_K}
    \]

    It is the slope of the isoquant. A diminishing MRTS (the isoquant flattens as we move right) means it becomes progressively harder to substitute labour for capital.

An **isocost line** shows all combinations of \(L\) and \(K\) that the firm can purchase for a given total cost \(C\):

\[
C = wL + rK \quad \Longrightarrow \quad K = \frac{C}{r} - \frac{w}{r}L
\]

The slope of the isocost line is \(-w/r\), the relative price of labour to capital.

### Cost Minimization

The firm minimizes cost by choosing the input combination where the isoquant is tangent to the lowest possible isocost line. At the tangency:

\[
\frac{MP_L}{MP_K} = \frac{w}{r}
\]

This can be rewritten as:

\[
\frac{MP_L}{w} = \frac{MP_K}{r}
\]

!!! model "The Last-Dollar Rule"
    Cost minimization requires that the last dollar spent on labour yields exactly the same additional output as the last dollar spent on capital. If \(MP_L / w > MP_K / r\), the firm can reduce cost by using more labour and less capital.

---

## Substitution and Scale Effects

When the wage changes in the long run, two distinct effects determine the firm's response.

### The Substitution Effect

A higher wage makes labour relatively more expensive than capital. The firm substitutes away from labour toward capital, moving along the *same* isoquant. This effect **always reduces** the quantity of labour demanded when the wage rises.

### The Scale Effect

A higher wage raises the firm's marginal cost of production. With higher costs, the firm produces less output, which reduces its demand for *all* inputs, including labour. The scale effect also **reduces** the quantity of labour demanded when the wage rises.

!!! model "Why Long-Run Demand Is More Elastic"
    In the short run, only the substitution effect is absent (capital is fixed), and the firm adjusts along its \(VMP_L\) curve. In the long run, **both** the substitution and scale effects operate, so the long-run labour demand curve is **flatter** (more elastic) than the short-run curve. The firm has more ways to economize on expensive labour when it can also adjust its capital stock.

---

## The Elasticity of Labour Demand

The **own-wage elasticity of labour demand** measures the percentage change in employment for a one-percent change in the wage:

\[
\eta = \frac{\% \Delta L}{\% \Delta w} = \frac{dL}{dw} \cdot \frac{w}{L}
\]

Because the demand curve slopes downward, \(\eta < 0\). Labour demand is said to be:

- **Elastic** if \(|\eta| > 1\): a wage increase leads to a proportionally larger decline in employment.
- **Inelastic** if \(|\eta| < 1\): employment declines proportionally less than the wage increase.

!!! empirical "Hamermesh's Consensus Estimate"
    Daniel Hamermesh's (1993) comprehensive survey of the empirical literature concluded that the own-wage elasticity of labour demand lies in the range of **-0.15 to -0.75**, with a "best guess" of around **-0.30**. This means a 10% increase in the wage leads to roughly a 3% decline in employment. The estimate varies by industry, skill level, and time horizon (long-run elasticities are larger in absolute value).

The **cross-wage elasticity** measures how demand for one type of labour responds to a change in the price of another input. If \(\eta_{ij} > 0\), inputs \(i\) and \(j\) are **substitutes**; if \(\eta_{ij} < 0\), they are **complements**.

---

## Marshall's Rules of Derived Demand

Alfred Marshall identified four conditions under which the elasticity of demand for labour will be **higher** (more elastic). Because firms demand labour not for its own sake but to produce output, labour demand is a *derived demand*.

!!! model "Marshall's Four Rules"
    The demand for labour is more elastic when:

    1. **The elasticity of substitution between labour and capital is high.** If it is easy to replace workers with machines (or vice versa), a small wage change induces large shifts in the input mix.

    2. **The elasticity of demand for the firm's output is high.** If consumers are price-sensitive, a wage-driven cost increase leads to a large drop in quantity demanded, and hence a large drop in employment.

    3. **Labour's share of total production costs is large.** When labour costs are a big fraction of total costs, a wage increase has a proportionally larger effect on product price. (This is sometimes called the "importance of being unimportant"---a factor with a *small* cost share has inelastic demand because even a large percentage wage increase barely affects the product price.)

    4. **The elasticity of supply of other factors is high.** If capital (or other inputs) can be supplied readily at constant prices, the firm can easily substitute away from labour when wages rise.

These rules have powerful policy implications. For example, a union representing workers in an industry where labour costs are a small share of total costs may be able to negotiate higher wages with relatively little employment loss.

---

## Factor Demand with Multiple Inputs

The two-input model extends naturally to settings with more than two types of labour---for instance, skilled workers (\(L_S\)) and unskilled workers (\(L_U\)). The key question becomes whether these inputs are **gross substitutes** or **gross complements**.

- **Gross substitutes**: An increase in the wage of skilled workers increases the demand for unskilled workers (firms switch to cheaper unskilled labour).
- **Gross complements**: An increase in the wage of skilled workers *decreases* the demand for unskilled workers (the scale effect dominates---less output means less of everything).

The distinction between substitutes and complements matters enormously for policy. If skilled and unskilled workers are complements, then policies that increase the supply of skilled workers (e.g., education subsidies) raise the demand for unskilled workers as well.

---

## Application: The Minimum Wage Debate

The theory developed above yields a clear prediction: a binding minimum wage (set above the equilibrium wage) should reduce employment. The magnitude of the employment loss depends on the elasticity of labour demand.

!!! empirical "Card and Krueger (1994): A Natural Experiment"
    In their landmark study, David Card and Alan Krueger compared fast-food employment in New Jersey (which raised its minimum wage) and Pennsylvania (which did not) using a difference-in-differences design. Contrary to the textbook prediction, they found **no significant decline in employment** after the minimum wage increase---and even a slight increase.

    This study ignited one of the most productive debates in empirical economics. Neumark and Wascher (2000) challenged the data and found employment losses using payroll data. Dube, Lester, and Reich (2010) later refined the approach by comparing contiguous counties across state borders, finding minimal disemployment effects for moderate minimum wage increases.

    The current consensus, as summarized by Dube (2019), is that moderate minimum wage increases have **small to negligible negative employment effects**, but very large increases may cause measurable job losses. The monopsony model (Chapter 4 extension) helps explain why small increases may not reduce employment.

!!! indian "Minimum Wages in India"
    India's minimum wage system is among the most complex in the world. The **Minimum Wages Act, 1948** empowers both central and state governments to set minimum wages for "scheduled employments." As a result, there are over **1,900 minimum wage rates** across states, sectors, and skill categories.

    Key features of the Indian system:

    - **State-level variation**: Minimum wages range from around Rs. 180/day in Bihar to over Rs. 700/day in Delhi (as of 2023), reflecting large differences in cost of living and state-level political economy.
    - **Low compliance**: Soundararajan (2019) found significant non-compliance, especially in the informal sector, which employs roughly 90% of India's workforce. The effective "bite" of the minimum wage is therefore weaker than the statutory rate suggests.
    - **The Code on Wages (2019)**: This consolidated four labour laws (including the Minimum Wages Act) and introduced the concept of a national minimum wage floor. Implementation of the Code has been gradual and varies by state.

    Soundararajan (2019) studied the effect of minimum wage increases in Indian states and found that, in sectors with higher compliance, minimum wage increases raised earnings for low-wage workers with **modest negative employment effects**---consistent with the international evidence.

---

## Key Takeaways

1. A profit-maximizing firm hires labour until \(VMP_L = w\). This is the fundamental condition driving labour demand.
2. In the short run, the firm's labour demand curve is the downward-sloping portion of the \(VMP_L\) curve. In the long run, demand is more elastic because both substitution and scale effects operate.
3. The cost-minimizing firm equates the marginal rate of technical substitution to the input price ratio: \(MP_L/MP_K = w/r\).
4. Marshall's four rules identify when labour demand is more elastic: high substitutability, elastic product demand, large labour cost share, and elastic supply of other inputs.
5. The minimum wage debate illustrates that theory and evidence must work together: while the competitive model predicts employment losses, empirical evidence suggests these are small for moderate minimum wage increases.

---

<div style="display: flex; justify-content: space-between; margin-top: 2rem; padding-top: 1rem; border-top: 1px solid var(--md-default-fg-color--lightest);">
<span>[:octicons-arrow-left-24: Ch. 2: Labor Supply](../02-labor-supply/index.md)</span>
<span>[Ch. 4: Labor Market Equilibrium :octicons-arrow-right-24:](../04-equilibrium/index.md)</span>
</div>
