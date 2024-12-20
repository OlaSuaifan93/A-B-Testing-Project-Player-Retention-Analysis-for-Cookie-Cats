# A-B-Testing-Project-Player-Retention-Analysis-for-Cookie-Cats
 Conducted an A/B test to evaluate the impact of shifting the first game progression gate from level 30 to level 40 on player retention and gameplay rounds.

This project focuses on analyzing the results of an A/B test conducted in the mobile game **Cookie Cats**, developed by Tactile Entertainment. The game features a "gate" mechanism requiring players to wait or make an in-app purchase to proceed. The A/B test moved the first gate from **level 30 (control group)** to **level 40 (test group)**, and the study aims to determine the impact on **player retention** and **number of game rounds played**.

---

### **Data Description**
The dataset contains information from **90,189 players** who were randomly assigned to the control or test group. The variables include:
- **`userid`**: Unique player identifier.
- **`version`**: Group assignment (`gate_30` or `gate_40`).
- **`sum_gamerounds`**: Number of game rounds played in the first week.
- **`retention_1`**: Whether the player returned the next day.
- **`retention_7`**: Whether the player returned after seven days.

No missing values were found, ensuring data integrity.

---

### **A/B Testing Methodology**
1. **Business Understanding & Data Preparation**:
   - Identified the objective of improving player retention.
   - Examined data for missing values, outliers, and anomalies.

2. **Exploratory Data Analysis (EDA)**:
   - Summarized statistics for `sum_gamerounds`, including means, medians, and distributions.
   - Visualized data using histograms and boxplots to identify extreme values.

3. **Outlier Removal**:
   - Removed extreme values to enhance test accuracy.
   - Reanalyzed summary statistics post-cleaning.

4. **Hypothesis Testing**:
   - **Tests Used**:
     - Normality: Shapiro-Wilk test.
     - Homogeneity of variances: Levene’s test.
     - A/B comparison: T-tests, Welch tests, Mann-Whitney U test (as needed).
   - Metrics: Mean `sum_gamerounds` and player retention rates (`retention_1` and `retention_7`).

---

### **Key Findings**
- **Game Rounds**:
  - The control group (`gate_30`) had a slightly higher average `sum_gamerounds` than the test group (`gate_40`).
  - Distribution analysis indicated differences in variability between the groups.

- **Retention**:
  - Retention rates for `retention_1` and `retention_7` were analyzed to assess the impact of the gate change.

---

### **Conclusion**
The A/B testing process provides insights into how changing the gate position affects player engagement. Results inform whether the gate modification leads to improved player retention and sustained gameplay, helping the business make data-driven decisions.

---

### **Skills & Tools Used**
- **Packages**: `pandas`, `numpy`, `scipy.stats`, `seaborn`, `matplotlib`.
- **Statistical Methods**: Hypothesis testing, summary statistics, and visualization.
- **Key Concepts**: A/B testing, data cleaning, outlier detection, and inferential statistics.

This project demonstrates the integration of statistical analysis with business goals to optimize game design decisions.
