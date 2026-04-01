---
title: "Chapter 11: Unemployment"
description: "Types of unemployment, search theory, the reservation wage, unemployment insurance, the steady-state rate, the Beveridge curve, the NAIRU, and India's unemployment paradox."
---

# 11. Unemployment

Why do some workers remain jobless even in prosperous economies? Unemployment is one of the most important indicators of labour market performance, yet its persistence puzzles economists. This chapter develops the theoretical framework for understanding unemployment --- distinguishing its types, modelling the search process, analysing the role of unemployment insurance, and connecting unemployment to macroeconomic policy through the Phillips curve and the Beveridge curve.

---

## Types of Unemployment

Not all unemployment is alike. Economists distinguish three types based on their underlying causes.

### Frictional Unemployment

Frictional unemployment arises because it takes time for workers and firms to find each other. Even in a perfectly functioning labour market, workers transitioning between jobs, new entrants searching for a first position, and re-entrants returning after a career break all experience spells of joblessness. Frictional unemployment is **inevitable** and, to some extent, **efficient** --- it allows workers and firms to find better matches rather than accepting the first option available. A new graduate spending three months sending applications, or a software engineer who quits to find a higher-paying position and is unemployed for two weeks, are both examples of frictional unemployment.

### Structural Unemployment

Structural unemployment results from a **mismatch** between the skills workers possess and the skills employers demand, or between the locations where jobs exist and where workers live. Causes include:

- **Technological change** that renders certain skills obsolete (e.g., automation of routine manufacturing tasks, displacement of clerks by software)
- **Geographic shifts** in production (e.g., deindustrialisation of the US Rust Belt, relocation of textile production from Surat to Bangladesh)
- **Institutional barriers** such as minimum wages set above the market-clearing level, or occupational licensing requirements that restrict entry

Structural unemployment is typically **longer-lasting** than frictional unemployment because it requires workers to acquire new skills, relocate, or wait for new industries to emerge. A coal miner who loses her job because the power plant switches to solar energy faces structural unemployment: the demand for her specific skill has permanently declined.

### Cyclical Unemployment

Cyclical unemployment fluctuates with the business cycle. During recessions, aggregate demand falls, firms reduce output, and layoffs increase. During expansions, hiring picks up and unemployment falls. Cyclical unemployment is the component that macroeconomic stabilisation policies --- fiscal and monetary --- aim to address. A construction worker laid off during a recession is cyclically unemployed: the demand for construction services will recover when the economy does.

---

## Measuring Unemployment

### The ILO Definition

The International Labour Organization (ILO) defines an individual as **unemployed** if they simultaneously satisfy three conditions:

1. **Without work** --- did not work even one hour during the reference period in paid or self-employment
2. **Available for work** --- ready to start working within a short specified period
3. **Seeking work** --- took active steps to find employment during a recent specified period

The **unemployment rate** is:

\[
u = \frac{U}{L} = \frac{\text{Number unemployed}}{\text{Labour force}} = \frac{U}{E + U}
\]

where \( E \) is the number of employed persons and \( U \) is the number of unemployed persons. The labour force \( L = E + U \) includes only those who are either working or actively seeking work. People who are neither employed nor searching --- students, retirees, homemakers, discouraged workers --- are classified as **out of the labour force**.

### Hidden Unemployment

The official unemployment rate systematically understates the true extent of labour market slack because it excludes several important groups:

- **Discouraged workers:** People who want a job but have stopped searching because they believe no work is available. Since they are not "seeking work," they fall outside the labour force and are not counted as unemployed.
- **Underemployed workers:** People working part-time who want full-time work, or workers in jobs far below their skill level. They are classified as employed despite being inadequately utilised.
- **Marginally attached workers:** People who want work and have searched recently but not within the specific reference period used by the survey.

The US Bureau of Labor Statistics publishes alternative measures (U-1 through U-6) that progressively broaden the definition. The U-6 rate, which includes discouraged workers and involuntary part-timers, is typically 4--7 percentage points higher than the headline U-3 rate.

---

## The Steady-State Unemployment Rate

A simple and powerful framework relates the unemployment rate to the flows of workers into and out of unemployment.

!!! model "The Flow Model of Unemployment"
    Define:

    - \( s \) = **job separation rate** (probability that an employed worker loses or leaves a job per period)
    - \( f \) = **job finding rate** (probability that an unemployed worker finds a job per period)
    - \( E \) = number of employed workers
    - \( U \) = number of unemployed workers
    - \( L = E + U \) = labour force

    In **steady state**, the flow into unemployment equals the flow out:

    \[
    s \cdot E = f \cdot U
    \]

    Since \( E = L - U \):

    \[
    s(L - U) = fU \implies sL = (s + f)U
    \]

    The **steady-state unemployment rate** is therefore:

    \[
    u^* = \frac{U}{L} = \frac{s}{s + f}
    \]

    This elegant formula tells us that unemployment is higher when:

    - The **separation rate** \( s \) is high --- jobs are unstable, layoffs are frequent, matches dissolve quickly
    - The **finding rate** \( f \) is low --- it is difficult to find new jobs, matching is slow, vacancies are scarce

    **Example:** If \( s = 0.02 \) (2% of employed workers lose jobs each month) and \( f = 0.20 \) (20% of unemployed workers find jobs each month), then:

    \[
    u^* = \frac{0.02}{0.02 + 0.20} = \frac{0.02}{0.22} \approx 9.1\%
    \]

    The expected duration of an unemployment spell is \( 1/f = 1/0.20 = 5 \) months.

!!! empirical "Job Flows in the US"
    Monthly data from the Job Openings and Labor Turnover Survey (JOLTS) reveals enormous gross flows: in a typical month, about 5--6 million workers are hired and a similar number separate from their employers. The unemployment rate changes slowly because these large gross flows nearly cancel out. During recessions, the separation rate spikes and the finding rate drops, widening the gap between inflows and outflows and increasing the unemployment rate. Shimer (2012) shows that most of the cyclical variation in the US unemployment rate is driven by fluctuations in the job finding rate rather than the separation rate.

---

## Search Theory: The Reservation Wage

Job search is costly: it takes time, effort, and money. Workers facing unemployment must decide how long to search and what wage offers to accept. **Search theory**, pioneered by George Stigler (1961, 1962), formalises this decision.

Stigler's key insight was that information about wages and jobs is not free. Workers must invest resources to discover what different employers are willing to pay. Because search is costly, a rational worker will not canvass every possible employer but will instead adopt an **optimal stopping rule** that balances the expected benefits of further search against its costs.

### The Reservation Wage Model

!!! model "Optimal Stopping and the Reservation Wage"
    An unemployed worker receives one wage offer per period, drawn from a known distribution \( F(w) \) with support \( [\underline{w}, \bar{w}] \). Each period the worker is unemployed, they receive a flow payoff \( b \) (unemployment benefits plus the value of leisure minus the direct costs of search). The worker must decide whether to accept the current offer or reject it and continue searching.

    The optimal strategy takes a remarkably simple form: a **reservation wage** \( w^R \) such that the worker accepts any offer at or above \( w^R \) and rejects any offer below it. The reservation wage satisfies:

    \[
    w^R = b + \frac{1}{1+r} \int_{w^R}^{\bar{w}} (w - w^R) \, dF(w)
    \]

    where \( r \) is the discount rate. The left-hand side is the value of accepting the marginal offer (at exactly \( w^R \)). The right-hand side has two components: the flow value of unemployment \( b \), and the **option value** of continued search --- the expected gain from possibly drawing a higher offer next period.

    **Comparative statics:**

    | Change | Effect on \( w^R \) | Effect on Duration | Intuition |
    |--------|-------------------|--------------------|-----------|
    | Higher benefits \( b \) | Increases | Longer | Unemployment is less costly; worker can afford to be picky |
    | Higher wage dispersion | Increases | Longer | Greater upside from continued search |
    | Higher offer arrival rate | Ambiguous/Decreases | Shorter | More chances to draw a good offer; less need to be picky per draw |
    | Higher discount rate \( r \) | Decreases | Shorter | Future offers are worth less; accept sooner |

### Determinants of Unemployment Duration

The expected duration of an unemployment spell is \( 1/f \), where \( f \) is the probability of receiving and accepting an offer. Duration depends on:

1. **Unemployment benefits:** More generous benefits raise the reservation wage, extending duration. This is the central prediction of search theory and the basis for the moral hazard debate around unemployment insurance.
2. **Labour market conditions:** In recessions, fewer vacancies reduce the offer arrival rate, mechanically increasing duration even without any change in worker behaviour.
3. **Worker characteristics:** Younger and less-skilled workers tend to have longer spells. Older workers may also face longer spells due to employer reluctance and specific human capital loss.
4. **Search intensity:** Workers who search more actively --- sending more applications, broadening their geographic scope, using multiple search channels --- find jobs faster.

!!! empirical "Duration Dependence and Employer Stigma"
    Unemployment duration exhibits **negative duration dependence**: the probability of exiting unemployment falls the longer a worker has been unemployed. Two competing explanations exist:

    - **Unobserved heterogeneity:** Workers with better unobservable characteristics (motivation, networks, interview skills) exit quickly, leaving a pool of harder-to-place workers. The declining exit rate reflects changing composition, not a causal effect of duration.
    - **True state dependence:** Unemployment itself worsens prospects. Skills depreciate with disuse, professional networks atrophy, and employers view long spells as a negative signal.

    Kroft, Lange, and Notowidigdo (2013) use a **correspondence study** to isolate the stigma channel. They sent fictitious resumes to real job postings, varying only the length of the listed unemployment spell. Resumes with longer spells received significantly fewer callbacks, even though all other qualifications were identical. This provides clean evidence that employers discriminate against the long-term unemployed --- true state dependence operates through employer screening.

---

## Unemployment Insurance

Unemployment insurance (UI) provides temporary income to workers who involuntarily lose their jobs. While UI is essential for consumption smoothing and efficient job matching, it also creates incentive distortions. The design of optimal UI requires balancing these forces.

### Design Parameters

Every UI system is characterised by three key parameters:

- **Eligibility conditions:** Who qualifies? Typically restricted to workers who were employed for a minimum period and who were laid off (not fired for cause or voluntarily quit).
- **Benefit duration:** How long can benefits be received? In the US, the standard is 26 weeks, extended during recessions. European systems are often more generous (up to 2 years in some countries).
- **Replacement rate:** What fraction of prior wages do benefits replace? Most OECD countries set this at 40--70% of the prior wage, sometimes with a cap.

### Moral Hazard vs. Liquidity

!!! model "UI and the Reservation Wage"
    Higher UI benefits increase the flow value of unemployment \( b \), which raises the reservation wage:

    \[
    \frac{\partial w^R}{\partial b} > 0
    \]

    This has two distinct effects:

    1. **Moral hazard (substitution effect):** UI reduces the cost of being unemployed, so workers search less intensely and are pickier about offers. This extends unemployment duration and represents a pure efficiency loss.
    2. **Liquidity effect:** UI allows cash-constrained workers to avoid accepting the first desperate offer. Workers who would otherwise grab a bad match out of financial necessity can now search for a better-quality job, leading to higher wages and longer tenure in the eventual match. This represents an efficiency *gain*.

    The crucial distinction is that moral hazard reflects a behavioural response to changed incentives (workers choose to search less), while the liquidity effect reflects the relaxation of a borrowing constraint (workers can now afford to search optimally).

!!! empirical "Chetty (2008): Separating Moral Hazard from Liquidity"
    Raj Chetty (2008) develops a method to decompose the UI-duration relationship into moral hazard and liquidity components. His approach exploits variation in workers' pre-unemployment wealth: if the effect of UI on duration is larger for workers with low savings (who are liquidity-constrained) than for wealthy workers (who are not), then the liquidity channel dominates.

    **Key finding:** Approximately **60%** of the increase in unemployment duration from higher UI reflects the liquidity effect, and only about **40%** is moral hazard. This has profound policy implications: much of what looks like "laziness" (workers staying unemployed longer with higher benefits) is actually efficient search by workers who would otherwise be forced into poor matches.

    **Card, Chetty, and Weber (2007)** exploit a discontinuity in Austrian UI eligibility rules and find consistent results. Workers eligible for longer UI remain unemployed about 2--3 weeks longer per 10 additional weeks of benefits, with the effect operating primarily through the liquidity channel for workers with few savings.

!!! policy "Optimal UI Design: The Baily-Chetty Formula"
    The optimal UI replacement rate balances two forces:

    - **Higher replacement rate:** Better consumption smoothing for unemployed workers (the insurance benefit).
    - **Higher replacement rate:** Longer unemployment spells due to moral hazard (the efficiency cost).

    Baily (1978) and Chetty (2006) derive an elegant formula for the optimal replacement rate:

    \[
    \frac{b^*}{w} \approx \frac{\gamma \cdot \Delta c / c}{\varepsilon_{d,b}}
    \]

    where \( \gamma \) is the coefficient of relative risk aversion, \( \Delta c / c \) is the proportional consumption drop upon job loss, and \( \varepsilon_{d,b} \) is the elasticity of unemployment duration with respect to benefits. Optimal benefits are higher when workers are more risk-averse, when the consumption drop upon job loss is larger, and when the duration elasticity is smaller.

---

## The Beveridge Curve

The **Beveridge curve** (named after William Beveridge) plots the relationship between the unemployment rate and the vacancy rate. It captures a fundamental feature of labour markets: when unemployment is high, vacancies tend to be low, and vice versa.

!!! model "The Vacancy-Unemployment Relationship"
    The Beveridge curve slopes downward because:

    - In a **booming economy**, firms post many vacancies and workers find jobs easily, so vacancies are high and unemployment is low.
    - In a **recession**, firms cut hiring and increase layoffs, so vacancies fall and unemployment rises.

    Movements **along** the curve reflect business-cycle fluctuations (changes in aggregate demand). The economy slides to the upper-left in expansions and to the lower-right in recessions.

    **Shifts** of the curve reflect changes in **matching efficiency** --- the ability of the labour market to connect available workers with available vacancies:

    - An **outward shift** (both unemployment and vacancies rise simultaneously) signals deteriorating matching efficiency. Possible causes: skills mismatch due to structural change, geographic mismatch, reduced search intensity, or information frictions.
    - An **inward shift** signals improved matching: better job-search technology (online platforms), active labour market programmes, or reduced mismatch.

    The matching function \( M = m(U, V) \), introduced by Diamond (1982), Mortensen (1982), and Pissarides (1985), formalises this relationship. In the commonly used Cobb-Douglas form:

    \[
    M = A \cdot U^\alpha V^{1-\alpha}
    \]

    where \( A \) is matching efficiency and \( \alpha \) is the elasticity of matches with respect to unemployment. The job finding rate is \( f = M/U = A \cdot (V/U)^{1-\alpha} \), which increases with labour market tightness \( V/U \).

!!! empirical "The US Beveridge Curve After the Great Recession"
    The US Beveridge curve shifted markedly outward after the 2008--09 recession: vacancies recovered to pre-crisis levels by 2014, but unemployment remained elevated for much longer. This suggested a deterioration in matching efficiency --- possibly due to geographic immobility (underwater homeowners could not relocate), skills mismatch, or the accumulation of long-term unemployed workers who employers were reluctant to hire. By the late 2010s, the curve had shifted back inward, and the post-COVID recovery saw an unprecedented combination of very high vacancies and moderate unemployment, straining the standard Beveridge curve framework.

---

## The Natural Rate of Unemployment and the NAIRU

### Friedman's Natural Rate Hypothesis

In his 1968 presidential address to the American Economic Association, Milton Friedman introduced the concept of the **natural rate of unemployment** --- the rate that prevails when the economy is at its long-run equilibrium, with neither accelerating nor decelerating inflation. The natural rate equals the sum of frictional and structural unemployment:

\[
u^* = u_{\text{frictional}} + u_{\text{structural}}
\]

The natural rate is **not** a constant. It changes over time with demographics (a younger workforce has higher frictional unemployment), institutions (employment protection legislation, union density, UI generosity), and technology (better matching platforms reduce frictional search times).

### The Expectations-Augmented Phillips Curve

!!! model "The Phillips Curve and the NAIRU"
    The original Phillips (1958) curve documented a negative relationship between unemployment and nominal wage growth in the UK (1861--1957). Friedman (1968) and Phelps (1968) introduced inflation expectations, transforming the curve into:

    \[
    \pi = \pi^e - \alpha(u - u^*)
    \]

    where \( \pi \) is actual inflation, \( \pi^e \) is expected inflation, \( u \) is the actual unemployment rate, and \( u^* \) is the **NAIRU** (Non-Accelerating Inflation Rate of Unemployment).

    Key implications:

    - When \( u < u^* \): labour markets are tight, wages rise faster than expected, and inflation **accelerates**.
    - When \( u > u^* \): labour markets are slack, wage growth slows, and inflation **decelerates**.
    - In the **long run**, expectations adjust fully (\( \pi = \pi^e \)), and the economy gravitates to \( u^* \). The long-run Phillips curve is **vertical** at the natural rate.

    Policymakers face a **short-run trade-off** between unemployment and inflation. Expansionary monetary or fiscal policy can temporarily push unemployment below the natural rate, but only at the cost of higher inflation. Once expectations adjust, the economy returns to \( u^* \) with a permanently higher inflation rate. Attempting to keep unemployment permanently below the natural rate produces not just high inflation but *accelerating* inflation.

---

## Policy Responses to Unemployment

!!! policy "Active vs. Passive Labour Market Policies"
    **Passive policies** provide income support to the unemployed:

    - Unemployment insurance benefits
    - Severance pay mandates
    - Social assistance and welfare programmes

    **Active policies** aim to move workers back into employment:

    - **Job search assistance:** Resume workshops, job fairs, employment services, career counselling
    - **Training and retraining:** Programmes to update skills of displaced workers for new industries
    - **Wage subsidies:** Payments to firms that hire long-term unemployed or disadvantaged workers
    - **Public employment programmes:** Direct job creation by the government (e.g., NREGA in India, the New Deal's Works Progress Administration in the US)

    Card, Kluve, and Weber (2018) conduct a meta-analysis of 207 active labour market programme evaluations. They find that **job search assistance** is the most cost-effective intervention, while **subsidised public employment** has limited long-term effects. Training programmes show modest positive effects that grow over time --- they are more effective two years after participation than immediately after.

---

## Unemployment in India

!!! indian "India's Unemployment Paradox: Low Rates, Deep Distress"
    India presents one of the most striking puzzles in the global unemployment landscape. Official unemployment rates --- among the lowest in the world --- coexist with pervasive labour market distress. Understanding this paradox requires careful attention to measurement, definitional choices, and the structure of the Indian economy.

    **Three measures, three pictures:**

    India's **Periodic Labour Force Survey (PLFS)** reports unemployment under three different concepts, each using a different reference period:

    | Measure | Definition | PLFS 2023--24 Rate |
    |---------|-----------|-------------------|
    | **UPSS** (Usual Principal + Subsidiary Status) | Unemployed for most of the reference year; counts even brief subsidiary employment as "employed" | ~3.2% |
    | **CWS** (Current Weekly Status) | Unemployed during the reference week | ~5.0% |
    | **CDS** (Current Daily Status) | Unemployed on the average day of the reference week | ~7.5% |

    The wide gap between these measures reveals India's massive **underemployment** problem. The UPSS rate appears low because it classifies anyone who worked even briefly during the reference year as "employed" --- a farmer who works intensively for four months during the sowing and harvest seasons and sits idle for eight months counts as employed under UPSS.

    **Disguised unemployment in agriculture:** India's agricultural sector employs roughly 42--45% of the workforce but contributes only about 15% of GDP. This implies that the marginal product of many agricultural workers is extremely low --- in the extreme case, near zero. Arthur Lewis (1954) called these workers "surplus labour": they are technically employed but contribute little to output. Removing them from the farm would not reduce agricultural production. This **disguised unemployment** is invisible to standard measures.

    **Educated youth unemployment:** Perhaps the most alarming feature of India's labour market is the inverse relationship between education and unemployment. Youth (aged 15--29) unemployment rates are substantially higher than for older workers, and among youth, those with graduate degrees and above face **higher** unemployment rates than those with only secondary education. The 2024 ILO India Employment Report documents that unemployment among educated youth (secondary and above) was approximately 18.4% in recent years. This reflects:

    - Rapid expansion of higher education without corresponding growth in formal-sector employment
    - Severe skills mismatch between academic curricula and employer requirements
    - **Wait unemployment:** Educated youth prefer to remain unemployed while queuing for formal-sector jobs (government positions, corporate employment) rather than accept informal-sector work that they consider beneath their qualifications

    **Discouraged workers:** The PLFS shows that India's labour force participation rate, particularly for women, is among the lowest in the world. Many potential workers --- especially women in rural areas --- are not even counted in the labour force because they have abandoned the search for work. If these discouraged workers were included, the effective unemployment rate would be substantially higher.

    **CMIE-CPHS data:** The Centre for Monitoring Indian Economy's Consumer Pyramids Household Survey, which uses a more frequent survey cycle and different methodology, often reports higher unemployment rates than the official PLFS, particularly during economic shocks (e.g., the COVID-19 lockdowns, demonetisation).

!!! policy "MGNREGA: Employment Guarantee as Unemployment Policy"
    The Mahatma Gandhi National Rural Employment Guarantee Act (MGNREGA, 2005) guarantees 100 days of unskilled manual work per year to every rural household that demands it. As an unemployment policy, MGNREGA serves multiple functions:

    1. **Counter-cyclical automatic stabiliser:** Demand for MGNREGA work rises during agricultural lean seasons and economic downturns. The programme automatically expands when it is most needed, without requiring new legislation or discretionary decisions.
    2. **Reservation wage floor:** By offering a guaranteed wage, MGNREGA sets a de facto minimum in rural labour markets, raising the outside option for agricultural and informal workers. Imbert and Papp (2015) estimate that MGNREGA increased private-sector wages by approximately **4.7%** and reduced private-sector employment, confirming the programme's role as an outside option.
    3. **Insurance against income shocks:** For households without access to formal unemployment insurance --- the vast majority of rural India --- MGNREGA provides a crucial safety net during crop failures, droughts, and economic downturns.
    4. **Asset creation:** Public works under MGNREGA (rural roads, irrigation channels, land development, watershed management) generate productive infrastructure with lasting benefits.

    **Limitations:** Administrative delays in wage payments (often weeks or months), restriction to unskilled manual work (does not address educated unemployment), the 100-day cap, wide variation in implementation quality across states, and inability to address urban unemployment. MGNREGA addresses the *quantity* of employment but not its *quality* --- it cannot solve the structural mismatch that drives educated youth unemployment.

---

## Key Takeaways

1. **Frictional unemployment** is the inevitable result of the time needed for matching; **structural unemployment** arises from skill and geographic mismatches; **cyclical unemployment** fluctuates with the business cycle. Together, frictional and structural unemployment constitute the natural rate.

2. The **steady-state unemployment rate** \( u^* = s/(s+f) \) provides a simple but powerful framework: unemployment depends on the rate at which jobs are destroyed (\( s \)) relative to the rate at which they are found (\( f \)).

3. **Search theory** (Stigler, 1961/1962) shows that workers optimally set a **reservation wage**, accepting offers above it and rejecting offers below it. Higher UI benefits, greater wage dispersion, and lower discount rates all raise the reservation wage and extend unemployment duration.

4. **Unemployment insurance** creates a trade-off between consumption smoothing (insurance) and moral hazard (reduced search). Chetty (2008) shows that approximately 60% of the UI-duration relationship reflects a **liquidity effect** --- enabling efficient search --- rather than moral hazard.

5. The **Beveridge curve** captures the negative relationship between vacancies and unemployment. Outward shifts signal deteriorating matching efficiency; inward shifts signal improvement. The matching function \( M = A \cdot U^\alpha V^{1-\alpha} \) formalises this relationship.

6. The **Phillips curve** describes a short-run trade-off between unemployment and inflation, but in the long run the curve is vertical at the **NAIRU**. Friedman (1968) showed that attempts to keep unemployment permanently below the natural rate produce accelerating inflation.

7. **India's unemployment** is best understood through its three measures (UPSS, CWS, CDS). Low headline rates mask severe **underemployment**, disguised unemployment in agriculture, an alarming educated **youth unemployment** crisis, and one of the world's lowest female labour force participation rates. **MGNREGA** serves as a counter-cyclical employment guarantee and rural wage floor but cannot address structural mismatches.

---

<div style="display: flex; justify-content: space-between; margin-top: 2rem;">
<a href="../10-incentive-pay/index.md">:octicons-arrow-left-24: Chapter 10: Incentive Pay</a>
<a href="../index.md">Back to Chapters Overview</a>
</div>
