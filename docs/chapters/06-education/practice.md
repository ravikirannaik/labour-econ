---
title: "Practice — Education"
---

# Practice: Education

Test your understanding of the human capital model, the Mincer equation, ability bias, and the signalling model. Click on a question to reveal the answer.

---

??? question "Q1. A worker is deciding whether to attend a 2-year MBA program. Her current salary is Rs 8 lakh per year. The MBA costs Rs 5 lakh per year in tuition. After the MBA, she expects to earn Rs 14 lakh per year. She plans to work for 30 more years after graduating. Should she enrol if the discount rate is 10%?"

    **Step 1: Calculate the costs (first 2 years).**

    Total annual cost = foregone earnings + tuition = Rs 8 lakh + Rs 5 lakh = Rs 13 lakh per year.

    Present value of costs:

    \[
    PV_{\text{costs}} = \frac{13}{1.10} + \frac{13}{(1.10)^2} = 11.82 + 10.74 = \text{Rs } 22.56 \text{ lakh}
    \]

    **Step 2: Calculate the benefits (years 3--32).**

    Annual wage gain = Rs 14 lakh - Rs 8 lakh = Rs 6 lakh per year for 30 years, starting in year 3.

    \[
    PV_{\text{benefits}} = \sum_{t=3}^{32} \frac{6}{(1.10)^t} = 6 \times \left[\frac{1 - (1.10)^{-30}}{0.10}\right] \times \frac{1}{(1.10)^2}
    \]

    The annuity factor for 30 years at 10% is \(\frac{1 - (1.10)^{-30}}{0.10} = 9.427\).

    Discounting back 2 years: \(PV_{\text{benefits}} = 6 \times 9.427 \times \frac{1}{1.21} = 6 \times 7.792 = \text{Rs } 46.75 \text{ lakh}\).

    **Step 3: Compare.**

    Net present value = Rs 46.75 - Rs 22.56 = **Rs 24.19 lakh > 0**.

    **Yes**, she should enrol. The MBA investment has a positive NPV at a 10% discount rate.

??? question "Q2. Explain the Mincer earnings equation. What does each coefficient represent, and why is the dependent variable in log form?"

    The Mincer earnings equation is:

    \[
    \ln w_i = \alpha + \beta s_i + \gamma_1 x_i + \gamma_2 x_i^2 + \varepsilon_i
    \]

    **Coefficients:**

    - \(\alpha\): the log wage of a worker with zero schooling and zero experience.
    - \(\beta\): the rate of return to schooling. An additional year of education is associated with a \(100\beta\)% increase in wages. Typical estimates: 0.06--0.12 (6--12%).
    - \(\gamma_1 > 0\): experience raises wages (learning-by-doing, on-the-job training).
    - \(\gamma_2 < 0\): the experience effect diminishes over time (the earnings-experience profile is concave). This reflects slowing skill acquisition and possible depreciation.

    **Why log wages?** The human capital model predicts that each year of schooling raises productivity by a constant **percentage** (not a constant amount). This implies \(w = e^{\alpha + \beta s + \ldots}\), so \(\ln w\) is linear in \(s\). The log form also means that \(\beta\) has a direct interpretation as an approximate percentage change, which is convenient.

??? question "Q3. What is ability bias? In which direction does it bias the OLS estimate of the return to schooling?"

    **Ability bias** arises because individuals with higher innate ability (intelligence, motivation, discipline) tend to both (a) acquire more education and (b) earn higher wages independently of their education. If ability is omitted from the regression:

    \[
    \hat{\beta}_{\text{OLS}} = \beta + \underbrace{\frac{\text{Cov}(s_i, a_i)}{\text{Var}(s_i)}}_{\text{ability bias}}
    \]

    Since \(\text{Cov}(s_i, a_i) > 0\) (more able people get more schooling), the OLS estimate is **upward biased** --- it overstates the causal return to education.

    **However**, the empirical evidence from IV studies (twins, compulsory schooling) suggests the bias is surprisingly **small**. IV estimates are often similar to or even larger than OLS. One explanation: if credit-constrained individuals (with high discount rates) have high marginal returns to schooling, their underinvestment creates a downward "discount rate bias" that partially offsets the upward ability bias.

??? question "Q4. Angrist and Krueger (1991) use quarter of birth as an instrument for years of schooling. Explain the identification strategy. What are the two conditions the instrument must satisfy?"

    **Identification strategy:** In the US, compulsory schooling laws require students to stay in school until a certain age (typically 16). Students born in the first quarter of the year (January--March) reach this minimum school-leaving age earlier in the academic year and are more likely to drop out with fewer years of education. Quarter of birth thus creates exogenous variation in schooling.

    **Two conditions for a valid instrument:**

    1. **Relevance:** Quarter of birth must affect years of schooling. This is verified empirically: Q1-born individuals do have slightly less education on average.

    2. **Exogeneity (exclusion restriction):** Quarter of birth must affect wages **only** through its effect on schooling --- it must not directly affect earnings or be correlated with unobserved ability. This is plausible since birth timing is largely random (though some researchers have raised concerns about seasonal patterns in births by socioeconomic status).

    **Result:** The IV estimate is approximately 7--8% per year of schooling, similar to OLS. This suggests that ability bias in the Mincer equation is small.

??? question "Q5. Explain the Spence signalling model. Under what conditions does a separating equilibrium exist?"

    In Spence's model, education does not increase productivity but serves as a **signal** of pre-existing ability to employers who cannot directly observe worker type.

    **Setup:**

    - Two types: High-ability (H) and low-ability (L), with productivities \(w_H > w_L\).
    - Education costs more for L-types: \(c_L > c_H\) per year.

    **Separating equilibrium:** There exists a threshold \(s^*\) such that H-types acquire \(s^*\) years and earn \(w_H\), while L-types acquire 0 years and earn \(w_L\), provided:

    \[
    \frac{w_H - w_L}{c_L} < s^* < \frac{w_H - w_L}{c_H}
    \]

    - The **left inequality** ensures L-types do not find it worthwhile to mimic H-types (the cost of acquiring \(s^*\) exceeds the wage gain).
    - The **right inequality** ensures H-types do find it worthwhile to signal (the wage gain exceeds their cost of \(s^*\) years).

    This equilibrium requires sufficient cost differential between types. If both types face similar costs, no separating equilibrium exists and education cannot serve as an effective signal.

??? question "Q6. What is the 'sheepskin effect'? How does it help distinguish between the human capital and signalling models?"

    The **sheepskin effect** refers to the observation that wages jump **discontinuously** upon completion of a degree (e.g., graduating from college), over and above the smooth return to additional years of schooling.

    For example, a worker with 15 years of education (3 years of college, no degree) earns less than a worker with 16 years (4 years, bachelor's degree), and the jump at year 16 is larger than what the Mincer equation would predict for a single additional year.

    **Implications:**

    - **Human capital model:** Predicts smooth returns --- each year of schooling adds roughly the same productivity. There should be no special jump at degree completion.
    - **Signalling model:** Predicts a jump at degree completion, because the degree is the signal that employers observe. Acquiring most of the coursework but not the credential does not convey the signal.

    The empirical finding of a sheepskin effect provides evidence that signalling plays **some** role. However, the effect is modest compared to the total return to schooling, suggesting that human capital accumulation remains the dominant channel.

??? question "Q7. Using the Mincer equation, a worker with 12 years of schooling and 10 years of experience earns Rs 25,000/month. If the estimated return to schooling is 8%, what is the predicted wage of an otherwise identical worker with 16 years of schooling?"

    The Mincer equation in levels (exponentiating the log equation) gives:

    \[
    \frac{w_{16}}{w_{12}} = e^{\beta(16-12)} = e^{0.08 \times 4} = e^{0.32}
    \]

    \[
    e^{0.32} \approx 1.377
    \]

    \[
    w_{16} = 25{,}000 \times 1.377 = \text{Rs } 34{,}430/\text{month}
    \]

    The predicted wage is approximately **Rs 34,430 per month** --- a 37.7% increase for 4 additional years of schooling. Note that we used the exact formula \(e^{0.32}\) rather than the linear approximation \(1 + 0.32 = 1.32\), which would underestimate the gain.

??? question "Q8. Why might the return to education in India differ between the formal and informal sectors?"

    Several factors explain higher returns in the formal sector:

    1. **Credentialism:** Formal-sector employers (government, large firms) use educational qualifications as screening devices for hiring and pay-scale placement. A degree is often a hard requirement for a job grade, creating a large wage jump.

    2. **Institutional wage-setting:** Government pay commissions and collective bargaining in the formal sector explicitly link pay scales to educational attainment. This creates a mechanical link between years of schooling and wages.

    3. **Productivity channel:** Formal-sector jobs may require more cognitive or technical skills where education genuinely raises productivity (e.g., engineering, accounting, IT).

    4. **Selection:** Workers who enter the formal sector are positively selected on ability. The education-wage correlation in the formal sector partly reflects this selection rather than a higher causal return.

    5. **Informal sector constraints:** In the informal sector, many jobs are physically intensive and do not require or reward educational credentials. Wages are determined by local bargaining and piece rates, not by qualifications. A domestic worker with a Class X certificate earns the same as one without it.

    **Implication:** Estimating a single Mincer return for all Indian workers obscures this heterogeneity. The high average return to education in India partly reflects the premium for accessing formal-sector employment, not just the productivity effect of schooling.

??? question "Q9. A researcher estimates the Mincer equation on Indian PLFS data and finds the coefficient on years of schooling is 0.10 for men and 0.14 for women. Does this mean education is more valuable for women?"

    The higher coefficient for women (\(\hat{\beta}_{\text{women}} = 0.14\)) means that each additional year of schooling is associated with a 14% increase in wages for women, compared to 10% for men. However, several caveats are needed:

    1. **Selection bias:** Women's labour force participation in India is very low (around 25--35%). Women who work are a **positively selected** subsample --- they tend to be better educated and in better jobs. The high estimated return may partly reflect this selection rather than the true productivity effect.

    2. **Base wage:** A 14% increase on a low base wage may be a smaller absolute gain than a 10% increase on a high base wage. If women's average wage is Rs 10,000 and men's is Rs 18,000, then the absolute gains are Rs 1,400 vs. Rs 1,800.

    3. **Occupational sorting:** Women with higher education may disproportionately enter high-return formal-sector occupations (teaching, nursing, banking), inflating the observed return.

    4. **Heckman correction:** To account for selection into employment, one should estimate a Heckman two-step model, using the first stage to model the participation decision and the second stage to correct the wage equation. The corrected return is typically lower.

    **Interpretation:** Education may genuinely be more transformative for women (opening doors that would otherwise be closed), but the high coefficient also reflects sample selection.

??? question "Q10. Explain the difference between private and social returns to education. Under the signalling model, which is larger?"

    - **Private return:** The wage gain that an individual receives from an additional year of schooling. This is what the Mincer equation measures.

    - **Social return:** The increase in aggregate output (GDP) from an additional year of schooling for one worker. This includes the private return plus any positive externalities (better health outcomes, lower crime, civic participation, knowledge spillovers).

    **Under the human capital model:** Education raises productivity, so the social return equals or exceeds the private return (due to externalities). Policy implication: subsidise education.

    **Under the signalling model:** Education merely reallocates workers across jobs without increasing total output. The private return is positive (the individual earns more), but the social return is **zero** --- one worker's gain comes at another's expense (the degree holder takes the job the non-degree holder would have gotten). Policy implication: education subsidies are wasteful because they encourage a costly arms race in credentials.

    **In practice:** The social return lies between the two extremes. Education is partly productive and partly signalling. Policies should focus on the kinds of education that genuinely build skills (vocational training, quality primary education) rather than simply extending credential requirements.

??? question "Q11. A government introduces a compulsory schooling law requiring all children to complete 10 years of education. Use the human capital framework to predict the effects on (a) average wages and (b) the distribution of wages."

    **(a) Average wages:**

    The law forces some individuals --- those who would have chosen fewer than 10 years of schooling --- to acquire more education. Under the human capital model, this additional schooling increases their productivity and wages. Average wages in the economy should **rise**.

    However, the marginal individuals (those forced to stay in school) had chosen less education because their marginal rate of return was below their discount rate. For them, the return to the additional years is lower than for those who would have chosen to stay anyway. The average return to the mandated additional years may be **lower** than the average return to voluntarily acquired schooling.

    **(b) Wage distribution:**

    The law compresses the education distribution from below (everyone now has at least 10 years). Since those at the bottom of the education distribution also tend to be at the bottom of the wage distribution, their wages rise. The result is a **compression** of the wage distribution --- wages become more equal.

    **Caveats:** If school quality is poor, the mandated years may produce limited human capital, weakening both effects. Also, general equilibrium effects matter: if the supply of workers with 10+ years of schooling increases sharply, the return to schooling may decline (supply shift along a downward-sloping demand curve for educated workers).

??? question "Q12. How would you run a Mincer regression in Stata using PLFS data?"

    !!! stata "Mincer Regression in Stata"

        ```stata
        * Load PLFS person-level data
        use "/path/to/plfs_person_2024.dta", clear

        * Generate experience variable (potential experience)
        gen experience = age - years_of_education - 6
        gen experience_sq = experience^2

        * Keep wage/salaried workers only
        keep if employment_status == 31 | employment_status == 41

        * Generate log wages (monthly earnings)
        gen ln_wage = ln(monthly_earnings)

        * Basic Mincer equation
        reg ln_wage years_of_education experience experience_sq

        * Extended Mincer with controls
        reg ln_wage years_of_education experience experience_sq ///
            i.female i.urban i.social_group, robust

        * Separate regressions by gender
        reg ln_wage years_of_education experience experience_sq ///
            if female == 0, robust
        estimates store male

        reg ln_wage years_of_education experience experience_sq ///
            if female == 1, robust
        estimates store female

        * Compare coefficients
        estimates table male female, b se
        ```

        **Interpreting the output:** The coefficient on `years_of_education` gives \(\hat{\beta}\) --- the estimated percentage return to schooling. A coefficient of 0.08 means an 8% wage increase per additional year. The experience terms trace out the concave earnings profile. The `robust` option corrects standard errors for heteroskedasticity.

---

<div style="display: flex; justify-content: space-between; margin-top: 2rem;">
<a href="../06-education/">:material-arrow-left: Chapter Content</a>
<a href="../06-education/resources/">Resources :material-arrow-right:</a>
</div>
