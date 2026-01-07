# Streaming Movie Profitability Analysis (Netflix vs HBO)

## Project Overview

This project analyzes the **relative profitability (impact efficiency)** of movies available on streaming platforms, comparing **Netflix and HBO** between **2010 and 2021**.

Due to the lack of publicly available data on real view counts and production budgets, the analysis relies on **proxy metrics** to estimate audience impact relative to production effort. These assumptions are explicitly documented and considered when interpreting results.

The project was developed using a combination of **traditional data analysis tools** and **generative AI–assisted workflows** to support reasoning, validation of methodological decisions, and documentation clarity. Analytical responsibility and final decisions remain fully human-led.

The objective is to identify which types of movies tend to deliver **higher impact per unit of effort**, and to assess whether there are systematic differences by platform, genre, and content exclusivity.

---

## Business Question

### Main question

Which types of movies (by genre and platform) show higher **relative impact efficiency** on Netflix and HBO?

### Sub-questions

- Are there consistent performance differences between Netflix and HBO catalogs?
- Which genres tend to generate higher audience impact relative to effort?
- Does movie duration (used as a proxy for production cost) affect impact efficiency?
- How has movie performance evolved over time?
- Do exclusive titles perform differently from shared titles across platforms?

---

## Methodological Approach

Streaming platforms do not provide public access to:

- Real view counts  
- Production budgets  

To address these limitations, the analysis uses commonly adopted **proxy variables**:

- **IMDb votes** as a proxy for audience reach or popularity  
- **IMDb score** as a proxy for perceived quality  
- **Movie runtime** as a proxy for relative production effort or cost  

Profitability is therefore treated as **relative impact efficiency**, rather than financial profit. All assumptions and constraints are transparently documented.

Generative AI tools were used selectively to assist with:
- Analytical reasoning refinement
- Validation of methodological alternatives
- Technical documentation clarity

All data processing, modeling choices, and interpretations remain analyst-driven.

---

## Data Sources

- Netflix movies catalog  
- HBO Max movies catalog  
- IMDb metadata (ratings and votes)  

**Analysis period:** 2010–2021

---

## Data Cleaning and Preparation

Key steps:

- Movies only (TV series excluded)
- Feature-length films only (runtime ≥ 60 minutes)
- Conversion of numeric fields imported as text
- Resolution of regional decimal format inconsistencies
- Normalization of multi-value genre fields
- Dataset unification via append (not joins)

### Duplicate handling

Movies available on both platforms were intentionally retained.

Each row represents availability on a specific platform, enabling platform-level and exclusivity analysis.

---

## Feature Engineering

A categorical variable was created:

- **Netflix Exclusive**
- **HBO Exclusive**
- **Shared**

This variable consolidates exclusivity information into a single field and removes redundancy.

---

## Final Dataset

Approx. **3,400 movies**


---

## Project Status

**Current stage**
- Data cleaning and modeling completed

**Next steps**
- Definition of impact efficiency metrics
- Comparative analysis
- Tableau dashboards

---

## Limitations

- No real streaming view counts
- No production budget data
- Results represent relative, not financial, profitability

