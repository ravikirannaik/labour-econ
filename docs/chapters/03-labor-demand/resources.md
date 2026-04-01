---
title: "Resources — Labor Demand"
---

# Resources: Labor Demand

---

## Required Reading

| Reading | Details |
|---------|---------|
| **Borjas, Chapter 3** | "Labor Demand." In *Labor Economics*, 8th ed., McGraw-Hill, 2020. |

---

## Key Empirical Papers

### Minimum Wage Effects

- **Card, David, and Alan B. Krueger.** "Minimum Wages and Employment: A Case Study of the Fast-Food Industry in New Jersey and Pennsylvania." *American Economic Review* 84, no. 4 (1994): 772--793. DOI: [10.3386/w4509](https://doi.org/10.3386/w4509). The landmark natural experiment using DiD to study the effect of New Jersey's minimum wage increase on fast-food employment. Found no significant negative employment effect.

- **Neumark, David, and William Wascher.** "Minimum Wages and Employment: A Case Study of the Fast-Food Industry in New Jersey and Pennsylvania: Comment." *American Economic Review* 90, no. 5 (2000): 1362--1396. DOI: [10.1257/aer.90.5.1362](https://doi.org/10.1257/aer.90.5.1362). Re-analysis of Card and Krueger using payroll data rather than survey data, finding negative employment effects.

- **Dube, Arindrajit, T. William Lester, and Michael Reich.** "Minimum Wage Effects Across State Borders." *Review of Economics and Statistics* 92, no. 4 (2010): 945--964. DOI: [10.1162/REST_a_00039](https://doi.org/10.1162/REST_a_00039). Contiguous-county border design showing minimal disemployment effects of minimum wages, improving on earlier identification strategies.

- **Dube, Arindrajit.** "Impacts of Minimum Wages: Review of the International Evidence." UK Government Report, 2019. [Link](https://www.gov.uk/government/publications/impacts-of-minimum-wages-review-of-the-international-evidence). Comprehensive survey of the global evidence, concluding that moderate minimum wage increases have small negative employment effects.

- **Cengiz, Doruk, Arindrajit Dube, Attila Lindner, and Ben Zipperer.** "The Effect of Minimum Wages on Low-Wage Jobs." *Quarterly Journal of Economics* 134, no. 3 (2019): 1405--1454. DOI: [10.1093/qje/qjz014](https://doi.org/10.1093/qje/qjz014). Bunching estimator applied to 138 state-level minimum wage changes; finds clear wage increases with little evidence of employment loss.

### Labour Demand Elasticities

- **Hamermesh, Daniel S.** *Labor Demand*. Princeton University Press, 1993. The definitive survey of the theory and empirics of labour demand. Establishes the consensus own-wage elasticity range of -0.15 to -0.75.

- **Lichter, Andreas, Andreas Peichl, and Sebastian Siegloch.** "The Own-Wage Elasticity of Labor Demand: A Meta-Regression Analysis." *European Economic Review* 80 (2015): 94--119. DOI: [10.1016/j.euroecorev.2015.08.007](https://doi.org/10.1016/j.euroecorev.2015.08.007). Meta-analysis of 942 estimates confirming Hamermesh's range, with long-run elasticities about twice as large as short-run.

---

## Indian Context Readings

- **Soundararajan, Vidhya.** "Heterogeneous Effects of Imperfectly Enforced Minimum Wages in Low-Income Countries." *Journal of Development Economics* 140 (2019): 355--374. DOI: [10.1016/j.jdeveco.2019.06.004](https://doi.org/10.1016/j.jdeveco.2019.06.004). Studies minimum wage effects in India, documenting low compliance in the informal sector and heterogeneous effects by enforcement intensity.

- **Basu, Arnab K., Nancy H. Chau, and Ravi Kanbur.** "Turning a Blind Eye: Costly Enforcement, Credible Commitment and Minimum Wage Laws." *Economic Journal* 120, no. 543 (2010): 244--269. DOI: [10.1111/j.1468-0297.2009.02322.x](https://doi.org/10.1111/j.1468-0297.2009.02322.x). Theoretical model of minimum wage enforcement in developing countries where compliance is endogenous.

- **Rani, Uma, Patrick Belser, Martin Oelz, and Setareh Ranjbar.** "Minimum Wage Coverage and Compliance in Developing Countries." *International Labour Review* 152, no. 3--4 (2013): 381--410. DOI: [10.1111/j.1564-913X.2013.00197.x](https://doi.org/10.1111/j.1564-913X.2013.00197.x). Cross-country evidence on minimum wage compliance, with data from India.

- **Government of India.** *Code on Wages, 2019*. [Link](https://labour.gov.in/code-on-wages). The consolidated legislation replacing the Minimum Wages Act, Payment of Wages Act, Payment of Bonus Act, and Equal Remuneration Act.

---

## Supplementary Readings

- **Hicks, John R.** *The Theory of Wages*. 2nd ed. London: Macmillan, 1963. Classic treatment of the theory of derived demand, including the original statement of what became known as the Hicks-Marshall rules.

- **Manning, Alan.** *Monopsony in Motion: Imperfect Competition in Labor Markets*. Princeton University Press, 2003. Argues that labour markets are better modelled as monopsonistic than perfectly competitive, which helps explain why moderate minimum wage increases may not reduce employment.

---

## Video Resources

- **Marginal Revolution University.** "Demand for Labor" and "Minimum Wage." Short video lectures covering the VMP condition and the minimum wage debate. Available at [mru.org](https://mru.org).

- **CORE Econ.** Unit 8: "Supply and Demand: Price-Taking and Competitive Markets." [core-econ.org](https://www.core-econ.org/the-economy/book/text/08.html). Free textbook chapter covering competitive labour markets and the firm's hiring decision.

---

## Stata Exercises

!!! stata "Computing Labour Demand Elasticities"
    ```stata
    * Load industry-level panel data
    use industry_panel.dta, clear

    * Log-log regression to estimate own-wage elasticity
    gen ln_emp = ln(employment)
    gen ln_wage = ln(avg_wage)
    gen ln_output_price = ln(price_index)

    * Basic OLS estimate (for illustration)
    reg ln_emp ln_wage ln_output_price i.year, cluster(industry)

    * The coefficient on ln_wage is the own-wage elasticity
    * Expect: negative, in the range -0.15 to -0.75
    ```

!!! stata "Simulating Minimum Wage Effects"
    ```stata
    * Generate a simple competitive labour market simulation
    clear
    set obs 100

    * Supply and demand parameters
    gen wage = _n * 0.5
    gen Ld = 1000 - 20 * wage    // Demand
    gen Ls = -200 + 40 * wage    // Supply

    * Find equilibrium
    gen excess = Ls - Ld
    * Equilibrium at wage = 20, employment = 600

    * Plot supply and demand
    twoway (line Ld wage) (line Ls wage), ///
        xline(20, lp(dash)) yline(600, lp(dash)) ///
        legend(label(1 "Demand") label(2 "Supply")) ///
        title("Competitive Labour Market") ///
        xtitle("Wage") ytitle("Employment (000s)")
    ```
