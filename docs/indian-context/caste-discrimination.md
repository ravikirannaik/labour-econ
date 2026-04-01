---
title: "Caste & Discrimination"
---

# Caste and Labour Market Discrimination in India

The caste system is one of the oldest and most deeply embedded systems of social stratification in the world. It assigns individuals to hierarchically ranked groups at birth, with historically prescribed occupations, rules of social interaction, and degrees of ritual purity. Although the Indian Constitution abolished untouchability in 1950 and affirmative action policies have been in place for over seven decades, caste continues to shape labour market outcomes in ways that are both measurable and substantial. For students of labour economics, the Indian caste system offers a powerful case study in discrimination -- testing the predictions of Becker's taste-based model, statistical discrimination theory, and the Oaxaca-Blinder decomposition in a context where group identity is ascribed, visible, and consequential.

---

## Caste and Occupational Segregation

The historical caste system linked social groups to specific occupations. Brahmins were priests and scholars; Kshatriyas were warriors and rulers; Vaishyas were merchants; Shudras were artisans and service workers; and the "untouchable" castes (now Scheduled Castes, or Dalits) were confined to occupations considered polluting -- sanitation, leather work, burial, and manual scavenging.

!!! indian "Occupational Persistence"
    Although legal occupational restrictions have been abolished, the legacy persists. Scheduled Caste workers remain disproportionately concentrated in casual labour, sanitation, and low-skilled services. Data from the PLFS 2023-24 show that SC workers are overrepresented in casual wage employment (~35 per cent of SC workers, compared to ~20 per cent for upper castes) and underrepresented in regular salaried jobs and self-employment in higher-return activities. Scheduled Tribe workers are concentrated in agriculture and forest-based occupations. This occupational segregation is a central driver of caste-based wage gaps.

The modern Indian classification system divides the population into four official categories for policy purposes:

| Category | Abbreviation | Approximate Population Share |
|----------|:------------:|:----------------------------:|
| Scheduled Castes | SC | ~16.6% |
| Scheduled Tribes | ST | ~8.6% |
| Other Backward Classes | OBC | ~41% (estimated) |
| Others (General/Upper Caste) | -- | ~33% |

---

## Wage Gaps: The Evidence

A large body of empirical research documents significant wage gaps between caste groups in India. The gaps are not small -- they are economically meaningful and persistent over time.

### Raw Wage Gaps

Using PLFS data, the raw (unconditional) wage gap between upper-caste and SC workers in regular salaried employment is typically 40-60 per cent. That is, upper-caste workers earn 40-60 per cent more than SC workers on average. For casual workers, the gap is smaller in percentage terms but still significant.

### Decomposition Evidence

The Oaxaca-Blinder decomposition (Chapter 9 of Borjas) separates the wage gap into an "explained" component (due to differences in observable characteristics like education, experience, and occupation) and an "unexplained" component (often interpreted as a measure of discrimination).

!!! model "The Oaxaca-Blinder Decomposition"
    The standard decomposition begins with separate wage equations for the two groups:

    \[
    \ln w_U = X_U \hat{\beta}_U + \hat{u}_U \quad \text{(Upper caste)}
    \]
    \[
    \ln w_{SC} = X_{SC} \hat{\beta}_{SC} + \hat{u}_{SC} \quad \text{(Scheduled Caste)}
    \]

    The mean log wage gap can be decomposed as:

    \[
    \overline{\ln w}_U - \overline{\ln w}_{SC} = \underbrace{(\bar{X}_U - \bar{X}_{SC})\hat{\beta}_U}_{\text{Explained (endowments)}} + \underbrace{\bar{X}_{SC}(\hat{\beta}_U - \hat{\beta}_{SC})}_{\text{Unexplained (discrimination)}}
    \]

    The "explained" part captures differences in human capital and job characteristics. The "unexplained" part captures differences in the returns to those characteristics -- the fact that SC workers with the same education and experience earn less than upper-caste workers.

**Madheswaran and Attewell (2007, *Economic and Political Weekly*)** conducted one of the most influential Oaxaca-Blinder decompositions for India using NSS 1999-2000 data. They found:

- The total SC-upper caste wage gap for regular urban male workers was approximately 35 per cent (in log points).
- About half of this gap was "explained" by differences in education, experience, and occupational distribution.
- The remaining half was "unexplained" -- consistent with labour market discrimination.

!!! empirical "Discrimination or Omitted Variables?"
    A persistent challenge with the Oaxaca-Blinder decomposition is that the "unexplained" component captures not just discrimination but also any omitted variables correlated with caste -- quality of education, social networks, inherited wealth, neighbourhood effects, and unobserved ability. The decomposition provides an upper bound on discrimination, not a precise estimate. This is why audit and correspondence studies (see below) are valuable complements.

More recent studies have confirmed and extended these findings:

- **Hnatkovska, Lahiri, and Paul (2012, *Journal of Development Economics*)** track wage convergence between SC/ST and upper-caste workers across NSS rounds (1983-2005) and find modest but statistically significant convergence, driven primarily by rising SC/ST educational attainment.

- **Deshpande and Sharma (2016, *World Development*)** use IHDS data and find that the unexplained wage gap between SC and upper-caste workers is larger in the private sector than in the public sector -- consistent with affirmative action in government employment reducing (but not eliminating) discrimination.

---

## Correspondence Studies: Thorat and Attewell (2007)

The most direct evidence of caste discrimination in Indian labour markets comes from **correspondence studies** (also called audit studies) -- a methodology discussed in Chapter 9 of Borjas.

!!! empirical "Thorat and Attewell (2007): The Landmark Study"
    Sukhadeo Thorat and Jessica Attewell (2007, *Economic and Political Weekly*) conducted India's first large-scale correspondence study. They sent fictitious resumes in response to job advertisements in English-language newspapers in Delhi, varying only the name of the applicant to signal caste identity:

    - **Upper-caste Hindu names** (e.g., Sharma, Trivedi)
    - **Dalit names** (e.g., Jaatav, Bairwa)
    - **Muslim names** (e.g., Ahmed, Khan)

    Resumes were otherwise identical in education, experience, and qualifications. The results were striking:

    - Applicants with upper-caste names received callbacks at significantly higher rates than applicants with Dalit or Muslim names.
    - Dalit applicants received about one-third fewer callbacks than upper-caste applicants for the same jobs.
    - Muslim applicants faced similar or greater penalties.

    This is powerful evidence of **taste-based discrimination** in the Becker sense -- employers are forgoing profit-maximising hires because of a preference against certain groups.

The Thorat-Attewell design has since been replicated and extended:

- **Banerjee, Bertrand, Datta, and Mullainathan (2009, *Journal of Comparative Economics*)** found caste discrimination in hiring for software jobs in India, with lower callback rates for lower-caste applicants even in the high-skill IT sector.

- **Siddique (2011, *Journal of Development Economics*)** conducted an audit study of caste discrimination in the Indian private sector and found significant discrimination against SC applicants at the interview stage, not just the callback stage.

---

## Becker's Taste-Based Discrimination Model Applied to India

!!! model "Becker's Model and Caste"
    In Becker's (1957) model, an employer with a taste for discrimination acts as if hiring a worker from the discriminated group imposes an additional cost -- a "discrimination coefficient" \(d\). The employer hires the SC worker only if:

    \[
    w_{SC} + d < w_U
    \]

    That is, the SC worker must accept a wage discount of at least \(d\) to be hired. In competitive markets, Becker predicted that discrimination is costly to the discriminating employer and should be competed away over time, as non-discriminating firms earn higher profits by hiring productive but underpaid workers from the discriminated group.

    In the Indian context, however, several factors sustain discrimination despite competitive pressures:

    - **Customer discrimination:** In service industries, employers may discriminate because customers prefer upper-caste workers (e.g., Brahmin cooks in restaurants, upper-caste workers in personal services).
    - **Co-worker discrimination:** Upper-caste employees may resist working alongside Dalits, particularly in occupations involving food preparation, physical proximity, or shared facilities.
    - **Network hiring:** Informal hiring through social networks (referrals, family connections) systematically excludes castes that are not part of the dominant network, even without explicit animus.

---

## Statistical Discrimination

Statistical discrimination (Arrow, 1973; Phelps, 1972) offers a complementary explanation. If employers use caste as a signal of unobserved productivity -- because, on average, SC workers have attended lower-quality schools, had less exposure to English, or possess weaker professional networks -- then caste-based screening can be individually "rational" for firms while being socially harmful.

!!! model "Statistical Discrimination and Self-Fulfilling Prophecy"
    The pernicious aspect of statistical discrimination is its self-reinforcing nature. If employers expect SC workers to be less productive and therefore invest less in their training and offer them fewer promotions, then SC workers will accumulate less human capital and will indeed be less productive on average -- confirming the original stereotype. This is the **self-fulfilling prophecy** of statistical discrimination, which creates a low-level equilibrium trap for the discriminated group.

---

## Reservation Policy

India's affirmative action policy -- known as **reservation** -- reserves seats in government jobs, educational institutions, and elected legislatures for Scheduled Castes, Scheduled Tribes, and (since 1991) Other Backward Classes.

**Constitutional provisions:**

- Article 15(4): Allows special provisions for the advancement of SC/ST in education.
- Article 16(4): Allows reservation in government employment.
- Currently, SC reservation is 15 per cent, ST is 7.5 per cent, and OBC is 27 per cent in central government jobs. The Supreme Court has capped total reservation at 50 per cent (Indra Sawhney v. Union of India, 1992), though some states have exceeded this limit.

**Effectiveness in the labour market:**

!!! policy "Does Reservation Work?"
    The evidence is mixed:

    - **Public sector:** Reservation has significantly increased SC/ST representation in government employment, particularly in Class I and II positions. Deshpande and Weisskopf (2014, *Oxford Development Studies*) show that SC representation in central government services has roughly matched their population share, though they remain underrepresented in the highest positions.

    - **Education:** Reservation in higher education has expanded SC/ST access to professional degrees. Bertrand, Hanna, and Mullainathan (2010, *American Economic Review*) study reservation in Indian engineering colleges and find that marginal beneficiaries of reservation earn less than non-reserved students after graduation, but still earn substantially more than they would have without the reserved seat.

    - **Private sector:** There is no reservation in private sector employment, and the debate over extending it is politically charged. The private sector remains overwhelmingly dominated by upper-caste workers in managerial and professional positions.

---

## Private Sector Discrimination

The absence of reservation in the private sector means that caste discrimination operates with fewer checks. Several studies document this:

- The Thorat-Attewell (2007) correspondence study described above focused on private-sector job advertisements.

- **Jodhka and Newman (2007, *Economic and Political Weekly*)** conducted qualitative interviews with Delhi employers and found that many openly acknowledged using caste and community as screening criteria -- preferring workers from "known" communities and avoiding workers from "lower" backgrounds.

- **Corporate boards and management:** Damodaran (2008) and Deshpande and Sharma (2016) document that SC/ST representation in corporate boards, senior management, and professional services (law, medicine, chartered accountancy) remains extremely low relative to population shares.

---

## Intersectionality: Caste and Gender

Caste discrimination does not operate in isolation. It intersects with gender to produce **compounded disadvantage** for Dalit women:

!!! indian "Double Discrimination"
    Dalit women face discrimination on two axes simultaneously. They earn less than upper-caste women (caste penalty), less than Dalit men (gender penalty), and the two penalties are **not simply additive** -- they interact. Deshpande and Weisskopf (2014) show that the wage gap facing SC women relative to upper-caste men is larger than the sum of the separate caste and gender gaps. This is the intersectionality insight that the simple Becker model, which considers one dimension of discrimination at a time, struggles to capture.

Occupational patterns reflect this intersection:

- Dalit women are disproportionately concentrated in **manual scavenging** (the most stigmatised occupation in India), domestic work, and casual agricultural labour.
- Upper-caste women who participate in the labour market are more likely to be in education, healthcare, and white-collar services.
- The "U-shaped" LFPR relationship with income (discussed in the Gender & LFPR essay) is steeper for Dalit women, whose participation at low income levels is driven by acute economic necessity rather than choice.

---

## Recent Developments

Several trends are reshaping the caste-discrimination landscape:

1. **Urbanisation and anonymity:** As workers move to cities, the visibility of caste markers diminishes (though surname-based identification persists). Some evidence suggests that caste wage gaps are narrower in urban settings, particularly in the modern service sector.

2. **Education convergence:** SC/ST educational attainment has been rising faster than that of upper castes, narrowing one major source of the "explained" wage gap. However, quality gaps in education persist.

3. **Digital platforms and gig work:** Platform-based work (ride-hailing, delivery, freelancing) may reduce face-to-face discrimination by intermediating the employer-worker relationship. Whether this actually reduces caste penalties is an active area of research.

4. **AI and algorithmic hiring:** The growing use of AI tools in hiring raises new questions about whether algorithms inherit or amplify caste biases embedded in training data. This is the subject of emerging research (see, for instance, the "Algorithmic Untouchability" research agenda).

---

## Connection to the Textbook

| Textbook Chapter | Connection to Caste Discrimination |
|-----------------|-------------------------------------|
| **Ch. 9: Discrimination** | The Becker taste-based model, statistical discrimination, the Oaxaca-Blinder decomposition, and audit studies all find direct application in the Indian caste context. India is one of the richest empirical laboratories for testing discrimination theory. |
| **Ch. 5: Compensating Differentials** | Caste-segregated occupations involve hazardous work (manual scavenging, leather tanning) without compensating wage premia, violating hedonic wage predictions. |
| **Ch. 6: Education** | The human capital model must be extended to account for unequal access to quality education by caste, and the role of reservation in expanding educational opportunities. |
| **Ch. 7: Wage Distribution** | Caste is a major contributor to wage inequality in India, alongside gender and education. |

---

**Key References**

- Thorat, Sukhadeo, and Jessica Attewell (2007). "The Legacy of Social Exclusion: A Correspondence Study of Job Discrimination in India." *Economic and Political Weekly*, 42(41), 4141-4145.
- Madheswaran, S., and Paul Attewell (2007). "Caste Discrimination in the Indian Urban Labour Market: Evidence from the National Sample Survey." *Economic and Political Weekly*, 42(41), 4146-4153.
- Becker, Gary S. (1957). *The Economics of Discrimination*. Chicago: University of Chicago Press.
- Banerjee, Abhijit, Marianne Bertrand, Saugata Datta, and Sendhil Mullainathan (2009). "Labor Market Discrimination in Delhi: Evidence from a Field Experiment." *Journal of Comparative Economics*, 37(1), 14-27. DOI: 10.1016/j.jce.2008.09.002.
- Deshpande, Ashwini, and Thomas E. Weisskopf (2014). "Does Affirmative Action Reduce Productivity? A Case Study of the Indian Railways." *World Development*, 64, 169-180. DOI: 10.1016/j.worlddev.2014.05.024.
- Hnatkovska, Viktoria, Amartya Lahiri, and Sourabh Paul (2012). "Castes and Labor Mobility." *American Economic Journal: Applied Economics*, 4(2), 274-307. DOI: 10.1257/app.4.2.274.
- Bertrand, Marianne, Rema Hanna, and Sendhil Mullainathan (2010). "Affirmative Action in Education: Evidence from Engineering College Admissions in India." *Journal of Public Economics*, 94(1-2), 16-29. DOI: 10.1016/j.jpubeco.2009.11.003.
- Jodhka, Surinder S., and Katherine Newman (2007). "In the Name of Globalisation: Meritocracy, Productivity and the Hidden Language of Caste." *Economic and Political Weekly*, 42(41), 4125-4132.

---

*This essay draws on published academic research, PLFS data, and policy documents. All figures are approximate and should be verified against primary sources.*
