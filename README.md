# Experiment 12: Categorical Data Analysis Using Python

**Name:** Arhan Nair  
**PRN:** 25070123169  


---

## 1. Theory

### Categorical Data in Pandas
Categorical data represents variables that contain label values rather than numeric measurements (e.g., Gender, Department, or Grade). Analyzing these variables requires specialized techniques to summarize the distribution and relationships between categories.

### Key Analytical Techniques
The following methods from the Pandas library were used in this experiment:
* **`value_counts()`**: Calculates the frequency of each unique value in a column. When the `normalize=True` parameter is used, it provides the percentage distribution of the categories.
* **`pd.crosstab()`**: A powerful tool for "cross-tabulation" that computes a frequency table of two or more factors. It is used to observe the relationship between two categorical variables (e.g., how Grades are distributed across different Genders).
* **`groupby()`**: Used to split the data into groups based on some criteria and apply functions (like counting) to each group.
* **`unique()` and `nunique()`**: Identifies the specific labels present in a column and the total count of those distinct labels, respectively.
* **Filtering**: Extracting a subset of the data that meets a specific categorical condition (e.g., all "Electronics" orders).

---

## 2. Implementation Overview

### Dataset A: Student Academic Records
The first part of the experiment analyzes a dataset of 60 students with parameters including **Gender**, **Department** (CSE, IT, ECE, Mechanical), and **Grade** (A, B, C).
* **Statistical Insight**: The analysis revealed that the "CSE" department has the highest number of students (20), and 40% of the total student population obtained a "B" grade.
* **Cross-Analysis**: A crosstab showed that Females (14) significantly outperformed Males (8) in achieving "A" grades.

### Dataset B: E-Commerce Orders
The second part involves a manually created dataset for order tracking, including **Category**, **Payment Method**, **Delivery Type**, and **Customer Type**.
* **Operational Insight**: "Electronics" is the most frequent category (40%), and all electronics orders in this dataset were paid via "UPI."
* **Cross-Analysis**: A crosstab highlighted specific consumer behaviors, such as "Card" payments being exclusively used for "Clothing" in this sample.

---

## 3. Conclusion

This experiment demonstrates that categorical analysis is vital for identifying patterns and trends that numerical summaries might miss. By utilizing frequency counts and cross-tabulations, we can derive actionable insights from non-numeric data.


**Key Takeaways:**
* **Frequency vs. Proportion**: `value_counts()` with normalization is essential for comparing datasets of different sizes.
* **Relationship Mapping**: `pd.crosstab()` is the primary tool for bivariate analysis of categorical data, allowing for the comparison of groups (like Department vs. Grade).
* **Data Integrity**: Tools like `isnull().sum()` and `duplicated()` ensure the categorical analysis is performed on clean, high-quality data.

---
