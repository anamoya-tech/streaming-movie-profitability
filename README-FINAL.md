## Project Wrap-Up, Questions & Key Takeaways

This project analyzed the **relative impact efficiency** of movies available on Netflix and HBO between 2010 and 2021. Due to the lack of publicly available data on real viewership and production budgets, the analysis relied on **transparent proxy metrics** and focused on **comparative patterns**, not absolute financial profitability.

Below is a summary of the analytical questions defined at the start of the project, how they were addressed, and the corresponding conclusions.

---

### Core Business Question

**Which types of movies show higher relative impact efficiency on Netflix and HBO?**

**Answer:**
Using *Impact per Minute* and *Quality-Weighted Impact* as proxy metrics, HBO movies show higher average relative impact efficiency than Netflix movies. This suggests platform-level differences in catalog composition and content strategy, although results should be interpreted as relative signals rather than financial outcomes.

This question is directly addressed in the final dashboard.

---

### Subquestion 1  
**Are there meaningful differences in relative performance between Netflix and HBO?**

**Answer:**
Yes. HBO consistently shows higher average impact efficiency under the defined proxy metrics, while Netflix displays more homogeneous distributions. These differences are observable both in raw impact efficiency and in quality-adjusted impact.

This comparison is a central component of the dashboard.

---

### Subquestion 2  
**Do exclusive titles perform differently from titles shared across platforms?**

**Answer:**
Yes. Titles shared across platforms tend to concentrate higher efficiency values than platform exclusives. HBO exclusives outperform Netflix exclusives on average, but exclusivity alone does not guarantee stronger relative performance.

This analysis is included in the dashboard because it adds strategic insight without increasing interpretive complexity.

---

### Subquestion 3  
**Does perceived quality influence relative impact efficiency?**

**Answer:**
Yes. When IMDb score is incorporated into the efficiency metric, shared titles continue to outperform exclusives, indicating that higher efficiency is not driven by audience reach alone but also by perceived quality.

This result reinforces the robustness of the main efficiency metric and is included in the dashboard.

---

### Subquestion 4  
**Which genres show higher relative impact efficiency?**

**Answer:**
Genre-level analysis reveals differentiated efficiency patterns across platforms, with HBO showing stronger relative performance in certain high-impact genres. However, differences in scale and uneven sample sizes across genres limit direct comparison.

For this reason, genre analysis was treated as **exploratory** and kept outside the final dashboard.

---

### Subquestion 5  
**Do longer movies tend to be less impact-efficient?**

**Answer:**
No strong relationship is observed between movie runtime and impact efficiency. The scatter plot analysis shows high dispersion and a weak trend, indicating that runtime—used as a proxy for production effort—does not explain relative performance on its own.

This finding was documented as an exploratory result rather than a dashboard insight.

---

## Methodological Considerations

- All metrics are based on **public proxy data** and represent relative comparisons.
- Movies available on multiple platforms were intentionally retained as separate records to reflect distinct availability contexts.
- Exploratory analyses were separated from the final dashboard to preserve clarity and avoid over-fragmentation.

---

## Final Conclusion

This project demonstrates an end-to-end analytical workflow, from problem formulation and data preparation to exploratory analysis and executive-level visualization. The analysis prioritizes methodological transparency, responsible use of proxy metrics, and clear separation between exploratory findings and communicated results.

The final dashboard answers the core strategic questions effectively, while additional analyses remain prepared for future extensions. Overall, the project reflects a realistic and professional approach to data analysis under real-world data constraints.
