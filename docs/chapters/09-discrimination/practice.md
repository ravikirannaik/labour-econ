---
title: "Practice — Labor Market Discrimination"
---

# Practice: Labor Market Discrimination

Test your understanding of discrimination theory, measurement, and policy. Questions range from conceptual to computational.

---

??? question "Q1. Becker's Discrimination Coefficient"
    An employer has a discrimination coefficient \( d = 0.25 \) against minority workers. The market wage for majority workers is $20 per hour. What is the maximum wage this employer would pay a minority worker?

    **Answer:**

    The discriminating employer treats the cost of hiring a minority worker as \( w_m(1 + d) \). The employer hires the minority worker only if:

    \[
    w_m(1 + d) \leq w_w
    \]

    Solving:

    \[
    w_m \leq \frac{w_w}{1 + d} = \frac{20}{1.25} = \$16
    \]

    The employer would pay the minority worker at most **$16 per hour**, creating a 20 percent wage gap. The discrimination coefficient of 0.25 translates into a wage gap of \( \frac{d}{1+d} = \frac{0.25}{1.25} = 0.20 \), or 20 percent.

??? question "Q2. Competition and the Survival of Discrimination"
    According to the Becker model, employer discrimination should be eliminated by competitive forces in the long run. Explain the logic of this prediction and provide two reasons why discrimination might persist despite competition.

    **Answer:**

    **Logic of the prediction:** Discriminating employers refuse to hire productive minority workers, restricting their labour pool and raising their costs. Non-discriminating firms hire these workers at lower wages, achieving lower costs and higher profits. In a competitive market, non-discriminating firms expand while discriminating firms shrink or exit. In the long run, discrimination is competed away.

    **Reasons for persistence:**

    1. **Imperfect competition and market power:** If product markets are not perfectly competitive, discriminating firms can survive because supernormal profits absorb the cost of prejudice. Monopolists can afford to discriminate.
    2. **Customer or employee discrimination:** Even if employers are unprejudiced, customer preferences or co-worker resistance may force firms to discriminate. A non-discriminating firm that integrates its workforce may lose customers or face higher turnover among prejudiced employees.

    Other valid reasons include search frictions, segregated networks, and collusion among employers.

??? question "Q3. Statistical Discrimination Scenario"
    A tech company receives 200 applications for a software engineering position. Historical data shows that 40% of graduates from University A pass the company's coding test, while 60% of graduates from University B pass. The company decides to interview only University B graduates. Is this taste-based or statistical discrimination? Does it matter whether University A has a higher share of minority students?

    **Answer:**

    This is **statistical discrimination**. The company is using group membership (university) as a signal of unobserved individual productivity (coding ability). The company is not acting on an animus or distaste --- it is using base rates to make a rational (though potentially unfair) screening decision.

    It matters greatly if University A has a higher share of minority students. In that case, a facially neutral screening criterion (university quality) produces **disparate impact** --- it disproportionately excludes minority applicants. Even without any taste-based prejudice, the screening rule perpetuates inequality. This is the core of the indirect/structural discrimination argument.

    Policy implication: Requiring the company to administer its coding test to all applicants (rather than pre-screening by university) would reduce statistical discrimination by providing individual-level signals.

??? question "Q4. Oaxaca-Blinder Decomposition Interpretation"
    A researcher estimates the following Oaxaca-Blinder decomposition of the male-female log wage gap:

    | Component | Value |
    |-----------|-------|
    | Total gap \( \overline{\ln w}_M - \overline{\ln w}_F \) | 0.30 |
    | Explained (endowments) | 0.12 |
    | Unexplained (coefficients) | 0.18 |

    (a) What percentage of the gap is explained by differences in observable characteristics?
    (b) Can we conclude that 18 log points of the gap is due to discrimination?
    (c) Give one reason the unexplained component might overstate discrimination and one reason it might understate it.

    **Answer:**

    **(a)** The explained share is \( 0.12 / 0.30 = 40\% \). Forty percent of the raw gap is accounted for by differences in education, experience, occupation, and other observables.

    **(b)** No. The unexplained component of 0.18 (approximately 18 percent) is often interpreted as an upper bound on discrimination, but it also captures the effects of any **omitted variables** correlated with gender. We cannot definitively attribute the entire unexplained component to discrimination.

    **(c)**

    - **Overstatement:** If women differ from men in unobserved ways that reduce productivity (e.g., less on-the-job training, weaker professional networks), the unexplained component captures these omitted factors along with discrimination.
    - **Understatement:** If pre-market discrimination reduces women's observable characteristics (e.g., women are steered away from STEM fields, reducing their measured "experience in high-paying occupations"), then the "explained" component itself partly reflects discrimination. Controlling for occupation can absorb the effect of discriminatory sorting.

??? question "Q5. Designing an Audit Study"
    You want to test whether caste discrimination exists in the Indian IT sector. Design a correspondence study. Specify: (a) What you would vary, (b) What you would hold constant, (c) Your outcome variable, and (d) One potential threat to validity.

    **Answer:**

    **(a) Vary:** Applicant names signalling caste identity. Use surnames clearly associated with upper-caste (e.g., Sharma, Iyer) and Dalit (e.g., Paswan, Valmiki) backgrounds. Following Thorat and Attewell (2007), one can also include Muslim names.

    **(b) Hold constant:** Education (e.g., B.Tech from the same tier of institution), years of experience, programming skills, certifications, GPA, and all other resume content. Rotate which resume template is paired with which name to avoid confounding name and resume quality.

    **(c) Outcome variable:** Callback rate --- whether the applicant is invited for an interview or phone screen. Secondary outcomes include time to callback and whether the callback is for the applied position or a lower-level one.

    **(d) Threat to validity:** If certain surnames are correlated with regional origin as well as caste, the estimated discrimination could reflect geographic preferences (e.g., preference for local candidates) rather than caste prejudice. Using surnames that are common across regions can mitigate this.

??? question "Q6. Wage Gap Decomposition Calculation"
    Male workers have average education of 14 years and average experience of 20 years. Female workers have average education of 15 years and average experience of 12 years. The male wage equation is:

    \[
    \ln w_M = 1.5 + 0.10 \times \text{Educ} + 0.03 \times \text{Exp}
    \]

    The female wage equation is:

    \[
    \ln w_F = 1.2 + 0.08 \times \text{Educ} + 0.02 \times \text{Exp}
    \]

    (a) Calculate predicted mean log wages for men and women.
    (b) Decompose the gap into explained and unexplained components using male coefficients as the reference.

    **Answer:**

    **(a)** Predicted mean log wages:

    \[
    \overline{\ln w}_M = 1.5 + 0.10(14) + 0.03(20) = 1.5 + 1.4 + 0.6 = 3.50
    \]

    \[
    \overline{\ln w}_F = 1.2 + 0.08(15) + 0.02(12) = 1.2 + 1.2 + 0.24 = 2.64
    \]

    Total gap: \( 3.50 - 2.64 = 0.86 \)

    **(b)** Oaxaca-Blinder decomposition using male coefficients:

    **Explained (endowment differences evaluated at male returns):**

    \[
    (\bar{X}_M - \bar{X}_F)\hat{\beta}_M = 0.10(14 - 15) + 0.03(20 - 12) = 0.10(-1) + 0.03(8) = -0.10 + 0.24 = 0.14
    \]

    **Unexplained (coefficient differences evaluated at female characteristics):**

    \[
    \text{Total gap} - \text{Explained} = 0.86 - 0.14 = 0.72
    \]

    Alternatively, computing directly:

    - Intercept difference: \( 1.5 - 1.2 = 0.30 \)
    - Education coefficient difference: \( (0.10 - 0.08) \times 15 = 0.30 \)
    - Experience coefficient difference: \( (0.03 - 0.02) \times 12 = 0.12 \)
    - Total unexplained: \( 0.30 + 0.30 + 0.12 = 0.72 \)

    The gap is predominantly unexplained (84%). The small explained component arises because women actually have more education but much less experience than men.

??? question "Q7. Employee vs. Customer Discrimination"
    A restaurant chain finds that its locations with diverse staff have 10% lower revenue than those with all-white staff, despite identical food quality and prices. The CEO argues this is evidence that diversity is bad for business. Evaluate this claim using Becker's framework. What type of discrimination is at work?

    **Answer:**

    This is consistent with **customer discrimination**. Customers with a discrimination coefficient \( d_c > 0 \) value the dining experience less when served by minority staff, leading to lower revenue at diverse locations.

    The CEO's conclusion that "diversity is bad for business" is partially correct in a narrow, short-run profit sense --- but it is misleading:

    1. The revenue loss reflects **customer prejudice**, not lower worker productivity. The "cost of diversity" is really the cost of customer discrimination.
    2. In the long run, customer preferences may change, making early investment in diversity advantageous.
    3. The argument ignores the **labour cost side**: if minority workers are paid less due to discrimination, the diverse locations may have lower costs, potentially offsetting the revenue loss.
    4. Ethically and legally, accommodating customer prejudice by segregating staff violates anti-discrimination law (Title VII in the US, constitutional protections in India).

??? question "Q8. Self-Fulfilling Statistical Discrimination"
    Explain how Arrow's model of statistical discrimination can produce a self-fulfilling prophecy. Use the example of employer beliefs about women's commitment to the labour force.

    **Answer:**

    **Step 1 --- Initial belief:** Employers believe women are more likely than men to leave the labour force (e.g., for childcare), so they expect a lower average tenure from female workers.

    **Step 2 --- Rational employer response:** Based on this belief, employers invest less in training women and assign them to positions with lower returns to tenure (flatter earnings profiles). They may also offer lower starting wages.

    **Step 3 --- Rational worker response:** Women, facing lower returns to staying in the labour force (less training, flatter profiles), find the opportunity cost of leaving lower. Some women who would have stayed in the labour force under equal treatment now rationally choose to exit.

    **Step 4 --- Confirmation:** The employer observes higher quit rates among women and concludes the initial belief was correct.

    The equilibrium is self-fulfilling: the discrimination creates the behaviour that appears to justify it. Crucially, there need be no inherent gender difference in commitment --- the gap is entirely produced by employer beliefs and the rational responses they induce. This is sometimes called a **coordination failure**: a non-discriminatory equilibrium also exists (where employers invest equally, women stay equally, and the belief is confirmed), but the economy is stuck in the discriminatory one.

??? question "Q9. Caste Discrimination in the Indian Labour Market"
    (a) Describe the key finding of Thorat and Attewell (2007).
    (b) Why is a correspondence study more convincing than a regression-based approach for establishing discrimination in the Indian context?
    (c) How does India's reservation policy address discrimination differently from US-style affirmative action?

    **Answer:**

    **(a)** Thorat and Attewell (2007) sent matched applications (identical qualifications, experience, and cover letters) to private-sector job openings in Delhi, varying only the applicant's name to signal caste (Dalit/SC), religious (Muslim), and upper-caste Hindu identities. They found that **Dalit applicants received significantly fewer callbacks** than equally qualified upper-caste Hindu applicants. Muslim applicants also faced discrimination. The discrimination was especially strong for customer-facing positions.

    **(b)** Regression-based approaches (like Oaxaca-Blinder) suffer from omitted variable bias --- it is difficult to fully control for school quality, English fluency, social networks, and other factors correlated with caste. A correspondence study **holds all observable characteristics constant** by construction. The only difference is the name on the resume. Any difference in callback rates is directly attributable to the caste signal, making the causal inference much stronger.

    **(c)** Key differences:

    - **India's reservation** mandates specific **quotas** (15% SC, 7.5% ST, 27% OBC) in public-sector jobs and educational institutions. It is constitutionally mandated and non-discretionary.
    - **US affirmative action** is a softer requirement to make "good faith efforts" to increase diversity, primarily targeting federal contractors. It does not mandate specific quotas (the Supreme Court has ruled rigid quotas unconstitutional).
    - India's reservation applies **only to the public sector**, leaving the large private sector unregulated. US affirmative action covers private firms through federal contracting requirements and voluntary diversity programmes.
    - India's system is based on **caste categories** (ascriptive, hereditary), while US affirmative action targets race and gender (partly overlapping with class).

??? question "Q10. Efficiency Costs of Discrimination"
    Hsieh et al. (2019) estimate that reduced discrimination against women and Black Americans between 1960 and 2010 can account for 20--40% of US per-capita GDP growth. Explain the economic logic behind this finding.

    **Answer:**

    The logic is one of **talent misallocation**:

    1. In 1960, discrimination (both taste-based and statistical) and social norms prevented many talented women and Black Americans from entering high-skilled occupations (medicine, law, engineering, management).
    2. These individuals were allocated to lower-productivity occupations, not because of lack of ability but because of barriers.
    3. As discrimination declined, talented individuals from previously excluded groups entered high-skill occupations, better matching talent to tasks.
    4. This improved allocation raised aggregate productivity: the economy now uses its human capital more efficiently.

    Formally, if the marginal product of talent in high-skill occupations exceeds that in low-skill occupations, removing barriers that prevent high-ability individuals from entering high-skill occupations raises total output. The 20--40% figure captures the cumulative effect of this reallocation over 50 years --- it is large because the initial misallocation was severe and the affected groups constitute a majority of the population (women alone are ~50%).

??? question "Q11. Policy Evaluation: Ban-the-Box"
    Several US cities have adopted "Ban the Box" policies that prohibit employers from asking about criminal history on initial job applications. The policy aims to reduce discrimination against formerly incarcerated individuals (disproportionately Black men). However, Agan and Starr (2018) find that after Ban the Box, the racial gap in callbacks *increased*. Explain this paradoxical result using the concept of statistical discrimination.

    **Answer:**

    Before Ban the Box, employers could observe criminal history directly. They discriminated against applicants with criminal records but did not need to rely on race as a proxy.

    After Ban the Box removed criminal history from applications, employers lost an individual-level signal. Under statistical discrimination, when individual information is removed, employers rely more heavily on **group-level statistics**. Because Black men have higher incarceration rates on average, employers who cannot observe criminal history use race as a proxy --- **increasing** racial discrimination against Black men without criminal records.

    This is a classic example of the tension between anti-discrimination policies: removing one source of information (criminal history) can amplify statistical discrimination along another dimension (race). The policy reduced discrimination against people with criminal records but increased discrimination against Black men as a group --- a form of the "veil of ignorance" backfiring when group base rates differ.

??? question "Q12. Comparing Models"
    Complete the following table comparing taste-based and statistical discrimination:

    | Feature | Taste-Based | Statistical |
    |---------|------------|-------------|
    | Motivation | ? | ? |
    | Long-run prediction under competition | ? | ? |
    | Effect of better information about individuals | ? | ? |
    | Policy remedy | ? | ? |

    **Answer:**

    | Feature | Taste-Based | Statistical |
    |---------|------------|-------------|
    | Motivation | Prejudice or animus (utility-based) | Profit maximisation under incomplete information |
    | Long-run prediction under competition | Discrimination eliminated as prejudiced firms incur costs and exit | Discrimination persists because it is rational given information constraints |
    | Effect of better information about individuals | No effect --- prejudice is not based on information | Reduces discrimination by replacing group averages with individual signals |
    | Policy remedy | Anti-discrimination laws, social change, increasing competition | Better signalling mechanisms (certifications, standardised tests), reducing information asymmetries |
