---
title: "Chapter 6: Education"
description: "Human capital theory, the Mincer earnings equation, ability bias and causal identification, the signalling model, general vs. specific training, and the college wage premium."
---

# 6. Education

> *"The most valuable of all capital is that invested in human beings."*
> --- Alfred Marshall, *Principles of Economics* (1890).

Why do workers with more education earn higher wages? Is it because schooling makes them more productive, or because a degree signals pre-existing ability to employers? This chapter develops the human capital model of education as an investment, derives the Mincer earnings equation, confronts the identification challenge of ability bias, and contrasts the human capital and signalling interpretations of the education-wage relationship. We then turn to firm-level training decisions --- who pays for general versus specific training --- and the age-earnings profiles that on-the-job training generates. Finally, we examine the dramatic rise in the college wage premium and what it means for India's expanding but quality-challenged higher education system.

Education is the single most studied topic in labour economics. Getting the answer right matters enormously --- for individuals deciding how long to stay in school, for governments allocating education budgets, and for understanding the sources of wage inequality.

---

## Education as an Investment: The Becker Model

Gary Becker's (1964) insight was to treat the decision to acquire education in exactly the same way as a firm's decision to invest in physical capital. Education is costly today but yields returns in the future through higher wages. A rational individual will invest in schooling as long as the expected benefits exceed the costs.

### Costs of Education

The full cost of an additional year of schooling has two components:

1. **Direct costs:** Tuition, fees, books, and supplies.
2. **Opportunity costs:** Foregone earnings --- the wages the student would have earned had she entered the labour market instead of attending school. For most students, opportunity costs are the **larger** component.

This point is frequently underappreciated. A student at a tuition-free public university still bears a large cost of attendance because she is giving up a year's wages. Opportunity costs explain why enrolment is sensitive to local labour market conditions: when unskilled wages are high (say, during a construction boom), the cost of staying in school rises, and some students drop out.

### The Present Value Framework

!!! model "The Schooling Decision: Present Value Calculation"

    Consider a worker choosing between two paths:

    - **No college:** Enter the labour market at age 18, earn \(w_H\) per year for 47 years (until age 65).
    - **College:** Attend college for 4 years (ages 18--21), paying direct costs \(C\) per year and earning nothing, then earn \(w_C\) per year for 43 years (ages 22--65).

    The worker attends college if the present value of the college path exceeds the present value of the no-college path:

    \[
    \sum_{t=1}^{4} \frac{-C}{(1+r)^t} + \sum_{t=5}^{47} \frac{w_C}{(1+r)^t} > \sum_{t=1}^{47} \frac{w_H}{(1+r)^t}
    \]

    Rearranging, college is worthwhile if:

    \[
    \underbrace{\sum_{t=5}^{47} \frac{w_C - w_H}{(1+r)^t}}_{\text{PV of wage gain}} > \underbrace{\sum_{t=1}^{4} \frac{w_H + C}{(1+r)^t}}_{\text{PV of total cost}}
    \]

    The **left side** is the present value of the lifetime wage gain from college. The **right side** is the total cost: four years of foregone earnings plus four years of tuition. The discount rate \(r\) represents the individual's time preference or the interest rate at which she can borrow.

### Who Goes to College? Key Predictions

The human capital model generates several testable predictions about who invests in education:

| Factor | Effect on College Attendance | Reasoning |
|--------|------------------------------|-----------|
| Higher college wage premium (\(w_C - w_H\)) | Increases | Benefits rise |
| Higher direct costs (\(C\)) | Decreases | Costs rise |
| Higher interest rate (\(r\)) | Decreases | Future benefits discounted more heavily |
| Longer time horizon (younger age) | Increases | More years to recoup investment |
| Higher ability | Increases (if ability raises the return to schooling) | Higher \(w_C\) relative to \(w_H\) |
| Credit constraints | Decreases | Effectively raises \(r\) for constrained students |

The prediction about interest rates is particularly important. Students from poor families who cannot borrow easily face a high effective discount rate. Even if the college premium is large, they may not invest in education because they cannot finance it. This provides an efficiency rationale for student loans and education subsidies: **credit constraints cause underinvestment in human capital**.

### The Stopping Rule

!!! model "The Marginal Rate of Return and the Stopping Rule"

    The present value framework can be generalised to a continuous schooling decision. Define the **marginal rate of return** \(\text{MRR}(s)\) as the internal rate of return to the \(s\)-th year of schooling. The MRR declines with schooling (diminishing returns): the first few years of primary school have enormous returns; the marginal year of a second PhD has very little.

    The optimal stopping rule is:

    \[
    \text{MRR}(s^*) = r
    \]

    A worker acquires education up to the point where the marginal rate of return equals her discount rate. Beyond this point, the next year of schooling costs more (in foregone earnings and time preference) than it returns.

    **Comparative statics:**

    - Workers with a **lower discount rate** (patient, not credit-constrained) acquire more schooling: their \(r\) is low, so they stop later.
    - Workers facing a **higher marginal return schedule** (high ability, better schools) also acquire more schooling: their MRR curve is higher, so it intersects \(r\) at a higher \(s^*\).

This framework explains why we observe a distribution of education levels across the population. People differ in both their discount rates (patience, access to credit) and their ability (which shifts the MRR schedule). The human capital model predicts that both factors matter, and the empirical evidence strongly supports this.

---

## The Mincer Earnings Function

Jacob Mincer (1974) derived an empirical specification that has become the workhorse of the field. The **Mincer equation** relates the log of earnings to years of schooling and labour market experience:

!!! model "The Mincer Earnings Equation"

    \[
    \ln w_i = \alpha + \beta s_i + \gamma_1 x_i + \gamma_2 x_i^2 + \varepsilon_i
    \]

    where:

    - \(w_i\) = earnings of individual \(i\)
    - \(s_i\) = years of schooling
    - \(x_i\) = years of labour market experience (typically approximated as \(\text{age} - s - 6\))
    - \(\varepsilon_i\) = error term

    **Interpretation of coefficients:**

    - \(\beta\) = the **rate of return to schooling** --- an additional year of schooling is associated with approximately a \(100\beta\)% increase in wages. A typical estimate is \(\beta \approx 0.06\text{--}0.10\), meaning each year of schooling raises wages by 6--10%.
    - \(\gamma_1 > 0\): earnings increase with experience (on-the-job learning, accumulation of firm-specific skills).
    - \(\gamma_2 < 0\): earnings increase at a **decreasing rate** --- the experience-earnings profile is concave. Learning slows with age, and skills depreciate, so the marginal return to an additional year of experience diminishes.

### Why Log Wages?

The log specification is not arbitrary --- it is derived from the human capital model itself. If each year of schooling raises productivity by a constant *percentage* (not a constant *amount*), then the earnings function is exponential in schooling:

\[
w = e^{\alpha + \beta s + \gamma_1 x + \gamma_2 x^2}
\]

Taking natural logs yields the linear Mincer equation. The log form also has the practical advantage that the coefficient \(\beta\) can be read directly as an approximate percentage change: if \(\beta = 0.08\), one more year of schooling is associated with approximately an 8% wage increase.

### What the Mincer Equation Does Not Tell Us

It is essential to recognise the limitations:

1. The Mincer return is an **average** across all individuals. Returns vary substantially by field of study, institution quality, and individual ability.
2. The equation assumes a **linear** return to schooling. In practice, the return may differ between primary, secondary, and tertiary levels.
3. The experience variable \(x = \text{age} - s - 6\) is a crude proxy. It assumes continuous employment from school-leaving to the present, which is particularly problematic for women who may have career interruptions.

!!! empirical "Global Estimates of the Return to Schooling"

    The Mincer equation has been estimated thousands of times across countries and time periods:

    - **United States:** OLS estimates typically yield \(\beta \approx 0.08\text{--}0.12\) in recent decades, implying an 8--12% wage increase per year of schooling.
    - **OECD average:** About 8--10% per year of schooling.
    - **Developing countries:** Returns tend to be **higher**, particularly for primary education (12--15%) and for women. Psacharopoulos and Patrinos (2018) document a global average return of about 9%.
    - **Trend:** Returns to schooling in the US have **increased** since the 1980s, driven by skill-biased technological change raising the demand for educated workers.
    - **By level:** Returns to primary education are highest in low-income countries; returns to tertiary education are highest in middle- and high-income countries.

---

## The Identification Problem: Ability Bias

The Mincer equation provides a **correlation** between schooling and wages, but does it identify the **causal effect** of education? The central concern is **ability bias** --- perhaps the most important identification problem in all of labour economics.

### The Problem

Suppose that individuals with higher innate ability (intelligence, motivation, conscientiousness) both (a) acquire more schooling and (b) earn higher wages regardless of their education level. Then schooling \(s_i\) is correlated with the error term \(\varepsilon_i\), and OLS is biased:

\[
\ln w_i = \alpha + \beta s_i + \underbrace{\gamma_1 x_i + \gamma_2 x_i^2}_{\text{controls}} + \underbrace{(a_i + u_i)}_{\varepsilon_i}
\]

If ability \(a_i\) is unobserved and \(\text{Cov}(s_i, a_i) > 0\) --- more able workers get more schooling --- then OLS overstates the causal return to education. Part of what we attribute to schooling actually reflects ability.

!!! model "Direction of Ability Bias"

    Decompose the OLS estimator:

    \[
    \hat{\beta}_{\text{OLS}} = \beta + \underbrace{\frac{\text{Cov}(s_i, a_i)}{\text{Var}(s_i)}}_{\text{ability bias} > 0}
    \]

    Since \(\text{Cov}(s_i, a_i) > 0\), we expect \(\hat{\beta}_{\text{OLS}} > \beta\). The OLS return to schooling is **upward biased**.

    However, the direction is actually ambiguous. There is a countervailing **discount rate bias**: if workers who face high borrowing costs (and thus invest less in schooling) actually have **high** marginal returns to education, then OLS may understate the return for these individuals. The net direction depends on which bias dominates.

---

## Empirical Strategies for Causal Identification

Labour economists have developed several ingenious strategies to address ability bias:

### 1. Twins Studies

Identical (monozygotic) twins share the same genes and family background. If one twin obtains more education than the other, comparing their wages identifies the return to schooling net of genetic ability:

\[
\ln w_{1} - \ln w_{2} = \beta (s_1 - s_2) + (u_1 - u_2)
\]

Since the genetic component \(a\) is identical for both twins, it differences out. Ashenfelter and Krueger (1994), using data from the Twinsburg Twins Festival in Ohio, find returns of about 8--10%, remarkably similar to OLS estimates. Ashenfelter and Rouse (1998) confirm this finding with improved measurement. The implication: **ability bias is small** in the standard Mincer regression.

A limitation of twins studies is that within-twin differences in schooling may be driven by measurement error (inflating the coefficient) or by non-genetic factors correlated with earnings (leaving some bias). Nonetheless, the consistency of estimates across multiple twins datasets is reassuring.

### 2. Instrumental Variables: Compulsory Schooling Laws

Angrist and Krueger (1991) exploit the interaction between compulsory schooling laws and quarter of birth as an instrumental variable. In the US, students born in the first quarter of the year reach the minimum school-leaving age earlier in the academic year and can legally drop out with less education. Quarter of birth thus creates **exogenous variation** in schooling that is plausibly unrelated to ability.

!!! empirical "Angrist and Krueger (1991): Quarter-of-Birth IV"

    **Instrument:** Quarter of birth interacted with compulsory schooling age.

    **First stage:** Students born in Q1 have approximately 0.1 fewer years of education than those born in Q4.

    **Second stage:** Using quarter of birth as an instrument for schooling, the IV estimate of the return to education is approximately **7--8%** per year.

    **Two IV conditions:**

    1. **Relevance:** Quarter of birth affects years of schooling. (Verified: F-statistic is significant, though the instrument is weak --- a concern raised by Bound, Jaeger, and Baker 1995.)
    2. **Exogeneity (exclusion restriction):** Quarter of birth affects wages **only** through its effect on schooling. Plausible, since birth timing is largely random --- though seasonal patterns in births by socioeconomic status have been noted.

    **Implication:** The IV estimate is close to OLS, again suggesting that ability bias is modest.

### 3. Regression Discontinuity Designs

Researchers have exploited sharp discontinuities in access to education --- such as admission cutoffs for selective schools or changes in compulsory schooling laws --- to estimate causal returns. Students just above and just below a cutoff are nearly identical in ability but differ in the education they receive, providing a quasi-experimental estimate.

Oreopoulos (2006) exploits changes in compulsory schooling laws across US states and Canadian provinces and finds large returns on the order of 10--14% per year for the marginal student compelled to stay in school.

!!! empirical "Card (1999): Summary of Causal Estimates"

    David Card's influential *Handbook of Labor Economics* survey reviews dozens of IV and natural experiment studies. His key findings:

    - IV estimates of the return to schooling are **at least as large as OLS** estimates, typically 8--14%.
    - This implies that ability bias in OLS is small, or that there is a countervailing discount rate bias. Individuals who face high borrowing costs (and thus invest less in schooling) actually have **high** marginal returns to education --- they are the "marginal students" whose education is affected by instruments like compulsory schooling laws.
    - The **causal return** to schooling is substantial and robust across identification strategies. Education genuinely makes workers more productive.

---

## The Signalling Model: Education as a Signal

An entirely different interpretation of the education-earnings correlation comes from Michael Spence's (1973) signalling model. In this view, education may not make workers more productive at all --- instead, it serves as a **signal** of pre-existing ability to employers who cannot directly observe productivity.

### The Setup

- Workers differ in ability: high-ability (\(H\)) and low-ability (\(L\)), with productivities \(w_H > w_L\).
- Employers cannot observe ability directly but can observe educational attainment.
- Education is **costly**, and crucially, it is **more costly** for low-ability workers: they find coursework harder, take longer to complete, and are more likely to drop out. The cost per year of education is \(c_L > c_H\).

### The Separating Equilibrium

If the cost difference between types is large enough, a **separating equilibrium** emerges in which education perfectly reveals type:

!!! model "Spence Signalling Equilibrium"

    A separating equilibrium exists with an education threshold \(s^*\) such that:

    - High-ability workers acquire \(s \geq s^*\) years and are paid \(w_H\).
    - Low-ability workers acquire \(s < s^*\) years and are paid \(w_L\).

    For the equilibrium to be self-enforcing, two incentive compatibility conditions must hold:

    \[
    w_H - w_L > c_H \cdot s^* \quad \text{(H-types find it worthwhile to signal)}
    \]

    \[
    w_H - w_L < c_L \cdot s^* \quad \text{(L-types find it too costly to mimic)}
    \]

    Combining these inequalities:

    \[
    \frac{w_H - w_L}{c_L} < s^* < \frac{w_H - w_L}{c_H}
    \]

    Any \(s^*\) in this range supports a separating equilibrium. Notice that there are **multiple equilibria** --- the model does not pin down a unique education level. This is an important theoretical limitation.

### The Sheepskin Effect: Evidence for Signalling

The **sheepskin effect** is the observation that wages jump **discontinuously** upon completion of a credential (degree, diploma), over and above the smooth return to additional years of schooling. For example, completing the fourth year of college and receiving the bachelor's degree confers a larger wage increase than completing the third year without a degree.

- Under **human capital theory**, each year of schooling adds roughly the same productivity. There should be no discontinuous jump at degree completion.
- Under **signalling theory**, the credential (not the coursework) is what employers observe. Completing 15 years without a degree is less valuable than 16 years with one.

Empirical studies (Hungerford and Solon 1987, Jaeger and Page 1996) find statistically significant sheepskin effects, particularly at 12 years (high school diploma) and 16 years (bachelor's degree). This provides evidence that signalling plays **some** role. However, the sheepskin effect accounts for only a modest fraction of the total return to education, suggesting that human capital accumulation remains the dominant channel.

### Human Capital vs. Signalling: Why It Matters

| Feature | Human Capital | Signalling |
|---------|--------------|------------|
| **Mechanism** | Education increases productivity | Education reveals pre-existing productivity |
| **Social return** | Private return \(\leq\) Social return (positive externalities) | Private return \(>\) Social return (zero-sum sorting) |
| **Policy implication** | Subsidise education (productive investment) | Education subsidies are wasteful (credential arms race) |
| **Prediction for degree holders** | Smooth return per year | Discontinuous jump at credential |

!!! policy "Policy Implications of the Signalling Model"

    If signalling is the dominant mechanism, then education subsidies are socially wasteful --- they encourage a costly arms race in credentials without increasing aggregate productivity. Workers would spend more years (and more money) in school simply to maintain their relative position.

    If human capital is dominant, education subsidies are efficient because they correct for credit constraints and positive externalities (educated workers generate spillovers --- better health outcomes, civic participation, knowledge diffusion).

    In practice, education serves **both** functions. The challenge for policymakers is to invest in the kinds of education that genuinely build skills (vocational training, quality primary education, STEM instruction) rather than simply extending credentialing requirements.

---

## General vs. Specific Training

Becker (1964) extended the human capital framework beyond formal schooling to **on-the-job training (OJT)**, distinguishing between two types:

### General Training

**General training** raises a worker's productivity at all firms equally. Examples: literacy, numeracy, programming in a widely used language, spoken English. Because general skills are portable, a trained worker can command a higher wage at any firm.

!!! model "Who Pays for General Training?"

    Becker's key prediction: **workers pay** for general training, not firms.

    The logic is simple. If Firm A pays for general training, the worker becomes more productive at all firms. Firm B can now poach the worker by offering a slightly higher wage. Competition among firms bids the trained worker's wage up to her new (higher) marginal product, leaving Firm A unable to recoup its training investment.

    Anticipating this, firms will not pay for general training in a competitive market. Instead, workers accept lower wages during the training period --- effectively paying for training through foregone earnings. After training, their wages rise to match their higher productivity.

    Implication: **apprenticeships** involve low wages during training (the worker is paying) and higher wages afterward (the worker reaps the return).

### Specific Training

**Specific training** raises a worker's productivity only at the current firm. Examples: learning the firm's proprietary software system, understanding the internal reporting hierarchy, building relationships with the firm's specific clients. These skills have zero value if the worker moves to a different firm.

!!! model "Who Pays for Specific Training?"

    Specific training creates a **bilateral monopoly** --- the trained worker is more productive at this firm than anywhere else, and the firm cannot easily replace the worker's firm-specific knowledge.

    Becker's prediction: the **costs and returns are shared** between the firm and the worker.

    - The firm pays part of the training cost (by paying the worker above her initial productivity during training).
    - The worker pays part (by accepting a wage below her post-training productivity at this firm).
    - After training, the worker earns a wage \(w\) that satisfies: \(w_{\text{alternative}} < w < \text{VMP}_{\text{this firm}}\).

    This sharing arrangement makes the match **durable** --- neither side wants to terminate it. The worker would earn less elsewhere; the firm would lose the investment in training.

### Wage-Tenure Profiles

The general/specific distinction explains why **wages rise with tenure** (years at the current firm). Workers who have accumulated specific training are paid a premium above their outside option, and this premium grows with the amount of specific capital accumulated. Long-tenured workers earn more not only because of experience (general human capital) but because of the firm-specific skills they have built.

---

## On-the-Job Training and Age-Earnings Profiles

### Why the Profile Is Concave

The Mincer equation's quadratic experience term (\(\gamma_2 < 0\)) generates a **concave** age-earnings profile: wages rise steeply early in the career, then flatten, and may decline slightly near retirement.

The human capital model explains this shape through the lens of OJT:

1. **Young workers invest heavily** in training because they have a long horizon over which to recoup the returns. They accept lower current wages in exchange for faster wage growth.
2. **As workers age**, the remaining working life shortens, reducing the return to new training. Workers invest less in skill acquisition and more in utilising existing skills.
3. **Near retirement**, depreciation of human capital may outpace new investment, causing a slight earnings decline.

!!! model "The Ben-Porath Model"

    Yoram Ben-Porath (1967) formalised this lifecycle investment logic. In his model, individuals allocate time between producing output and producing human capital. The key insight: because the return to human capital investment depends on the remaining working life, **investment is front-loaded**. Young workers devote a large fraction of their time to learning (low earnings, high growth); older workers devote most of their time to production (high earnings, low growth).

    This explains the stylised fact that age-earnings profiles are steeper for more educated workers --- they invest more in OJT as well, because their higher human capital raises the return to further investment.

### Why Training Declines with Age

The human capital model predicts that **training investment declines monotonically with age**. An older worker has fewer remaining years to benefit from new skills, so the present value of any training investment is lower. This explains:

- Why firms are less likely to send older workers to training programmes
- Why retraining displaced older workers is difficult and often yields modest returns
- Why mandatory retirement, where it exists, is sometimes efficient from the firm's perspective

---

## The College Wage Premium

The **college wage premium** --- the percentage by which college graduates' wages exceed high school graduates' wages --- is one of the most closely watched indicators in labour economics.

!!! empirical "Trends in the US College Wage Premium"

    - **1980:** The college premium was roughly 40--50%.
    - **2000:** It had risen to approximately 80%.
    - **2020s:** It has remained at or above 80%, with some evidence of further increases for advanced degrees (master's, professional).
    - **Goldin and Katz (2008):** In *The Race Between Education and Technology*, they document 120 years of US data and argue that the college premium reflects a "race" between two forces:
        - **Demand:** Technology raises the demand for educated workers (skill-biased technological change, SBTC).
        - **Supply:** Education policy and social norms expand the supply of college graduates.
    - When supply growth outpaces demand growth (as in the 1950s--70s), the premium falls. When demand growth outpaces supply (as since 1980), the premium rises.
    - **The post-1980 surge:** The supply of college graduates slowed (the baby-boom cohort had graduated, and college costs rose), while demand accelerated (computerisation, globalisation). The result: a dramatic widening of the college premium and overall wage inequality.

!!! policy "Should Everyone Go to College?"

    The high average college premium does not mean that college is the right investment for every individual. The relevant comparison is the **marginal** return for the marginal student --- and for students at the margin of attending college (lower academic preparation, higher risk of dropout), the return may be much lower, or even negative if they incur debt without completing a degree.

    Policy should focus on: (a) reducing credit constraints so that high-ability, low-income students can attend college; (b) improving information about the returns to different fields and institutions; and (c) strengthening alternative pathways (vocational training, apprenticeships) for students whose comparative advantage lies outside traditional academic education.

---

## Education in India

!!! indian "Returns to Education in India"

    The Indian context presents several distinctive features that make the study of education and earnings especially complex.

    **High returns, especially for higher education:**

    - Duraisamy (2002) estimates returns to education using NSS data across three rounds (1983, 1987--88, 1993--94) and finds returns of 10--14% per year of schooling, with higher returns for post-secondary education and for women. Returns increased over this period, particularly at the tertiary level.
    - Agrawal (2012) uses NSS 2004--05 data and finds returns to higher education in India of approximately 12--17% per year, substantially above the global average reported by Psacharopoulos and Patrinos (2018).
    - Chamarbagwala (2010) documents rising returns to tertiary education during India's liberalisation era (1983--2005), driven by skill-biased technological change and the IT sector boom.
    - Kijima (2006) uses NSS data to show that returns to tertiary education in urban India rose sharply in the 1990s, contributing to rising wage inequality.
    - Returns vary sharply by sector: formal-sector workers earn much higher returns to education than informal-sector workers, suggesting that credentialism and institutional wage-setting amplify the education premium.

    **The massive higher education expansion:**

    - India's Gross Enrolment Ratio (GER) in higher education rose from about 10% in 2000 to over 28% by 2022. The number of universities increased from around 250 in 2000 to over 1,100 by 2023.
    - However, quantity has dramatically outpaced quality. The ASER (Annual Status of Education Report) consistently documents alarming learning deficits: in 2022, only 42% of Class V students in rural India could read a Class II-level text, and only 25% could do basic division.

    **Skill mismatch and the engineering surplus:**

    - India produces over 1.5 million engineering graduates annually --- more than the US and China combined per capita. Yet surveys consistently find that only 20--40% are "employable" by industry standards (Aspiring Minds, 2019).
    - The result is a paradox: India faces a shortage of skilled workers *and* a surplus of degree-holders simultaneously. The "educated unemployed" --- graduates who cannot find work matching their qualifications --- is a persistent feature of the Indian labour market.
    - This is partly a signalling story: students pursue engineering degrees not because they expect to work as engineers but because the degree signals general cognitive ability to employers in IT, banking, and management consulting.

    **Caste and gender dimensions:**

    - Returns to education are lower for Scheduled Castes and Scheduled Tribes, reflecting labour market discrimination that reduces the payoff to human capital investment for these groups. This creates a vicious circle: lower returns reduce the incentive to invest, which perpetuates educational gaps.
    - Women's returns to education are typically higher than men's (measured as percentage wage increase), but women face lower base wages and much lower labour force participation (around 25--35% in India), complicating the interpretation. The high coefficient partly reflects severe selection --- only the most qualified women enter the labour market.
    - Quality variation across institutions is extreme: an IIT or IIM degree commands a premium many multiples of the return to a degree from an unaccredited private college. This heterogeneity means that the average Mincer return masks enormous variation.

!!! policy "The Right to Education Act (RTE), 2009"

    The **Right of Children to Free and Compulsory Education Act** guarantees free education for all children aged 6--14 in India. Key provisions:

    - **Universal access:** Free and compulsory education in government and aided schools.
    - **No detention policy:** Students could not be held back or expelled until Class VIII (recently amended to allow exams at Classes V and VIII).
    - **Infrastructure norms:** Minimum standards for classrooms, teachers, pupil-teacher ratios (1:30), and facilities.
    - **25% reservation:** Private unaided schools must reserve 25% of seats for children from economically weaker sections (EWS) and disadvantaged groups.

    **Impact assessment:**

    - **Enrolment:** Near-universal enrolment achieved at the primary level. The number of out-of-school children dropped significantly.
    - **Learning outcomes:** Evidence is mixed. Muralidharan and Prakash (2017) find that the RTE's input-based mandates had limited impact on learning. The no-detention policy may have weakened incentives for effort by both students and teachers.
    - **Teacher shortages:** Teacher vacancies remain high, particularly in rural and remote areas. Many states rely on contract teachers with lower qualifications and pay.

    **Implications for human capital theory:** The RTE illustrates the critical distinction between *years of schooling* and *actual skill acquisition*. If school quality is low, additional years of schooling may generate limited human capital even though enrolment rises. This implies that the Mincer return to a "year of schooling" is not a fixed parameter --- it depends on what is learned during that year. India's challenge is not primarily about expanding access (which has been largely achieved at the primary level) but about improving quality.

!!! policy "New Education Policy (NEP) 2020"

    The NEP 2020 aims to overhaul India's education system with several relevant reforms:

    - **5+3+3+4 structure** replacing the 10+2 system, with emphasis on early childhood education.
    - **Multidisciplinary degrees** and flexible exit points (certificate after 1 year, diploma after 2, degree after 3, honours after 4).
    - **Vocational integration** from Class 6, with internships and apprenticeships.
    - **Target GER of 50%** in higher education by 2035.

    From a human capital perspective, the most significant reform may be the emphasis on learning outcomes and vocational skills rather than mere credential accumulation --- a potential shift from signalling toward genuine human capital formation.

---

## Key Takeaways

1. **Education is an investment** in human capital. Rational individuals compare the present value of future earnings gains against the direct and opportunity costs of schooling. The optimal level of education equates the marginal rate of return to the individual's discount rate.

2. The **Mincer earnings function** \(\ln w = \alpha + \beta s + \gamma_1 x + \gamma_2 x^2\) is the empirical workhorse. The coefficient \(\beta\) estimates the percentage return to an additional year of schooling, typically 6--12% across countries.

3. **Ability bias** threatens the causal interpretation of the Mincer return. More able individuals both acquire more schooling and earn more, potentially inflating OLS estimates. However, IV strategies --- twins studies (Ashenfelter and Krueger 1994), compulsory schooling laws (Angrist and Krueger 1991), and regression discontinuity designs --- consistently find that the bias is small.

4. The **signalling model** (Spence 1973) offers an alternative interpretation: education reveals ability rather than creating it. The sheepskin effect provides evidence that signalling plays some role, but human capital accumulation is the dominant channel. The policy stakes are high: if signalling dominates, education subsidies are wasteful.

5. **General training** is paid for by workers (through lower wages during training), while **specific training** costs are shared between the firm and the worker. This distinction explains wage-tenure profiles and why firms invest in retaining long-tenured employees.

6. **Age-earnings profiles are concave** because on-the-job training investment is front-loaded: young workers with long horizons invest heavily in skills, while older workers focus on utilising existing capital.

7. The **college wage premium** has roughly doubled in the US since 1980. Goldin and Katz (2008) attribute this to a race between technology (raising demand for skill) and education (raising supply). When supply growth slows, the premium rises.

8. In **India**, returns to education are high but vary enormously by gender, caste, sector, and institution quality. Despite massive enrolment gains, learning outcomes remain weak and skill mismatch is pervasive --- highlighting the distinction between years of schooling and actual human capital acquisition.

---

<div style="display: flex; justify-content: space-between; margin-top: 2rem;">
<a href="../05-compensating-differentials/">:material-arrow-left: Ch 5: Compensating Differentials</a>
<a href="../07-wage-distribution/">Ch 7: The Wage Distribution :material-arrow-right:</a>
</div>
