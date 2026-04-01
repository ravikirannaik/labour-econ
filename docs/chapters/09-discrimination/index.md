---
title: "Labor Market Discrimination"
---

# 9. Labor Market Discrimination

Why do equally productive workers sometimes earn different wages? Labour market discrimination occurs when workers who are identical in their productive characteristics are treated differently because of personal attributes such as race, gender, or caste. This chapter develops the theoretical frameworks for understanding discrimination, examines how economists measure it, and discusses the effectiveness of anti-discrimination policies.

---

## Race and Gender Gaps in Earnings: Stylised Facts

Persistent wage gaps across demographic groups are among the most robust findings in labour economics. In the United States, women earn approximately 82 cents for every dollar earned by men. Black men earn about 73 percent of what white men earn. These raw gaps have narrowed over the past half-century but remain substantial.

Several important patterns emerge from the data:

- **Gender gap:** The male-female wage ratio rose from about 0.60 in 1960 to roughly 0.82 by the 2010s, driven partly by women's rising educational attainment and labour force experience.
- **Racial gap:** The black-white earnings ratio among men improved sharply in the 1960s and 1970s following the Civil Rights Act, but progress slowed markedly after 1980.
- **Intersectionality:** Gaps compound across categories. Black women face both a race penalty and a gender penalty, though the interaction is not simply additive.

!!! empirical "Decomposing the Gap"
    Not all of the raw wage gap reflects discrimination. Differences in education, experience, occupation, and industry explain a substantial share. The critical question is how much of the gap remains **after** controlling for all observable productivity-related characteristics. This unexplained residual is the standard (though imperfect) measure of labour market discrimination.

---

## Taste-Based Discrimination: The Becker Model (1957)

Gary Becker's pioneering model treats prejudice as a "taste" --- an aversion to interacting with members of a particular group. The firm does not simply maximise profit; it also acts on its distaste for associating with certain workers.

### Employer Discrimination

Suppose a prejudiced employer has a **discrimination coefficient** \( d > 0 \). When deciding whether to hire a minority worker at wage \( w \), the employer acts as though the cost of employing that worker is \( w(1 + d) \) rather than \( w \). The employer perceives a higher cost than the actual wage.

!!! model "The Discrimination Coefficient"
    A prejudiced employer hires minority workers only if:

    \[
    w_m(1 + d) \leq w_w
    \]

    where \( w_m \) is the minority wage and \( w_w \) is the majority wage. In equilibrium, minority workers must accept a lower wage to compensate for employer prejudice:

    \[
    w_m = \frac{w_w}{1 + d}
    \]

    The wage gap between majority and minority workers equals \( \frac{d}{1+d} \times w_w \).

### Employee Discrimination

Some majority workers may demand a compensating wage differential to work alongside minority colleagues. If white workers have a discrimination coefficient \( d_e \), they behave as if their wage in an integrated firm is \( w(1 - d_e) \). Firms must either segregate their workforce or pay white workers a premium to work alongside minority workers.

### Customer Discrimination

Customers may prefer to be served by members of a particular group. If customers have a discrimination coefficient \( d_c \), they value a product sold by a minority worker at \( p(1 - d_c) \) rather than \( p \). This generates occupational segregation, pushing minority workers out of customer-facing roles.

### The Market's Self-Correcting Mechanism

A crucial prediction of the Becker model is that **discrimination is costly to the discriminator**. Prejudiced employers who refuse to hire productive minority workers forgo profitable opportunities. Non-discriminating firms hire these workers at lower wages and earn higher profits.

!!! model "Competition Erodes Discrimination"
    In a perfectly competitive labour market with free entry:

    1. Discriminating firms have higher labour costs than non-discriminating firms.
    2. Non-discriminating firms earn higher profits and expand.
    3. In the long run, competitive pressure should **eliminate** employer discrimination.

    This stark prediction raises a puzzle: if discrimination is costly, why does it persist? Possible explanations include imperfect competition, segregated social networks, and complementarities between employer and employee discrimination.

---

## Statistical Discrimination

Unlike taste-based discrimination, statistical discrimination arises from **rational** profit-maximising behaviour under incomplete information. Employers use group membership as a signal of unobserved productivity.

### The Phelps (1972) Model

Suppose an employer observes a noisy signal \( s \) of a worker's true productivity \( q \):

\[
s = q + \varepsilon
\]

If the employer believes that Group A has a lower average productivity \( \bar{q}_A < \bar{q}_B \), the employer's best estimate of a worker's productivity is a weighted average of the individual signal and the group mean:

!!! model "Statistical Discrimination: Bayesian Updating"
    The employer's estimate of worker productivity:

    \[
    E[q | s, \text{group}] = \alpha \cdot s + (1 - \alpha) \cdot \bar{q}_{\text{group}}
    \]

    where \( \alpha \) reflects the reliability of the individual signal. When \( \alpha \) is small (the signal is noisy), group membership carries more weight. Two workers with **identical** test scores from different groups receive different wage offers.

### The Arrow (1973) Model and Self-Fulfilling Prophecies

Kenneth Arrow extended the analysis by showing that statistical discrimination can be **self-fulfilling**. If employers believe that minority workers are less productive and invest less in training them, minority workers rationally invest less in their own skills --- confirming the employer's initial belief. This creates a **discriminatory equilibrium** that is stable even though it is not based on any true underlying productivity difference.

!!! empirical "Distinguishing Taste-Based from Statistical Discrimination"
    The distinction matters for policy:

    - **Taste-based:** Employers pay a cost to indulge their prejudice. Providing more information about individual workers does not help.
    - **Statistical:** Employers profit-maximise using imperfect information. Better signals (e.g., certifications, standardised testing) reduce discrimination.

    Empirically, Altonji and Pierret (2001) find that the black-white wage gap **widens** as employers learn more about workers --- consistent with statistical discrimination playing a role early in careers.

---

## Measuring Discrimination: The Oaxaca-Blinder Decomposition

The most widely used method for measuring wage discrimination is the Oaxaca (1973) and Blinder (1973) decomposition. It separates the raw wage gap into an "explained" component (due to differences in characteristics) and an "unexplained" component (often interpreted as discrimination).

!!! model "Oaxaca-Blinder Decomposition"
    Estimate separate wage regressions for two groups (e.g., men and women):

    \[
    \ln w_M = X_M \hat{\beta}_M \quad \text{and} \quad \ln w_F = X_F \hat{\beta}_F
    \]

    The mean log wage gap decomposes as:

    \[
    \underbrace{\overline{\ln w}_M - \overline{\ln w}_F}_{\text{Total gap}} = \underbrace{(\bar{X}_M - \bar{X}_F)\hat{\beta}_M}_{\text{Explained (endowments)}} + \underbrace{\bar{X}_F(\hat{\beta}_M - \hat{\beta}_F)}_{\text{Unexplained (coefficients)}}
    \]

    The **explained** part captures differences in observable characteristics (education, experience, occupation). The **unexplained** part captures differences in returns to those characteristics and is often attributed to discrimination --- though it also reflects any omitted variables correlated with group membership.

!!! warning "Limitations"
    The unexplained component is an **upper bound** on discrimination if there are omitted productive characteristics correlated with group membership that favour the majority group. It is a **lower bound** if pre-market discrimination (e.g., unequal schooling quality) reduces minority workers' observed characteristics.

---

## Audit and Correspondence Studies

Experimental methods provide the most compelling evidence of discrimination by holding all observable characteristics constant except group membership.

### Audit Studies

Matched pairs of testers --- identical in qualifications but differing in race or gender --- apply for the same jobs or housing. Differences in callback rates or offers reveal discrimination directly. Audit studies avoid the omitted-variable problems that plague regression-based methods.

### Correspondence Studies

Correspondence studies send fictitious resumes to real job postings, varying only the applicant's name (to signal race, ethnicity, or gender).

!!! empirical "Are Emily and Greg More Employable? (Bertrand & Mullainathan, 2004)"
    In a landmark correspondence study, resumes with "white-sounding" names (Emily, Greg) received **50 percent more callbacks** than identical resumes with "African-American-sounding" names (Lakisha, Jamal). Importantly, improving resume quality (adding more experience and credentials) helped white-named applicants much more than Black-named applicants, suggesting that discrimination and skill are not simply substitutes.

These experimental approaches have become the gold standard for measuring hiring discrimination and have been replicated in dozens of countries and labour market contexts.

---

## Discrimination in Indian Labour Markets

!!! indian "Caste Discrimination: Evidence from Correspondence Studies"
    **Thorat and Attewell (2007)** conducted a pioneering correspondence study in India, sending matched applications to private-sector job openings in Delhi. They found that applicants with Dalit (SC) and Muslim names received significantly fewer callbacks than upper-caste Hindu applicants with identical qualifications. The discrimination was especially pronounced for jobs that involved customer contact, consistent with Becker's model of customer discrimination.

    **Madheswaran and Attewell (2007)** used Oaxaca-Blinder decompositions on NSS data and found that SC/ST workers earn 15--20 percent less than upper-caste workers even after controlling for education, experience, and occupation. The unexplained gap --- the portion attributable to discrimination --- was substantial and persistent across sectors.

### Key Dimensions of Caste-Based Discrimination

1. **Hiring discrimination:** Lower callback rates for Dalit and Muslim applicants in private-sector jobs.
2. **Wage discrimination:** Significant unexplained wage gaps even within the same occupation and education level.
3. **Occupational segregation:** Historical caste-occupation linkages persist, concentrating SC/ST workers in low-wage occupations.
4. **Self-employment barriers:** Caste networks limit access to credit, markets, and business opportunities for lower-caste entrepreneurs.

!!! empirical "Gender Discrimination in India"
    India's female labour force participation rate is among the lowest in the world (approximately 37 percent in PLFS 2023-24), and the gender wage gap remains large. Estimates from PLFS data suggest that women earn 25--35 percent less than men in regular salaried employment. Norms around women's mobility, safety concerns, and household responsibilities compound market-based discrimination.

---

## Anti-Discrimination Policy

!!! policy "Anti-Discrimination Legislation: A Comparative View"
    **United States:**

    - **Equal Pay Act (1963):** Prohibits sex-based wage discrimination for substantially equal work.
    - **Civil Rights Act, Title VII (1964):** Prohibits employment discrimination based on race, color, religion, sex, or national origin. Created the EEOC.
    - **Affirmative action:** Executive orders and court rulings requiring federal contractors to take "affirmative steps" to increase minority and female representation.

    **India:**

    - **Article 15 & 16 of the Constitution:** Prohibit discrimination in employment on grounds of religion, race, caste, sex, or place of birth.
    - **Scheduled Castes and Scheduled Tribes (Prevention of Atrocities) Act, 1989:** Criminalises caste-based violence and discrimination.
    - **Reservation policy:** Reserves a proportion of public-sector jobs and educational seats for SC (15%), ST (7.5%), and OBC (27%) candidates.
    - **Equal Remuneration Act, 1976:** Mandates equal pay for equal work regardless of gender.

### Does Affirmative Action Work?

The evidence on affirmative action is mixed:

- **Employment effects:** Affirmative action has increased minority and female representation in covered firms, particularly in higher-skilled positions.
- **Mismatch concern:** Critics argue that preferences may place beneficiaries in positions where they are less likely to succeed, generating stigma and reducing incentives to invest in skills.
- **Indian reservation policy:** Studies find that reservation has substantially increased SC/ST representation in government employment and legislative bodies, though private-sector effects are limited since reservation applies only to the public sector.

!!! empirical "Efficiency Costs of Discrimination"
    Hsieh et al. (2019) estimate that the declining discrimination against women and Black Americans in the US between 1960 and 2010 accounts for 20--40 percent of US GDP growth per capita over that period. Discrimination represents a massive misallocation of talent, and reducing it generates substantial aggregate efficiency gains.

---

## Key Takeaways

1. **Raw wage gaps overstate discrimination** because they include differences in productive characteristics. The Oaxaca-Blinder decomposition separates explained and unexplained components.
2. **Becker's taste-based model** predicts that discrimination is costly and should be competed away in the long run --- yet it persists, suggesting market imperfections matter.
3. **Statistical discrimination** is profit-maximising under incomplete information but can be self-fulfilling, trapping minority groups in low-productivity equilibria.
4. **Audit and correspondence studies** provide the strongest causal evidence of discrimination by holding qualifications constant.
5. **Caste discrimination in India** is well-documented through correspondence studies (Thorat & Attewell, 2007) and wage decompositions (Madheswaran & Attewell, 2007), affecting hiring, wages, and occupational access.
6. **Anti-discrimination policies** (legislation, affirmative action, reservation) can reduce but not eliminate discrimination; their effectiveness depends on enforcement and market structure.

---

<div style="display: flex; justify-content: space-between; margin-top: 2rem;">
<a href="../08-mobility/index.md">&larr; Chapter 8: Labor Mobility</a>
<a href="../10-incentive-pay/index.md">Chapter 10: Incentive Pay &rarr;</a>
</div>
