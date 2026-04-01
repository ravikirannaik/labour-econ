---
title: "Practice — Labor Mobility"
description: "Practice problems on migration decisions, the Roy model, immigration surplus, job turnover, and Indian internal migration"
---

# Practice: Labor Mobility

Test your understanding of Chapter 8. Questions progress from the migration investment framework to the Roy model, the immigration surplus, and Indian-context applications. Click on any question to reveal the answer.

---

??? question "Q1. Migration as Investment: NPV Calculation"
    A worker in a small town earns Rs 30,000 per month. She is considering moving to Bengaluru, where she expects to earn Rs 50,000 per month. The one-time cost of migration (moving expenses, security deposit, job search) is Rs 2,00,000. She has 20 remaining working years. Assume an annual discount rate of 5% and ignore taxes.

    **(a)** Calculate the annual earnings gain from migration.

    **(b)** Calculate the present value of the earnings gain over 20 years.

    **(c)** Should she migrate? Show your calculation.

    **(d)** How would your answer change if she had only 5 remaining working years?

    ---

    **Answer:**

    **(a)** Annual gain = (50,000 - 30,000) x 12 = Rs 2,40,000 per year.

    **(b)** Present value of an annuity of Rs 2,40,000 for 20 years at 5%:

    \[
    PV = 2{,}40{,}000 \times \frac{1 - (1.05)^{-20}}{0.05} = 2{,}40{,}000 \times 12.462 = Rs \; 29{,}90{,}880
    \]

    **(c)** Net present value = PV of gains - migration cost = 29,90,880 - 2,00,000 = **Rs 27,90,880 > 0**. Yes, she should migrate. The present value of the earnings gain far exceeds the one-time cost.

    **(d)** With only 5 years remaining:

    \[
    PV = 2{,}40{,}000 \times \frac{1 - (1.05)^{-5}}{0.05} = 2{,}40{,}000 \times 4.329 = Rs \; 10{,}38{,}960
    \]

    NPV = 10,38,960 - 2,00,000 = Rs 8,38,960 > 0. She should still migrate, but the gain is much smaller. This illustrates why older workers are less likely to migrate --- the payback period is shorter, and for smaller wage gaps the NPV could turn negative.

---

??? question "Q2. The Age-Migration Relationship"
    Using the migration investment model, explain why the migration rate typically peaks for workers in their 20s and declines with age. Identify at least three distinct mechanisms.

    ---

    **Answer:**

    Three mechanisms explain the age-migration pattern:

    **1. Shorter payback period.** Older workers have fewer remaining working years (\( T \) is smaller), so the present value of the annual wage gain is lower. For the same wage gap and migration cost, the NPV is smaller and may fall below zero.

    **2. Higher location-specific investments.** Older workers have accumulated more location-specific capital: homeownership (selling costs), children enrolled in local schools, a spouse with a local job, established social networks, familiarity with local institutions. These increase the effective cost of migration (\( C \) is larger).

    **3. Lower expected wage gains.** Younger workers are still early in their careers, where the return to finding a better match is highest. Older workers have already sorted into jobs and locations that reasonably match their skills. The expected wage gain from moving (\( w_d - w_o \)) may be smaller because good matches have already been found.

    A fourth mechanism, sometimes cited: older workers are more risk-averse on average (or face higher costs of failure, e.g., they cannot easily move back in with parents), which effectively raises the discount rate or the risk premium embedded in \( C \).

---

??? question "Q3. Roy Model: Positive vs. Negative Selection"
    Two countries have the following wage structures:

    | Country | Mean log wage (\( \mu \)) | Std. dev. of log wages (\( \sigma \)) |
    |---------|:-:|:-:|
    | Country A (origin) | 2.5 | 0.4 |
    | Country B (destination) | 3.0 | 0.8 |

    **(a)** Does Country B have more or less wage inequality than Country A?

    **(b)** According to the Roy model, will migration from A to B be positively or negatively selected? Explain.

    **(c)** Now suppose the destination is Country C, with \( \mu = 3.2 \) and \( \sigma = 0.2 \). How does the selection pattern change?

    ---

    **Answer:**

    **(a)** Country B has **more** wage inequality. Its standard deviation of log wages (0.8) is twice that of Country A (0.4), meaning wages are much more dispersed.

    **(b)** Migration from A to B will be **positively selected**. Country B has higher returns to skill (\( \sigma_B = 0.8 > \sigma_A = 0.4 \)). High-skilled workers in Country A are "under-rewarded" relative to what they would earn in B, where the skill premium is larger. The most talented workers gain the most from moving to a high-inequality destination. Migrants will be drawn disproportionately from the *upper* tail of Country A's skill distribution.

    **(c)** Country C has **lower** wage inequality (\( \sigma_C = 0.2 < \sigma_A = 0.4 \)). Migration from A to C will be **negatively selected**. Low-skilled workers in Country A, who earn low wages in A's more unequal distribution, would benefit from C's compressed wages and higher floor. The least-skilled workers gain the most from moving to a low-inequality destination. Migrants will be drawn from the *lower* tail of Country A's skill distribution.

---

??? question "Q4. Immigration Surplus"
    A small economy has GDP of Rs 100 crore, with labour's share equal to 70%. The labour demand elasticity is -0.3. Immigrants currently constitute 10% of the labour force.

    **(a)** Calculate the approximate immigration surplus using Borjas's formula.

    **(b)** Explain why the surplus is small relative to GDP even though immigration may have large effects on individual wages.

    **(c)** Who gains and who loses from immigration in this framework?

    ---

    **Answer:**

    **(a)** Immigration surplus \( \approx \frac{1}{2} \times |e| \times s^2 \times \text{GDP} \)

    \[
    = \frac{1}{2} \times 0.3 \times (0.10)^2 \times 100 = \frac{1}{2} \times 0.3 \times 0.01 \times 100 = \textbf{Rs 0.15 crore}
    \]

    This is **0.15% of GDP** --- a very small net gain.

    **(b)** The surplus is small because it represents a *triangle* (the efficiency gain from employing immigrants at a wage below their marginal product at the initial labour supply). The redistribution --- from native workers (who face wage competition) to capital owners (who benefit from cheaper labour) --- is a *rectangle* and is much larger. In this example, the wage reduction for native workers transfers income to employers, but the net effect on natives as a whole (the surplus) is just the small triangle. Immigration is approximately a "wash" for native welfare in aggregate, even though it reshuffles income significantly.

    **(c)** **Winners**: Capital owners and employers benefit from lower labour costs and higher profits. Native workers whose skills *complement* immigrants (e.g., managers supervising immigrant workers, or skilled workers in industries expanded by immigrant labour) also gain.

    **Losers**: Native workers whose skills *substitute* for immigrants face wage competition and earn lower wages. The loss is concentrated among workers in the same skill group as the immigrant inflow (e.g., low-skilled natives when immigrants are predominantly low-skilled).

---

??? question "Q5. Short-Run vs. Long-Run Immigration Effects"
    Explain why the wage effects of immigration may differ between the short run and the long run. Use the concepts of capital adjustment and economic expansion in your answer.

    ---

    **Answer:**

    **Short run**: The capital stock is fixed. When immigrants arrive, they increase the labour supply while the amount of capital remains unchanged. The capital-labour ratio falls, and marginal productivity of labour declines. Wages for substitutable workers fall. This is the standard downward-sloping demand curve effect.

    **Long run**: Capital adjusts. Higher returns to capital (generated by the short-run wage decline) attract new investment. Firms build more factories, offices, and infrastructure. New firms enter industries where immigrant labour makes production profitable. As the capital stock expands, the capital-labour ratio rises back toward its original level.

    In the extreme case of perfectly mobile capital (an open economy with free capital flows), the long-run capital-labour ratio returns to exactly its pre-immigration level, and wages return to their original level. In this case, immigration has *no* long-run wage effect --- the entire benefit manifests as a larger economy (more output, more workers, more capital) at the same wage.

    In practice, capital adjustment is not instantaneous. Empirical evidence suggests it takes roughly 5--10 years for wages to recover from an immigration shock, depending on the size of the inflow and the flexibility of the capital market.

---

??? question "Q6. The Mariel Boatlift"
    In 1980, Fidel Castro allowed 125,000 Cubans to leave from the port of Mariel. Most settled in Miami, increasing the city's labour force by approximately 7% in a matter of months.

    **(a)** What does the standard competitive model predict should happen to wages in Miami?

    **(b)** Card (1990) found essentially no effect on wages or employment of native workers in Miami. Provide two possible explanations for this finding.

    **(c)** Why is this natural experiment considered more credible than cross-sectional comparisons of cities with different immigrant shares?

    ---

    **Answer:**

    **(a)** The competitive model predicts that a sudden 7% increase in labour supply should shift the supply curve right, lowering equilibrium wages for workers who are substitutes for the Cuban immigrants (primarily low-skilled workers). Employment of natives might fall if wages are sticky.

    **(b)** Two explanations for the null finding:

    1. **Absorption through industry expansion**: Miami's economy expanded to absorb the additional workers. New businesses opened, existing businesses expanded, and industries that used low-skilled labour (garment manufacturing, construction, services) grew. The demand curve shifted rightward roughly in proportion to the supply shift.

    2. **Native outmigration**: Some native workers (or potential native in-migrants) may have left Miami or chosen not to move there in response to increased competition. If native labour supply in Miami decreased to partially offset the immigrant inflow, the net effect on wages would be attenuated.

    **(c)** Cross-sectional comparisons (comparing high-immigration cities to low-immigration cities) suffer from **endogeneity**: immigrants choose to settle in cities where wages are high and labour demand is strong. This creates a positive correlation between immigration and wages that masks the causal effect. The Mariel Boatlift is a natural experiment because the decision to open the port was Castro's political decision, unrelated to Miami's labour market conditions. The immigrant inflow was exogenous to local demand, making causal inference more credible.

---

??? question "Q7. Job Turnover and Match Quality"
    **(a)** Why do quit rates decline with job tenure? Provide two explanations --- one based on match quality and one based on firm-specific human capital.

    **(b)** Topel and Ward (1992) found that about one-third of early-career wage growth comes from job-to-job transitions. What does this imply about the role of job mobility in the labour market?

    ---

    **Answer:**

    **(a)**

    **Match quality explanation**: Workers in bad matches (low productivity, poor fit) quit quickly. Workers in good matches stay. Over time, the pool of workers with long tenure is increasingly composed of good matches, because bad matches have already been dissolved. This *selection effect* causes average quit rates to fall with tenure.

    **Firm-specific human capital explanation**: As workers accumulate firm-specific skills (knowledge of internal systems, client relationships, institutional memory), the value of the current match increases relative to outside options. The cost of quitting rises because firm-specific capital is destroyed upon separation. Workers with more tenure have more to lose from leaving, so they quit less.

    Both mechanisms operate simultaneously and are difficult to disentangle empirically.

    **(b)** It implies that **job mobility is productive, not wasteful**. A significant share of wage growth comes not from getting better at one job but from finding a better job. This "job shopping" is an efficient process of information discovery: workers learn about their own skills and preferences, and firms learn about worker quality, through a sequence of matches. Policies that reduce job mobility (e.g., excessive employment protection, non-compete clauses, pension systems that penalise job changers) may reduce wage growth by preventing workers from finding their best match.

---

??? question "Q8. Specific vs. General Training and Mobility"
    A worker receives two years of training at her current firm. In Scenario A, the training is entirely general (e.g., learning Python programming). In Scenario B, the training is entirely firm-specific (e.g., learning the firm's proprietary CRM system).

    **(a)** In which scenario is the worker more likely to leave the firm after training? Why?

    **(b)** In which scenario will the firm pay for the training? Why?

    **(c)** How does firm-specific training create a "wedge" between the worker's current wage and her outside option?

    ---

    **Answer:**

    **(a)** The worker is more likely to leave in **Scenario A** (general training). General skills (Python) are valued by all employers. The worker's outside option rises by the full value of the training. If any other firm offers even slightly more, she will leave. In Scenario B, the firm-specific skills have no value outside the firm, so the outside option is unchanged. Leaving would mean losing the returns to firm-specific training.

    **(b)** The firm will pay for training in **Scenario B** (firm-specific). In Scenario A, general training raises the worker's market wage, so the firm cannot capture the returns --- the worker could leave and earn the higher wage elsewhere. Rational firms will not invest in general training (workers must pay for it themselves, e.g., through lower wages during training). In Scenario B, the firm can share the returns with the worker because the skills are not portable: the worker's outside option does not rise, so the firm can pay less than the worker's full post-training productivity while still keeping her.

    **(c)** After firm-specific training, the worker's productivity at the current firm exceeds her productivity at any other firm. Her current wage is set between these two values: above her outside option (so she does not quit) but below her full productivity (so the firm captures some return). This creates a wedge:

    \[
    w_{\text{outside}} < w_{\text{current}} < \text{VMP}_{\text{current firm}}
    \]

    This wedge makes the worker less mobile (quitting means dropping to the lower outside wage) and gives both the firm and the worker an incentive to maintain the match. It also means the worker is partially "locked in" and vulnerable to wage adjustments within this band.

---

??? question "Q9. Indian Internal Migration"
    **(a)** Distinguish between seasonal/circular migration and permanent migration in India. Why is seasonal migration difficult to measure in standard surveys?

    **(b)** Identify three barriers to interstate migration in India that have no equivalent in the US labour market.

    **(c)** Kone et al. (2018) argue that India's internal migration rate is "too low" relative to its regional wage differences. What welfare implications does this have?

    ---

    **Answer:**

    **(a)** **Seasonal/circular migration**: Workers migrate for 3--8 months per year, typically during the agricultural off-season, to work in construction, brick kilns, or urban informal jobs. They maintain their primary residence in the village and return for planting/harvesting. **Permanent migration**: Workers relocate indefinitely to a new location, often for regular salaried employment, with no intention of returning except for visits.

    Seasonal migration is difficult to measure because: (i) surveys typically enumerate households at their "usual place of residence," so workers who are temporarily away are counted at home, not at their destination; (ii) short-duration moves (under 6 months) are often excluded from migration definitions; (iii) seasonal migrants are concentrated in informal employment with no payroll records.

    **(b)** Three India-specific barriers:

    1. **Language barriers**: India has 22 officially recognised languages. A worker from Bihar (Hindi) moving to Tamil Nadu (Tamil) faces severe communication constraints --- unlike a worker moving from Ohio to Texas within the English-speaking US.
    2. **Non-portable entitlements**: PDS ration cards, Ayushman Bharat health insurance, state-specific housing schemes, and children's school admissions are often tied to state of domicile. Moving interstate means losing access to these benefits until new registration is completed (which can take years). The US has federal social programmes (Social Security, Medicare, SNAP) that are portable across states.
    3. **"Sons of the soil" politics**: Political parties in several states actively campaign against migrants from other states, sometimes leading to violence (e.g., anti-Bihari sentiment in Maharashtra). There is no equivalent political hostility to interstate migration in the US.

    **(c)** If migration is "too low" relative to the wage differentials that should incentivise movement, workers are stuck in low-productivity locations when they could earn more (and produce more) elsewhere. This implies:

    - **Allocative inefficiency**: Labour is not flowing to its highest-value use. GDP is lower than it would be under freer mobility.
    - **Persistent regional inequality**: Without sufficient out-migration from poor states, wages in those states remain depressed and convergence is slow.
    - **Unrealised individual welfare gains**: Workers who *would* benefit from migrating are prevented from doing so by institutional barriers, meaning their lifetime income is lower than it could be.

    Reducing migration barriers (portable entitlements, affordable urban housing, language support) would generate welfare gains analogous to the gains from trade --- allowing people to move to where they are most productive.

---

??? question "Q10. Policy Analysis: Open Borders"
    Some economists (e.g., Clemens, 2011) have argued that removing barriers to international migration --- "open borders" --- would roughly double world GDP.

    **(a)** Using the migration investment framework, explain why the wage gains from international migration are so large.

    **(b)** Identify two reasons why host-country governments resist open borders despite the efficiency gains.

    **(c)** How does the Roy model help predict the composition of migrants under an open-borders regime?

    ---

    **Answer:**

    **(a)** The wage gaps between rich and poor countries are enormous --- a construction worker earns 5--10 times more doing the same job in the US than in India. This means the annual earnings gain (\( w_d - w_o \)) from international migration is very large. Under the migration investment framework, the present value of moving from a low-wage to a high-wage country far exceeds the costs for most workers. The total efficiency gain from allowing all welfare-improving moves would be massive because it would move hundreds of millions of workers from low-productivity environments to high-productivity ones. Clemens (2011) calls these "trillion-dollar bills on the sidewalk."

    **(b)** Two reasons for resistance:

    1. **Distributional concerns**: While open borders would increase aggregate welfare, native workers in host countries who compete with immigrants would face wage declines. The political opposition comes from those who bear the costs, not from those who reap the benefits (employers, consumers, immigrants themselves). The losses are concentrated and visible; the gains are diffuse.
    2. **Fiscal costs and public services**: Large-scale immigration strains public services (schools, hospitals, housing, infrastructure). If immigrants initially earn low wages and pay low taxes while consuming public services, native taxpayers bear a fiscal cost --- at least in the short run.

    **(c)** Under open borders, the Roy model predicts that the composition of migrants depends on the relative wage structures of origin and destination:

    - From highly unequal countries moving to compressed-wage destinations (e.g., a worker from Brazil moving to Scandinavia): **negative selection** --- low-skilled workers benefit most from the destination's high wage floor.
    - From compressed-wage countries moving to highly unequal destinations (e.g., a worker from Scandinavia moving to the US): **positive selection** --- high-skilled workers benefit most from the destination's high returns to skill.

    In practice, under open borders with heterogeneous origin countries, the migrant flow would be a complex mixture of positively and negatively selected streams, depending on the specific origin-destination pair.

---

*[Back to Chapter 8](index.md)* | *[Resources](resources.md)* | *[Previous: Chapter 7 Practice](../07-wage-distribution/practice.md)*
