Streaming Movie Profitability Analysis (Netflix vs HBO)
Project Overview

This project analyzes the relative profitability (impact efficiency) of movies available on streaming platforms, comparing Netflix and HBO between 2010 and 2021.

Due to the lack of publicly available data on real view counts and production budgets, the analysis relies on proxy metrics to estimate audience impact relative to production effort. These assumptions are explicitly documented and considered when interpreting results.

The project was developed using a combination of traditional data analysis tools and generative AI–assisted workflows to support reasoning, validation of methodological decisions, and documentation clarity. Analytical responsibility and final decisions remain fully human-led.

The objective is to identify which types of movies tend to deliver higher impact per unit of effort, and to assess whether there are systematic differences by platform, genre, and content exclusivity.

Business Question
Main question

Which types of movies (by genre and platform) show higher relative impact efficiency on Netflix and HBO?

Sub-questions

Are there consistent performance differences between Netflix and HBO catalogs?

Which genres tend to generate higher audience impact relative to effort?

Does movie duration (used as a proxy for production cost) affect impact efficiency?

How has movie performance evolved over time?

Do exclusive titles perform differently from shared titles across platforms?

Methodological Approach

Streaming platforms do not provide public access to:

Real view counts

Production budgets

To address these limitations, the analysis uses commonly adopted proxy variables:

IMDb votes as a proxy for audience reach or popularity

IMDb score as a proxy for perceived quality

Movie runtime as a proxy for relative production effort or cost

Profitability is therefore treated as relative impact efficiency, rather than financial profit. All assumptions, proxies, and constraints are transparently documented.

Generative AI tools were used selectively to:

Assist in refining analytical reasoning

Validate methodological alternatives

Improve clarity and structure of technical documentation

All data processing, modeling choices, and interpretations were defined and reviewed by the analyst.

Data Sources

Public datasets were selected after evaluating multiple alternatives to ensure consistency and adequate coverage:

Netflix movies catalog

HBO Max movies catalog

IMDb metadata (ratings and votes)

Analysis period: 2010–2021
The time frame was limited based on data availability and consistency across sources.

Data Cleaning and Preparation

Data preparation was performed using Google Sheets and included the following steps:

Filtering movies only (TV series excluded)

Restricting the dataset to feature-length films (runtime ≥ 60 minutes)

Limiting the analysis to the 2010–2021 period

Converting numeric fields imported as text:

imdb_score

imdb_votes

runtime

Resolving regional decimal format inconsistencies (. vs ,)

Normalizing multi-value and JSON-like genre fields into a single main_genre_clean

Adding a platform variable (Netflix / HBO)

Unifying both catalogs using append rather than joins

Duplicate handling

Movies available on both platforms were intentionally retained.

Each row represents movie availability on a specific platform, enabling platform-level comparisons and exclusivity analysis. These records are not treated as duplicates.

Feature Engineering

An additional categorical variable was created to model content availability:

exclusivity

Netflix Exclusive

HBO Exclusive

Shared

This variable consolidates exclusivity information into a single field, eliminating redundant columns and simplifying comparative analysis.

Final Dataset

The final unified dataset contains approximately 3,400 movies and includes the following columns:

platform
title
type
release_year
runtime
main_genre_clean
imdb_score
imdb_votes
exclusivity


All numeric fields were validated and formatted for direct use in analytical and visualization tools.

Repository Structure
streaming-movie-profitability/
├── README.md
├── data/
│   └── ALL_PLATFORMS_clean.csv
├── docs/
│   └── data_cleaning_summary.md
└── analysis/
    └── (to be added)

Project Status

Current stage

Data cleaning, validation, and modeling completed

Next steps

Definition of impact efficiency metrics

Comparative analysis by platform, genre, and exclusivity

Development of Tableau dashboards

Synthesis of insights and documented limitations

Limitations

No access to real streaming view counts

No detailed production budget data

Results represent relative comparisons, not financial profitability

Author

Data analysis project developed as part of a professional portfolio, combining analytical reasoning, domain knowledge, and AI-assisted workflows.
