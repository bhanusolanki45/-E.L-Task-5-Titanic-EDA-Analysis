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

🔹 Univariate Analysis
Feature	Insight
Survival Rate	~38.4% passengers survived, indicating high fatality overall.
Passenger Class	Most passengers belonged to 3rd class, followed by 1st and 2nd.
Gender Distribution	Males outnumbered females, yet had a significantly lower survival rate.
Age Distribution	Age ranged from infants to elderly; most were aged between 20–40 years.

🔹 Bivariate Analysis
Relationship Analyzed	Key Finding
Survival by Gender	Females had much higher survival rates than males.
Survival by Passenger Class	1st class passengers had the highest chance of survival.
Survival by Embarked Port	Passengers embarking from Cherbourg (C) had a higher survival rate.
Age vs Survival	Younger passengers showed a slightly better survival rate.

📌 Conclusion
Socioeconomic status and gender played a significant role in determining survival.

The project successfully uses EDA techniques to extract meaningful insights and builds a solid foundation for predictive modeling in the future.


# Summary Report
print("\n" + "="*50)
print("SUMMARY REPORT")
print("="*50)

print("""
TITANIC DATASET ANALYSIS SUMMARY

Dataset Overview:
- Total passengers analyzed: """ + str(len(df)) + """
- Features analyzed: """ + str(len(df.columns)) + """ variables
- Missing data handled: Age and Embarked columns

Key Patterns Discovered:
1. Gender was the strongest predictor of survival (Women > Men)
2. Passenger class significantly affected survival chances (1st > 2nd > 3rd)
3. Age played a role with children having better survival rates
4. Family size had optimal survival rates for small families (2-4 members)
5. Higher fare passengers had better survival chances

Strongest Correlations with Survival:
- Gender (Female advantage)
- Passenger Class (Higher class advantage)
- Fare (Higher fare advantage)

Data Quality:
- Clean dataset after handling missing values
- No major outliers that would skew analysis
- Representative sample of Titanic passengers

Recommendations for Further Analysis:
1. Investigate cabin location impact on survival
2. Analyze specific embarkation port effects
3. Study family composition in more detail
4. Examine crew vs passenger survival rates
""")

print("\n" + "="*50)
print("ANALYSIS COMPLETE!")
print("="*50)
