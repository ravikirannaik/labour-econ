---
title: "Unemployment"
description: "Borjas Chapter 12 — Presentation and Concept Map"
---

# 12. Unemployment

**Borjas Chapter 12 | 3 lecture hours**

---

## :material-presentation: Presentation

<iframe src="../../slides/ch12-unemployment.html" width="100%" height="500" frameborder="0" allowfullscreen></iframe>

---

## :material-sitemap: Concept Map

<div class="concept-map" markdown>

```mermaid
flowchart TD
    UE["<b>Unemployment</b>"] --> TYPES["Types of<br/>Unemployment"]
    UE --> SEARCH["Job Search<br/>Model"]
    UE --> UI["Unemployment<br/>Insurance"]
    UE --> BEV["Beveridge<br/>Curve"]

    TYPES --> FRIC["Frictional"]
    TYPES --> STRUC["Structural"]
    TYPES --> CYC["Cyclical"]
    FRIC & STRUC --> NAT["Natural Rate<br/>of Unemployment"]

    SEARCH --> RW2["Reservation<br/>Wage"]
    SEARCH --> OFFERS["Wage Offer<br/>Distribution"]
    RW2 & OFFERS --> DUR["Expected<br/>Duration"]

    UI --> BENE["Benefits ↑"]
    BENE --> RW3["Reservation<br/>Wage ↑"]
    RW3 --> LONGER["Longer Search<br/>Duration"]
    BENE --> MATCH2["Better<br/>Matches?"]

    BEV --> VAC["Vacancies"]
    BEV --> UNEMP["Unemployment"]
    VAC & UNEMP --> CURVE["Inverse<br/>Relationship"]
    CURVE --> SHIFT["Shifts = Structural<br/>Change"]

    UE --> STEADY["Steady-State<br/>Rate"]
    STEADY --> FLOWS["Inflow Rate /<br/>Outflow Rate"]

    style UE fill:#0000DC,color:#fff
    style NAT fill:#F01928,color:#fff
    style SEARCH fill:#F01928,color:#fff
```

</div>
