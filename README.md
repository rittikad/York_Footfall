# York Footfall Analysis 🚶‍♂️📊

🎯 **Objective**  
This project analyzes pedestrian foot traffic across York to determine the optimal location for a promoter's stall. By understanding daily and weekend visitor patterns, the project provides actionable recommendations to maximize engagement and visibility.

---

📚 **Dataset**  
**Source:** York Footfall Data (Automated street sensors)  
**Period:** 2019 (Pre-pandemic trends)  
**Frequency:** Daily  

**Variables:**  
- **Date:** Day of recorded footfall  
- **LocationName:** Street or specific location in York  
- **WeekDay:** Day of the week  
- **TotalCount:** Number of pedestrians counted  
- **Recording_ID:** Unique identifier  

**Why This Dataset?**  
- Captures real-world pedestrian activity → ideal for location-based decision making  
- Includes multiple streets and all days of the week → allows comprehensive comparisons  
- Reflects pre-pandemic trends → baseline for normal foot traffic  

---

⚙️ **Methodology**

1. **Data Cleaning & Quality Check**  
   - Removed duplicate rows and entries with missing footfall counts  
   - Retained outliers to reflect real-world high-traffic events (e.g., holiday spikes)  

2. **Summary Statistics**  
   - Computed for each location:  
     - First and last measurement dates  
     - Average daily footfall  
     - Standard deviation, minimum, and maximum daily footfall  
   - Purpose: Understand general foot traffic patterns and variability  

3. **Visualization**  
   - Histograms of daily footfall for each street  
   - Focused on **2019** to identify pre-pandemic traffic trends  

4. **Statistical Analysis**  
   - **Two-sample t-tests** to compare Coney Street and Stonegate:  
     1. **All days:** Tests if average daily footfall differs significantly  
     2. **Weekends only:** Tests if footfall differs on high-traffic leisure days  

5. **Recommendations**  
   - Derived from summary statistics and t-test results  
   - Helps promoter choose street based on traffic trends and variability  

---

🧠 **Execution & Tools**  
- **Analysis:** Data cleaning, summary statistics, t-tests, visualizations  
- **Tools:** R, tidyverse, kableExtra, ggplot2  
- **Goal:** Translate raw foot traffic data into clear, actionable business insights  

---

## 📂 Quick Access
- **[R Script](https://github.com/rittikad/York_Footfall/blob/main/Code/5594410.Rmd)** – Complete code for data cleaning, analysis, and visualization  
- **[Dataset](https://github.com/rittikad/York_Footfall/tree/main/Data)** – Raw footfall dataset  
- **[HTML Report](https://github.com/rittikad/York_Footfall/tree/main/HTML_Report)** – Final report with tables, plots, and explanations

---

📊 **Results & Insights**

| Analysis | Observation | Key Takeaway |
|----------|------------|---------------|
| Summary Statistics | Coney Street & Parliament Street have highest daily traffic | Best locations for consistent daily engagement |
| 2019 Footfall Distribution | Coney Street shows consistently high traffic; Stonegate is variable; Micklegate lower | Visualizes street traffic trends for decision-making |
| All-days t-test | Coney Street (avg. 20,817) > Stonegate (avg. 19,204), p = 0.0008 | Coney Street is statistically superior for daily stall placement |
| Weekends t-test | Coney Street (avg. 25,863) ≈ Stonegate (avg. 26,167), p = 0.77 | Either street is suitable for weekend operations |

💡 **Key Findings**  
- **Coney Street** is the optimal location for **every day of the week** due to higher, consistent foot traffic.  
- **Weekends:** Both Coney Street and Stonegate attract similar crowds; either street is effective.  
- Seasonal and high-traffic events were preserved in analysis → realistic recommendations.  

---

🚀 **Recommendations**  
1. **Daily Stall Placement:**  
   - Prioritize **Coney Street** for consistent visitor engagement and higher exposure.  
2. **Weekend Operations:**  
   - Either **Coney Street** or **Stonegate** is acceptable; choose based on other factors (e.g., rent, accessibility).  
3. **Event Planning:**  
   - Leverage seasonal peaks (e.g., Christmas) on high-traffic streets to maximize promotional impact.  

---

🌍 **Impact**  
This project demonstrates the ability to:  
- Transform raw pedestrian data into actionable business insights  
- Support real-world marketing decisions with statistical evidence  
- Communicate findings effectively for both technical and non-technical stakeholders  
- Enable strategic decision-making based on foot traffic trends  

---

🛠️ **Skills Showcased**  
R · Data Cleaning · Statistical Analysis · Data Visualization · Analytical Thinking · Business Decision Support · Reporting  

---

📈 **Conclusion**  
- **Coney Street**: Best choice for consistent, high daily foot traffic.  
- **Stonegate**: Comparable on weekends; suitable if Coney Street is unavailable.  
- Preserving outliers and analyzing trends ensures recommendations are realistic and practical.  
- Data-driven insights from this project can be directly applied to optimize promotional stall placement, increasing visibility and potential customer engagement.
