---
title: "NREGA"
---

# NREGA: India's Employment Guarantee

The Mahatma Gandhi National Rural Employment Guarantee Act (MGNREGA, commonly called NREGA) is one of the most ambitious social protection programmes in the world. Enacted in 2005, it guarantees 100 days of unskilled manual wage employment per year to every rural household whose adult members volunteer to do such work. For students of labour economics, NREGA is not merely a welfare programme -- it is a **labour market intervention** that directly alters reservation wages, rural wage dynamics, migration patterns, and the equilibrium distribution of employment. It is a living experiment in the textbook models of Chapters 2, 4, and 11.

---

## Design and Key Features

### The Legal Guarantee

NREGA is unique among workfare programmes because it provides a **legal right** to employment. If a rural household demands work and the local government (gram panchayat) fails to provide it within 15 days, the household is entitled to an unemployment allowance. This demand-driven design distinguishes NREGA from supply-driven programmes where the government decides when and where to create jobs.

!!! indian "Key Design Features"
    | Feature | Detail |
    |---------|--------|
    | **Eligibility** | Any rural household (adult members willing to do unskilled manual work) |
    | **Entitlement** | 100 days of guaranteed employment per household per financial year |
    | **Wage** | State-specific NREGA wage rate (notified annually; ranges from Rs. 234 to Rs. 374 per day across states in 2024-25) |
    | **Works** | Water conservation, drought proofing, rural connectivity, land development, flood control |
    | **Gender** | At least one-third of workers must be women (actual share has exceeded 50% nationally) |
    | **Childcare** | If 5 or more children under 6 are at a worksite, a crèche must be provided |
    | **Transparency** | All expenditures are publicly available through the MIS portal (nrega.nic.in) |
    | **Implementation** | Gram panchayats plan and execute works; funds flow from central to state to district to GP |

### Self-Targeting Mechanism

!!! model "Self-Targeting: An Elegant Design"
    NREGA uses a **self-targeting** mechanism: the programme offers hard manual labour at a relatively low wage. This means that only those who truly need the work will demand it. Better-off workers with higher reservation wages voluntarily opt out. In the textbook framework:

    - A worker participates in NREGA if and only if their market wage \( w_m \) is less than the NREGA wage \( w_N \):

    \[
    \text{Participate if } w_m < w_N
    \]

    - Workers whose skills command a market wage above \( w_N \) self-select out of the programme.

    This elegantly avoids the need for costly means testing (verifying who is "poor enough" to qualify). The work requirement itself filters out non-poor applicants. This is the classic **workfare vs. welfare** distinction that the labour supply model in Chapter 2 illuminates.

---

## Labour Market Effects

NREGA's effects on the rural labour market have been extensively studied and are among the best-documented programme impacts in development economics.

### The Reservation Wage Floor

The most fundamental effect of NREGA is that it sets a **floor on the reservation wage** of rural workers. Before NREGA, a casual agricultural labourer in a slack season had no outside option -- accept whatever wage the local employer offers, or starve. With NREGA, the same worker can refuse wages below the NREGA rate, because they have an alternative source of employment.

!!! model "NREGA as a Reservation Wage Shifter"
    In the Chapter 2 framework, the reservation wage \( w^* \) is the minimum wage at which a worker is willing to supply labour. NREGA effectively sets:

    \[
    w^* = \max(w^*_{\text{original}}, w_N)
    \]

    For workers whose original reservation wage was below the NREGA wage, the programme raises \( w^* \) to \( w_N \). This shifts the labour supply curve to the left (at any wage below \( w_N \), fewer workers are available to private employers), which puts **upward pressure on private-sector wages**. This is precisely what the empirical evidence finds.

### Impact on Rural Wages

!!! empirical "Wages: The Key Finding"
    **Imbert and Papp (2015, *American Economic Review*)** provide the most rigorous evidence on NREGA's wage effects. Using a difference-in-differences strategy that exploits the phased rollout of NREGA across districts (Phase 1 in 2006, Phase 2 in 2007, Phase 3 in 2008), they find:

    - NREGA raised casual wages in the private sector by approximately **4.7 per cent** during the agricultural lean season.
    - The effect was concentrated in the dry season, when NREGA activity peaks and private agricultural labour demand is low.
    - The effect was larger in districts with better NREGA implementation (measured by actual employment generated).
    - The wage increase benefited not only NREGA participants but all casual workers in treated districts -- a **general equilibrium effect** through the labour market.

    This is a clean example of the competitive equilibrium model (Chapter 4): a positive supply shock to one employer (the government) tightens the labour market for other employers, raising the equilibrium wage for all.

### Impact on Migration

NREGA was also expected to reduce distress migration by providing employment in the home village. The evidence on this is more nuanced:

- **Imbert and Papp (2015)** find that NREGA reduced **temporary out-migration** from rural areas during the lean season by about 10 per cent. Workers who would have migrated to urban construction sites or brick kilns stayed home to work on NREGA projects.

- **Zimmermann (2020, *Journal of Labor Economics*)** examines the migration channel more carefully and finds that NREGA induced a **reallocation of labour** from the private to the public sector during the lean season, but did not significantly reduce permanent migration. Seasonal and circular migration, however, declined.

!!! model "NREGA and the Harris-Todaro Model"
    NREGA complicates the standard Harris-Todaro framework. In that model, rural workers migrate to urban areas when the expected urban wage exceeds the certain rural wage. NREGA raises the "certain rural wage" (by providing guaranteed employment at \( w_N \)), which should reduce migration. In equilibrium:

    \[
    w_N + \text{NREGA employment probability} \times w_N > w_R \quad \Rightarrow \quad \text{Migration falls}
    \]

    The phased-rollout evidence is broadly consistent with this prediction, at least for seasonal migration.

### Impact on Agricultural Labour Markets

NREGA's wage effects had ripple consequences for agricultural employers. Several studies document that:

- **Landowners responded** to higher wages by shifting toward mechanisation (tractors, harvesters) and less labour-intensive crops. Berg, Bhatt, and"; show evidence of this substitution effect in parts of Rajasthan and Andhra Pradesh.

- **Labour rationing during peak season** became a complaint of farmers in states with high NREGA activity, though this claim is disputed -- NREGA activity falls sharply during the peak agricultural season (kharif sowing/harvest), suggesting complementarity rather than conflict.

---

## Key Research Papers

Beyond Imbert and Papp, several other major studies have shaped our understanding of NREGA:

**Muralidharan, Niehaus, and Sukhtankar (2023, *American Economic Review*)** study the effect of **biometric smartcard-based payments** for NREGA in Andhra Pradesh. They find that improving the payment system (reducing delays and leakage) increased the effective wage received by workers, increased NREGA participation, and raised private-sector casual wages through the reservation wage channel. This paper demonstrates that programme design details -- how workers are paid, not just how much -- have first-order labour market effects.

**Zimmermann (2020, *Journal of Labor Economics*)** uses the phased rollout and finds that NREGA raised private-sector wages by shifting labour supply. She emphasises the **general equilibrium** nature of the effect: even non-participants benefit from tighter labour markets.

**Klonner and Oldiges (2014)** find that NREGA reduced rural poverty in early-phase districts, consistent with the programme's role as an income floor.

**Dutta, Murgai, Ravallion, and van de Walle (2012, *World Bank Economic Review*)** provide a more cautious assessment, showing that rationing is severe -- many households that demand NREGA work do not receive it, and those who do often get far fewer than 100 days.

---

## Implementation Challenges

The gap between NREGA's elegant design and its on-the-ground reality is substantial.

### Delayed Payments

!!! policy "The Payment Problem"
    Perhaps the most persistent implementation failure is **delayed wage payments**. NREGA mandates payment within 15 days of work completion, but studies have found average delays of 30-90 days in many states. Delayed payments effectively reduce the present value of the NREGA wage, discouraging participation by precisely the poorest workers who cannot afford to wait. Khera (2011, *Economic and Political Weekly*) documents cases where workers waited months for payment, defeating the programme's purpose as a timely safety net. The shift to direct bank transfers and Aadhaar-linked payments has improved timeliness in some states, but the problem persists in others.

### Rationing and Unmet Demand

Despite the legal guarantee of 100 days, the average number of days worked per household nationally has been around 45-50 days in recent years. Many households receive zero days. This rationing reflects both supply-side constraints (insufficient budget allocation, slow administrative processes) and local political economy factors (panchayat leaders prioritising certain areas or groups).

### Corruption and Leakage

NREGA is not immune to the governance challenges that afflict Indian public programmes. Common problems include:

- **Ghost workers:** Fictitious names on muster rolls, with wages siphoned by officials.
- **Inflated material expenditures:** Claiming higher-than-actual costs for materials (cement, gravel), leaving less for wages.
- **Measurement fraud:** Recording fewer days worked than actually performed, or recording work that was never done.

Social audits -- a mandatory feature of NREGA -- have been most effective in Andhra Pradesh/Telangana, where an independent state-level agency conducts audits. In most other states, social audit capacity is weak.

### Quality of Assets

NREGA creates **durable assets** -- ponds, roads, irrigation channels, land levelling -- in addition to providing employment. The quality of these assets has been variable. Some studies (Mani et al., 2020; Shah and Mehta, 2020) find that well-planned NREGA works have improved agricultural productivity and water availability. Others find hastily constructed works that deteriorate within a year.

---

## Gender and NREGA

One of NREGA's notable successes is **high female participation**:

!!! indian "Women in NREGA"
    Nationally, women constitute over 55 per cent of NREGA person-days worked, far exceeding the statutory minimum of one-third. In states like Kerala and Tamil Nadu, female participation exceeds 80 per cent. This is significant because:

    1. **NREGA offers work close to home**, which reduces the mobility constraint that limits women's access to other employment.
    2. **NREGA wages are the same for men and women** by law, which means women receive the full notified wage rather than the gender-discounted wage prevalent in private agricultural labour markets.
    3. **NREGA may increase women's bargaining power** within households by providing an independent source of income. Afridi, Mukhopadhyay, and Sahoo (2016, *Journal of Development Economics*) find evidence that NREGA employment is associated with improved nutrition among children in participant households, consistent with women directing NREGA income toward food.

    However, women also face specific challenges: they are more likely to receive delayed payments, less likely to receive unemployment allowance when work is not provided, and often perform the most labour-intensive tasks (earth-moving, water-carrying).

---

## NREGA in the COVID-19 Crisis

NREGA played a crucial role during the COVID-19 pandemic:

- During the nationwide lockdown (March-June 2020), millions of migrant workers returned to rural areas (see the Migration essay). NREGA was one of the few programmes that could absorb this sudden influx of labour.
- Demand for NREGA spiked: in FY 2020-21, NREGA generated 389 crore person-days of employment -- the highest since its inception.
- The government increased the NREGA wage by Rs. 20 and raised the budget allocation from Rs. 61,500 crore to over Rs. 1,11,000 crore during the crisis year.
- NREGA's demand-driven design proved its value: unlike supply-driven programmes that could not scale quickly, NREGA could accommodate rising demand (albeit with delays and rationing).

---

## Fiscal Cost and Sustainability

NREGA is a significant fiscal commitment. The annual budget allocation has typically been Rs. 60,000-90,000 crore (approximately USD 7-11 billion), making it one of India's largest social protection programmes. Critics argue that:

- The programme crowds out more productive public investment.
- The fiscal cost is high relative to the poverty reduction achieved.
- The work created has limited productivity impact relative to direct cash transfers.

Supporters counter that:

- NREGA's **insurance function** (providing income during shocks) is worth more than the direct wage payment, because it prevents asset depletion and distress migration.
- The **asset creation** component generates returns that are difficult to capture in standard cost-benefit analysis.
- The **general equilibrium wage effects** benefit all rural casual workers, not just programme participants.

!!! policy "NREGA vs. Cash Transfers: A Textbook Debate"
    The comparison between NREGA (in-kind transfer of employment) and unconditional cash transfers maps directly onto the Chapter 2 analysis of in-kind vs. cash transfers. The labour supply model predicts that cash transfers are weakly preferred by recipients (they can always choose to work if they want to). The argument for NREGA-style workfare is threefold: (1) self-targeting reduces fiscal cost by screening out the non-poor; (2) the work requirement may be politically sustainable in ways that cash transfers are not; (3) the asset creation component provides public goods. The optimal design depends on the relative importance of these factors, which is ultimately an empirical question.

---

## Connection to the Textbook

| Textbook Chapter | Connection to NREGA |
|-----------------|---------------------|
| **Ch. 2: Labor Supply** | NREGA as a reservation wage shifter; the work-leisure model applied to programme participation; in-kind vs. cash transfer analysis; self-targeting through the work requirement. |
| **Ch. 4: Equilibrium** | General equilibrium wage effects of a large public employer entering the rural labour market; the impact on private-sector wages and employment; multi-sector models. |
| **Ch. 8: Mobility** | NREGA reduces seasonal migration by raising the rural reservation wage; this is a direct application of the migration-as-investment model. |
| **Ch. 11: Unemployment** | NREGA as a form of unemployment insurance for rural India; the programme's relationship to search theory (lowering the cost of job search by providing a fallback option). |

---

**Key References**

- Imbert, Clement, and John Papp (2015). "Labor Market Effects of Social Programs: Evidence from India's Employment Guarantee." *American Economic Journal: Applied Economics*, 7(2), 233-263. DOI: 10.1257/app.20130401.
- Zimmermann, Laura (2020). "Why Guarantee Employment? Evidence from a Large Indian Public-Works Program." *Journal of Labor Economics*, 38(3), 621-655. DOI: 10.1086/706090.
- Muralidharan, Karthik, Paul Niehaus, and Sandip Sukhtankar (2023). "General Equilibrium Effects of (Improving) Public Employment Programs: Experimental Evidence from India." *American Economic Review*, 113(5), 1498-1529. DOI: 10.1257/aer.20210059.
- Dutta, Puja, Rinku Murgai, Martin Ravallion, and Dominique van de Walle (2012). "Does India's Employment Guarantee Scheme Guarantee Employment?" *Economic and Political Weekly*, 47(16), 55-64.
- Khera, Reetika (2011). "The UID Project and Welfare Schemes." *Economic and Political Weekly*, 46(9), 37-43.
- Afridi, Farzana, Abhiroop Mukhopadhyay, and Soham Sahoo (2016). "Female Labor Force Participation and Child Education in India: Evidence from the National Rural Employment Guarantee Scheme." *Journal of Development Economics*, 118, 199-215. DOI: 10.1016/j.jdeveco.2015.06.004.
- MGNREGA Official Portal: [nrega.nic.in](https://nrega.nic.in/) -- real-time data on employment generated, wages paid, and works completed.

---

*This essay draws on published academic research, official NREGA MIS data, and policy analyses. Figures are approximate and reflect data available as of early 2026.*
