**📘 Insurance Claims Case Study (Python):**
This project delivers a complete solution to an Insurance Claims Case Study using Python, Pandas, NumPy, Matplotlib, Seaborn, and SciPy.
It includes data cleaning, feature engineering, EDA, visualizations, and statistical hypothesis testing.
The goal is to understand customer behavior, claim characteristics, fraud patterns, and statistical relationships across the insurance dataset.

**🎯 Objective:**
To build a 360° analytical view of insurance customers and their claims, identify risk segments, detect fraud indicators, and validate patterns using statistical hypothesis tests.

**🛠️ Steps Performed:**
**1️⃣ Data Loading & 360° Merge**
•	Imported claims.csv and cust_demographics.csv
•	Joined both datasets using customer_id
•	Created a unified dataset for all analysis

**2️⃣ Data Cleaning & Standardization**
•	Audited data types and inconsistent values
•	Converted monetary fields (claim_amount) by removing $ and converting to float
•	Parsed date fields (claim_date, DateOfBirth) into datetime formats

**3️⃣ Feature Engineering**
•	Injury Police Alert flag for injury claims without police reports
•	Most recent claim per customer retained using date-based deduplication
•	Missing value imputation:
o	Numerical → mean
o	Categorical → mode
•	Age calculation as of 1-Oct-2018
•	Age buckets: Children, Youth, Adult, Senior

**4️⃣ Exploratory Data Analysis**
Insights generated:
•	Average claim amount by customer segment
•	Total claim amount by incident cause for eligible claims
•	Number of claims and customers in driver-related incidents (TX, DE, AK adults)
•	Gender-wise and segment-wise claim amount distribution (pie charts)
•	Driver-related claim comparison between genders
•	Fraudulent claims by age group
•	Monthly trend of total claim amounts
•	Facetted bar charts showing claim amount patterns by gender × age group × fraud status
All visualizations use Matplotlib/Seaborn with clear labels and titles.

**5️⃣ Hypothesis Testing (Q16–Q20)**
Q16 — Claim Amount Difference Between Males & Females
Test: Independent two-sample t-test
Goal: Check whether average claim amounts differ between men and women
Q17 — Relationship Between Age Group & Customer Segment
Test: Chi-square test of independence
Goal: Determine whether age groups are associated with specific customer segments
Q18 — Current Year Claim Amount vs Benchmark $10,000
Test: One-sample t-test (one-sided)
Goal: Verify if the current year’s mean claim amount is significantly higher than $10,000
Q19 — Claim Amount Variation Across Age Groups
Test: One-way ANOVA
Goal: Compare mean claim amounts among Children, Youth, Adults, and Seniors
Q20 — Relationship Between Total Policy Claims & Claim Amount
Test: Pearson correlation
Goal: Identify if customers with more policy claims also file higher-value claims

**📈 Key Outcomes:**
•	Built a refined dataset with customer demographics + claims
•	Identified high-risk groups and fraudulent patterns
•	Found strong age and segment-level behaviour differences

**🧮 Tech Stack:**
•	Python
•	Pandas, NumPy
•	Matplotlib, Seaborn
•	SciPy
•	Jupyter Notebook
•	Detected significant trends in claims over time
•	Confirmed (or rejected) assumptions using statistical tests
