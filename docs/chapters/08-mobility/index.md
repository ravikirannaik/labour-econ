---
title: "Labor Mobility"
description: "Chapter 8 — Migration as investment, the Roy model, immigration surplus, job turnover, and internal migration in India"
---

# 8. Labor Mobility

> *"The history of mankind is the history of migration."*
> --- Kofi Annan

Workers are not bolted to the factory floor. They move --- across jobs, across firms, across cities, and across national borders. These movements are among the most consequential decisions in a worker's life, and they reshape the economies that send and receive migrants. A software engineer who leaves Patna for Bengaluru, a construction worker who migrates seasonally from Bihar to Kerala, a nurse who emigrates from Kerala to the Gulf --- each is making an investment decision, trading current costs for future returns.

This chapter applies the human capital framework from Chapter 6 to geographic and job mobility. We develop the economic model of migration, analyse who chooses to move and why, examine the labour market effects of immigration, and study job turnover as a mechanism for improving match quality. Throughout, we pay special attention to India's massive internal migration flows, which differ fundamentally from the stylised US labour market that dominates textbook treatments.

---

## Migration as a Human Capital Investment

The decision to migrate follows the same logic as the decision to invest in education: a worker compares the present value of benefits (higher wages, better opportunities in the destination) against the costs (moving expenses, foregone earnings during the transition, psychic costs of leaving family and community).

!!! model "The Migration Decision Rule"
    A worker currently in region \( o \) (origin) considers moving to region \( d \) (destination). Migration is worthwhile if the present value of net gains exceeds zero:

    \[
    \sum_{t=1}^{T} \frac{w_d(t) - w_o(t)}{(1+r)^t} - C > 0
    \]

    where:

    - \( w_d(t) \) = earnings in the destination in year \( t \)
    - \( w_o(t) \) = earnings in the origin in year \( t \) (the opportunity cost)
    - \( r \) = discount rate
    - \( C \) = direct costs of migration (moving expenses, job search, psychic costs)
    - \( T \) = remaining working years

    This framework generates several testable predictions:

    1. **Workers are more likely to migrate when the wage gap is large** --- a higher \( w_d(t) - w_o(t) \) raises the present value of migration.
    2. **Young workers are more likely to migrate** --- they have more years (\( T \)) over which to collect returns, so the present value of a given annual gain is larger.
    3. **Workers are less likely to migrate when costs are high** --- distance, language barriers, family ties, immigration restrictions, and uncertainty all increase \( C \).
    4. **Workers with higher discount rates are less likely to migrate** --- a high \( r \) reduces the present value of future gains relative to upfront costs.

!!! empirical "Age and Migration"
    The prediction that migration rates decline with age is one of the most robust findings in the literature. In the United States, the interstate migration rate for workers aged 20--24 is approximately three times the rate for workers aged 45--54. The same pattern holds in India: the 2011 Census shows that migration rates peak sharply in the 20--30 age group and decline thereafter. Young workers have more to gain and less to lose --- fewer location-specific investments (homeownership, children's schooling, spousal employment) that are destroyed by moving.

---

## The Roy Model: Self-Selection in Migration

Not all workers are equally likely to migrate. The **Roy model** (Roy, 1951), adapted to migration by Borjas (1987), provides a framework for understanding *who* selects into migration --- and whether migrants are drawn from the top or the bottom of the origin's skill distribution.

!!! model "The Roy Model of Self-Selection"
    Consider two regions. Region 1 has a compressed wage distribution (low inequality, high taxes, strong unions). Region 2 has a dispersed wage distribution (high inequality, low taxes, weak institutions).

    The wage a worker earns depends on their skill level and the region's returns to skill:

    \[
    \ln w_1 = \mu_1 + \sigma_1 \cdot s \qquad \text{(Region 1)}
    \]
    \[
    \ln w_2 = \mu_2 + \sigma_2 \cdot s \qquad \text{(Region 2)}
    \]

    where \( s \) is the worker's skill level (standardised), \( \mu_j \) is the base wage, and \( \sigma_j \) measures the returns to skill (or wage dispersion) in region \( j \).

    **Case 1: Positive selection** --- When the destination has *higher* returns to skill (\( \sigma_2 > \sigma_1 \)), the highest-skilled workers gain the most from moving to Region 2. Migration is positively selected: the movers are drawn from the *upper* tail of the origin's skill distribution.

    *Example*: A highly skilled engineer in Sweden (compressed wages) moves to the US (dispersed wages) where her exceptional ability is better rewarded.

    **Case 2: Negative selection** --- When the destination has *lower* returns to skill (\( \sigma_2 < \sigma_1 \)), the lowest-skilled workers benefit most from moving to Region 2, where the wage floor is relatively higher. Migration is negatively selected: the movers are drawn from the *lower* tail.

    *Example*: A low-skilled worker in a highly unequal developing country moves to a welfare state with a generous safety net and compressed wages.

The Roy model's key insight is that migration is **not random** --- the composition of the migrant flow depends on the relative wage structures of origin and destination. This has profound implications for immigration policy: the skills and productivity of immigrants depend not just on who wants to come, but on the economic incentives created by the origin and destination wage distributions.

---

## Internal Migration: Determinants and Consequences

Internal migration --- movement within a country's borders --- is driven by the same wage-gap logic as international migration, but typically faces lower costs (no visa restrictions, shared language, legal right to move).

### The Gravity Model of Migration

Empirically, internal migration flows are well described by a **gravity model**:

!!! model "Gravity Model of Migration"
    The flow of migrants from region \( o \) to region \( d \) is approximately:

    \[
    M_{od} = k \cdot \frac{P_o \cdot P_d}{D_{od}^\gamma}
    \]

    where \( P_o \) and \( P_d \) are the populations (proxying for economic size) of the origin and destination, \( D_{od} \) is the distance between them (proxying for migration costs), \( \gamma \) is the distance elasticity, and \( k \) is a constant. Augmented versions include wage differences, unemployment rates, and amenities.

In the long run, internal migration should drive wages toward convergence across regions. Workers leave low-wage areas (reducing labour supply, pushing wages up) and arrive in high-wage areas (increasing labour supply, pushing wages down). The speed of convergence depends on the magnitude of migration costs and institutional barriers.

!!! empirical "Wage Convergence in the US"
    Barro and Sala-i-Martin (1992) estimated that US states converge in per-capita income at a rate of approximately 2% per year --- meaning half the gap between a poor state and a rich state closes in about 35 years. Internal migration is a key mechanism, along with capital flows and technology diffusion. Southern states, which had much lower wages than the North in the early 20th century, experienced massive outmigration (the Great Migration of African Americans) that contributed to regional convergence.

---

## International Migration: The Immigration Surplus

When workers cross national borders, the effects on the receiving country's labour market depend on whether immigrants complement or substitute for native workers.

### The Basic Framework

!!! model "The Immigration Surplus"
    Consider a simple economy with native workers and capital. The labour demand curve is downward-sloping. An inflow of immigrants shifts the labour supply curve to the right, which:

    1. **Reduces wages** for workers who compete with immigrants (substitutes)
    2. **Increases returns to capital** (firms benefit from cheaper labour)
    3. **Generates an immigration surplus** --- a net gain to the native economy

    The immigration surplus arises because the value of output produced by immigrants exceeds the wages paid to them (the difference accrues to capital owners and complementary workers). Borjas (1995) estimated the surplus as:

    \[
    \text{Immigration Surplus} \approx \frac{1}{2} \cdot e \cdot s^2 \cdot \text{GDP}
    \]

    where \( e \) is the elasticity of labour demand and \( s \) is the immigrant share of the labour force. For the United States (with \( e \approx -0.3 \) and \( s \approx 0.15 \)), the surplus is quite small --- roughly 0.3% of GDP --- though the *redistribution* from workers to capital owners is much larger.

    The critical distinction: immigration creates a small net gain for natives as a whole, but this gain masks a large transfer from native workers (who face lower wages) to native capital owners (who earn higher returns). Immigration is a net positive, but it has distributional consequences.

### Short-Run vs. Long-Run Effects

The time horizon matters enormously:

- **Short run**: Immigrants increase labour supply in a fixed set of industries and locations. Wages fall for competing workers. The Mariel Boatlift study (Card, 1990) found that the sudden arrival of 125,000 Cuban immigrants in Miami had virtually no effect on wages or employment of native workers, suggesting rapid absorption --- though this finding has been debated (Borjas, 2017).

- **Long run**: Capital adjusts, new firms enter, and the economy expands. In the long run, if capital is perfectly mobile, wages return to their pre-immigration level and the entire benefit of immigration accrues as an increase in the size of the economy. Empirical estimates suggest adjustment takes 5--10 years.

!!! policy "Immigration Policy Frameworks"
    Countries use different mechanisms to select immigrants:

    - **Points-based systems** (Canada, Australia): score applicants on education, language, age, and job offers. Designed to maximise positive selection on observable skills.
    - **Employment-based quotas** (US H-1B visa): tied to employer sponsorship. Selects workers with specific skills demanded by firms but creates dependency on the sponsoring employer.
    - **Family reunification** (dominant in US permanent immigration): admits relatives of existing residents. Skill selection is indirect and often weaker.
    - **Free movement** (EU Schengen): no restrictions on labour mobility within the zone. Allows market forces to allocate workers across regions.

    The design of immigration policy determines the skill composition of the immigrant flow and therefore whether the effects on native wages are concentrated among high-skill or low-skill workers.

---

## Job Turnover and Match Quality

Labour mobility is not only geographic. Workers also move between jobs within the same city --- and this job-to-job mobility is a crucial mechanism for improving **match quality** between workers and firms.

### The Theory of Job Matching

Not all worker-firm pairings are equally productive. A worker may be talented but poorly matched to her current employer. Job turnover allows workers to search for better matches, improving both their own earnings and aggregate productivity.

!!! model "Match Quality and Tenure"
    The match-quality framework predicts:

    1. **Wages rise with tenure** --- partly because of firm-specific human capital accumulation (Becker), and partly because workers in good matches stay while those in bad matches leave (selection).
    2. **Turnover rates decline with tenure** --- the longer a worker has been at a firm, the more likely it is a good match (bad matches have already ended). This explains why quit rates fall sharply with job tenure.
    3. **Young workers have high turnover** --- early in a career, workers engage in "job shopping," trying different jobs to learn about their own abilities and preferences. Turnover rates are highest in the first few years of labour market experience.

    Topel and Ward (1992) found that the typical US worker holds 7 jobs in the first 10 years of their career, and that about one-third of total wage growth over the first decade comes from job-to-job transitions rather than within-job raises.

### Specific vs. General Training and Mobility

The distinction between **firm-specific** and **general** human capital (Chapter 6) has direct implications for mobility:

- **General human capital** (literacy, numeracy, programming languages) is portable across firms. Workers with mostly general skills face low mobility costs and are more likely to change jobs.
- **Firm-specific human capital** (knowledge of the firm's internal systems, client relationships, institutional procedures) is destroyed when the worker leaves. Workers with substantial firm-specific capital face high opportunity costs of quitting, and firms face high costs of losing them. Both sides have incentives to maintain the match.

This generates a key prediction: wages in the current job will partly reflect firm-specific capital that would be lost upon separation, creating a *wedge* between the worker's current wage and her outside option. This wedge makes long-tenured workers less mobile and more vulnerable to wage cuts that remain above their (lower) outside option.

---

## Indian Context: Internal Migration

!!! indian "Internal Migration in India"
    India's internal migration landscape is vast, complex, and poorly captured by standard economic models that assume frictionless mobility.

    **Scale**: The 2011 Census recorded approximately 450 million internal migrants (people living in a place different from their place of birth), roughly 37% of the population. However, this includes marriage-related migration (which dominates female migration) and long-settled moves. Economic migration is harder to measure precisely.

    **Types of economic migration:**

    - **Seasonal/circular migration**: An estimated 100+ million workers migrate seasonally, moving to construction sites, brick kilns, farms, and urban informal sectors for 3--8 months per year and returning home for planting/harvesting. These workers are largely invisible in standard surveys because they are away during enumeration.
    - **Semi-permanent rural-urban migration**: Workers who move to cities for extended periods (1--5 years) but maintain strong ties to their village of origin, sending remittances and returning for festivals and family events.
    - **Permanent migration**: Workers who relocate permanently, typically for regular salaried employment or education.

    **Key corridors**: Bihar and UP to Delhi, Maharashtra, and Gujarat; Odisha and Jharkhand to Tamil Nadu and Kerala; Rajasthan to Gujarat; North-Eastern states to Bengaluru, Delhi, and Pune.

    **Barriers to migration** (Munshi and Rosenzweig, 2016; Kone et al., 2018):

    1. **Caste and community networks**: Mobility is heavily mediated by caste-based networks that provide information, housing, and job referrals in the destination. Workers without network connections face much higher migration costs.
    2. **Language**: India's linguistic diversity (22 official languages, hundreds of dialects) creates significant communication barriers, particularly for low-skilled workers crossing state lines.
    3. **Portability of entitlements**: Access to subsidised food (PDS), housing (PM-AWAS), health insurance (Ayushman Bharat), and children's education is often tied to the state of domicile, making interstate migration costly.
    4. **Housing and urban infrastructure**: Migrants in cities face extremely high housing costs relative to their wages, often living in overcrowded slums without basic amenities. The absence of affordable rental housing markets is a binding constraint.
    5. **"Sons of the soil" politics**: Political movements that oppose migration from other states (e.g., anti-migrant rhetoric in Maharashtra, hostility toward "outsiders" in the Northeast) create a hostile environment and occasionally physical danger for migrants.

    Kone et al. (2018) estimated that India's internal migration rate is significantly lower than what would be predicted by its regional wage differences, suggesting that barriers to mobility are substantial. They calculate that removing these barriers could generate large welfare gains.

    **COVID-19 and the migrant crisis**: The 2020 lockdown laid bare the vulnerability of India's migrant workforce. An estimated 10--11 million workers attempted to return to their home states, many on foot, after losing employment and housing overnight. The crisis exposed the absence of portable social protection, the informal sector's fragility, and the extraordinary dependence of urban economies on migrant labour.

---

## Key Takeaways

1. **Migration is a human capital investment.** Workers compare the present value of higher earnings at the destination against the costs of moving. This explains why young workers, workers facing large wage gaps, and workers with low moving costs are most likely to migrate.

2. **The Roy model explains self-selection.** Migrants are not a random sample of the origin population. When the destination rewards skill more than the origin (higher inequality), migration is positively selected (high-skill workers move). When the destination compresses wages (lower inequality), migration is negatively selected.

3. **Internal migration drives regional wage convergence**, but the speed of convergence depends on migration costs, institutional barriers, and the portability of skills and entitlements.

4. **Immigration generates a small net surplus for natives** but redistributes income from competing workers to capital owners and complementary workers. The size of the surplus depends on the skill composition of immigrants and the elasticity of labour demand.

5. **Short-run and long-run effects differ.** In the short run, immigration may depress wages for substitutes. In the long run, capital adjustment and economic expansion attenuate or eliminate the wage effects.

6. **Job turnover improves match quality.** Workers "shop" for jobs early in their careers, and a significant fraction of wage growth comes from job-to-job transitions rather than within-job raises.

7. **Firm-specific human capital reduces mobility.** Workers with substantial firm-specific skills face high costs of quitting, creating a wedge between their current wage and their outside option.

8. **India's internal migration** is massive but constrained by language barriers, non-portable entitlements, caste networks, housing costs, and political hostility. These barriers keep migration rates below efficient levels and reduce potential welfare gains.

---

*[Previous: Chapter 7 --- The Wage Distribution](../07-wage-distribution/index.md)* | *[Practice Problems](practice.md)* | *[Resources](resources.md)* | *[Next: Chapter 9 --- Labor Market Discrimination](../09-discrimination/index.md)*
