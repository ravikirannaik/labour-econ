---
title: "The Wage Distribution"
description: "Chapter 7 — Measuring wage inequality, skill-biased technological change, superstar effects, and the role of institutions"
---

# 7. The Wage Distribution

> *"The central economic fact of our time is the extraordinary rise in inequality."*
> --- Joseph Stiglitz

Why does a software engineer in Bengaluru earn ten times more than a construction worker in the same city? Why has the gap between college-educated and high-school-educated workers widened so dramatically since the 1980s? And why do a handful of CEOs, athletes, and entertainers earn more in a year than most people earn in a lifetime?

This chapter moves beyond the competitive model's prediction of a single equilibrium wage and confronts the reality that wages are distributed across a wide --- and widening --- range. We examine how economists measure wage inequality, what forces drive changes in the wage distribution, and why some workers are pulled toward the top while others are pushed toward the bottom. The analysis draws on one of the most active research areas in labour economics: the race between education and technology.

---

## Measuring Wage Inequality

Before explaining why inequality changes, we need tools to measure it. Labour economists rely on several complementary measures, each capturing a different dimension of the wage distribution.

### The Gini Coefficient

The **Gini coefficient** summarises the entire distribution in a single number between 0 (perfect equality) and 1 (perfect inequality). It is derived from the Lorenz curve, which plots the cumulative share of total wages earned by the bottom \( x\% \) of workers.

!!! model "Gini Coefficient"
    The Gini coefficient equals twice the area between the Lorenz curve and the 45-degree line of perfect equality:

    \[
    G = \frac{A}{A + B}
    \]

    where \( A \) is the area between the line of equality and the Lorenz curve, and \( B \) is the area below the Lorenz curve. Equivalently:

    \[
    G = 1 - 2 \int_0^1 L(p) \, dp
    \]

    where \( L(p) \) is the Lorenz curve --- the cumulative share of income held by the bottom fraction \( p \) of the population.

    A Gini of 0.25 indicates moderate inequality; a Gini above 0.40 indicates high inequality. The US wage Gini rose from approximately 0.35 in 1980 to above 0.45 by 2020.

### Percentile Ratios

Percentile ratios compare wages at specific points in the distribution without summarising the entire curve. The three most commonly used are:

- **90/10 ratio**: the wage at the 90th percentile divided by the wage at the 10th percentile. This captures overall dispersion.
- **90/50 ratio**: measures inequality in the upper half of the distribution (upper-tail inequality).
- **50/10 ratio**: measures inequality in the lower half (lower-tail inequality).

The distinction between upper-tail and lower-tail inequality turns out to be empirically important. In the United States, the 90/50 ratio has risen steadily since 1980, while the 50/10 ratio rose sharply in the 1980s but flattened in the 1990s and 2000s. This divergence suggests that different forces operate at different points in the distribution.

### Variance of Log Wages

The **variance of log wages** is the workhorse measure in empirical research because of its convenient decomposition properties:

!!! model "Variance Decomposition"
    The total variance of log wages can be decomposed into a **between-group** component and a **within-group** component:

    \[
    \text{Var}(\ln w) = \underbrace{\sum_j p_j (\bar{w}_j - \bar{w})^2}_{\text{between groups}} + \underbrace{\sum_j p_j \, \sigma_j^2}_{\text{within groups}}
    \]

    where \( p_j \) is the share of workers in group \( j \), \( \bar{w}_j \) is the mean log wage in group \( j \), \( \bar{w} \) is the overall mean, and \( \sigma_j^2 \) is the variance of log wages within group \( j \).

    Between-group inequality captures differences across observable categories (education, experience, occupation). Within-group inequality captures wage dispersion among workers who look identical on paper --- so-called "residual inequality."

A striking empirical finding is that within-group inequality accounts for the majority of total inequality and has grown substantially. Two workers with the same education, experience, gender, and occupation can earn very different wages. Understanding this residual inequality is one of the field's open puzzles.

---

## Trends in US Wage Inequality

The United States provides the most extensively documented case of rising wage inequality, and the patterns observed there --- with important variations --- have appeared across many advanced economies.

**Key stylised facts since 1970:**

1. **The college premium collapsed and then surged.** The wage gap between college graduates and high-school graduates fell during the 1970s (as college supply expanded rapidly) but rose sharply from the early 1980s onward. By 2020, college graduates earned roughly 65--70% more than high-school graduates, up from about 40% in 1980.

2. **Upper-tail inequality rose steadily.** The 90/50 ratio increased continuously from 1980 to the present, driven by rapid wage growth at the top.

3. **Lower-tail inequality rose, then stabilised.** The 50/10 ratio surged in the 1980s but stopped growing (and in some measures declined) after the mid-1990s. This pattern is consistent with a changing role for institutional forces like the minimum wage.

4. **Within-group inequality grew.** Even among workers with the same education and experience, wage dispersion widened --- suggesting that skills not captured by standard measures (cognitive ability, interpersonal skills, adaptability) became more valuable.

5. **Male wage inequality grew more than female.** Real wages for men at the bottom of the distribution actually *fell* in absolute terms between 1980 and 2000, while women's wages at the bottom grew modestly.

!!! empirical "The Great Divergence in Numbers"
    Between 1979 and 2019, real hourly wages in the US grew by approximately:

    - **90th percentile**: +41%
    - **50th percentile (median)**: +15%
    - **10th percentile**: +4%

    At the very top, income growth was even more extreme. The share of total income going to the top 1% roughly doubled from about 10% in 1980 to over 20% by 2019 (Piketty and Saez, 2003, updated).

---

## The Race Between Education and Technology

The most influential framework for understanding the rise in wage inequality is the **Tinbergen model**, formalised and extended by Goldin and Katz (2008) in their landmark study *The Race between Education and Technology*.

### Tinbergen's Framework

Jan Tinbergen (1975) proposed that the wage distribution is shaped by two opposing forces:

- **Technology** increases the demand for skilled workers, pushing the skill premium *up*.
- **Education** increases the supply of skilled workers, pushing the skill premium *down*.

The observed skill premium at any point in time reflects the balance --- or the "race" --- between these two forces.

!!! model "Supply and Demand for Skills"
    In a simple two-skill model, the economy has skilled workers (\( S \)) and unskilled workers (\( U \)). The relative wage (skill premium) is determined by:

    \[
    \ln \left( \frac{w_S}{w_U} \right) = \frac{1}{\sigma} \left[ \ln D - \ln \left( \frac{S}{U} \right) \right]
    \]

    where \( D \) captures the relative demand for skilled labour (driven by technology), \( S/U \) is the relative supply of skills (driven by educational attainment), and \( \sigma \) is the elasticity of substitution between skilled and unskilled labour.

    - When demand growth (\( \ln D \)) outpaces supply growth (\( \ln(S/U) \)), the skill premium rises.
    - When supply growth outpaces demand, the premium falls.

### Goldin and Katz: The Historical Narrative

Goldin and Katz (2008) documented that for most of the 20th century, the US educational system expanded rapidly --- high school graduation rates surged, college enrolment grew, and the supply of skilled workers kept pace with or exceeded demand growth. The skill premium was relatively stable or even declining.

Starting around 1980, however, the growth of educational attainment slowed sharply. College completion rates stagnated for cohorts born after 1950. Meanwhile, technological change --- particularly the spread of computers and information technology --- continued to accelerate the demand for skilled workers. Education fell behind in the race. The result: a widening skill premium and rising between-group inequality.

---

## Skill-Biased Technological Change (SBTC)

The hypothesis that technological change has been **skill-biased** --- that is, it disproportionately increases the productivity and demand for skilled workers --- is the dominant explanation for rising wage inequality.

The mechanism is straightforward: new technologies (computers, software, automation) *complement* the tasks performed by educated workers (analysis, problem-solving, communication) while *substituting* for the routine tasks performed by less-educated workers (data entry, assembly-line work, bookkeeping).

!!! empirical "Evidence for SBTC"
    Autor, Katz, and Kearney (2008) documented **job polarisation**: employment grew rapidly in high-skill, high-wage occupations and in low-skill, low-wage occupations, but *declined* in middle-skill, middle-wage occupations (clerical work, manufacturing). This "hollowing out" of the middle is consistent with technology replacing routine tasks concentrated in middle-skill jobs, while complementing abstract (high-skill) tasks and leaving manual (low-skill) tasks largely unaffected.

    This pattern --- growth at the top and bottom, decline in the middle --- is sometimes called the "polarisation hypothesis" and explains why upper-tail inequality continued rising while lower-tail inequality stabilised.

---

## Superstar Effects

At the very top of the wage distribution, standard supply-and-demand analysis struggles to explain the enormous concentration of earnings. Sherwin Rosen's (1981) theory of **superstar markets** provides an elegant explanation.

!!! model "Rosen's Superstar Model"
    Superstar markets arise when two conditions hold:

    1. **Imperfect substitution**: consumers strongly prefer the best performer. A slightly better surgeon, lawyer, or musician is not just marginally more valuable --- they may be *much* more valuable because quality differences are magnified.

    2. **Scale technology**: the best performers can serve very large markets at low marginal cost. A singer can reach millions through recordings; a CEO can manage a firm with billions in revenue; a software developer can write code used by a billion people.

    Under these conditions, small differences in talent translate into enormous differences in earnings. The top performer captures a disproportionate share of the total market revenue. Rosen showed that the resulting earnings distribution will be highly skewed, with a long right tail --- exactly the pattern observed in entertainment, sports, law, medicine, and increasingly in technology and finance.

The rise of digital technology has dramatically expanded the reach of superstars. A musician in the 1950s could perform for a few thousand people per year. Today, a single viral track reaches hundreds of millions. This technological amplification of scale has contributed to the explosion of top-end earnings.

---

## The Role of Institutions

Technology and education are not the only forces shaping the wage distribution. **Institutional factors** --- minimum wages, unions, deregulation, and norms about pay --- play a significant role, particularly in the lower half of the distribution.

### Minimum Wages

The **real (inflation-adjusted) minimum wage** in the United States fell by nearly 30% between 1968 and 1990 as Congress failed to raise the nominal minimum to keep pace with inflation. This erosion coincided with the sharp rise in lower-tail inequality during the 1980s. When the minimum wage was increased in the 1990s, lower-tail inequality stabilised.

!!! policy "The Minimum Wage Debate"
    The employment effects of the minimum wage remain contested. The textbook competitive model predicts job losses when a binding minimum wage exceeds the equilibrium wage. However, Card and Krueger's (1994) influential study of fast-food employment in New Jersey and Pennsylvania found no significant job loss after a minimum wage increase. The debate continues: a comprehensive CBO (2019) analysis estimated that raising the US federal minimum to $15 would lift 1.3 million workers out of poverty but also reduce employment by 1.3 million.

    The consensus view is that moderate minimum wage increases have small or negligible employment effects while compressing the lower tail of the wage distribution.

### Unions

Union membership in the United States fell from about 35% of the private-sector workforce in the 1950s to under 7% by 2020. Unions historically compressed the wage distribution both by raising wages at the bottom and by standardising pay within firms and industries. Their decline contributed to rising inequality, particularly among men.

### Deregulation and Globalisation

The deregulation of key industries (airlines, trucking, telecommunications) in the 1970s and 1980s reduced the rents previously shared with workers in those sectors. Increased trade with low-wage countries put downward pressure on the wages of less-skilled workers in tradeable sectors.

---

## Changes in Between-Group and Within-Group Inequality

The variance decomposition introduced earlier reveals an important pattern:

- **Between-group inequality** (the education premium, the experience premium) rose from the early 1980s, driven by SBTC and the slowdown in educational supply.
- **Within-group (residual) inequality** also rose, and in fact accounts for the larger share of the total increase.

Rising within-group inequality means that education and experience explain a *smaller* fraction of wage variation today than they did in 1980. Workers who look identical on observable characteristics --- same degree, same years of experience, same industry --- earn increasingly different wages. Possible explanations include:

- Growing returns to unmeasured skills (cognitive ability, creativity, social skills)
- Increased dispersion in firm-level productivity and pay policies
- Greater sorting of high-ability workers into high-paying firms
- Rise of performance-based pay and winner-take-all compensation structures

!!! indian "Wage Inequality in India"
    India's wage distribution presents a complex picture shaped by the rural-urban divide, the formal-informal sector gap, and caste-based stratification:

    **Rural-urban gap**: Urban workers earn roughly 2--3 times rural workers on average. The gap is even larger for regular salaried employment versus casual labour.

    **Formal-informal divide**: Only about 20--25% of India's workforce is in formal employment with written contracts, social security, and legal protections. Informal sector wages are substantially lower and more dispersed. The Periodic Labour Force Survey (PLFS 2023-24) reports median daily wages for casual workers at around Rs 350, compared to Rs 700+ for regular salaried workers.

    **Rising returns to education**: Kijima (2006) documented that returns to education in India increased significantly during the 1990s, particularly for tertiary education, consistent with skill-biased demand shifts driven by IT-sector growth and economic liberalisation. Azam (2012) confirmed that the college premium in India rose sharply between 1983 and 2005, mirroring (with a lag) the patterns observed in the United States.

    **Caste-based wage gaps**: Even after controlling for education, experience, occupation, and sector, significant wage gaps persist between upper-caste workers and SC/ST workers. Decomposition studies (Madheswaran and Attewell, 2007) find that a substantial portion of the caste wage gap is "unexplained" --- consistent with discrimination or unmeasured differences in quality of education.

    **Gender wage gap**: Women in India earn approximately 20--30% less than men with similar observable characteristics. The gap is larger in rural areas and in informal employment. Female labour force participation remains low (approximately 37% in PLFS 2023-24), meaning the wage distribution captures only a selected subset of women.

---

## Key Takeaways

1. **Wage inequality is measured** using the Gini coefficient, percentile ratios (90/10, 90/50, 50/10), and the variance of log wages. Each captures different dimensions of dispersion.

2. **US wage inequality rose sharply** after 1980, with the college premium widening, upper-tail inequality growing continuously, and within-group inequality expanding.

3. **The Tinbergen framework** models the skill premium as a race between technology (demand for skills) and education (supply of skills). When education falls behind, inequality rises.

4. **Skill-biased technological change (SBTC)** increases the relative demand for educated workers. The "polarisation" variant explains the hollowing-out of middle-skill jobs.

5. **Superstar effects** (Rosen, 1981) explain extreme earnings concentration at the top, driven by imperfect substitution and scale technologies.

6. **Institutions matter**: declining minimum wages, union erosion, and deregulation contributed to rising inequality, particularly in the lower tail.

7. **Within-group inequality** --- wage dispersion among observably similar workers --- accounts for the majority of total inequality and has grown substantially, suggesting increasing returns to unmeasured skills.

8. **India's wage distribution** is shaped by the rural-urban gap, the formal-informal divide, rising returns to education, and persistent caste and gender wage differentials.

---

*[Previous: Chapter 6 --- Education](../06-education/index.md)* | *[Practice Problems](practice.md)* | *[Resources](resources.md)* | *[Next: Chapter 8 --- Labor Mobility](../08-mobility/index.md)*
