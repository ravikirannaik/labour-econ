---
title: "Practice — The Wage Distribution"
description: "Practice problems on wage inequality measurement, SBTC, superstar effects, and institutional determinants"
---

# Practice: The Wage Distribution

Test your understanding of Chapter 7. Questions progress from definitions and interpretation to analytical problems and Indian-context applications. Click on any question to reveal the answer.

---

??? question "Q1. Interpreting the Gini Coefficient"
    Country A has a wage Gini coefficient of 0.28 and Country B has a wage Gini of 0.52.

    **(a)** Which country has greater wage inequality?

    **(b)** If Country B's Gini rises to 0.58 over a decade, what does this tell us about changes in its Lorenz curve?

    **(c)** Can two countries with the same Gini have different patterns of inequality? Explain.

    ---

    **Answer:**

    **(a)** Country B has greater wage inequality. A higher Gini indicates the Lorenz curve is further from the 45-degree line of equality.

    **(b)** The Lorenz curve has shifted further away from the line of equality. The area between the Lorenz curve and the 45-degree line has increased, meaning the wage distribution has become more concentrated --- the bottom earners receive a smaller cumulative share of total wages.

    **(c)** Yes. The Gini is a summary statistic and two different Lorenz curves can enclose the same area. For example, one country could have inequality concentrated at the top (a long right tail) while another has inequality spread across the entire distribution. Both might yield the same Gini, but the 90/50 and 50/10 ratios would look very different.

---

??? question "Q2. Percentile Ratio Calculations"
    The following data describe the hourly wage distribution in a labour market:

    | Percentile | Wage (Rs) |
    |-----------|-----------|
    | 10th | 120 |
    | 25th | 180 |
    | 50th (median) | 300 |
    | 75th | 520 |
    | 90th | 900 |

    **(a)** Calculate the 90/10, 90/50, and 50/10 ratios.

    **(b)** Is inequality more pronounced in the upper or lower half of the distribution? How do you know?

    **(c)** If a minimum wage is set at Rs 200, which ratio is most likely to be affected? Why?

    ---

    **Answer:**

    **(a)**

    - 90/10 = 900/120 = **7.50**
    - 90/50 = 900/300 = **3.00**
    - 50/10 = 300/120 = **2.50**

    **(b)** Upper-tail inequality is more pronounced. The 90/50 ratio (3.00) exceeds the 50/10 ratio (2.50), meaning the distance between the top and the middle is proportionally larger than the distance between the middle and the bottom.

    **(c)** The 50/10 ratio is most likely to be affected. A minimum wage at Rs 200 would compress the lower tail by raising wages for workers currently between Rs 120 and Rs 200, pushing the 10th percentile upward. This would reduce the 50/10 ratio and the 90/10 ratio, while the 90/50 ratio (which depends on the upper half) would be largely unaffected.

---

??? question "Q3. Variance Decomposition"
    An economy has two groups of workers: college-educated (Group C) and non-college (Group N). The data are:

    | Group | Share of workers (\( p_j \)) | Mean log wage (\( \bar{w}_j \)) | Variance of log wages (\( \sigma_j^2 \)) |
    |-------|:-:|:-:|:-:|
    | College (C) | 0.40 | 3.20 | 0.18 |
    | Non-college (N) | 0.60 | 2.60 | 0.22 |

    **(a)** Calculate the overall mean log wage.

    **(b)** Calculate the between-group and within-group components of the total variance.

    **(c)** What fraction of total inequality is "between-group"?

    ---

    **Answer:**

    **(a)** Overall mean:

    \[
    \bar{w} = p_C \bar{w}_C + p_N \bar{w}_N = 0.40(3.20) + 0.60(2.60) = 1.28 + 1.56 = 2.84
    \]

    **(b)**

    Between-group variance:

    \[
    \sum_j p_j (\bar{w}_j - \bar{w})^2 = 0.40(3.20 - 2.84)^2 + 0.60(2.60 - 2.84)^2
    \]
    \[
    = 0.40(0.36)^2 + 0.60(-0.24)^2 = 0.40(0.1296) + 0.60(0.0576) = 0.0518 + 0.0346 = 0.0864
    \]

    Within-group variance:

    \[
    \sum_j p_j \sigma_j^2 = 0.40(0.18) + 0.60(0.22) = 0.072 + 0.132 = 0.204
    \]

    Total variance = 0.0864 + 0.204 = **0.2904**

    **(c)** Between-group share = 0.0864 / 0.2904 = **29.8%**

    Within-group inequality accounts for about 70% of total inequality --- consistent with the empirical finding that residual inequality dominates.

---

??? question "Q4. The Tinbergen Framework"
    In the supply-demand model for skills:

    \[
    \ln \left( \frac{w_S}{w_U} \right) = \frac{1}{\sigma} \left[ \ln D - \ln \left( \frac{S}{U} \right) \right]
    \]

    **(a)** Suppose \( \sigma = 1.5 \). If relative demand (\( \ln D \)) grows by 3% per year and relative supply (\( \ln(S/U) \)) grows by 1% per year, what happens to the skill premium each year?

    **(b)** What would need to happen to stabilise the skill premium?

    **(c)** During the 1970s in the US, the skill premium fell. Using this framework, provide a plausible explanation.

    ---

    **Answer:**

    **(a)** The annual change in the log skill premium is:

    \[
    \Delta \ln \left( \frac{w_S}{w_U} \right) = \frac{1}{1.5} (0.03 - 0.01) = \frac{0.02}{1.5} \approx 0.0133
    \]

    The skill premium grows by approximately **1.33 percentage points per year**. Demand growth outpaces supply growth, so the premium rises.

    **(b)** To stabilise the premium, supply growth must match demand growth: \( \Delta \ln(S/U) = \Delta \ln D = 3\% \). This would require a faster expansion of college-educated workers relative to non-college workers --- through higher enrolment, completion, or immigration of skilled workers.

    **(c)** During the 1970s, the Baby Boom generation flooded the labour market with college graduates. Supply growth exceeded demand growth (\( \Delta \ln(S/U) > \Delta \ln D \)), causing the skill premium to fall. Education was winning the race against technology.

---

??? question "Q5. Skill-Biased Technological Change"
    Explain the difference between the **SBTC** hypothesis and the **job polarisation** hypothesis. Can both be true simultaneously?

    ---

    **Answer:**

    **SBTC (Skill-Biased Technological Change)** is the hypothesis that technological change increases the relative productivity and demand for skilled (educated) workers, widening the gap between high-skill and low-skill wages. It predicts a monotonic relationship: the more skilled you are, the more you benefit from technological change.

    **Job polarisation** (Autor, Katz, and Kearney, 2008) refines this prediction. It argues that technology primarily replaces *routine* tasks --- tasks that follow explicit rules and procedures (clerical work, bookkeeping, assembly). These routine tasks are concentrated in middle-skill occupations. High-skill abstract tasks (analysis, management, creativity) are complemented by technology, and low-skill manual tasks (cleaning, cooking, personal care) are difficult to automate. The result is growth at the top and bottom, with a hollowing out of the middle.

    **Both can be true simultaneously**, and indeed the polarisation hypothesis is best understood as a more nuanced version of SBTC. SBTC explains the widening of the overall skill premium (90/10 and 90/50 growth). Polarisation explains why the 50/10 ratio stopped growing --- because low-skill non-routine service jobs were not displaced by technology, so wages at the bottom stabilised even as the middle hollowed out.

---

??? question "Q6. Superstar Markets"
    **(a)** State the two conditions required for a superstar market according to Rosen (1981).

    **(b)** Explain why the market for pop musicians exhibits superstar effects while the market for plumbers does not.

    **(c)** How has digital technology affected superstar earnings?

    ---

    **Answer:**

    **(a)** The two conditions are:

    1. **Imperfect substitution**: consumers strongly prefer higher quality. A slightly better performer is disproportionately more valuable, not just marginally more valuable.
    2. **Scale technology (joint consumption)**: the best performer can serve a very large market at low marginal cost.

    **(b)** Pop musicians satisfy both conditions. Listeners strongly prefer their favourite artist (imperfect substitution) and a single recording can reach billions of listeners worldwide at near-zero marginal cost (scale). Plumbers satisfy neither: customers generally care about competence rather than marginal differences in quality, and a plumber can only serve one household at a time --- there is no scale technology.

    **(c)** Digital technology (streaming, social media, global distribution) has massively expanded the scale at which top performers can reach audiences. A single song on Spotify can be streamed 5 billion times. This amplifies the earnings of the top performers while reducing revenue for mid-tier artists. The same logic applies to CEOs of global firms, software developers whose code runs on billions of devices, and content creators on YouTube. Technology has made superstar markets more extreme.

---

??? question "Q7. Minimum Wages and the Wage Distribution"
    A country has a wage distribution where the 10th percentile wage is Rs 150/hour and the median wage is Rs 400/hour. The government introduces a minimum wage of Rs 200/hour.

    **(a)** What is the expected effect on the 50/10 ratio?

    **(b)** Using the competitive model, what is the predicted effect on employment?

    **(c)** Card and Krueger (1994) found no significant employment effects from a minimum wage increase. Provide two explanations for why the competitive prediction might fail.

    ---

    **Answer:**

    **(a)** The minimum wage compresses the lower tail. Workers who previously earned between Rs 150 and Rs 200 now earn Rs 200. The 10th percentile wage rises toward Rs 200. The 50/10 ratio falls from 400/150 = 2.67 toward 400/200 = 2.00. Lower-tail inequality decreases.

    **(b)** In the competitive model, a binding minimum wage (above the equilibrium wage for low-skill workers) creates a surplus of labour at that wage --- i.e., unemployment. Firms hire fewer workers because the marginal cost of labour now exceeds the marginal revenue product for some workers.

    **(c)** Two explanations:

    1. **Monopsony power**: If employers have wage-setting power (e.g., a dominant employer in a small town), the equilibrium wage is below the competitive level. A moderate minimum wage can actually *increase* employment by moving the market closer to the competitive outcome.
    2. **Demand-side effects**: Higher wages increase the purchasing power of low-wage workers, boosting consumer spending and product demand, which may offset the direct labour-cost increase.

---

??? question "Q8. Union Decline and Inequality"
    US private-sector union membership fell from about 35% in 1955 to under 7% by 2020. Explain two mechanisms through which union decline could contribute to rising wage inequality.

    ---

    **Answer:**

    **Mechanism 1: Wage compression within firms.** Unions typically negotiate standardised pay scales that compress the wage distribution within unionised workplaces --- raising wages at the bottom and restraining wages at the top. As unions declined, firms had more flexibility to differentiate pay based on individual performance, bargaining power, or market conditions. This increased within-firm and within-group inequality.

    **Mechanism 2: Reduced bargaining power for less-skilled workers.** Unions primarily organised in middle-skill, blue-collar occupations (manufacturing, construction, transport). Union wage premiums raised these workers' earnings above the competitive level. As union coverage fell, these workers lost the premium and their wages converged downward toward non-union levels. This widened the gap between educated/professional workers and less-educated manual workers, increasing between-group inequality.

    Card, Lemieux, and Riddell (2004) estimated that declining unionisation explains roughly 15--20% of the rise in US male wage inequality between 1980 and 2000.

---

??? question "Q9. Indian Wage Inequality"
    **(a)** Identify three structural features of the Indian labour market that shape its wage distribution differently from the US.

    **(b)** Kijima (2006) found that returns to education in India rose sharply during the 1990s. Using the Tinbergen framework, explain this finding.

    **(c)** What role does caste play in India's wage distribution?

    ---

    **Answer:**

    **(a)** Three structural features:

    1. **The formal-informal divide**: About 75--80% of India's workforce is in informal employment, where wages are lower, more dispersed, and disconnected from productivity-based pricing. The formal-informal gap is a major source of wage dispersion that has no equivalent in the US.
    2. **Rural-urban dualism**: The rural economy (still employing roughly 45% of workers) features agricultural wages far below urban wages, creating a large spatial dimension to inequality.
    3. **Caste-based segmentation**: Occupational segregation and discrimination based on caste restrict mobility and generate wage gaps even after controlling for human capital.

    **(b)** The 1990s saw India's economic liberalisation, the growth of the IT sector, and expansion of services. These developments increased the relative demand for educated workers (\( \ln D \) rose). However, the supply of college graduates, while growing, did not keep pace with the surge in demand --- particularly for English-speaking, technically skilled graduates. In the Tinbergen framework, demand growth outstripped supply growth, so the college premium rose.

    **(c)** Caste generates wage inequality through multiple channels: (i) differences in access to quality education and social networks limit human capital accumulation for SC/ST groups; (ii) occupational segregation concentrates lower-caste workers in low-paying jobs; (iii) direct labour market discrimination depresses wages for lower-caste workers even when they have the same qualifications. Madheswaran and Attewell (2007) found that a significant portion of the SC/ST wage gap remains unexplained after controlling for education, experience, and occupation --- consistent with discrimination.

---

??? question "Q10. Between-Group vs. Within-Group Inequality"
    A researcher finds that in Country X, the variance of log wages increased from 0.30 in 2000 to 0.42 in 2020. Decomposing by education group, she finds:

    | Year | Between-group variance | Within-group variance |
    |------|:---:|:---:|
    | 2000 | 0.08 | 0.22 |
    | 2020 | 0.12 | 0.30 |

    **(a)** How much of the total increase in variance is attributable to between-group changes?

    **(b)** How much is attributable to within-group changes?

    **(c)** What economic forces could explain rising within-group inequality?

    ---

    **Answer:**

    **(a)** Total increase = 0.42 - 0.30 = **0.12**. Between-group increase = 0.12 - 0.08 = **0.04**. Share attributable to between-group = 0.04 / 0.12 = **33.3%**.

    **(b)** Within-group increase = 0.30 - 0.22 = **0.08**. Share attributable to within-group = 0.08 / 0.12 = **66.7%**.

    **(c)** Rising within-group inequality means workers with the same education earn increasingly different wages. Possible explanations:

    - **Growing returns to unmeasured skills**: cognitive ability, social skills, adaptability, and specific technical competencies not captured by broad education categories.
    - **Increased firm-level pay dispersion**: high-productivity firms pay more, and sorting of workers into firms has become more assortative (high-ability workers cluster in high-paying firms).
    - **Performance pay**: the spread of bonuses, stock options, and commission-based pay widens earnings among workers in the same education group.
    - **Superstar and winner-take-all dynamics**: within any field, the top performers earn disproportionately more due to scale technologies and reputation effects.

---

*[Back to Chapter 7](index.md)* | *[Resources](resources.md)* | *[Next: Chapter 8 --- Labor Mobility](../08-mobility/index.md)*
