---
title: "Resources — Labor Market Equilibrium"
---

# Resources: Labor Market Equilibrium

---

## Required Reading

| Reading | Details |
|---------|---------|
| **Borjas, Chapter 4** | "Labor Market Equilibrium." In *Labor Economics*, 8th ed., McGraw-Hill, 2020. |

---

## Key Empirical Papers

### Immigration

- **Card, David.** "The Impact of the Mariel Boatlift on the Miami Labor Market." *Industrial and Labor Relations Review* 43, no. 2 (1990): 245--257. DOI: [10.1177/001979399004300205](https://doi.org/10.1177/001979399004300205). Exploits the 1980 Mariel boatlift as a natural experiment; finds no significant effect on wages or unemployment of non-Cuban workers in Miami.

- **Borjas, George J.** "The Labor Demand Curve Is Downward Sloping: Reexamining the Impact of Immigration on the Labor Market." *Quarterly Journal of Economics* 118, no. 4 (2003): 1335--1374. DOI: [10.1162/003355303322552810](https://doi.org/10.1162/003355303322552810). Uses variation in immigrant inflows across education-experience cells to estimate that a 10% immigration-induced supply increase reduces wages by 3--4%.

- **Borjas, George J.** "The Wage Impact of the Marielitos: A Reappraisal." *Industrial and Labor Relations Review* 70, no. 5 (2017): 1077--1110. DOI: [10.1177/0019793917692945](https://doi.org/10.1177/0019793917692945). Re-examines the Mariel Boatlift, focusing on high-school dropouts, and finds significant wage declines---challenging Card's earlier findings.

- **Peri, Giovanni, and Chad Sparber.** "Task Specialization, Immigration, and Wages." *American Economic Journal: Applied Economics* 1, no. 3 (2009): 135--169. DOI: [10.1257/app.1.3.135](https://doi.org/10.1257/app.1.3.135). Shows that native and immigrant workers specialize in different tasks, reducing direct competition and attenuating the negative wage effect of immigration.

### Payroll Taxes and Mandated Benefits

- **Gruber, Jonathan.** "The Incidence of Mandated Maternity Benefits." *American Economic Review* 84, no. 3 (1994): 622--641. [JSTOR](https://www.jstor.org/stable/2118071). Finds that the cost of state-mandated maternity health insurance was shifted almost entirely to the wages of women of childbearing age, with minimal employment effects.

- **Gruber, Jonathan.** "The Incidence of Payroll Taxation: Evidence from Chile." *Journal of Labor Economics* 15, no. S3 (1997): S72--S101. DOI: [10.1086/209877](https://doi.org/10.1086/209877). Studies Chile's payroll tax reform, finding that payroll tax reductions were passed through to higher wages, consistent with standard incidence theory.

- **Kugler, Adriana, and Maurice Kugler.** "Labor Market Effects of Payroll Taxes in Developing Countries: Evidence from Colombia." *Economic Development and Cultural Change* 57, no. 2 (2009): 335--358. DOI: [10.1086/592839](https://doi.org/10.1086/592839). Finds that payroll tax increases in Colombia reduced wages by 1.5--2.4 percentage points per 10-point tax increase, confirming partial pass-through to workers.

### Cobweb and Market Dynamics

- **Freeman, Richard B.** "A Cobweb Model of the Supply and Starting Salary of New Engineers." *Industrial and Labor Relations Review* 29, no. 2 (1976): 236--248. DOI: [10.1177/001979397602900206](https://doi.org/10.1177/001979397602900206). Empirical evidence that the market for engineers exhibits cobweb-like dynamics, with enrolment responding to lagged wages.

---

## Indian Context Readings

### Internal Migration

- **Imbert, Clement, and John Papp.** "Labor Market Effects of Social Programs: Evidence from India's Employment Guarantee." *American Economic Journal: Applied Economics* 7, no. 2 (2015): 233--263. DOI: [10.1257/app.20130401](https://doi.org/10.1257/app.20130401). Finds that NREGA implementation reduced seasonal migration and raised wages in rural areas, consistent with the equilibrium model's prediction that raising the reservation wage tightens the migrant labour supply.

- **Munshi, Kaivan, and Mark Rosenzweig.** "Networks and Misallocation: Insurance, Migration, and the Rural-Urban Wage Gap." *American Economic Review* 106, no. 1 (2016): 46--98. DOI: [10.1257/aer.20131365](https://doi.org/10.1257/aer.20131365). Shows that caste-based rural insurance networks discourage migration to cities, contributing to persistent rural-urban wage gaps in India.

- **Tumbe, Chinmay.** *India Moving: A History of Migration*. Penguin Viking, 2018. Accessible overview of internal migration patterns in India, covering colonial and post-independence periods.

### EPF and Labour Regulation

- **Hasan, Rana, and Karl Robert L. Jandoc.** "The Distribution of Firm Size in India: What Can Survey Data Tell Us?" ADB Economics Working Paper Series No. 213, 2010. Documents India's "missing middle"---few medium-sized firms---and links it to labour regulations that apply at firm-size thresholds.

- **Besley, Timothy, and Robin Burgess.** "Can Labor Regulation Hinder Economic Performance? Evidence from India." *Quarterly Journal of Economics* 119, no. 1 (2004): 91--134. DOI: [10.1162/003355304772839533](https://doi.org/10.1162/003355304772839533). Exploits cross-state variation in amendments to the Industrial Disputes Act to show that pro-worker regulations reduced output, employment, and investment in formal manufacturing.

- **Government of India.** *Employees' Provident Funds and Miscellaneous Provisions Act, 1952*. [Link](https://www.epfindia.gov.in/site_docs/PDFs/Downloads_PDFs/EPFAct1952.pdf). The statutory framework for India's EPF system.

- **Government of India.** *Employees' State Insurance Act, 1948*. [Link](https://www.esic.nic.in/esi-act). The statutory framework for India's ESI system.

---

## Supplementary Readings

- **Borjas, George J.** *Immigration Economics*. Harvard University Press, 2014. Book-length treatment of the economics of immigration, extending the surplus model and addressing the empirical debates.

- **Summers, Lawrence H.** "Some Simple Economics of Mandated Benefits." *American Economic Review* 79, no. 2 (1989): 177--183. [JSTOR](https://www.jstor.org/stable/1827753). Classic framework paper distinguishing mandated benefits from taxes based on how much workers value the benefit.

---

## Video Resources

- **Marginal Revolution University.** "Tax Incidence" and "Immigration and Labor Markets." Short animated lectures on payroll tax burden sharing and the immigration surplus. Available at [mru.org](https://mru.org).

- **CORE Econ.** Unit 9: "The Labour Market: Wages, Profits, and Unemployment." [core-econ.org](https://www.core-econ.org/the-economy/book/text/09.html). Covers labour market equilibrium with institutional detail.

---

## Stata Exercises

!!! stata "Payroll Tax Simulation"
    ```stata
    * Simulate the effect of a payroll tax on equilibrium
    clear
    set obs 200

    * Market parameters (per Q1 in Practice)
    gen wage = _n * 0.5
    gen Ld = 800 - 10 * wage
    gen Ls = -100 + 20 * wage

    * After tax t = 6 on employers
    gen Ld_tax = 740 - 10 * wage

    * Plot
    twoway (line Ld wage, lc(blue)) ///
           (line Ls wage, lc(red)) ///
           (line Ld_tax wage, lc(blue) lp(dash)), ///
        legend(label(1 "Demand") label(2 "Supply") ///
               label(3 "Demand after tax")) ///
        title("Payroll Tax Incidence") ///
        xtitle("Wage") ytitle("Employment (000s)") ///
        xline(28 30 34, lp(dot) lc(gray))
    ```

!!! stata "Immigration Wage Effects — Borjas Cell Approach"
    ```stata
    * Illustration of the education-experience cell approach
    * (Requires PLFS or CPS micro-data)

    use worker_panel.dta, clear

    * Create education-experience cells
    gen edu_group = cond(edu_years < 12, 1, ///
                   cond(edu_years < 16, 2, 3))
    gen exp_group = floor(experience / 5)

    * Calculate immigrant share by cell and year
    bysort edu_group exp_group year: ///
        egen imm_share = mean(immigrant)

    * Cell-level average wage
    bysort edu_group exp_group year: ///
        egen avg_lnwage = mean(ln_wage)

    * Regression: wage on immigrant share with cell and year FEs
    reghdfe avg_lnwage imm_share, ///
        absorb(edu_group#exp_group year) cluster(edu_group#exp_group)

    * Coefficient on imm_share estimates the wage effect
    * Borjas (2003) finds approximately -0.3 to -0.4
    ```
