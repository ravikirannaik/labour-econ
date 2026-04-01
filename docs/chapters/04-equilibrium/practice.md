---
title: "Practice — Labor Market Equilibrium"
---

# Practice: Labor Market Equilibrium

These problems cover the key concepts from Chapter 4: competitive equilibrium, payroll tax incidence, immigration effects, mandated benefits, the cobweb model, and deadweight loss. Work through each problem before revealing the answer.

---

??? question "Q1. Finding the Competitive Equilibrium"
    The labour market for factory workers in a city is characterized by:

    - Demand: \(L^D = 800 - 10w\)
    - Supply: \(L^S = -100 + 20w\)

    where \(w\) is the daily wage (in Rs. 100s) and \(L\) is employment (in thousands).

    **(a)** Find the equilibrium wage and employment.
    **(b)** Calculate the worker surplus and producer surplus at equilibrium.
    **(c)** What is the total surplus?

    **Answer:**

    **(a)** Set \(L^D = L^S\):

    \[
    800 - 10w = -100 + 20w \implies 900 = 30w \implies w^* = 30
    \]

    \[
    L^* = 800 - 10(30) = 500 \text{ thousand}
    \]

    Equilibrium: wage = Rs. 3,000/day, employment = 500 thousand.

    **(b)**

    - **Worker surplus** = area below \(w^*\) and above the supply curve = \(\frac{1}{2} \times 500 \times (30 - 5) = \frac{1}{2} \times 500 \times 25 = 6{,}250\)
        - (The supply curve intersects \(L = 0\) at \(w = 5\), i.e., the reservation wage of the marginal entrant.)
    - **Producer surplus** = area above \(w^*\) and below the demand curve = \(\frac{1}{2} \times 500 \times (80 - 30) = \frac{1}{2} \times 500 \times 50 = 12{,}500\)
        - (The demand curve intersects \(L = 0\) at \(w = 80\).)

    **(c)** Total surplus = \(6{,}250 + 12{,}500 = \mathbf{18{,}750}\).

---

??? question "Q2. Payroll Tax — Who Bears the Burden?"
    Using the market from Q1, the government imposes a payroll tax of Rs. 600/day (\(t = 6\) in our units) per worker on employers.

    **(a)** Write the new demand equation (after the tax).
    **(b)** Find the new equilibrium wage received by workers and the total cost per worker to the firm.
    **(c)** How is the tax burden shared between workers and firms?
    **(d)** What is the employment effect?

    **Answer:**

    **(a)** The tax shifts the demand curve down by \(t = 6\). The firm's willingness to pay a wage falls by the tax amount:

    \[
    L^D_{\text{new}} = 800 - 10(w + 6) = 740 - 10w
    \]

    (Equivalently, the demand curve in wage-space shifts down by 6.)

    **(b)** New equilibrium: set \(740 - 10w = -100 + 20w\):

    \[
    840 = 30w \implies w_1 = 28
    \]

    - Wage received by workers: **Rs. 2,800/day** (down from 3,000).
    - Total cost to firm per worker: \(w_1 + t = 28 + 6 = 34\), i.e., **Rs. 3,400/day** (up from 3,000).

    **(c)** Tax burden:

    - **Workers bear**: \(30 - 28 = 2\) units = Rs. 200/day (one-third of the tax).
    - **Firms bear**: \(34 - 30 = 4\) units = Rs. 400/day (two-thirds of the tax).

    Workers bear a smaller share because labour supply (slope = 1/20 in wage-employment space) is more elastic than labour demand (slope = 1/10). The more elastic side of the market escapes more of the tax.

    **(d)** New employment: \(L_1 = -100 + 20(28) = 460\) thousand. Employment falls by 40 thousand (from 500 to 460).

---

??? question "Q3. Does It Matter Who Pays the Tax?"
    Suppose instead that the same Rs. 600/day tax from Q2 is levied on employees rather than employers. Show that the equilibrium outcomes (wage cost to employer, wage received by worker, employment) are the same.

    **Answer:**

    With the tax on employees, the supply curve shifts up (leftward) by \(t = 6\):

    \[
    L^S_{\text{new}} = -100 + 20(w - 6) = -220 + 20w
    \]

    Set equal to the original demand: \(800 - 10w = -220 + 20w\):

    \[
    1020 = 30w \implies w = 34
    \]

    - Wage paid by firm (gross wage): **Rs. 3,400/day** (= 34 units).
    - Wage received by worker (after tax): \(34 - 6 = 28\) units = **Rs. 2,800/day**.
    - Employment: \(L = 800 - 10(34) = 460\) thousand.

    These are **identical** to Q2. The firm pays Rs. 3,400, the worker takes home Rs. 2,800, and employment is 460 thousand---regardless of whether the tax is statutorily on the employer or the employee. **Statutory incidence does not determine economic incidence.**

---

??? question "Q4. Deadweight Loss of the Payroll Tax"
    Calculate the deadweight loss from the payroll tax in Q2.

    **Answer:**

    The deadweight loss is the triangle between the supply and demand curves, over the range of employment that is eliminated (from 460 to 500 thousand):

    At \(L = 460\):

    - Demand price (what firm would pay): \(w^D = (800 - 460)/10 = 34\)
    - Supply price (what worker requires): \(w^S = (460 + 100)/20 = 28\)

    At \(L = 500\) (original equilibrium): both equal 30.

    \[
    DWL = \frac{1}{2} \times (500 - 460) \times (34 - 28) = \frac{1}{2} \times 40 \times 6 = \mathbf{120}
    \]

    The deadweight loss is 120 (in thousands of wage-unit-days). This represents the value of 40 thousand employment relationships that would have been mutually beneficial but are destroyed by the tax.

---

??? question "Q5. Immigration — Wage and Employment Effects"
    The market for low-skilled workers has:

    - Demand: \(L^D = 500 - 5w\)
    - Native supply: \(L^S_N = 100 + 10w\)

    An inflow of 60 thousand immigrant workers shifts the supply curve rightward.

    **(a)** Find the pre-immigration equilibrium.
    **(b)** Write the new (post-immigration) supply function and find the new equilibrium.
    **(c)** What is the effect on the wage of native workers?
    **(d)** What is the effect on total employment?

    **Answer:**

    **(a)** Pre-immigration equilibrium: \(500 - 5w = 100 + 10w\):

    \[
    400 = 15w \implies w_0 = 26.67 \quad (\text{approximately})
    \]

    \[
    L_0 = 500 - 5(26.67) = 366.67 \text{ thousand}
    \]

    **(b)** The new total supply adds 60 to the native supply at every wage:

    \[
    L^S_{\text{total}} = (100 + 10w) + 60 = 160 + 10w
    \]

    New equilibrium: \(500 - 5w = 160 + 10w\):

    \[
    340 = 15w \implies w_1 = 22.67 \quad (\text{approximately})
    \]

    \[
    L_1 = 500 - 5(22.67) = 386.67 \text{ thousand}
    \]

    **(c)** The wage falls from Rs. 2,667 to Rs. 2,267/day --- a decline of Rs. 400/day (approximately 15%).

    **(d)** Total employment rises from 367 to 387 thousand (an increase of about 20 thousand). Note that total employment rises by less than the 60 thousand immigrants because the lower wage induces some native workers to leave the market. Native employment at the new wage: \(L^S_N(22.67) = 100 + 10(22.67) = 326.7\), down from 366.7. About 40 native workers withdraw.

---

??? question "Q6. The Immigration Surplus"
    Using the results from Q5:

    **(a)** Who gains and who loses from immigration?
    **(b)** Calculate the change in producer surplus (employer gains).
    **(c)** Explain why the immigration surplus (net gain to natives) is positive but small.

    **Answer:**

    **(a)**

    - **Employers gain**: They hire more workers at a lower wage. Both effects increase producer surplus.
    - **Native workers lose**: Their wage falls from 26.67 to 22.67. Those who remain employed earn less; some leave the market entirely.
    - **Immigrants gain**: They earn 22.67, which exceeds their opportunity wage in the home country (otherwise they would not have migrated).

    **(b)** The change in producer surplus can be decomposed:

    - Rectangle: existing employment (367) times the wage reduction (4) = \(367 \times 4 = 1{,}468\). This is a transfer from native workers to employers.
    - Triangle: \(\frac{1}{2} \times (387 - 367) \times 4 = \frac{1}{2} \times 20 \times 4 = 40\). This is the net new surplus.

    Total change in producer surplus: \(1{,}468 + 40 = 1{,}508\).

    **(c)** The **immigration surplus** is the net gain to the native population:

    - Employer gain: +1,508
    - Native worker loss: approximately -1,468 (the wage reduction times native employment, minus the reservation wage savings of those who exit)

    The net gain (immigration surplus) is approximately the triangle = **40**. It is positive because employing immigrants at a wage below their marginal product generates surplus. But it is **small** relative to total GDP because it depends on the *square* of the immigration share and on the demand elasticity. Immigration is primarily a redistribution from native labour to native capital, not a large net gain.

---

??? question "Q7. Mandated Benefits"
    A government requires employers to provide a health insurance benefit that costs Rs. 50/day per worker. Workers value this benefit at Rs. 30/day.

    Using the market from Q1 (demand: \(L^D = 800 - 10w\), supply: \(L^S = -100 + 20w\)):

    **(a)** How does the demand curve shift?
    **(b)** How does the supply curve shift?
    **(c)** Find the new equilibrium wage and employment.
    **(d)** Compare the employment effect to a pure tax of Rs. 50/day (where \(b = 0\)).

    **Answer:**

    Working in units of Rs. 100s: cost \(c = 0.5\), value \(b = 0.3\).

    **(a)** Demand shifts down by \(c = 0.5\):

    \[
    L^D_{\text{new}} = 800 - 10(w + 0.5) = 795 - 10w
    \]

    **(b)** Supply shifts down (rightward) by \(b = 0.3\), since workers accept a lower cash wage:

    \[
    L^S_{\text{new}} = -100 + 20(w + 0.3) = -94 + 20w
    \]

    **(c)** New equilibrium: \(795 - 10w = -94 + 20w\):

    \[
    889 = 30w \implies w_1 = 29.63
    \]

    \[
    L_1 = -94 + 20(29.63) = 498.67 \text{ thousand}
    \]

    The cash wage falls from 30 to 29.63 (a drop of Rs. 37/day), but total compensation (wage + benefit value) is \(29.63 + 0.3 = 29.93\), barely below the original 30. Employment falls by only about 1,330 workers.

    **(d)** With a pure tax of 0.5 (\(b = 0\)): demand shifts down by 0.5, supply unchanged.

    \[
    795 - 10w = -100 + 20w \implies 895 = 30w \implies w = 29.83
    \]

    \[
    L = -100 + 20(29.83) = 496.67
    \]

    Employment falls by 3,330 workers---**more than twice the decline** with the valued benefit. This confirms the theory: when workers value the mandated benefit, the employment cost is lower because workers "pay" for part of the benefit through lower wage demands.

---

??? question "Q8. The Cobweb Model"
    The market for IT engineers has the following structure:

    - Demand: \(w^D_t = 100 - 0.1L_t\) (wage firms offer in year \(t\) given supply \(L_t\))
    - Supply responds to *last period's* wage: \(L_t = 200 + 2w_{t-1}\)

    Starting from \(w_0 = 60\):

    **(a)** Calculate employment and wages for years 1 through 4.
    **(b)** Is this cobweb stable or unstable?
    **(c)** What is the equilibrium if the market were in static equilibrium (\(L^S = L^D\) simultaneously)?

    **Answer:**

    **(a)** Calculations:

    - **Year 1**: \(L_1 = 200 + 2(60) = 320\). Wage: \(w_1 = 100 - 0.1(320) = 68\).
    - **Year 2**: \(L_2 = 200 + 2(68) = 336\). Wage: \(w_2 = 100 - 0.1(336) = 66.4\).
    - **Year 3**: \(L_3 = 200 + 2(66.4) = 332.8\). Wage: \(w_3 = 100 - 0.1(332.8) = 66.72\).
    - **Year 4**: \(L_4 = 200 + 2(66.72) = 333.44\). Wage: \(w_4 = 100 - 0.1(333.44) = 66.66\).

    The oscillations are damping: wages converge toward 66.67.

    **(b)** The cobweb is **stable**. The supply slope in wage-employment space is \(dL/dw = 2\), so \(dw/dL = 0.5\) for supply. The demand slope is \(dw/dL = -0.1\). Since the supply curve is steeper than the demand curve (in wage-employment space, \(|0.5| > |-0.1|\)), the oscillations converge.

    **(c)** Static equilibrium: substitute the supply into the demand relation by setting \(w_t = w_{t-1} = w^*\):

    \[
    L = 200 + 2w^*, \quad w^* = 100 - 0.1(200 + 2w^*)
    \]

    \[
    w^* = 100 - 20 - 0.2w^* \implies 1.2w^* = 80 \implies w^* = 66.67
    \]

    \[
    L^* = 200 + 2(66.67) = 333.33
    \]

    The cobweb converges to this equilibrium.

---

??? question "Q9. Multiple Labour Markets and Equilibrium"
    Consider two regional labour markets, North and South, for the same type of worker:

    - **North**: \(L^D_N = 600 - 5w_N\), \(L^S_N = 10w_N\)
    - **South**: \(L^D_S = 400 - 5w_S\), \(L^S_S = 10w_S\)

    **(a)** Find the equilibrium wage in each market when there is no migration.
    **(b)** If workers can freely migrate between the two markets, what is the economy-wide equilibrium wage?
    **(c)** Which region gains workers and which loses them?

    **Answer:**

    **(a)** Without migration:

    - **North**: \(600 - 5w = 10w \implies 600 = 15w \implies w_N = 40\), \(L_N = 400\).
    - **South**: \(400 - 5w = 10w \implies 400 = 15w \implies w_S = 26.67\), \(L_S = 266.67\).

    **(b)** With free migration, wages must equalize: \(w_N = w_S = w^*\). Aggregate:

    \[
    L^D_{\text{total}} = (600 - 5w) + (400 - 5w) = 1000 - 10w
    \]

    \[
    L^S_{\text{total}} = 10w + 10w = 20w
    \]

    \[
    1000 - 10w = 20w \implies w^* = 33.33
    \]

    **(c)** At \(w^* = 33.33\):

    - North: \(L^D_N = 600 - 5(33.33) = 433.33\), \(L^S_N = 10(33.33) = 333.33\). Demand exceeds local supply by 100 --- North **gains** 100 thousand workers via migration.
    - South: \(L^D_S = 400 - 5(33.33) = 233.33\), \(L^S_S = 333.33\). Local supply exceeds demand by 100 --- South **loses** 100 thousand workers.

    Workers migrate from the low-wage South to the high-wage North until wages equalize. The North's wage falls (from 40 to 33.33) and the South's rises (from 26.67 to 33.33).

---

??? question "Q10. Internal Migration in India"
    India has large interstate wage differentials (e.g., Bihar vs. Maharashtra). Apply the Borjas equilibrium framework to explain:

    **(a)** Why do workers migrate from low-income states to high-income states?
    **(b)** What factors prevent the wage equalization predicted by the competitive model?
    **(c)** Imbert and Papp (2015) studied the effect of NREGA on internal migration in India. What would the equilibrium model predict about the impact of a rural employment guarantee on migration flows?

    **Answer:**

    **(a)** The competitive model predicts that workers migrate from low-wage regions (e.g., Bihar, Uttar Pradesh, Odisha) to high-wage regions (e.g., Maharashtra, Delhi, Gujarat) to arbitrage wage differentials. Migration increases labour supply in the destination and reduces it in the origin, pushing wages toward equalization. India's large internal migration flows---the 2011 Census recorded over 450 million migrants---are broadly consistent with this prediction.

    **(b)** Several factors impede full wage equalization:

    - **Language and cultural barriers**: India has 22 official languages; moving across linguistic borders is costly.
    - **Housing costs**: High wages in Mumbai or Delhi are partly offset by extremely high housing costs, reducing the real wage gain from migration.
    - **Social networks and information**: Migration is facilitated by networks; workers from regions without established migrant communities face higher search costs.
    - **Informal labour markets**: Migrants often work in the informal sector where wages may not fully reflect market equilibrium.
    - **Administrative barriers**: Although the Constitution guarantees freedom of movement, access to ration cards, voter ID, and government services in destination states can be difficult for migrants.
    - **Skill mismatch**: Rural migrants may lack the skills demanded in urban labour markets.

    **(c)** NREGA (Mahatma Gandhi National Rural Employment Guarantee Act) provides a wage floor in rural areas by guaranteeing 100 days of employment at a minimum wage. In the equilibrium framework:

    - NREGA raises the effective reservation wage in rural areas, making migration less attractive at the margin.
    - The supply of migrant labour to urban areas should decrease (leftward shift of urban supply).
    - Urban wages should rise slightly, and rural-urban wage differentials should narrow.

    Imbert and Papp (2015) found exactly this: NREGA implementation reduced seasonal migration from treated districts and increased wages for casual labourers in both rural and urban areas nearby. The programme effectively tightened rural labour supply, with spillover effects consistent with the equilibrium framework.
