---
title: "Practice — Unemployment"
description: "Practice problems on unemployment types, the steady-state rate, search theory, UI design, the Beveridge curve, the Phillips curve, and India's labour market."
---

# Practice: Unemployment

Test your understanding of unemployment theory, search models, and macroeconomic connections. Questions range from definitional to computational.

---

??? question "Q1. Classifying Unemployment"
    Classify each of the following as frictional, structural, or cyclical unemployment. Briefly justify your classification.

    (a) A coal miner loses her job because the power plant switches to solar energy.

    (b) A recent college graduate spends three months searching for a first job.

    (c) A construction worker is laid off during a recession.

    (d) A software engineer quits to find a better-paying job and is unemployed for two weeks.

    (e) A textile worker in Surat loses her job because production moves to Bangladesh.

    ??? success "Answer"
        **(a) Structural.** The demand for coal miners has permanently declined due to technological change (shift to renewable energy). The worker's existing skills are no longer demanded in the new energy sector. This is not a temporary downturn but a permanent shift in the structure of the economy.

        **(b) Frictional.** The graduate is searching for an appropriate match. This is a normal part of labour market functioning --- it takes time to find the right job, and the graduate is acquiring information about available positions. The unemployment is voluntary in the sense that the graduate could presumably accept *some* job immediately.

        **(c) Cyclical.** Construction is highly sensitive to the business cycle. The layoff is driven by a fall in aggregate demand, not by a permanent change in the worker's skills or the industry's structure. When the economy recovers, construction hiring will resume.

        **(d) Frictional.** The worker voluntarily quit and is between jobs. This is a short-duration search reflecting the normal matching process. The worker is moving to a better match, which is efficient.

        **(e) Structural.** The job loss is due to a permanent geographic shift in production (globalisation/offshoring). The worker's skills may still be relevant but the jobs have relocated internationally. Retraining or geographic mobility may be required.

??? question "Q2. Steady-State Unemployment Rate Calculation"
    In a labour market with 1 million workers:

    - Each month, 2% of employed workers lose their jobs (\( s = 0.02 \)).
    - Each month, 20% of unemployed workers find jobs (\( f = 0.20 \)).

    (a) Calculate the steady-state unemployment rate.

    (b) How many workers are unemployed in steady state?

    (c) What is the expected duration of an unemployment spell?

    (d) If the government implements a job-matching programme that raises \( f \) to 0.30, what happens to the unemployment rate and expected duration?

    ??? success "Answer"
        **(a)** The steady-state unemployment rate:

        \[
        u^* = \frac{s}{s + f} = \frac{0.02}{0.02 + 0.20} = \frac{0.02}{0.22} = 0.0909 \approx 9.1\%
        \]

        **(b)** Unemployed workers \( = u^* \times L = 0.0909 \times 1{,}000{,}000 \approx 90{,}900 \) workers.

        **(c)** Expected duration \( = 1/f = 1/0.20 = 5 \) months.

        **(d)** With \( f = 0.30 \):

        \[
        u^* = \frac{0.02}{0.02 + 0.30} = \frac{0.02}{0.32} = 6.25\%
        \]

        Expected duration \( = 1/0.30 \approx 3.3 \) months.

        The unemployment rate falls from 9.1% to **6.25%** and expected duration falls from 5 months to 3.3 months. The job-matching programme reduces unemployment by increasing the rate at which unemployed workers find jobs. This illustrates why active labour market policies focused on matching can be effective.

??? question "Q3. Reservation Wage and Job Search"
    An unemployed worker receives one wage offer per week drawn from the following distribution: \$400 with probability 0.3, \$600 with probability 0.5, and \$1,000 with probability 0.2. While unemployed, the worker receives UI benefits of \$350 per week.

    (a) If the worker's reservation wage is \$600, what is the probability of accepting an offer in any given week?

    (b) What is the expected duration of unemployment (in weeks)?

    (c) What is the expected accepted wage?

    (d) If UI benefits are cut to \$200 per week, predict what happens to the reservation wage and unemployment duration. Explain.

    ??? success "Answer"
        **(a)** The worker accepts offers at or above \$600:

        \[
        P(\text{accept}) = P(w = 600) + P(w = 1000) = 0.5 + 0.2 = 0.70
        \]

        The **probability of accepting** in any given week is **70%**.

        **(b)** Expected duration:

        \[
        E[\text{duration}] = \frac{1}{P(\text{accept})} = \frac{1}{0.70} \approx 1.43 \text{ weeks}
        \]

        **(c)** The expected accepted wage, conditional on acceptance:

        \[
        E[w \mid w \geq 600] = \frac{0.5 \times 600 + 0.2 \times 1000}{0.5 + 0.2} = \frac{300 + 200}{0.70} = \frac{500}{0.70} \approx \$714
        \]

        **(d)** If UI benefits fall from \$350 to \$200:

        - The flow value of being unemployed \( b \) decreases.
        - The cost of continued search increases (the worker forgoes consumption during each additional week of search with less income support).
        - The reservation wage **falls** --- the worker becomes less selective.
        - If the reservation wage drops to \$400, the acceptance probability rises to 1.0, expected duration falls to 1 week, but the expected accepted wage falls to \( 0.3 \times 400 + 0.5 \times 600 + 0.2 \times 1000 = \$620 \), lower than the \$714 under the higher reservation wage.

        This illustrates the dual nature of UI effects: cutting benefits reduces duration (less moral hazard) but may also worsen match quality (the liquidity argument for UI --- workers take worse jobs out of financial desperation).

??? question "Q4. Unemployment Insurance: Moral Hazard vs. Liquidity"
    A country offers UI benefits equal to 60% of the prior wage for up to 26 weeks. The government proposes extending benefits to 52 weeks.

    (a) Using search theory, predict the effect on unemployment duration.

    (b) Distinguish between the moral hazard effect and the liquidity effect of this extension.

    (c) Based on Chetty (2008), which effect is likely larger for low-wealth workers? What does this imply for UI policy?

    ??? success "Answer"
        **(a)** Extending the benefit duration from 26 to 52 weeks **increases unemployment duration**. Workers who approach the 26-week exhaustion point often intensify their search --- empirical studies document a "spike" in the job-finding rate just before benefits expire. Extending to 52 weeks pushes this spike back by 26 weeks, allowing workers to remain unemployed longer.

        **(b)**

        - **Moral hazard effect:** With more weeks of benefits, workers reduce search effort because the cost of continued unemployment is lower. They may also raise their reservation wage, rejecting offers they would otherwise accept. This is a pure efficiency loss.
        - **Liquidity effect:** Cash-constrained workers who would otherwise be forced to accept a poor-quality job out of desperation can now afford to continue searching for a better match. The extension relaxes a borrowing constraint, enabling more efficient search and better worker-firm matches. This is an efficiency gain.

        **(c)** Chetty (2008) finds that the liquidity effect accounts for roughly **60%** of the UI-duration relationship for low-wealth workers. These workers have little savings and face binding liquidity constraints --- without UI, they would be forced into suboptimal matches. For wealthier workers who already have savings to smooth consumption, the effect operates more through moral hazard.

        **Policy implication:** UI extensions are most valuable for workers with low savings (where the liquidity effect dominates) and least efficient for wealthy workers (where moral hazard dominates). This suggests that UI design could be improved by conditioning benefits on wealth or by combining UI with access to borrowing facilities.

??? question "Q5. Phillips Curve Analysis"
    The expectations-augmented Phillips curve for an economy is:

    \[
    \pi = \pi^e - 0.5(u - 6)
    \]

    where \( \pi \) is the inflation rate (%), \( \pi^e \) is expected inflation (%), and \( u \) is the unemployment rate (%).

    (a) What is the NAIRU?

    (b) If expected inflation is 3% and the actual unemployment rate is 4%, what is the inflation rate?

    (c) If expected inflation is 3% and the actual unemployment rate is 8%, what is the inflation rate?

    (d) Suppose the government tries to keep unemployment at 4% permanently. Trace the path of inflation over three periods, assuming adaptive expectations (\( \pi^e_t = \pi_{t-1} \)) and \( \pi_0^e = 3\% \). Why is this unsustainable?

    ??? success "Answer"
        **(a)** The NAIRU is the unemployment rate at which \( \pi = \pi^e \):

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

        **(d)** Tracing the path with \( u = 4\% \) throughout and adaptive expectations:

        - **Period 1:** \( \pi^e = 3\% \), so \( \pi = 3 - 0.5(4-6) = 4\% \).
        - **Period 2:** \( \pi^e = 4\% \), so \( \pi = 4 - 0.5(4-6) = 5\% \).
        - **Period 3:** \( \pi^e = 5\% \), so \( \pi = 5 - 0.5(4-6) = 6\% \).

        Inflation **accelerates** by 1 percentage point each period. The government can keep unemployment below the NAIRU only at the cost of ever-increasing inflation. In the long run, the only sustainable unemployment rate is \( u^* = 6\% \), and any attempt to permanently push below it produces not just high inflation but accelerating inflation. This is the core of Friedman's (1968) natural rate hypothesis: the long-run Phillips curve is vertical at \( u^* \).

??? question "Q6. The Beveridge Curve"
    The Beveridge curve plots the unemployment rate against the vacancy rate. Consider three points:

    - **Point A:** unemployment 6%, vacancies 3%
    - **Point B:** unemployment 8%, vacancies 2%
    - **Point C:** unemployment 7%, vacancies 4%

    (a) Is the movement from A to B a movement along the Beveridge curve or a shift? What economic event could cause it?

    (b) What does the movement from A to C imply about the matching efficiency of the labour market?

    (c) After the 2008--09 Great Recession, the US experienced a combination of recovering vacancies but persistently high unemployment. What does this suggest about the Beveridge curve?

    ??? success "Answer"
        **(a)** The movement from A (6%, 3%) to B (8%, 2%) is a **movement along** the Beveridge curve (downward and to the right). Unemployment rises while vacancies fall --- both variables move in opposite directions, consistent with a stable curve. This movement is consistent with a **recession**: aggregate demand falls, firms reduce hiring (fewer vacancies) and increase layoffs (more unemployment).

        **(b)** The movement from A (6%, 3%) to C (7%, 4%) represents an **outward shift** of the Beveridge curve. Both unemployment and vacancies have increased simultaneously --- there are more unfilled jobs and more jobless workers at the same time. This implies that **matching efficiency has deteriorated**: the labour market is less effective at connecting workers with vacancies. Possible causes:

        - Increased **skills mismatch** (e.g., vacancies require IT skills but unemployed workers have manufacturing skills)
        - **Geographic mismatch** (jobs in cities, workers in rural areas)
        - Extended UI benefits reducing search intensity
        - Employer stigma against the long-term unemployed

        **(c)** This pattern --- vacancies recovering while unemployment stays high --- is precisely an **outward shift** of the Beveridge curve. It suggests that the Great Recession was not purely cyclical but also had structural dimensions: skills mismatch, geographic immobility (homeowners with underwater mortgages could not relocate), and the accumulation of long-term unemployed workers who employers were reluctant to hire. The matching function parameter \( A \) had declined.

??? question "Q7. Indian Unemployment Measurement"
    India's PLFS reports three unemployment rates for 2023--24: UPSS at 3.2%, CWS at 5.0%, and CDS at approximately 7.5%.

    (a) Explain why these three measures give such different numbers.

    (b) Which measure best captures the extent of labour underutilisation in India? Justify your answer.

    (c) Why might even the highest measure (CDS) understate the true extent of labour market distress?

    ??? success "Answer"
        **(a)** The three measures differ in their **reference period** and **classification thresholds**:

        - **UPSS (Usual Principal + Subsidiary Status):** Classifies a person based on their primary activity over the **entire year**. Anyone who worked even briefly in a subsidiary capacity during the year is "employed." This yields the lowest rate because seasonal and intermittent workers count as employed.
        - **CWS (Current Weekly Status):** Classifies based on activity during the **reference week**. Someone who was employed last month but jobless this week is counted as unemployed. Captures more short-duration and seasonal unemployment.
        - **CDS (Current Daily Status):** Classifies based on activity on **each day** of the reference week and averages across days. A worker employed Monday--Wednesday but idle Thursday--Saturday registers as partially unemployed. Yields the highest rate because it captures within-week underemployment.

        **(b)** The **CDS rate** arguably best captures labour underutilisation because:

        - It accounts for partial unemployment within a week, which is pervasive in India's casual and seasonal labour market.
        - India's informal economy features extensive day-labour arrangements where workers may find work on some days but not others.
        - The UPSS rate is misleadingly low --- it classifies a farmer who works intensively for four months and sits idle for eight as "employed."

        However, no single measure is "correct." Each captures a different dimension of slack, and a comprehensive assessment requires examining all three together along with underemployment measures.

        **(c)** Even the CDS rate understates true labour market distress because:

        - **Disguised unemployment:** Workers in agriculture with near-zero marginal productivity are counted as "employed." India has ~42% of its workforce in agriculture producing ~15% of GDP.
        - **Discouraged workers:** People who have given up searching (especially women in rural areas) are classified as "not in the labour force," not as unemployed. India's female LFPR is among the world's lowest.
        - **Involuntary part-time work:** Workers who want full-time work but can only find a few hours of casual work are classified as employed.
        - **Quality of employment:** The CDS does not distinguish between productive formal employment and survival activities (unpaid family work, subsistence farming, petty vending).
        - **Wait unemployment of educated youth** is partially captured but the aspiration mismatch --- graduates working as delivery drivers or security guards --- is not reflected in unemployment figures at all.

??? question "Q8. MGNREGA and the Steady-State Framework"
    (a) How does MGNREGA function as an automatic stabiliser in rural India?

    (b) Using the steady-state unemployment framework \( u^* = s/(s+f) \), explain the channels through which MGNREGA affects unemployment.

    (c) What are three limitations of MGNREGA as a solution to India's overall unemployment problem?

    ??? success "Answer"
        **(a)** MGNREGA is **demand-driven**: any rural household that requests work must be provided employment within 15 days (or receive an unemployment allowance). During lean agricultural seasons or economic downturns, more households demand MGNREGA work, and the programme automatically expands. This counter-cyclical property operates without requiring new legislation or discretionary policy decisions --- similar to how UI automatically expands during US recessions.

        **(b)** In the steady-state framework:

        - **Increasing \( f \):** MGNREGA guarantees a job-finding option for rural workers. When private-sector jobs are scarce (low \( f \) in the private market), MGNREGA ensures that the effective \( f > 0 \) --- workers can always find employment on public works. This raises the overall job-finding rate and lowers the steady-state unemployment rate.
        - **Reducing duration dependence:** Workers who would otherwise be long-term unemployed (with deteriorating skills and morale) remain active through MGNREGA, maintaining their employability for when private-sector jobs return.
        - **Potential offset through \( s \):** By raising the reservation wage floor, MGNREGA may increase separations from very low-wage private employment (workers quit bad jobs knowing MGNREGA is available). This could partially offset the reduction in \( u^* \).

        **(c)** Three limitations:

        1. **Only unskilled manual labour:** MGNREGA offers earthwork, road-building, and watershed construction --- irrelevant for educated youth who seek formal-sector careers. It cannot address the structural skills mismatch driving educated unemployment.
        2. **Rural only:** Urban unemployment and underemployment are not covered. India is rapidly urbanising, and urban youth face severe joblessness.
        3. **Quantity not quality:** MGNREGA provides 100 days of low-wage work but no career progression, skill development, or pathway to formal employment. It addresses immediate income needs but not the structural transformation required for sustained employment generation.

??? question "Q9. Duration Dependence: Heterogeneity vs. State Dependence"
    The probability of exiting unemployment often falls with duration --- a phenomenon called negative duration dependence.

    (a) Explain the **unobserved heterogeneity** interpretation of this pattern.

    (b) Explain the **true state dependence** interpretation.

    (c) Describe how the correspondence study by Kroft, Lange, and Notowidigdo (2013) helps distinguish between these two explanations. What did they find?

    ??? success "Answer"
        **(a) Unobserved heterogeneity:** Workers differ in qualities that are hard to measure --- motivation, interview skills, network quality, appearance, soft skills. High-quality workers find jobs quickly and exit the unemployment pool early. Over time, the remaining pool is increasingly composed of harder-to-place workers. The **declining exit rate** reflects changing pool composition, not a causal effect of unemployment duration itself. If you could observe all relevant worker characteristics, the duration dependence might disappear.

        **(b) True state dependence:** Unemployment itself *causes* worsening prospects through several mechanisms:

        - **Human capital depreciation:** Skills erode with disuse --- a programmer who has not coded for a year may fall behind.
        - **Network decay:** Professional contacts weaken without regular interaction.
        - **Psychological effects:** Prolonged unemployment can reduce confidence, motivation, and mental health.
        - **Employer stigma:** Employers view a long unemployment spell as a negative signal about the worker's quality, creating a self-fulfilling prophecy.

        **(c)** Kroft et al. (2013) sent **fictitious resumes** to real job postings. The resumes were identical in qualifications, education, and experience --- only the **length of the current unemployment spell** was varied (1 month to 36 months). Since the resume content was held constant by design, any difference in callback rates must reflect employer behaviour (stigma), not actual differences in worker quality.

        **Findings:** Resumes with longer unemployment spells received significantly **fewer callbacks**. A resume showing 8+ months of unemployment received roughly 45% fewer callbacks than an otherwise identical resume showing 1 month. This provides clean evidence for the employer stigma channel of true state dependence --- employers use duration as a screening signal, creating a vicious cycle for the long-term unemployed.

??? question "Q10. Comparing Labour Markets Across Countries"
    The following data are given:

    | Country | Separation Rate \( s \) | Finding Rate \( f \) |
    |---------|------------------------|---------------------|
    | Country A | 0.01 | 0.20 |
    | Country B | 0.03 | 0.15 |
    | Country C | 0.02 | 0.40 |

    (a) Calculate the steady-state unemployment rate for each country.

    (b) Which country has the most dynamic (fluid) labour market? Explain.

    (c) Country B implements a strict employment protection law that reduces \( s \) to 0.01 but also reduces \( f \) to 0.05. Calculate the new unemployment rate. What happens to expected unemployment duration? Comment on the "Eurosclerosis" phenomenon.

    ??? success "Answer"
        **(a)** Steady-state unemployment rates:

        - Country A: \( u^* = \frac{0.01}{0.01 + 0.20} = \frac{0.01}{0.21} = 4.76\% \)
        - Country B: \( u^* = \frac{0.03}{0.03 + 0.15} = \frac{0.03}{0.18} = 16.67\% \)
        - Country C: \( u^* = \frac{0.02}{0.02 + 0.40} = \frac{0.02}{0.42} = 4.76\% \)

        **(b)** **Country C** has the most dynamic labour market. It has the highest finding rate (\( f = 0.40 \)) and a moderate separation rate (\( s = 0.02 \)). The high turnover means workers move quickly between jobs. Countries A and C have the same unemployment rate (4.76%), but C achieves it with much higher flow rates --- it resembles a flexible, Anglo-Saxon style labour market.

        **(c)** With the new parameters for Country B (\( s = 0.01, f = 0.05 \)):

        \[
        u^* = \frac{0.01}{0.01 + 0.05} = \frac{0.01}{0.06} = 16.67\%
        \]

        The unemployment rate **stays the same** at 16.67%! The strict employment protection reduced separations (good) but also discouraged hiring (bad) by an exactly offsetting amount.

        However, expected duration changes dramatically:

        - Before: \( 1/f = 1/0.15 = 6.7 \) months
        - After: \( 1/f = 1/0.05 = 20 \) months

        This is the **"Eurosclerosis"** phenomenon observed in many European countries: rigid labour market regulations reduce both separations and hiring. The unemployment rate may not change, but the *nature* of unemployment transforms --- from many short spells to fewer but much longer spells. Long-term unemployment is more damaging (human capital depreciation, stigma, psychological harm) than an equal amount of short-term unemployment.

??? question "Q11. Steady-State with a Shock"
    An economy is initially in steady state with \( s = 0.015 \) and \( f = 0.25 \). A recession hits, and the separation rate doubles to \( s' = 0.03 \) while the finding rate halves to \( f' = 0.125 \).

    (a) Calculate the pre-recession and recession steady-state unemployment rates.

    (b) By what factor does the expected duration of unemployment change?

    (c) Which change contributes more to the rise in unemployment: the increase in \( s \) or the decrease in \( f \)? (Hint: calculate \( u^* \) with only one parameter changed at a time.)

    ??? success "Answer"
        **(a)**

        - Pre-recession: \( u^* = \frac{0.015}{0.015 + 0.25} = \frac{0.015}{0.265} = 5.66\% \)
        - Recession: \( u^* = \frac{0.03}{0.03 + 0.125} = \frac{0.03}{0.155} = 19.35\% \)

        The unemployment rate rises from 5.66% to **19.35%** --- more than tripling.

        **(b)** Expected duration:

        - Pre-recession: \( 1/f = 1/0.25 = 4 \) months
        - Recession: \( 1/f' = 1/0.125 = 8 \) months

        Duration **doubles** from 4 to 8 months.

        **(c)** Decomposing the contributions:

        - Only \( s \) changes (\( s = 0.03, f = 0.25 \)): \( u^* = \frac{0.03}{0.03 + 0.25} = \frac{0.03}{0.28} = 10.71\% \). Rise: \( 10.71 - 5.66 = 5.05 \) pp.
        - Only \( f \) changes (\( s = 0.015, f = 0.125 \)): \( u^* = \frac{0.015}{0.015 + 0.125} = \frac{0.015}{0.14} = 10.71\% \). Rise: \( 10.71 - 5.66 = 5.05 \) pp.

        In this symmetric example, both contribute equally. However, Shimer (2012) shows that in practice, most of the cyclical variation in US unemployment is driven by changes in the **finding rate** rather than the separation rate --- the difficulty of finding new jobs matters more than the rate of job loss.

??? question "Q12. Stata: Computing Unemployment Rates from PLFS"
    You have PLFS person-level microdata. Describe the steps (in Stata pseudocode or logic) to compute:

    (a) The CWS unemployment rate for the 15+ population.

    (b) The CWS unemployment rate separately for youth (15--29) and prime-age (30--59) workers.

    (c) The CWS unemployment rate by education level (below secondary, secondary, graduate and above).

    ??? success "Answer"
        ```stata
        * Load PLFS person-level data
        use plfs_person_2024, clear

        * (a) Define unemployment under CWS
        * CWS activity status codes: 81-82 = unemployed seeking/available
        * Activity status 11-72 = various forms of employment
        gen unemployed_cws = (cws_status >= 81 & cws_status <= 82)
        gen in_lf_cws = (cws_status >= 11 & cws_status <= 82)

        * Overall CWS unemployment rate (15+ population)
        sum unemployed_cws if in_lf_cws == 1 & age >= 15 [aw = weight]
        * The mean of the dummy = unemployment rate

        * (b) Unemployment rate by age group
        gen age_group = .
        replace age_group = 1 if age >= 15 & age <= 29
        replace age_group = 2 if age >= 30 & age <= 59
        label define agegrp 1 "Youth (15-29)" 2 "Prime (30-59)"
        label values age_group agegrp

        table age_group if in_lf_cws == 1 [aw = weight], ///
            stat(mean unemployed_cws) nformat(%9.3f)

        * (c) Unemployment rate by education level
        gen edu_group = .
        replace edu_group = 1 if education < 10   // below secondary
        replace edu_group = 2 if education >= 10 & education < 15  // secondary
        replace edu_group = 3 if education >= 15   // graduate and above
        label define edugrp 1 "Below Secondary" 2 "Secondary" ///
            3 "Graduate+"
        label values edu_group edugrp

        table edu_group if in_lf_cws == 1 [aw = weight], ///
            stat(mean unemployed_cws) nformat(%9.3f)

        * Key finding to verify: Graduate+ unemployment rate should be
        * HIGHER than below-secondary — India's educated unemployment paradox
        ```

        **Key interpretation:** If your results show that graduate unemployment exceeds below-secondary unemployment, this confirms India's educated unemployment paradox: more education is associated with *higher* unemployment, reflecting wait unemployment and aspiration mismatch.
