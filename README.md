# -E.L-Task-5-Titanic-EDA-Analysis
Exploratory Data Analysis of Titanic Dataset using Python

# Key Findings and Insights

📝 Project Summary: Titanic Dataset Analysis
This project explores the Titanic dataset using Python in Google Colab. It involves data cleaning, univariate and bivariate analysis, and derives key insights using visualizations and statistical methods.

✅ Objective
To analyze passenger demographics and travel classes from the Titanic dataset and uncover patterns that influenced survival rates.

🔧 Tools & Libraries Used
Python (Pandas, NumPy)

Matplotlib & Seaborn (Data Visualization)

Google Colab (Development Environment)

📊 Key Exploratory Findings
🔹 Data Cleaning
Missing values were handled:

Age: Filled with median value.

Cabin: Replaced with "Unknown".

Embarked: Filled with most common value "S".

🚨 Critical Survival Factors
1. Gender Impact (Strongest Predictor)

Female Survival Rate: ~74.2%
Male Survival Rate: ~18.9%
Key Insight: "Women and children first" policy was clearly implemented
Statistical Significance: Gender had the strongest correlation with survival

2. Social Class Hierarchy

1st Class Survival: ~63.0%
2nd Class Survival: ~47.3%
3rd Class Survival: ~24.2%
Key Insight: Economic status directly influenced access to lifeboats

3. Age Factor Analysis

Children (<18): Higher survival rates (~58%)
Adults (18-64): Moderate survival rates (~38%)
Elderly (65+): Lower survival rates (~25%)
Key Insight: Age-based priority system favored children

🏠 Family Dynamics
4. Family Size Optimization

Traveling Alone: ~30% survival rate
Small Families (2-4): ~55% survival rate
Large Families (5+): ~16% survival rate
Key Insight: Small family groups had survival advantages

5. Sibling & Spouse Impact

0 Siblings/Spouse: Lower survival
1-2 Siblings/Spouse: Optimal survival
3+ Siblings/Spouse: Decreased survival
Key Insight: Moderate family connections were beneficial

💰 Economic Indicators
6. Fare Analysis

Average Fare (Survivors): ~$48.40
Average Fare (Non-survivors): ~$22.10
Key Insight: Higher-paying passengers had better survival odds

7. Embarkation Port Patterns

Cherbourg (C): ~55% survival rate
Queenstown (Q): ~39% survival rate
Southampton (S): ~34% survival rate
Key Insight: Cherbourg passengers (often wealthier) survived more

📌 Conclusion
Socioeconomic status and gender played a significant role in determining survival.
