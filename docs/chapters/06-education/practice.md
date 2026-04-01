---
title: "Practice — Education"
description: "Practice problems on human capital investment, the Mincer equation, ability bias, signalling, and training."
---

# Practice: Education

Test your understanding of the human capital model, the Mincer equation, ability bias, the signalling model, and on-the-job training. Click on a question to reveal the answer.

---

??? question "Q1. Present Value of the Schooling Decision"

    A worker is deciding whether to attend a 2-year MBA programme. Her current salary is Rs 8 lakh per year. The MBA costs Rs 5 lakh per year in tuition. After the MBA, she expects to earn Rs 14 lakh per year. She plans to work for 30 more years after graduating. Should she enrol if the discount rate is 10%?

    ??? success "Answer"

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

        **Yes**, she should enrol. The MBA has a positive NPV at a 10% discount rate.

        **Follow-up:** At what discount rate would the NPV equal zero? That rate is the **internal rate of return (IRR)** of the MBA investment. Since the NPV is comfortably positive at 10%, the IRR must be substantially higher --- the MBA is a good investment unless the worker is extremely impatient or faces very high borrowing costs.

??? question "Q2. The Stopping Rule and Discount Rates"

    Two workers, Anya and Bunty, face the same marginal rate of return schedule for schooling: \(\text{MRR}(s) = 0.20 - 0.01s\), where \(s\) is years of schooling. Anya's discount rate is 5% and Bunty's is 12%. How much schooling does each acquire? Explain the economic intuition.

    ??? success "Answer"

        The stopping rule says each worker acquires schooling until \(\text{MRR}(s^*) = r\).

        **Anya** (\(r = 0.05\)):

        \[
        0.20 - 0.01 s^* = 0.05 \implies s^* = \frac{0.20 - 0.05}{0.01} = 15 \text{ years}
        \]

        **Bunty** (\(r = 0.12\)):

        \[
        0.20 - 0.01 s^* = 0.12 \implies s^* = \frac{0.20 - 0.12}{0.01} = 8 \text{ years}
        \]

        **Intuition:** Anya is more patient (lower discount rate) --- she values future earnings more highly, so she is willing to stay in school longer. Bunty is impatient or credit-constrained --- he discounts the future heavily and drops out earlier, even though the 9th through 15th years of schooling have positive returns. This is why **credit constraints cause underinvestment in human capital**: workers like Bunty would benefit from more schooling but cannot afford to wait.

        **Policy implication:** Student loans or scholarships that effectively lower Bunty's discount rate from 12% to 5% would induce him to acquire 7 more years of schooling --- a large efficiency gain.

??? question "Q3. Interpreting the Mincer Equation"

    A researcher estimates the following Mincer equation on Indian PLFS data:

    \[
    \ln w_i = 6.80 + 0.085 \, s_i + 0.045 \, x_i - 0.0007 \, x_i^2
    \]

    (a) What is the estimated return to schooling? (b) At what experience level do earnings peak? (c) What is the predicted monthly wage for a worker with 16 years of schooling and 10 years of experience?

    ??? success "Answer"

        **(a)** The estimated return to schooling is \(\hat{\beta} = 0.085\), or **8.5% per year**. Each additional year of education is associated with an 8.5% increase in wages, holding experience constant.

        **(b)** Earnings peak where the first derivative with respect to experience equals zero:

        \[
        \frac{\partial \ln w}{\partial x} = 0.045 - 2(0.0007)x = 0.045 - 0.0014x = 0
        \]

        \[
        x^* = \frac{0.045}{0.0014} \approx 32.1 \text{ years}
        \]

        Earnings peak at approximately **32 years of experience**. This is a typical finding --- earnings rise through most of the career and begin to decline only in the last decade before retirement.

        **(c)** Predicted log wage:

        \[
        \ln w = 6.80 + 0.085(16) + 0.045(10) - 0.0007(100) = 6.80 + 1.36 + 0.45 - 0.07 = 8.54
        \]

        \[
        w = e^{8.54} \approx 5{,}112
        \]

        The predicted monthly wage is approximately **Rs 5,112**. (The level depends on whether the dependent variable is log of daily, weekly, or monthly earnings, and on the currency unit. The key skill is the calculation procedure.)

??? question "Q4. Direction of Ability Bias"

    Explain ability bias in the Mincer regression. In which direction does it bias the OLS estimate? Under what circumstances could the bias be downward rather than upward?

    ??? success "Answer"

        **Ability bias** arises because innate ability \(a_i\) (intelligence, motivation, conscientiousness) is unobserved in the Mincer regression but is correlated with both schooling and wages:

        \[
        \hat{\beta}_{\text{OLS}} = \beta + \frac{\text{Cov}(s_i, a_i)}{\text{Var}(s_i)}
        \]

        Since more able individuals tend to acquire more schooling (\(\text{Cov}(s_i, a_i) > 0\)), the OLS estimate is **upward biased** --- it attributes to education what is really a return to ability.

        **When could the bias be downward?**

        Card (1999) notes a **discount rate bias** that works in the opposite direction. If individuals who are most responsive to instruments like compulsory schooling laws (those at the margin of dropping out) have **higher-than-average marginal returns** to schooling, then OLS --- which estimates the average return --- may actually *understate* the return for these marginal individuals. The IV estimate (which captures the local average treatment effect for compliers) can therefore exceed OLS.

        Empirically, IV estimates are often similar to or slightly larger than OLS, suggesting that ability bias and discount rate bias roughly cancel out, or that ability bias is modest.

??? question "Q5. The Angrist-Krueger Quarter-of-Birth Instrument"

    Angrist and Krueger (1991) use quarter of birth as an instrument for years of schooling. (a) Explain the identification strategy. (b) State the two conditions the instrument must satisfy. (c) What is a potential threat to the exclusion restriction?

    ??? success "Answer"

        **(a) Identification strategy:** In the US, compulsory schooling laws require students to remain in school until a specified age (typically 16). Students born in the first quarter (January--March) reach this minimum age earlier in the academic year, so they can legally drop out with slightly fewer completed years of schooling. Quarter of birth thus generates exogenous variation in education that is unrelated to ability.

        **(b) Two IV conditions:**

        1. **Relevance:** Quarter of birth must affect years of schooling. Verified empirically: Q1-born students average about 0.1 fewer years of education.
        2. **Exclusion restriction (exogeneity):** Quarter of birth must affect wages *only* through its effect on schooling --- it must not directly affect earnings or be correlated with unobserved determinants of earnings.

        **(c) Potential threats:**

        - **Seasonal fertility patterns:** If higher-SES families are more likely to have children in certain quarters, then quarter of birth is correlated with family background (and hence ability). Some evidence for this exists but the effects are small.
        - **Weak instrument problem:** Bound, Jaeger, and Baker (1995) show that the first-stage effect is very small (only 0.1 years), making the instrument weak. Weak instruments can produce severely biased IV estimates and unreliable inference. This is a serious methodological concern.
        - **Age-at-school-entry effects:** Quarter of birth also affects the age at which a child starts school, which could independently affect cognitive development and later earnings.

??? question "Q6. Signalling: Constructing the Separating Equilibrium"

    In a labour market, high-ability workers have productivity \(w_H = 60{,}000\) and low-ability workers have productivity \(w_L = 30{,}000\). The cost of a year of education is Rs 5,000 for H-types and Rs 12,000 for L-types. (a) Find the range of education thresholds \(s^*\) that support a separating equilibrium. (b) Is \(s^* = 4\) a valid separating equilibrium?

    ??? success "Answer"

        **(a)** The wage premium from being identified as high-ability is:

        \[
        w_H - w_L = 60{,}000 - 30{,}000 = 30{,}000
        \]

        For a separating equilibrium, we need:

        \[
        \frac{w_H - w_L}{c_L} < s^* < \frac{w_H - w_L}{c_H}
        \]

        \[
        \frac{30{,}000}{12{,}000} < s^* < \frac{30{,}000}{5{,}000}
        \]

        \[
        2.5 < s^* < 6
        \]

        Any integer threshold \(s^* \in \{3, 4, 5\}\) supports a separating equilibrium. (Non-integer values are also valid in continuous versions of the model.)

        **(b)** Check \(s^* = 4\):

        - **H-type incentive:** Benefit of signalling = 30,000. Cost = \(5{,}000 \times 4 = 20{,}000\). Since \(30{,}000 > 20{,}000\), H-types are willing to acquire 4 years.
        - **L-type incentive:** Cost of mimicking = \(12{,}000 \times 4 = 48{,}000\). Since \(30{,}000 < 48{,}000\), L-types are *not* willing to mimic.

        **Yes**, \(s^* = 4\) is a valid separating equilibrium. H-types acquire 4 years and earn 60,000; L-types acquire 0 years and earn 30,000.

        **Note the inefficiency:** Education produces zero social value in this model --- it only sorts workers. Yet H-types spend Rs 20,000 on education. This is a deadweight loss of the signalling equilibrium.

??? question "Q7. The Sheepskin Effect"

    What is the sheepskin effect? A researcher estimates the following wage regression with education dummies (omitted category: less than high school):

    | Education Level | Coefficient | Implied Wage Premium |
    |---|---|---|
    | Some high school (10--11 years) | 0.08 | 8% |
    | High school diploma (12 years) | 0.25 | 28% |
    | Some college (13--15 years) | 0.35 | 42% |
    | Bachelor's degree (16 years) | 0.60 | 82% |

    What does this pattern reveal about human capital vs. signalling?

    ??? success "Answer"

        The **sheepskin effect** is the discontinuous jump in wages upon completion of a credential, over and above the return to additional years of schooling.

        **Evidence from the table:**

        - Going from "some high school" to "high school diploma" (roughly 1--2 years) increases the premium from 8% to 25% --- a jump of **17 percentage points** for acquiring the credential.
        - Going from "some college" to "bachelor's degree" (roughly 1 year) increases the premium from 35% to 60% --- a jump of **25 percentage points**.

        If each year of schooling added the same productivity (pure human capital), we would expect roughly equal increments per year. Instead, the jump at 12 years (diploma) and 16 years (degree) is **much larger** than the increments at intermediate years.

        **Interpretation:** The sheepskin effect supports the **signalling hypothesis** --- employers reward the credential, not just the years of coursework. However, the smooth increases between credential years (from 8% to 8%, from 25% to 35%) show that **human capital accumulation also operates**. Both channels matter, but the sheepskin effect at degree boundaries is consistent with signalling playing a significant role.

??? question "Q8. General vs. Specific Training"

    A software firm can send a junior developer to either (a) a Python programming bootcamp (general training) or (b) a training programme on the firm's proprietary internal code management system (specific training). Who should pay for each? What happens to wages in each case?

    ??? success "Answer"

        **(a) Python bootcamp (general training):**

        Python skills are valued by all firms in the industry. If the firm pays for the training, the developer becomes more productive everywhere, and competing firms can poach her by offering a higher wage. The firm cannot recoup its investment.

        **Becker's prediction:** The **worker pays** --- either through a direct fee or by accepting a lower wage during the training period. After training, her wage rises to reflect her higher general productivity across all firms.

        *In practice:* Some firms do pay for general training (Google, for example, funds employees' external courses). This can be explained by labour market frictions --- if job search is costly, firms retain some monopsony power and can recoup part of the training investment through wages below marginal product. Acemoglu and Pischke (1999) formalise this idea.

        **(b) Proprietary code system (specific training):**

        This knowledge is valuable only at the current firm. The developer gains no outside value from learning it.

        **Becker's prediction:** **Costs and returns are shared.** The firm pays part of the cost (by maintaining the developer's wage during training even though she is not fully productive). The developer accepts a post-training wage below her firm-specific marginal product. The resulting wage is between her outside option and her productivity at the firm:

        \[
        w_{\text{alternative}} < w < \text{VMP}_{\text{this firm}}
        \]

        This sharing arrangement creates a **durable match** --- neither party wants to terminate it unilaterally.

??? question "Q9. Returns to Education in India: Formal vs. Informal Sector"

    Why might the Mincer return to education differ between India's formal and informal sectors? An economist estimates \(\hat{\beta}_{\text{formal}} = 0.12\) and \(\hat{\beta}_{\text{informal}} = 0.04\). Discuss possible explanations.

    ??? success "Answer"

        Several factors explain the large gap:

        1. **Credentialism in formal hiring:** Government jobs and large firms use educational qualifications as screening devices. Pay commissions explicitly link pay scales to degree level (Class I officer requires a degree, Class II requires graduation, etc.). This creates a mechanical education-wage link independent of productivity.

        2. **Technology and skill complementarity:** Formal-sector jobs (IT, banking, engineering, pharmaceuticals) use technologies that are complementary with education. A more educated worker is substantially more productive in these settings. Informal-sector jobs (construction labour, domestic work, street vending) are physically intensive and do not differentially reward education.

        3. **Selection bias:** Workers who enter the formal sector are positively selected on ability. The correlation between education and ability is stronger among those who successfully pass formal-sector screening. The high \(\hat{\beta}\) partly reflects this selection.

        4. **Union and institutional wage-setting:** Formal-sector wages are often set by collective bargaining or government pay scales that reward education directly. Informal-sector wages are determined by spot-market bargaining and piece rates.

        5. **Measurement:** Informal-sector earnings are harder to measure (irregular, in-kind components, seasonal variation), introducing attenuation bias that pushes \(\hat{\beta}\) toward zero.

        **Implication:** A single Mincer return for all Indian workers is misleading. The return to education depends heavily on the segment of the labour market the worker enters --- and access to the formal sector is itself partly determined by education, creating a self-reinforcing cycle.

??? question "Q10. India's Engineering Surplus: Human Capital or Signalling?"

    India produces over 1.5 million engineering graduates annually, yet surveys find that only 20--40% are "employable." How does the signalling model help explain this phenomenon? What are the policy implications?

    ??? success "Answer"

        **Signalling explanation:**

        Students pursue engineering degrees not primarily to acquire technical engineering skills but because the degree signals cognitive ability, quantitative aptitude, and perseverance to employers. The engineering entrance exam (JEE, state CETs) serves as a screening device. Employers in IT services, consulting, and banking recruit from engineering colleges because they believe the credential identifies high-ability workers --- not because the job requires thermodynamics or circuit theory.

        This is a classic **credential arms race**: as more students pursue engineering degrees, the signal becomes noisier. Students who might have been perfectly employable with a commerce or science degree now "need" an engineering degree to compete. The result is massive overinvestment in engineering education that produces graduates without the skills their degree nominally certifies.

        **Evidence consistent with signalling:**

        - Many engineering graduates work in jobs entirely unrelated to their field of study (HR, marketing, banking).
        - The wage premium for an IIT/NIT degree is several times larger than for a generic private engineering college, even though the curriculum content is similar --- the signal value of the institution matters more than the knowledge acquired.
        - Employers routinely administer aptitude tests during campus recruitment, effectively re-screening candidates despite their degree.

        **Policy implications:**

        - If signalling dominates, expanding engineering colleges further is socially wasteful. Resources would be better invested in (a) improving quality at existing institutions, (b) developing credible vocational alternatives that provide genuine skills, and (c) reforming employer hiring practices to evaluate skills directly rather than relying on degree proxies.
        - The NEP 2020's emphasis on multidisciplinary education and skill-based assessment is a step in the right direction, potentially reducing the signalling premium attached to the engineering credential.

??? question "Q11. Compulsory Schooling and the Wage Distribution"

    A government introduces a compulsory schooling law requiring all children to complete 10 years of education. Using the human capital framework, predict the effects on (a) average wages and (b) wage inequality. What complication arises if school quality is low?

    ??? success "Answer"

        **(a) Average wages:**

        The law forces individuals who would have chosen fewer than 10 years of schooling to acquire more education. Under the human capital model, this additional schooling increases their productivity and wages, so **average wages rise**.

        However, the marginal individuals (those compelled to stay) had chosen less education because their marginal rate of return was below their discount rate. For them, the return to the additional years is likely lower than for voluntary attendees. The average return to the mandated additional years may therefore be **lower** than the average return to voluntarily acquired schooling.

        **(b) Wage inequality:**

        The law compresses the education distribution from below --- everyone now has at least 10 years. Since those at the bottom of the education distribution also tend to be at the bottom of the wage distribution, their wages rise. The result is a **compression of the wage distribution** --- inequality decreases.

        **General equilibrium caveat:** If the supply of workers with 10+ years of schooling increases sharply, the return to schooling may decline (supply shift along a downward-sloping demand curve for educated workers). This would partially offset the wage gains.

        **Quality complication:** If school quality is poor --- as the ASER reports document for much of rural India --- the mandated additional years may produce minimal human capital. Students may sit in classrooms without learning. In this case, the enrolment increase does not translate into a productivity increase, and the predicted wage gains fail to materialise. The policy achieves more years of *schooling* without more years of *learning* --- a distinction that is central to India's education challenge.

??? question "Q12. Mincer Regression in Stata"

    How would you estimate a Mincer equation using PLFS microdata in Stata? Write the code and explain how to interpret the output and test for sheepskin effects.

    ??? success "Answer"

        !!! stata "Mincer Regression with Sheepskin Test"

            ```stata
            * === Mincer Earnings Equation: PLFS 2024 ===

            use "/path/to/plfs_person_2024.dta", clear

            * Potential experience (Mincer proxy)
            gen experience = age - years_of_education - 6
            replace experience = 0 if experience < 0
            gen experience_sq = experience^2

            * Keep wage/salaried workers only
            keep if inlist(employment_status, 31, 41)

            * Generate log monthly earnings
            gen ln_wage = ln(monthly_earnings)
            drop if missing(ln_wage)

            * ── Basic Mincer ──
            reg ln_wage years_of_education experience experience_sq, robust

            * coeff on years_of_education = β ≈ % return per year
            * coeff on experience > 0, on experience_sq < 0 → concave profile

            * ── Extended with controls ──
            reg ln_wage years_of_education experience experience_sq ///
                i.female i.urban i.social_group i.state, robust

            * ── Sheepskin test: Education dummies ──
            * Replace continuous years with categorical dummies
            reg ln_wage i.education_level experience experience_sq ///
                i.female i.urban, robust

            * Compare jumps: if the jump at 12 years (HS diploma) or
            * 16 years (bachelor's) is larger than at intermediate years,
            * this is evidence of a sheepskin (signalling) effect.

            * ── Formal vs. Informal sector ──
            reg ln_wage years_of_education experience experience_sq ///
                if sector == 1, robust
            estimates store formal

            reg ln_wage years_of_education experience experience_sq ///
                if sector == 2, robust
            estimates store informal

            estimates table formal informal, b(%9.4f) se
            ```

        **Interpreting the output:**

        - The coefficient on `years_of_education` is \(\hat{\beta}\) --- the estimated percentage return per year. A coefficient of 0.085 means each year of schooling is associated with an 8.5% wage increase.
        - The experience terms trace out the concave earnings profile. Peak experience = \(-\hat{\gamma}_1 / (2\hat{\gamma}_2)\).
        - The `robust` option corrects standard errors for heteroskedasticity.
        - In the sheepskin test, look for **discontinuous jumps** at degree-completion years. If the coefficient on "bachelor's degree" is much larger than what a smooth interpolation from "some college" would predict, this is evidence for signalling.

---

<div style="display: flex; justify-content: space-between; margin-top: 2rem;">
<a href="../06-education/">:material-arrow-left: Chapter Content</a>
<a href="../06-education/resources/">Resources :material-arrow-right:</a>
</div>
