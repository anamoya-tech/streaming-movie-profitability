# 🎬 Streaming Movie Profitability Analysis (Netflix vs HBO)

## 📌 Project Overview
This project analyzes the **relative profitability of movies on streaming platforms**, comparing **Netflix** and **HBO** between **2010 and 2021**.

Due to the lack of publicly available data on real view counts and production budgets, the analysis uses **proxy metrics** (IMDb votes, ratings, and runtime) to estimate audience impact and production effort.

The objective is to identify **which types of movies tend to deliver higher impact relative to effort**, and whether there are meaningful differences between platforms.

---

## ❓ Business Question

**Main question:**
> Which types of movies (by genre and platform) show higher relative profitability on Netflix and HBO?

**Sub-questions:**
- Are there differences in performance between Netflix and HBO catalogs?
- Which genres tend to generate higher audience impact?
- Does movie duration (as a proxy for production cost) affect profitability?
- How has movie performance evolved over time?

---

## 🧠 Methodological Approach

Streaming platforms do not provide public data on:
- real view counts
- production budgets

To address this limitation, the analysis relies on **commonly used proxy variables**:

- **IMDb votes** → proxy for audience reach / number of viewers  
- **IMDb score** → proxy for perceived quality  
- **Movie runtime** → proxy for production effort or cost  

These assumptions are explicitly documented and considered when interpreting results.

---

## 📊 Data Sources

Public datasets were selected after evaluating multiple alternatives to ensure consistency and coverage:

- Netflix movies catalog
- HBO movies catalog
- IMDb metadata (ratings and votes)

📅 **Analysis period:** 2010–2021  
(The period was limited based on data availability and consistency across sources.)

---

## 🧹 Data Cleaning & Preparation

Data preparation was performed using **Google Sheets** and included:

- Filtering only **movies** (excluding TV shows)
- Restricting data to **2010–2021**
- Converting numeric fields imported as text:
  - `imdb_score`
  - `imdb_votes`
  - `runtime`
- Resolving regional decimal format issues (`.` vs `,`)
- Removing records with missing critical metrics
- Normalizing multi-value genres into a single `main_genre`
- Cleaning categorical values stored as JSON-like lists
- Adding a `platform` column (Netflix / HBO)
- Unifying both datasets into a single analytical table

### Final unified dataset columns:
platform
title
type
release_year
runtime
main_genre
imdb_score
imdb_votes

---

## 📁 Repository Structure

streaming-movie-profitability/
├── README.md
├── data/
│ └── ALL_PLATFORMS_clean.csv
├── docs/
│ └── data_cleaning_summary.md
└── analysis/
└── (to be added)

---

## 🚧 Project Status

**Current stage:**  
✅ Data cleaning and dataset unification completed

**Next steps:**
- Define and calculate a **relative profitability metric**
- Perform comparative analysis by platform and genre
- Create visualizations and dashboards
- Summarize insights and recommendations

---

## ⚠️ Limitations

- No access to real streaming view counts
- No detailed production budget data
- Results represent **relative comparisons**, not exact financial profitability

---

## 👤 Author
Data analysis project developed as part of a professional portfolio.
