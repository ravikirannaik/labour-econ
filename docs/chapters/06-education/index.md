---
title: "Education"
description: "Borjas Chapter 6 — Presentation and Concept Map"
---

# 6. Education

**Borjas Chapter 6 | 4 lecture hours**

---

## :material-presentation: Presentation

<iframe src="../../slides/ch6-education.html" width="100%" height="500" frameborder="0" allowfullscreen></iframe>

---

## :material-sitemap: Concept Map

<div class="concept-map" markdown>

```mermaid
flowchart TD
    EDU["<b>Education &<br/>Human Capital</b>"] --> HC["Human Capital<br/>Model"]
    EDU --> SIG["Signalling<br/>Model"]

    HC --> INV["Schooling as<br/>Investment"]
    INV --> MB["Marginal Benefit:<br/>Higher Earnings"]
    INV --> MC["Marginal Cost:<br/>Tuition + Foregone"]
    MB & MC --> OPT["Optimal Years<br/>of Schooling"]

    HC --> MINCER["Mincer Earnings<br/>Equation"]
    MINCER --> ROS["Rate of Return<br/>to Schooling"]
    ROS --> BIAS["Ability<br/>Bias"]
    BIAS --> IV["Instrumental<br/>Variables"]

    SIG --> SCREEN["Education as<br/>a Signal"]
    SCREEN --> SEP["Separating<br/>Equilibrium"]
    SCREEN --> POOL["Pooling<br/>Equilibrium"]

    EDU --> TRAIN["On-the-Job<br/>Training"]
    TRAIN --> GEN["General<br/>Training"]
    TRAIN --> SPEC["Specific<br/>Training"]
    GEN -->|"Worker pays"| WAGE1["Flat then<br/>Rising Profile"]
    SPEC -->|"Shared cost"| WAGE2["Gradual<br/>Rising Profile"]

    style EDU fill:#0000DC,color:#fff
    style OPT fill:#F01928,color:#fff
    style MINCER fill:#F01928,color:#fff
```

</div>
