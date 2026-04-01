---
title: "PLFS Data Guide"
---

# Periodic Labour Force Survey (PLFS) -- A Student's Guide

The Periodic Labour Force Survey is India's most important source of labour market statistics. If you want to make any empirical claim about Indian employment, wages, or unemployment, the PLFS is almost certainly the dataset you will turn to first. This guide introduces the survey, explains its core concepts, and helps you read and interpret PLFS annual reports.

---

## What is the PLFS?

The PLFS is a nationwide household survey conducted by the **National Statistical Office (NSO)**, which is part of the Ministry of Statistics and Programme Implementation (MoSPI). It was launched in **2017-18** as a successor to the quinquennial Employment-Unemployment Surveys (EUS) that the NSO had conducted since the 1970s under the National Sample Survey (NSS) framework.

!!! indian "Why the PLFS Matters"
    Before 2017-18, India's official employment data came once every five years (the last EUS was in 2011-12). The PLFS was introduced to provide **annual estimates** of labour force indicators and, for urban areas, **quarterly estimates**. This was a major upgrade in the timeliness of India's labour statistics.

The PLFS follows a **rotational panel design** in urban areas: the urban sample is divided into four panels, each surveyed for four consecutive quarters, with one panel rotating out each quarter. This means 75 per cent of the urban sample is common between two consecutive quarters, allowing for more reliable estimation of quarter-on-quarter changes. The rural sample, by contrast, is surveyed only once during the annual survey period (July to June for earlier rounds; January to December from PLFS 2024 onward).

The survey covers the entire territory of India except a few inaccessible areas in Andaman and Nicobar Islands. Sample sizes are large: the PLFS 2023-24, for instance, covered approximately 1,01,655 households and over 4,00,000 individuals.

---

## Key Concepts: Activity Status

The most important conceptual framework in the PLFS is the classification of individuals by **activity status** -- that is, what they were doing during a specified reference period. The PLFS collects activity status using three different reference periods, each yielding a different picture of the labour market.

### Usual Principal Status (UPS)

- **Reference period:** 365 days preceding the survey date.
- **Definition:** The activity on which a person spent the **major part** (i.e., more than 6 months) of the reference year.
- **Use:** Gives a broad, structural picture of employment. A person is classified as employed, unemployed, or out of the labour force based on what they did for most of the year.

### Usual Principal and Subsidiary Status (UPSS)

- **Reference period:** 365 days preceding the survey date.
- **Definition:** Extends UPS by adding a **subsidiary activity** for persons who were classified as unemployed or out of the labour force under UPS, but who pursued some economic activity for at least 30 days during the reference year.
- **Use:** The **most commonly cited** activity status in PLFS reports. UPSS captures a broader set of workers than UPS alone, because it picks up people whose primary status is non-working but who did some work on the side.

!!! model "Why UPSS Matters for Measurement"
    Consider a woman who spends most of the year on domestic duties but works on the family farm for two months during the harvest season. Under UPS, she is classified as "not in the labour force." Under UPSS, she is classified as **employed** (subsidiary status). This distinction is crucial for understanding female LFPR in India, where a large share of women's work is seasonal or part-time.

### Current Weekly Status (CWS)

- **Reference period:** 7 days preceding the survey date.
- **Definition:** A person is classified as employed if they pursued any economic activity for **at least one hour on any day** during the reference week.
- **Use:** Provides a shorter-term snapshot. CWS estimates of unemployment are typically higher than UPSS estimates, because they capture people who may be employed for most of the year but happen to be without work in the reference week.

### Current Daily Status (CDS)

- **Reference period:** Each day of the 7 days preceding the survey date.
- **Definition:** Activity status is determined for each day of the reference week (each day assigned one of two "half-day" slots). A person-day is the unit of measurement.
- **Use:** Gives the most granular picture and captures **underemployment** effectively. CDS unemployment rates are the highest among the three measures because they pick up even partial-week idleness.

!!! empirical "Comparing the Three Measures (PLFS 2023-24)"
    | Measure | Unemployment Rate |
    |---------|:-----------------:|
    | UPSS    | ~3.2%             |
    | CWS     | ~4.1%             |
    | CDS     | ~5.0%             |

    The gap between these rates reflects the extent of intermittent and seasonal unemployment that UPSS smooths over. When reading PLFS reports, always check which definition is being used -- headlines citing different activity statuses can paint very different pictures of the same labour market.

---

## Core Labour Market Indicators

The PLFS reports several key indicators. Here are the definitions you need:

**Labour Force Participation Rate (LFPR):** The proportion of the population (aged 15 years and above) that is either employed or unemployed (i.e., seeking or available for work).

\[
\text{LFPR} = \frac{\text{Labour Force (Employed + Unemployed)}}{\text{Population aged 15+}} \times 100
\]

**Worker Population Ratio (WPR):** The proportion of the population (aged 15+) that is employed.

\[
\text{WPR} = \frac{\text{Employed}}{\text{Population aged 15+}} \times 100
\]

**Unemployment Rate (UR):** The proportion of the labour force that is unemployed.

\[
\text{UR} = \frac{\text{Unemployed}}{\text{Labour Force}} \times 100
\]

Note that the PLFS often reports these for persons aged 15 and above as well as for all ages (including children aged 5-14, for subsidiary activities). The standard international practice -- and what you should use in your assignments -- is the 15+ definition.

---

## Key Variables and Codes

When working with PLFS unit-level data, you will encounter the following important variables:

| Variable | Description | Key Codes |
|----------|-------------|-----------|
| **NIC** (National Industrial Classification) | Industry of employment | 2-digit and 5-digit codes per NIC-2008 |
| **NCO** (National Classification of Occupations) | Occupation | 2-digit and 3-digit codes per NCO-2004 |
| **Status Code** | Activity status | 11-51 = employed; 81 = unemployed (sought); 91-98 = not in labour force |
| **Type of Enterprise** | Formal/informal sector proxy | Proprietary, partnership, employer categories |
| **Social Group** | Caste category | ST = 1, SC = 2, OBC = 3, Others = 9 |
| **Wage/Earnings** | Weekly earnings for CWS | Reported in rupees for regular/casual workers |
| **Education Level** | Highest completed level | Coded 01 (not literate) through 13 (postgraduate and above) |

!!! stata "Working with PLFS Microdata"
    PLFS unit-level data can be downloaded from the MoSPI website after registration. The data arrives as fixed-width text files (.TXT) with separate record layouts for household and person records. You will need to apply the NSO's provided layout to read these into Stata or Python. Sample Stata workflow:

    ```stata
    * Read person-level records using NSO layout
    infix using plfs_person_layout.dct, using(plfs_person.txt)
    * Generate employment dummy
    gen employed = inrange(status_code, 11, 51)
    * Compute LFPR
    gen in_lf = inrange(status_code, 11, 82)
    ```

---

## How to Read PLFS Annual Reports

The NSO publishes annual PLFS reports (typically with a lag of about one year). Here is a roadmap for navigating them:

1. **Executive Summary (first few pages):** Key headline indicators -- LFPR, WPR, UR -- by UPSS and CWS, separately for rural/urban and male/female.

2. **Statement Tables:** Numbered tables (e.g., Statement 4, Statement 5) are the main data source. These provide cross-tabulations by state, age group, education level, social group, industry, and occupation. Learn to cite these by Statement number.

3. **Appendix Tables:** More detailed breakdowns, often by individual states.

4. **Methodology Section:** Explains sample design, weighting procedures, and response rates. Always check this when doing research, because PLFS has changed its reference period (from July-June to January-December starting in 2024), and comparability across rounds requires care.

!!! policy "Watch for Breaks in Series"
    The PLFS underwent a significant methodological change in 2024, shifting from a July-June survey period to a **January-December** calendar year. This means direct comparisons between PLFS 2022-23 and PLFS 2024 require caution. Additionally, the COVID year (2020-21) had a truncated survey period due to lockdowns. Always flag these breaks when presenting time-series data.

---

## Limitations and Caveats

No survey is perfect, and the PLFS has several known limitations that you should keep in mind:

- **Undercounting of women's work:** Despite improvements over the old EUS, the PLFS still relies on a single household informant in many cases, and domestic/care work is systematically undercounted. The UPSS activity-status approach has been criticised for missing the episodic and part-time nature of much of women's employment.

- **No income data for self-employed:** The PLFS collects **earnings data only for regular wage/salaried and casual workers**. The roughly 55 per cent of workers who are self-employed do not report earnings in the PLFS. This is a major limitation for wage analysis.

- **Urban bias in quarterly estimates:** Quarterly bulletins cover only urban areas, so short-term trends in rural labour markets are invisible between annual rounds.

- **Panel attrition:** The rotational panel in urban areas suffers from attrition, particularly among migrants and mobile populations -- precisely the groups of most interest for studying labour market dynamics.

- **Comparability with NSS-EUS:** Although the PLFS uses the same conceptual framework as the old EUS rounds, differences in questionnaire design, sample design, and reference periods mean that pre-2017 and post-2017 series are not directly comparable without adjustments.

---

## Useful Links

- **PLFS Annual Reports:** [MoSPI PLFS page](https://mospi.gov.in/publication/plfs-annual-report) -- official annual reports and quarterly bulletins.
- **Unit-Level Data:** Available through the MoSPI microdata portal after free registration.
- **NSO Documentation:** Concepts and definitions aligned with ILO standards are described in the NSO's *Sources and Methods* volume.
- **ILO ILOSTAT:** [ilostat.ilo.org](https://ilostat.ilo.org/) -- for cross-country comparisons using harmonised definitions.

---

!!! indian "Bottom Line for Students"
    The PLFS is your go-to source for Indian labour market data. When you cite an employment or unemployment figure for India, always specify: (1) the **PLFS round** (e.g., 2023-24), (2) the **activity status** (UPSS, CWS, or CDS), (3) the **age group** (15+ or all ages), and (4) whether the figure is for **rural, urban, or all-India**. Failing to specify these will make your analysis ambiguous.

---

*This guide is based on PLFS reports and methodology documents published by MoSPI/NSO. For the latest data, always consult the official MoSPI website.*
