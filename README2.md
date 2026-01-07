## Phase 2 – Data Visualization & Exploratory Analysis

In this phase, Tableau was used to transform the cleaned and unified dataset into analytical visualizations aimed at answering the core questions of the project.

The **final dashboard** was intentionally designed to focus on insights that can be interpreted quickly and without extensive contextual explanation. More complex or highly segmented analyses were developed as **exploratory views** and kept outside the dashboard to preserve clarity.

### Visualizations included in the final dashboard
- Comparison of relative impact efficiency between Netflix and HBO using **Impact per Minute**
- Analysis by content exclusivity (Netflix Exclusive, HBO Exclusive, Shared)
- Quality-adjusted impact using a weighted metric (**Quality-Weighted Impact**)
- Distribution of IMDb scores by exclusivity

These views were selected because they communicate high-level patterns clearly while supporting the main analytical objective of the project.

### Exploratory analyses (not included in the dashboard)
- Genre-level efficiency analysis, including a **genre × platform heatmap** to highlight relative patterns while avoiding visual distortion caused by scale differences
- Runtime vs impact efficiency analysis using a **scatter plot with trend lines** to assess whether longer movies tend to be less efficient

Exploratory views were intentionally excluded from the final dashboard to avoid over-fragmentation, while remaining available for deeper analytical extension.

---

## Final Conclusions

The analysis shows clear differences in **relative impact efficiency** between Netflix and HBO, with HBO exhibiting higher average efficiency under the proxy metrics used. Titles shared across platforms tend to concentrate higher efficiency values, suggesting that widely distributed or well-established content outperforms platform exclusives on average.

Genre-level analysis reveals differentiated patterns between platforms, although these results are treated as exploratory due to differences in scale and uneven sample sizes. Additionally, no strong relationship is observed between movie runtime and impact efficiency, indicating that duration alone—used as a proxy for production effort—does not explain relative performance.

Overall, this project demonstrates a realistic analytical approach, responsible use of proxy metrics, clear separation between exploratory analysis and executive-level communication, and transparency regarding data limitations. All results should be interpreted as **relative comparisons**, not as estimates of actual financial profitability.
