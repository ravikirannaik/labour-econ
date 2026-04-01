---
title: "Stata Resources"
description: "A practical Stata guide for ECON207 Labour Economics students at FLAME University"
---

# Stata for Labour Economics

A practical guide to using Stata for empirical analysis in ECON207. This page covers the essentials you need for the course -- from navigating the interface to running Mincer regressions on Indian labour market data.

---

## Why Stata?

Stata is the industry-standard software for applied microeconometrics and labour economics research. The vast majority of published empirical papers in labour economics -- from Card and Krueger's minimum wage study to Oaxaca-Blinder wage decompositions -- were produced in Stata. Learning Stata is not just a course requirement; it is a transferable skill for any career in economic research, policy analysis, or data-driven consulting.

**Why Stata for this course specifically?**

- **FLAME lab access.** Stata is installed on all Economics Lab machines. You do not need to purchase a personal license (though student licenses are affordable).
- **Reproducibility.** Stata do-files create a permanent record of every step in your analysis, from data cleaning to final tables. This is essential for the group assignments.
- **Ecosystem.** The Stata community has developed thousands of user-written commands for labour economics tasks (decompositions, matching estimators, instrumental variables diagnostics).

!!! stata "Your first command"
    Open Stata, type the following in the Command window, and press Enter:

    ```stata
    display "Hello, Labour Economics!"
    ```

    If you see the output, you are ready to go.

---

## Getting Started: The Stata Interface

When you open Stata, you will see five main areas:

| Panel | Purpose |
|-------|---------|
| **Command window** | Type individual commands here |
| **Results window** | Output from commands appears here |
| **Variables window** | Lists all variables in the current dataset |
| **Properties window** | Shows variable labels, types, and formats |
| **Review window** | History of commands you have run (click to re-run) |

### Command Window vs. Do-File

You can run Stata commands in two ways:

1. **Interactively** -- type commands one at a time in the Command window. Good for exploration.
2. **Via a do-file** -- write a script containing multiple commands, then execute it. **This is what you should use for assignments.**

!!! stata "Creating a do-file"
    Go to **File > New > Do-file** (or press ++ctrl+9++). Write your commands, then click the **Execute (Do)** button or press ++ctrl+d++ to run the entire file. Always begin your do-file with:

    ```stata
    * ECON207 Labour Economics — Assignment X
    * Author: Your Name
    * Date: YYYY-MM-DD
    * -----------------------------------------------

    clear all
    set more off
    cap log close
    log using "assignment_X.log", replace
    ```

    And end with:

    ```stata
    log close
    ```

    This creates a complete record of your work.

---

## Essential Commands by Task

### Data Management

These commands form the backbone of every Stata workflow. You will use them in every assignment.

!!! stata "Loading and inspecting data"

    ```stata
    * Load a Stata dataset
    use "plfs_2024_person.dta", clear

    * Describe variables (names, types, labels)
    describe

    * Quick summary statistics
    summarize age wage hours_worked

    * Detailed summary with percentiles
    summarize wage, detail

    * Frequency table
    tabulate education_level

    * Two-way cross-tabulation
    tabulate gender employment_status
    ```

!!! stata "Creating and modifying variables"

    ```stata
    * Generate a new variable
    gen log_wage = ln(wage)

    * Generate a dummy variable
    gen female = (gender == 2)

    * Generate experience and its square
    gen exper = age - education_years - 6
    gen exper_sq = exper^2

    * Replace values conditionally
    replace sector = "Informal" if contract_type == 0

    * Keep only relevant observations
    keep if age >= 15 & age <= 65

    * Drop variables you do not need
    drop temp_var1 temp_var2

    * Label your variables
    label variable log_wage "Log of monthly wage (Rs.)"
    label variable female "Female (=1)"
    ```

### Descriptive Statistics and Visualisation

Before running regressions, always explore your data visually and numerically.

!!! stata "Summary statistics and tables"

    ```stata
    * Mean wage by gender
    tabstat wage, by(gender) stat(mean sd n)

    * Mean and standard error (useful for reporting)
    mean wage, over(gender)

    * Detailed tabulation with percentages
    tab education_level gender, row col
    ```

!!! stata "Graphs for labour economics"

    ```stata
    * Histogram of log wages
    histogram log_wage, ///
        title("Distribution of Log Wages") ///
        xtitle("Log Monthly Wage") ///
        color(navy%70) ///
        normal

    * Bar chart of LFPR by education and gender
    graph bar (mean) in_labour_force, ///
        over(education_level) over(gender) ///
        title("Labour Force Participation Rate") ///
        ytitle("Proportion in Labour Force") ///
        legend(order(1 "Male" 2 "Female"))

    * Scatter plot with fitted line
    twoway (scatter log_wage exper, msize(tiny) mcolor(navy%30)) ///
           (lfit log_wage exper, lcolor(red) lwidth(medthick)), ///
        title("Experience-Earnings Profile") ///
        xtitle("Years of Experience") ///
        ytitle("Log Wage")

    * Export graphs for your assignment
    graph export "wage_histogram.png", replace width(1200)
    ```

### Regression Analysis

Regression is the workhorse of empirical labour economics. The commands below cover the regressions you will encounter in ECON207.

!!! stata "OLS regression -- the Mincer equation (Ch. 6)"

    ```stata
    * Basic Mincer earnings function
    regress log_wage education_years exper exper_sq

    * With robust standard errors (always use these)
    regress log_wage education_years exper exper_sq, robust

    * Adding controls
    regress log_wage education_years exper exper_sq female urban, robust

    * Interpret: the coefficient on education_years is the
    * approximate rate of return to one additional year of schooling

    * Store results for comparison
    estimates store model1
    ```

!!! stata "Instrumental variables -- addressing ability bias (Ch. 6)"

    ```stata
    * Two-stage least squares (2SLS)
    * Instrument: quarter of birth, distance to college, etc.
    ivregress 2sls log_wage exper exper_sq (education_years = distance_college), robust

    * First-stage diagnostics
    estat firststage

    * Overidentification test (if multiple instruments)
    estat overid
    ```

!!! stata "Oaxaca-Blinder decomposition (Ch. 9)"

    ```stata
    * Install the user-written oaxaca command (one time only)
    ssc install oaxaca

    * Decompose the male-female wage gap
    oaxaca log_wage education_years exper exper_sq urban, ///
        by(female) robust

    * Interpret:
    * "Explained" = portion due to differences in characteristics
    * "Unexplained" = portion due to differences in coefficients
    *   (may reflect discrimination + unobserved factors)
    ```

### Labour-Specific Analyses

These examples connect directly to the topics in each chapter.

!!! stata "Labour force participation tabulations (Ch. 2)"

    ```stata
    * LFPR by age group and gender
    gen age_group = .
    replace age_group = 1 if age >= 15 & age <= 24
    replace age_group = 2 if age >= 25 & age <= 54
    replace age_group = 3 if age >= 55 & age <= 65
    label define age_lbl 1 "15-24" 2 "25-54" 3 "55-65"
    label values age_group age_lbl

    tab age_group in_labour_force if gender == 1 [aw=weight], row
    tab age_group in_labour_force if gender == 2 [aw=weight], row
    ```

!!! stata "Wage equation with compensating differentials (Ch. 5)"

    ```stata
    * Hedonic wage regression
    regress log_wage education_years exper exper_sq ///
        hazardous_job night_shift outdoor_work, robust

    * The coefficient on hazardous_job estimates the
    * compensating differential for risky work
    ```

!!! stata "Unemployment duration analysis (Ch. 11)"

    ```stata
    * Summarise unemployment duration
    summarize unemp_duration if unemployed == 1, detail

    * Kaplan-Meier survival curve (if panel data available)
    * stset unemp_duration, failure(found_job)
    * sts graph, title("Survival in Unemployment")
    ```

---

## Working with PLFS Data in Stata

The Periodic Labour Force Survey (PLFS) is India's primary labour market dataset. For the group assignments, you will use cleaned PLFS microdata in `.dta` format.

!!! stata "Loading PLFS data"

    ```stata
    * Set your working directory
    cd "/path/to/your/data/"

    * Load the person-level file
    use "plfs_2024_person.dta", clear

    * Inspect the dataset
    describe
    summarize
    ```

### Key PLFS Variables

| Variable | Description | Notes |
|----------|-------------|-------|
| `age` | Age in years | Working age: 15+ |
| `sex` | Sex (1=Male, 2=Female) | |
| `sector` | Rural (1) / Urban (2) | |
| `nss_region` | NSS region code | For regional analysis |
| `usual_status` | Usual principal activity status | 11-51 = employed; 81 = unemployed; 91-97 = NILF |
| `current_weekly_status` | CWS activity status | More current measure |
| `nco_2d` | 2-digit NCO occupation code | For occupation-level analysis |
| `nic_2d` | 2-digit NIC industry code | For industry-level analysis |
| `education` | Highest education level | General education categories |
| `wage_salary` | Wage/salary earnings | Available for regular and casual workers |
| `weight` | Sampling weight (multiplier) | **Always use weights for population estimates** |

!!! stata "Weighted estimates"

    ```stata
    * IMPORTANT: Always use sampling weights for population-level statistics

    * Weighted mean
    mean wage_salary [pw=weight]

    * Weighted tabulation
    tab education sex [aw=weight], row

    * Weighted regression
    regress log_wage education_years exper exper_sq [pw=weight], robust
    ```

!!! indian "PLFS Activity Status Codes"
    The PLFS uses a detailed activity classification. The key codes for labour force status are:

    - **11-51**: Employed (self-employed, regular wage, casual)
    - **81**: Unemployed (seeking/available for work)
    - **91-97**: Not in labour force (student, domestic duties, rentier, etc.)

    To construct the labour force dummy:

    ```stata
    gen in_lf = (usual_status >= 11 & usual_status <= 82)
    gen employed = (usual_status >= 11 & usual_status <= 51)
    gen unemployed = (usual_status == 81)
    ```

---

## Tips for Assignments

1. **Always use a do-file.** Never run commands only in the Command window. Your do-file is your submission.
2. **Comment your code generously.** Use `*` for full-line comments and `//` for inline comments.
3. **Use `robust` standard errors** in all regressions unless instructed otherwise.
4. **Always use sampling weights** when computing population-level statistics from PLFS data.
5. **Export tables and graphs** in publication-ready format. Use `esttab` (from the `estout` package) for regression tables and `graph export` for figures.
6. **Reproduce before you extend.** First replicate the textbook result, then add the Indian context.

!!! stata "Installing useful packages"

    ```stata
    * Run these once to install commonly needed commands
    ssc install estout      // For publication-quality tables
    ssc install oaxaca      // Oaxaca-Blinder decomposition
    ssc install coefplot    // Coefficient plots
    ssc install binscatter  // Binned scatter plots
    ```

---

## Recommended Stata Resources

| Resource | Description | Link |
|----------|-------------|------|
| **UCLA OARC Stata Resources** | Comprehensive tutorials, from basics to advanced topics. The best free Stata learning resource. | [UCLA OARC](https://stats.oarc.ucla.edu/stata/) |
| **Stata Documentation** | Official manuals and help files. Type `help commandname` in Stata for built-in documentation. | [Stata Docs](https://www.stata.com/manuals/) |
| **Statalist** | Stata's official user forum. Search before posting; most beginner questions have been answered. | [Statalist](https://www.statalist.org/) |
| **Baum, C.F. (2006)** | *An Introduction to Modern Econometrics Using Stata*. Stata Press. An excellent applied textbook. | [Stata Press](https://www.stata-press.com/) |
| **PLFS Documentation** | NSO methodology reports and questionnaires for PLFS rounds. | [MoSPI](https://www.mospi.gov.in/) |
| **Asjad Naqvi's Stata Guide** | Beautiful, modern Stata visualisation tutorials with code. | [Medium](https://medium.com/the-stata-guide) |

---

## Quick Reference Card

A cheat sheet of the most-used commands for ECON207:

| Task | Command |
|------|---------|
| Load data | `use "file.dta", clear` |
| Summary statistics | `summarize var1 var2, detail` |
| Frequency table | `tabulate var1` |
| Cross-tab | `tabulate var1 var2, row col` |
| New variable | `gen newvar = expression` |
| Conditional replace | `replace var = value if condition` |
| OLS regression | `regress y x1 x2 x3, robust` |
| IV regression | `ivregress 2sls y x1 (x2 = z1), robust` |
| Decomposition | `oaxaca y x1 x2, by(group) robust` |
| Histogram | `histogram var, normal` |
| Scatter plot | `twoway (scatter y x) (lfit y x)` |
| Export table | `esttab using "table.tex", se star(* 0.10 ** 0.05 *** 0.01)` |
| Export graph | `graph export "fig.png", replace width(1200)` |
| Save data | `save "file_clean.dta", replace` |

---

*For questions about Stata, ask during office hours or post on the course discussion forum. The UCLA OARC and Statalist archives can answer most technical questions faster than any individual can.*
