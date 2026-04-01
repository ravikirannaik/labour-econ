---
title: "Practice — Unemployment"
---

# Practice: Unemployment

Test your understanding of unemployment theory, search models, and macroeconomic connections. Questions range from definitional to computational.

---

??? question "Q1. Classifying Unemployment"
    Classify each of the following as frictional, structural, or cyclical unemployment:

    (a) A coal miner loses her job because the power plant switches to solar energy.
    (b) A recent college graduate spends three months searching for a first job.
    (c) A construction worker is laid off during a recession.
    (d) A software engineer quits to find a better-paying job and is unemployed for two weeks.
    (e) A textile worker in Surat loses her job because production moves to Bangladesh.

    **Answer:**

    **(a) Structural.** The demand for coal miners has permanently declined due to technological change (shift to renewable energy). The worker's existing skills are not demanded in the new energy sector.

    **(b) Frictional.** The graduate is searching for an appropriate match. This is a normal part of labour market functioning --- it takes time to find the right job, and the graduate is acquiring information about available positions.

    **(c) Cyclical.** Construction is highly sensitive to the business cycle. The layoff is driven by a fall in aggregate demand, not by a permanent change in the worker's skills or the industry's structure.

    **(d) Frictional.** The worker voluntarily quit and is between jobs. This is a short-duration search reflecting the normal matching process.

    **(e) Structural.** The job loss is due to a permanent geographic shift in production (globalisation/offshoring). The worker's skills may still be relevant but the jobs have relocated internationally.

??? question "Q2. Steady-State Unemployment Rate Calculation"
    In a labour market with 1 million workers:

    - Each month, 2% of employed workers lose their jobs (\( s = 0.02 \)).
    - Each month, 20% of unemployed workers find jobs (\( f = 0.20 \)).

    (a) Calculate the steady-state unemployment rate.
    (b) How many workers are unemployed in steady state?
    (c) If the government implements a job-matching programme that raises \( f \) to 0.30, what happens to the unemployment rate?

    **Answer:**

    **(a)** The steady-state unemployment rate:

    \[
    u^* = \frac{s}{s + f} = \frac{0.02}{0.02 + 0.20} = \frac{0.02}{0.22} = 0.0909 \approx 9.1\%
    \]

    **(b)** Unemployed workers = \( u^* \times L = 0.0909 \times 1{,}000{,}000 = 90{,}909 \approx 90{,}900 \) workers.

    **(c)** With \( f = 0.30 \):

    \[
    u^* = \frac{0.02}{0.02 + 0.30} = \frac{0.02}{0.32} = 0.0625 = 6.25\%
    \]

    The unemployment rate falls from 9.1% to **6.25%** --- a reduction of 2.85 percentage points. The job-matching programme reduces unemployment by increasing the rate at which unemployed workers find jobs. This illustrates why active labour market policies focused on matching can be effective.

??? question "Q3. Reservation Wage and Search"
    An unemployed worker receives one wage offer per week from the distribution: $400 with probability 0.3, $600 with probability 0.5, and $1,000 with probability 0.2. While unemployed, the worker receives UI benefits of $350/week.

    (a) If the worker's reservation wage is $600, what is the probability of accepting an offer in any given week?
    (b) What is the expected duration of unemployment (in weeks)?
    (c) If UI benefits are cut to $200/week, predict what happens to the reservation wage and explain why.

    **Answer:**

    **(a)** The worker accepts offers at or above $600. The probability of receiving an acceptable offer is:

    \[
    P(\text{accept}) = P(w = 600) + P(w = 1000) = 0.5 + 0.2 = 0.70
    \]

    The **probability of accepting an offer** in any given week is **70%**.

    **(b)** The expected duration of unemployment is:

    \[
    E[\text{duration}] = \frac{1}{P(\text{accept})} = \frac{1}{0.70} \approx 1.43 \text{ weeks}
    \]

    On average, the worker will be unemployed for about **1.4 weeks**.

    **(c)** If UI benefits fall from $350 to $200:

    - The flow value of being unemployed decreases.
    - The cost of continued search increases (the worker forgoes consumption during each additional week of search).
    - The reservation wage **falls** --- the worker becomes less picky and accepts lower offers.
    - If the reservation wage drops to $400, the acceptance probability rises to 1.0 and expected duration falls to 1 week.

    This is the moral hazard channel: higher UI benefits raise the reservation wage and extend unemployment duration. Cutting benefits reduces duration but may result in worse matches (lower wages, shorter tenure).

??? question "Q4. Unemployment Insurance Moral Hazard"
    A country offers UI benefits equal to 60% of the prior wage for up to 26 weeks. The government proposes extending benefits to 52 weeks.

    (a) Using search theory, predict the effect on unemployment duration.
    (b) Distinguish between the moral hazard effect and the liquidity effect of this extension.
    (c) Based on Chetty (2008), which effect is likely larger for low-wealth workers?

    **Answer:**

    **(a)** Extending the benefit duration from 26 to 52 weeks **increases unemployment duration**. Workers who approach the 26-week exhaustion point often intensify their search (a "spike" in the exit rate just before benefits expire). Extending to 52 weeks pushes this spike back, allowing workers to remain unemployed longer.

    **(b)**

    - **Moral hazard effect:** With more weeks of benefits, workers reduce search effort because the cost of continued unemployment is lower. They may also set a higher reservation wage, rejecting offers they would otherwise accept.
    - **Liquidity effect:** Cash-constrained workers who would otherwise be forced to accept a poor-quality job out of desperation can now afford to continue searching for a better match. The extension relaxes a borrowing constraint, enabling more efficient search.

    **(c)** Chetty (2008) finds that the liquidity effect accounts for roughly **60%** of the UI-duration relationship for low-wealth workers. These workers have little savings and face binding liquidity constraints. For them, the extension primarily enables better search rather than encouraging laziness. For wealthier workers who already have savings to smooth consumption, the effect operates more through moral hazard (they can search longer regardless, but benefits reduce their motivation to accept quickly).

??? question "Q5. Phillips Curve Analysis"
    The expectations-augmented Phillips curve for an economy is:

    \[
    \pi = \pi^e - 0.5(u - 6)
    \]

    where \( \pi \) is the inflation rate (%), \( \pi^e \) is expected inflation (%), and \( u \) is the unemployment rate (%).

    (a) What is the NAIRU?
    (b) If expected inflation is 3% and the actual unemployment rate is 4%, what is the inflation rate?
    (c) If expected inflation is 3% and the actual unemployment rate is 8%, what is the inflation rate?
    (d) Explain why the long-run Phillips curve is vertical.

    **Answer:**

    **(a)** The NAIRU is the unemployment rate at which inflation equals expected inflation (\( \pi = \pi^e \)):

    \[
    \pi = \pi^e - 0.5(u^* - 6) \implies 0 = -0.5(u^* - 6) \implies u^* = 6\%
    \]

    The **NAIRU is 6%**.

    **(b)** With \( \pi^e = 3\% \) and \( u = 4\% \):

    \[
    \pi = 3 - 0.5(4 - 6) = 3 - 0.5(-2) = 3 + 1 = 4\%
    \]

    Inflation is **4%** --- above expected inflation because the economy is overheating (\( u < u^* \)).

    **(c)** With \( \pi^e = 3\% \) and \( u = 8\% \):

    \[
    \pi = 3 - 0.5(8 - 6) = 3 - 1 = 2\%
    \]

    Inflation is **2%** --- below expected inflation because the economy has slack (\( u > u^* \)).

    **(d)** The long-run Phillips curve is vertical because expectations eventually adjust. If the government tries to keep \( u = 4\% \) permanently:

    - Period 1: \( \pi^e = 3\% \), \( \pi = 4\% \). Workers are surprised.
    - Period 2: Workers update expectations to \( \pi^e = 4\% \). Now \( \pi = 4 - 0.5(4-6) = 5\% \). Inflation accelerates.
    - Period 3: \( \pi^e = 5\% \), \( \pi = 6\% \)...

    Inflation keeps accelerating. In the long run, the only sustainable unemployment rate is \( u^* = 6\% \), and any inflation rate is consistent with it. The long-run curve is vertical at \( u = u^* \).

??? question "Q6. Indian Unemployment Measurement"
    India's PLFS reports three unemployment rates for 2023-24: UPSS at 3.2%, CWS at 5.0%, and CDS at approximately 7.5%.

    (a) Explain why these three measures give different numbers.
    (b) Which measure best captures the extent of unemployment in India? Justify your answer.
    (c) Why might even the CDS rate understate the true extent of labour underutilisation?

    **Answer:**

    **(a)** The three measures differ in their **reference period** and **classification thresholds**:

    - **UPSS (Usual Principal + Subsidiary Status):** Classifies a person based on their primary activity over the **entire year**. Anyone who worked even briefly in a subsidiary capacity during the year is "employed." This gives the lowest rate.
    - **CWS (Current Weekly Status):** Classifies based on activity during the **reference week**. Someone unemployed this week but employed last month is counted as unemployed. Captures more short-duration unemployment.
    - **CDS (Current Daily Status):** Classifies based on activity on **each day** of the reference week and averages across days. Captures day-to-day unemployment and underemployment, yielding the highest rate.

    **(b)** The **CDS rate** arguably best captures the extent of unemployment because:

    - It accounts for partial unemployment within a week (e.g., a worker employed Monday--Wednesday but jobless Thursday--Saturday).
    - India's labour market features extensive casual and seasonal work, making daily status more informative than yearly status.
    - The UPSS rate is misleadingly low because it classifies people with even minimal work during the year as employed.

    However, there is no single "correct" measure --- each captures a different dimension of labour market slack.

    **(c)** Even the CDS rate understates labour underutilisation because:

    - **Disguised unemployment:** Workers in agriculture with near-zero marginal productivity are counted as "employed."
    - **Discouraged workers:** People who have given up searching are classified as "not in the labour force," not as unemployed.
    - **Involuntary part-time:** Workers who want full-time work but can only find part-time work are classified as employed.
    - **Quality of employment:** The CDS does not distinguish between productive employment and survival activities (e.g., unpaid family work, subsistence agriculture).

??? question "Q7. NREGA as Unemployment Policy"
    (a) How does NREGA function as an automatic stabiliser?
    (b) Using the steady-state unemployment framework, explain the channels through which NREGA reduces unemployment.
    (c) What are the limitations of NREGA as a solution to India's youth unemployment problem?

    **Answer:**

    **(a)** NREGA is **demand-driven**: any rural household that demands work must be provided employment within 15 days. During lean agricultural seasons (when private-sector employment falls) or during economic downturns, more households demand NREGA work. The programme automatically expands without requiring new legislation or discretionary spending decisions. This counter-cyclical property makes it an automatic stabiliser, similar to how UI automatically expands during US recessions.

    **(b)** In the steady-state framework \( u^* = s/(s+f) \), NREGA operates through:

    - **Increasing \( f \):** NREGA provides a guaranteed job-finding option for rural workers. When private-sector jobs are scarce (low \( f \)), NREGA ensures \( f > 0 \) --- workers can always find employment on public works. This raises the effective job-finding rate and reduces the unemployment rate.
    - **Reducing duration dependence:** Workers who would otherwise be long-term unemployed (with deteriorating skills and morale) remain active through NREGA work, maintaining their employability.

    **(c)** NREGA is a poor solution for youth unemployment because:

    - It offers only **unskilled manual labour** (digging, road-building), which does not match the aspirations or skills of educated youth.
    - **Urban youth** are not covered (NREGA is rural only).
    - It does not address the **skills mismatch** that drives educated unemployment --- graduates need jobs in services, IT, and manufacturing, not earthwork.
    - The wage rate (Rs. 250--350/day in most states) is too low to attract educated youth who have higher reservation wages.
    - NREGA addresses the **quantity** of employment but not its **quality** --- educated youth seek formal-sector jobs with career prospects, not daily-wage manual work.

??? question "Q8. Beveridge Curve"
    The Beveridge curve plots the unemployment rate against the vacancy rate. Suppose the economy moves from point A (unemployment 6%, vacancies 3%) to point B (unemployment 8%, vacancies 2%).

    (a) Is this a movement along the Beveridge curve or a shift of the curve?
    (b) What economic event could cause this movement?
    (c) Now suppose the economy moves from point A to point C (unemployment 7%, vacancies 4%). What does this shift imply about the matching efficiency of the labour market?

    **Answer:**

    **(a)** The movement from A (6%, 3%) to B (8%, 2%) is a **movement along** the Beveridge curve (downward and to the right). Both unemployment rises and vacancies fall, which is consistent with a movement along a stable curve.

    **(b)** This movement is consistent with a **recession**: aggregate demand falls, firms reduce hiring (fewer vacancies) and increase layoffs (more unemployment). The economy slides along the Beveridge curve toward the lower-right.

    **(c)** The movement from A (6%, 3%) to C (7%, 4%) represents an **outward shift** of the Beveridge curve. Both unemployment and vacancies have increased --- there are more unfilled jobs and more jobless workers simultaneously. This implies that **matching efficiency has deteriorated**: the labour market is less effective at connecting available workers with available jobs. Possible causes include:

    - Increased **skills mismatch** (e.g., due to technological change)
    - **Geographic mismatch** (jobs in different regions from workers)
    - Extended UI benefits reducing search intensity
    - Structural changes in the economy creating mismatches

??? question "Q9. Duration Dependence"
    Explain why the probability of exiting unemployment often falls with duration. Distinguish between two competing explanations and describe how a correspondence study can help differentiate them.

    **Answer:**

    **Observation:** The longer a worker is unemployed, the lower the probability of finding a job in any given week. This is negative duration dependence.

    **Explanation 1 --- Unobserved heterogeneity:** Workers differ in unobservable qualities (motivation, interview skills, network quality). High-quality workers find jobs quickly and exit the unemployment pool early. Over time, the remaining pool is increasingly composed of hard-to-place workers. The falling exit rate reflects changing composition, not a causal effect of duration itself.

    **Explanation 2 --- True state dependence:** Unemployment itself causes worsening prospects. Skills depreciate with disuse (human capital erosion), professional networks weaken, and employers view long unemployment spells as a negative signal (stigma). The longer the spell, the harder it becomes to exit.

    **Using a correspondence study:** Kroft, Lange, and Notowidigdo (2013) sent fictitious resumes to real job postings, varying only the **length of the unemployment spell** listed on the resume. They found that resumes with longer unemployment spells received significantly fewer callbacks, even though all other qualifications were identical. This isolates the **employer stigma** channel (true state dependence) from the heterogeneity explanation, since the resume content (and hence worker quality) is held constant by design.

??? question "Q10. Comparing Unemployment Across Countries"
    The following data are given:

    | Country | Separation Rate \( s \) | Finding Rate \( f \) |
    |---------|------------------------|---------------------|
    | Country A | 0.01 | 0.20 |
    | Country B | 0.03 | 0.15 |
    | Country C | 0.02 | 0.40 |

    (a) Calculate the steady-state unemployment rate for each country.
    (b) Which country has the most dynamic (fluid) labour market?
    (c) Country B implements a strict employment protection law that reduces \( s \) to 0.01 but also reduces \( f \) to 0.05. What happens to its unemployment rate?

    **Answer:**

    **(a)** Steady-state unemployment rates:

    - Country A: \( u^* = \frac{0.01}{0.01 + 0.20} = \frac{0.01}{0.21} = 4.76\% \)
    - Country B: \( u^* = \frac{0.03}{0.03 + 0.15} = \frac{0.03}{0.18} = 16.67\% \)
    - Country C: \( u^* = \frac{0.02}{0.02 + 0.40} = \frac{0.02}{0.42} = 4.76\% \)

    **(b)** **Country C** has the most dynamic labour market. It has the highest finding rate (0.40) --- unemployed workers find jobs very quickly --- and a moderate separation rate. The high flow rates (both in and out of unemployment) indicate a fluid, flexible market. Countries A and C have the same unemployment rate, but C achieves this with much higher turnover.

    **(c)** With the new parameters for Country B:

    \[
    u^* = \frac{0.01}{0.01 + 0.05} = \frac{0.01}{0.06} = 16.67\%
    \]

    The unemployment rate **stays the same** at 16.67%. The strict employment protection reduced separations (good) but also reduced hiring (bad) by an offsetting amount. This illustrates the "Eurosclerosis" phenomenon: rigid labour market regulations may reduce both separations and hiring, leaving the unemployment rate unchanged but increasing average unemployment **duration** dramatically (workers who lose jobs take much longer to find new ones: \( 1/f = 20 \) months instead of \( 1/0.15 = 6.7 \) months).
