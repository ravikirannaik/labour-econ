---
title: "Practice — Labor Demand"
---

# Practice: Labor Demand

These problems cover the key concepts from Chapter 3: marginal productivity, short-run and long-run labour demand, Marshall's rules, isoquant-isocost analysis, elasticities, and the minimum wage. Work through each problem before revealing the answer.

---

??? question "Q1. Computing the Marginal Product of Labour"
    A firm's short-run production function is \(q = 120L - 2L^2\), where \(L\) is the number of workers.

    **(a)** What is the marginal product of labour?
    **(b)** At what level of employment does diminishing returns set in?
    **(c)** What is the maximum output the firm can produce?

    **Answer:**

    **(a)** The marginal product of labour is the derivative of the production function with respect to \(L\):

    \[
    MP_L = \frac{dq}{dL} = 120 - 4L
    \]

    **(b)** Diminishing returns set in immediately, since \(MP_L\) is a decreasing function of \(L\) for all \(L > 0\). (More precisely, the second derivative \(d^2q/dL^2 = -4 < 0\) everywhere.) Diminishing returns apply from the very first worker.

    **(c)** Output is maximized where \(MP_L = 0\):

    \[
    120 - 4L = 0 \implies L = 30
    \]

    Maximum output: \(q = 120(30) - 2(30)^2 = 3600 - 1800 = 1800\).

---

??? question "Q2. The Hiring Decision — VMP = w"
    Using the production function from Q1, suppose the output price is \(p = 5\) and the wage is \(w = 200\).

    **(a)** Write the value of marginal product function.
    **(b)** How many workers does the profit-maximizing firm hire?
    **(c)** If the wage rises to \(w = 300\), what happens to employment?

    **Answer:**

    **(a)** The value of marginal product is:

    \[
    VMP_L = p \times MP_L = 5(120 - 4L) = 600 - 20L
    \]

    **(b)** Set \(VMP_L = w\):

    \[
    600 - 20L = 200 \implies 20L = 400 \implies L^* = 20
    \]

    The firm hires 20 workers.

    **(c)** At \(w = 300\):

    \[
    600 - 20L = 300 \implies 20L = 300 \implies L^* = 15
    \]

    Employment falls from 20 to 15 workers. This illustrates the inverse relationship between wages and employment along the labour demand curve.

---

??? question "Q3. Shifts in Labour Demand"
    Explain whether each of the following shifts the labour demand curve to the left, to the right, or causes a movement along the curve:

    **(a)** A technological innovation that raises each worker's productivity.
    **(b)** An increase in the market wage.
    **(c)** An increase in the price of the firm's output.
    **(d)** A decrease in the price of capital, assuming labour and capital are gross substitutes.

    **Answer:**

    **(a)** **Right shift.** Higher productivity raises \(MP_L\) at every employment level, so \(VMP_L = p \times MP_L\) shifts outward.

    **(b)** **Movement along the curve.** A wage change moves the firm along its existing demand curve---it does not shift the curve. The firm moves up-left (hiring fewer workers at a higher wage).

    **(c)** **Right shift.** A higher output price raises \(VMP_L = p \times MP_L\) at every employment level, shifting the demand curve outward.

    **(d)** **Left shift.** If labour and capital are gross substitutes, cheaper capital leads firms to substitute toward capital and away from labour. The substitution effect dominates: labour demand shifts left. (If they were gross complements, cheaper capital would increase output and raise the demand for labour---a right shift.)

---

??? question "Q4. Isoquant and Isocost Analysis"
    A firm produces output using the production function \(q = L^{0.5} K^{0.5}\). The wage is \(w = 10\) and the rental rate of capital is \(r = 40\).

    **(a)** What is the MRTS of labour for capital?
    **(b)** Find the cost-minimizing input ratio \(K/L\).
    **(c)** If the firm wants to produce \(q = 100\), how much labour and capital does it use?
    **(d)** What is the total cost?

    **Answer:**

    **(a)** The marginal products are:

    \[
    MP_L = \frac{0.5 K^{0.5}}{L^{0.5}} = \frac{0.5K^{0.5}}{L^{0.5}}, \qquad MP_K = \frac{0.5 L^{0.5}}{K^{0.5}}
    \]

    \[
    MRTS_{LK} = \frac{MP_L}{MP_K} = \frac{K}{L}
    \]

    **(b)** Cost minimization requires \(MRTS = w/r\):

    \[
    \frac{K}{L} = \frac{10}{40} = \frac{1}{4} \implies K = \frac{L}{4}
    \]

    The firm uses 4 times as much labour as capital (since labour is cheaper).

    **(c)** Substitute into the production function:

    \[
    100 = L^{0.5} \left(\frac{L}{4}\right)^{0.5} = L^{0.5} \cdot \frac{L^{0.5}}{2} = \frac{L}{2}
    \]

    \[
    L^* = 200, \qquad K^* = \frac{200}{4} = 50
    \]

    **(d)** Total cost: \(C = wL + rK = 10(200) + 40(50) = 2000 + 2000 = 4000\).

---

??? question "Q5. The Substitution and Scale Effects"
    Suppose the wage of unskilled workers increases. Using isoquant-isocost diagrams (describe the graphical intuition), explain:

    **(a)** The substitution effect on the demand for unskilled labour.
    **(b)** The scale effect on the demand for unskilled labour.
    **(c)** Why the long-run demand curve is more elastic than the short-run curve.

    **Answer:**

    **(a)** **Substitution effect:** The isocost line becomes steeper (since \(w/r\) has increased). The new tangency point on the *same* isoquant involves less labour and more capital. The firm substitutes away from the now-more-expensive unskilled labour. This effect always reduces the quantity of labour demanded.

    **(b)** **Scale effect:** Higher wages raise the firm's marginal cost, which leads to a higher product price and lower output. The firm moves to a *lower* isoquant, reducing its demand for all inputs including unskilled labour. The scale effect also reduces labour demand.

    **(c)** In the short run, capital is fixed, so only a movement along the \(VMP_L\) curve occurs. In the long run, the firm adjusts both inputs: the substitution effect (replacing workers with capital) and the scale effect (producing less) both reduce employment. Because two effects operate rather than one, the long-run response to a wage change is larger, making the long-run demand curve flatter (more elastic).

---

??? question "Q6. Marshall's Rules — Application"
    Consider two industries:

    - **Industry A**: Labour costs are 70% of total costs, product demand is highly elastic, and machines can easily replace workers.
    - **Industry B**: Labour costs are 10% of total costs, product demand is inelastic, and there is no close substitute for the workers' skills.

    In which industry will a union wage increase lead to a larger employment decline? Explain using Marshall's rules.

    **Answer:**

    **Industry A will experience the larger employment decline.** Applying Marshall's four rules:

    1. **Substitutability**: High in A (machines can replace workers), low in B. This makes demand more elastic in A.
    2. **Product demand elasticity**: High in A, low in B. Consumers of A's product will buy much less when prices rise, magnifying job losses in A.
    3. **Labour's cost share**: Large in A (70%), small in B (10%). In A, the wage increase significantly raises product price, triggering a larger output and employment decline. In B, even a big wage increase barely affects the product price.
    4. **Supply of substitutes**: Implied to be readily available in A (machines are easy to deploy), less so in B.

    All four rules point in the same direction: Industry A has more elastic labour demand. A union in Industry B occupies a more powerful position---it can raise wages with less fear of employment loss, precisely because it is "unimportant" in the cost structure and hard to replace.

---

??? question "Q7. Own-Wage Elasticity Calculation"
    A study estimates that a 15% increase in the wage rate leads to a 6% decline in employment.

    **(a)** Calculate the own-wage elasticity of labour demand.
    **(b)** Is demand elastic or inelastic?
    **(c)** If the firm currently employs 500 workers at a wage of Rs. 400/day, and the wage rises to Rs. 440/day, how many workers will it employ?

    **Answer:**

    **(a)** The own-wage elasticity is:

    \[
    \eta = \frac{\% \Delta L}{\% \Delta w} = \frac{-6\%}{15\%} = -0.40
    \]

    **(b)** Since \(|\eta| = 0.40 < 1\), demand is **inelastic**. Employment declines proportionally less than the wage increase.

    **(c)** The percentage wage increase is:

    \[
    \% \Delta w = \frac{440 - 400}{400} \times 100 = 10\%
    \]

    Using the elasticity:

    \[
    \% \Delta L = \eta \times \% \Delta w = -0.40 \times 10\% = -4\%
    \]

    New employment: \(500 \times (1 - 0.04) = 500 \times 0.96 = 480\) workers.

---

??? question "Q8. Cross-Wage Elasticity"
    Suppose a 10% increase in the wage of skilled workers leads to a 5% *increase* in the employment of unskilled workers.

    **(a)** Calculate the cross-wage elasticity.
    **(b)** Are skilled and unskilled workers gross substitutes or gross complements?
    **(c)** How would you expect the result to differ in the short run versus the long run?

    **Answer:**

    **(a)** The cross-wage elasticity is:

    \[
    \eta_{US} = \frac{\% \Delta L_U}{\% \Delta w_S} = \frac{+5\%}{+10\%} = +0.50
    \]

    **(b)** Since \(\eta_{US} > 0\), skilled and unskilled workers are **gross substitutes**. When skilled workers become more expensive, firms replace them with unskilled workers.

    **(c)** In the short run, with capital fixed, the substitution effect between worker types is limited. In the long run, the firm can adjust all inputs, so the cross-wage elasticity is likely larger in absolute value. Additionally, the scale effect (higher costs reduce output) would work against unskilled employment, partially offsetting the substitution toward unskilled labour.

---

??? question "Q9. Short-Run vs. Long-Run Demand"
    A firm currently employs 1,000 workers. The government mandates a 20% wage increase.

    **(a)** If the short-run elasticity of labour demand is \(-0.2\), how many workers are laid off in the short run?
    **(b)** If the long-run elasticity is \(-0.5\), how many are employed in the long run?
    **(c)** What economic mechanisms explain the difference between (a) and (b)?

    **Answer:**

    **(a)** Short-run employment change:

    \[
    \% \Delta L = -0.2 \times 20\% = -4\%
    \]

    Workers laid off: \(1000 \times 0.04 = 40\). Employment falls to **960**.

    **(b)** Long-run employment change:

    \[
    \% \Delta L = -0.5 \times 20\% = -10\%
    \]

    Employment falls to \(1000 \times 0.90 = \mathbf{900}\).

    **(c)** In the short run, only the output (scale) effect operates: higher costs reduce output, which reduces labour demand. In the long run, the **substitution effect** kicks in as well: the firm can replace workers with capital (automation, new machinery). In addition, the long-run scale effect may also be larger as competitors adjust and the product market reaches a new equilibrium. Together, these mechanisms produce a more elastic long-run response: 100 jobs lost in the long run versus 40 in the short run.

---

??? question "Q10. The Minimum Wage — Competitive Model"
    The labour market for low-skilled workers is characterized by:

    - Demand: \(L^D = 1000 - 20w\)
    - Supply: \(L^S = -200 + 40w\)

    where \(w\) is the hourly wage and \(L\) is employment (in thousands).

    **(a)** Find the equilibrium wage and employment.
    **(b)** The government sets a minimum wage of \(w_{min} = 25\). What is the new employment level? How many workers are unemployed?
    **(c)** Calculate the deadweight loss from the minimum wage.

    **Answer:**

    **(a)** Set \(L^D = L^S\):

    \[
    1000 - 20w = -200 + 40w \implies 1200 = 60w \implies w^* = 20
    \]

    \[
    L^* = 1000 - 20(20) = 600 \text{ (thousand workers)}
    \]

    **(b)** At \(w_{min} = 25\):

    - Demand: \(L^D = 1000 - 20(25) = 500\)
    - Supply: \(L^S = -200 + 40(25) = 800\)

    Employment is determined by demand (firms will not hire more than they want): **500 thousand**. Unemployment = \(L^S - L^D = 800 - 500 = 300\) thousand.

    **(c)** The deadweight loss is the triangle between the supply and demand curves over the range of employment reduction (from 600 to 500):

    At \(L = 500\): \(w^D = (1000 - 500)/20 = 25\) and \(w^S = (500 + 200)/40 = 17.5\).
    At \(L = 600\): both equal 20.

    \[
    DWL = \frac{1}{2} \times (600 - 500) \times (25 - 17.5) = \frac{1}{2} \times 100 \times 7.5 = 375
    \]

    The deadweight loss is **375** (in thousands of wage-units), representing the value of transactions that would have been mutually beneficial but no longer occur.

---

??? question "Q11. Minimum Wage — Empirical Evidence"
    Explain the key difference in research design between Card and Krueger (1994) and Dube, Lester, and Reich (2010) in studying the employment effects of minimum wages. Why does the choice of comparison group matter?

    **Answer:**

    **Card and Krueger (1994)** used a **difference-in-differences** (DiD) design, comparing fast-food restaurants in New Jersey (treatment, which raised its minimum wage) with those in eastern Pennsylvania (control). They surveyed restaurants before and after the minimum wage increase and found no significant employment decline in New Jersey.

    **Dube, Lester, and Reich (2010)** refined this approach by comparing **contiguous counties that straddle a state border** where one side raised its minimum wage and the other did not. Their key insight was that Card and Krueger's comparison (entire states) might mix up the minimum wage effect with other state-level economic differences. By comparing adjacent counties, Dube et al. ensured that the treatment and control groups faced similar local economic conditions (cost of living, consumer demand, labour markets), isolating the minimum wage effect more cleanly.

    **Why the comparison group matters:** If the control group differs systematically from the treatment group in ways that also affect employment (e.g., a booming economy in one state versus a recession in the other), the DiD estimate will be biased. Contiguous-county designs minimize this problem by ensuring geographic and economic similarity. Both studies found small or negligible disemployment effects, strengthening the conclusion that moderate minimum wage increases do not cause large job losses.

---

??? question "Q12. Minimum Wages in India"
    India has over 1,900 minimum wage rates set by central and state governments.

    **(a)** Why does India have so many different minimum wage rates?
    **(b)** Soundararajan (2019) found that minimum wage compliance is low in many sectors. What does this imply about the employment effects of minimum wage increases in India?
    **(c)** How might the large informal sector affect the analysis of minimum wage policy in India compared to the United States?

    **Answer:**

    **(a)** The **Minimum Wages Act, 1948** allows both central and state governments to set minimum wages for "scheduled employments" (specific industries and occupations). States set rates independently based on local conditions, and rates differ by industry, skill level (unskilled, semi-skilled, skilled, highly skilled), and sometimes by region within a state. This produces a very large number of distinct rates.

    **(b)** Low compliance means that statutory minimum wages often **do not bind** in practice. Many workers---especially in the informal sector---are paid below the legal minimum. This implies that the employment effects of a minimum wage increase will be **smaller** than the competitive model predicts, not because the theory is wrong, but because the policy is not enforced. The "effective" minimum wage faced by most workers is well below the statutory level.

    **(c)** In the US, the vast majority of employment is in the formal sector, so minimum wage laws cover most workers and firms. In India, roughly 90% of workers are in the informal sector, where compliance with labour regulations is low and enforcement is weak. This means:

    - Minimum wage increases primarily affect the **formal sector**, potentially widening the formal-informal wage gap.
    - Workers displaced from the formal sector may move into **informal employment** rather than becoming unemployed, making the employment effect appear smaller even if the welfare effect is negative.
    - The relevant elasticity for India may be the elasticity of **formal employment**, not total employment, with respect to the minimum wage.
