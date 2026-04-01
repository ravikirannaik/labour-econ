---
title: "Resources — Labor Market Discrimination"
---

# Resources: Labor Market Discrimination

---

## Required Reading

- **Borjas, George J.** *Labor Economics*, 8th edition, Chapter 9: "Labor Market Discrimination." McGraw-Hill, 2020.

---

## Key Academic Papers

### Foundational Theory

- **Becker, Gary S.** *The Economics of Discrimination*. University of Chicago Press, 1957.
    - The foundational treatment of taste-based discrimination. Introduces the discrimination coefficient and shows that prejudice is costly to discriminating employers.

- **Phelps, Edmund S.** "The Statistical Theory of Racism and Sexism." *American Economic Review* 62(4): 659--661, 1972.
    - Introduces statistical discrimination: employers use group membership as a proxy for unobserved productivity when individual signals are noisy.

- **Arrow, Kenneth J.** "The Theory of Discrimination." In *Discrimination in Labor Markets*, edited by Orley Ashenfelter and Albert Rees, 3--33. Princeton University Press, 1973.
    - Extends statistical discrimination to show how employer beliefs can be self-fulfilling, creating stable discriminatory equilibria.

### Measurement: Decomposition Methods

- **Oaxaca, Ronald.** "Male-Female Wage Differentials in Urban Labor Markets." *International Economic Review* 14(3): 693--709, 1973.
    - Develops the canonical decomposition of wage gaps into explained (endowment) and unexplained (coefficient) components.

- **Blinder, Alan S.** "Wage Discrimination: Reduced Form and Structural Estimates." *Journal of Human Resources* 8(4): 436--455, 1973.
    - Independently develops the same decomposition technique as Oaxaca, now known as the Oaxaca-Blinder method.

### Experimental Evidence: Audit and Correspondence Studies

- **Bertrand, Marianne, and Sendhil Mullainathan.** "Are Emily and Greg More Employable Than Lakisha and Jamal? A Field Experiment on Labor Market Discrimination." *American Economic Review* 94(4): 991--1013, 2004. [DOI: 10.1257/0002828042002561](https://doi.org/10.1257/0002828042002561)
    - Landmark correspondence study. White-sounding names receive 50% more callbacks. Higher resume quality helps white names more than Black names.

- **Neumark, David.** "Detecting Discrimination in Audit and Correspondence Studies." *Journal of Human Resources* 47(4): 1128--1157, 2012. [DOI: 10.3368/jhr.47.4.1128](https://doi.org/10.3368/jhr.47.4.1128)
    - Methodological analysis of audit study designs, discussing inference challenges and best practices.

- **Agan, Amanda, and Sonja Starr.** "Ban the Box, Criminal Records, and Racial Discrimination: A Field Experiment." *Quarterly Journal of Economics* 133(1): 191--235, 2018. [DOI: 10.1093/qje/qjx028](https://doi.org/10.1093/qje/qjx028)
    - Shows that Ban the Box policies increased racial discrimination in callbacks --- an example of statistical discrimination intensifying when individual signals are removed.

### Returns to Reducing Discrimination

- **Hsieh, Chang-Tai, Erik Hurst, Charles I. Jones, and Peter J. Klenow.** "The Allocation of Talent and U.S. Economic Growth." *Econometrica* 87(5): 1439--1474, 2019. [DOI: 10.3982/ECTA11427](https://doi.org/10.3982/ECTA11427)
    - Estimates that declining discrimination against women and Black Americans accounts for 20--40% of per-capita GDP growth between 1960 and 2010.

- **Altonji, Joseph G., and Rebecca M. Blank.** "Race and Gender in the Labor Market." In *Handbook of Labor Economics*, Vol. 3C, edited by Orley Ashenfelter and David Card, 3143--3259. Elsevier, 1999.
    - Comprehensive survey of evidence on racial and gender wage gaps, discrimination, and policy interventions.

---

## Indian Context

### Caste Discrimination

- **Thorat, Sukhadeo, and Paul Attewell.** "The Legacy of Social Exclusion: A Correspondence Study of Job Discrimination in India." *Economic and Political Weekly* 42(41): 4141--4145, 2007.
    - First correspondence study of caste discrimination in Indian private-sector hiring. Dalit and Muslim applicants receive significantly fewer callbacks.

- **Madheswaran, S., and Paul Attewell.** "Caste Discrimination in the Indian Urban Labour Market: Evidence from the National Sample Survey." *Economic and Political Weekly* 42(41): 4146--4153, 2007.
    - Uses Oaxaca-Blinder decomposition on NSS data to estimate the caste wage gap. Finds a substantial unexplained component attributable to discrimination.

- **Banerjee, Abhijit, Marianne Bertrand, Saugato Datta, and Sendhil Mullainathan.** "Labor Market Discrimination in Delhi: Evidence from a Field Experiment." *Journal of Comparative Economics* 37(1): 14--27, 2009. [DOI: 10.1016/j.jce.2008.09.002](https://doi.org/10.1016/j.jce.2008.09.002)
    - Correspondence study in Delhi examining caste and religion discrimination in hiring for call-centre and software jobs.

- **Deshpande, Ashwini.** *Affirmative Action in India*. Oxford University Press, 2013.
    - Comprehensive analysis of India's reservation policy, its effects on labour market outcomes for SC/ST, and the debate over extending reservations to the private sector.

### Gender Discrimination

- **Deshpande, Ashwini, and Deepti Goel.** "Who Gets a Job in India? The Role of Caste, Religion, and Gender." Working Paper, 2015.
    - Analyses intersections of caste, religion, and gender in determining employment access using NSS data.

### Reservation Policy

- **Bertrand, Marianne, Rema Hanna, and Sendhil Mullainathan.** "Affirmative Action in Education: Evidence from Engineering College Admissions in India." *Journal of Public Economics* 94(1--2): 16--29, 2010. [DOI: 10.1016/j.jpubeco.2009.11.003](https://doi.org/10.1016/j.jpubeco.2009.11.003)
    - Evaluates the effects of caste-based reservations in Indian engineering colleges on admission and labour market outcomes.

---

## Data Sources

| Source | Coverage | Key Variables |
|--------|----------|---------------|
| **PLFS** (Periodic Labour Force Survey) | Annual, all-India | Wages, caste (SC/ST/OBC), gender, education, occupation |
| **NSS Employment-Unemployment Rounds** | Quinquennial (historical) | Detailed wage and employment data by social group |
| **IHDS** (India Human Development Survey) | Panel, 2005 & 2012 | Caste, discrimination experience, household income |
| **CPS** (Current Population Survey, US) | Monthly, US | Race, gender, education, earnings |
| **EEOC Data** (US) | Annual | Employer-level data on workforce composition by race and gender |

---

## Videos and Lectures

- **Marginal Revolution University:** [Discrimination and Labor Markets](https://mru.org) --- Short videos on Becker's model and statistical discrimination.
- **NBER Lecture:** Kerwin Charles, "Prejudice and Wages" --- Survey of empirical evidence on discrimination.

---

## Stata Exercises

!!! stata "Oaxaca-Blinder Decomposition in Stata"
    Stata provides a dedicated command for the Oaxaca-Blinder decomposition:

    ```stata
    * Install the oaxaca package if needed
    ssc install oaxaca

    * Basic decomposition: male-female wage gap
    oaxaca lnwage educ exper tenure, by(female) weight(1)

    * Option weight(1) uses Group 1 (male) coefficients as reference
    * weight(2) uses Group 2 (female) coefficients
    * weight(0) uses pooled coefficients (Neumark approach)

    * Detailed decomposition showing each variable's contribution
    oaxaca lnwage educ exper tenure i.occupation, by(female) detail

    * For caste-based decomposition using PLFS:
    oaxaca lnwage educ exper i.industry i.state, by(sc_st) weight(1)
    ```

!!! stata "Testing for Discrimination with Regression"
    ```stata
    * Basic Mincer regression with group indicator
    reg lnwage educ exper exper2 female
    * Coefficient on 'female' = adjusted gender gap

    * Interaction terms to test differential returns
    reg lnwage c.educ##female c.exper##female c.exper2##female

    * Chow test for structural break by group
    reg lnwage educ exper exper2 if female == 0
    estimates store male
    reg lnwage educ exper exper2 if female == 1
    estimates store female
    suest male female
    test [male_mean]educ = [female_mean]educ
    ```
