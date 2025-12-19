# Ownership and Governance in U.S. Medicare Hospitals

This repository examines how ownership and control are structured within Medicare-enrolled hospitals in the United States using public data from the Centers for Medicare & Medicaid Services (CMS).

Rather than treating hospitals as isolated facilities, the analysis focuses on **governance structure, role accumulation, and legal organization** to understand how control is exercised and disclosed in hospital systems.

---

## Research Focus

Public discussions of hospital ownership often rely on surface-level labels such as *nonprofit*, *for-profit*, *health system*, or *chain*. While these categories describe legal status, they rarely explain how decision-making authority is distributed in practice.

This project addresses three core questions:

- How often is control concentrated through **multiple formal roles held by the same individual or entity** within a hospital?
- To what extent do **repeat owners** appear across multiple hospitals?
- What **legal structures** dominate hospital ownership disclosures, and what do they imply for transparency and accountability?

The goal is to analyse hospital governance as a **structural system**, not to evaluate clinical performance or financial outcomes.

---

## Data Source

The analysis uses the **CMS Hospital All Owners** dataset, accessed via the CMS Open Data API.

Each record represents a declared ownership or control relationship between a hospital and an associated individual or organisation. Multiple records per hospital are expected and reflect layered governance structures rather than duplication.

Key attributes include:
- Ownership and control roles (e.g. owner, corporate officer, operational control)
- Percentage ownership indicators
- Legal and organisational classifications (LLC, holding company, chain home office)
- Cross-hospital ownership relationships

---

## Methodology

The dataset is treated as an **ownership and governance network**, not a facility-level table.

The analysis focuses on:
- **Role stacking**: identifying owners who hold multiple formal roles within the same hospital
- **Cross-hospital influence**: identifying owners associated with multiple hospitals
- **Legal structure analysis**: evaluating the prevalence of LLCs, holding companies, and related entities as ownership vehicles

All analysis was conducted in Python using Pandas, with an emphasis on aggregation and relational inference rather than predictive modelling.

---

## Key Findings

- Hospital ownership is more formalised than in long-term care, with a higher presence of holding companies and chain home offices.
- **Role stacking persists**, though it is less extreme than in skilled nursing facilities.
- A subset of owners appears across **multiple hospitals**, indicating networked control beyond individual facilities.
- Explicit declarations of private equity ownership are rare, suggesting that financial influence is embedded indirectly through legal structures.

These patterns indicate that hospital governance relies on layered control and legal insulation rather than straightforward ownership transparency.

---

## Limitations

- Ownership data is self-reported and constrained by CMS classification categories.
- Legal ownership structures may not reflect ultimate beneficial ownership.
- The analysis does not assess quality of care, staffing, financial performance, or regulatory outcomes.

The findings are descriptive and structural, intended to inform further research rather than establish causality.

---

## Related Work

This repository is part of a broader research series examining structural concentration and governance in U.S. healthcare.

Companion analyses include:
- **Skilled Nursing Facility enrolment concentration**
- **Ownership and governance in skilled nursing facilities**

These repositories analyse different datasets but apply a consistent structural lens.

---

## Code and Reproducibility

The full analysis is contained in a single Jupyter notebook and can be reproduced using standard Python data science libraries.

---

## Author

Ofile Seneo Mfetane  
Business Intelligence & Data Analytics  
