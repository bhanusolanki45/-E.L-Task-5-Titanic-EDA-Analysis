# -E.L-Task-5-Titanic-EDA-Analysis
Exploratory Data Analysis of Titanic Dataset using Python

# Key Findings and Insights
print("\n" + "="*50)
print("KEY FINDINGS AND INSIGHTS")
print("="*50)

print("\n1. SURVIVAL INSIGHTS:")
print(f"   • Overall survival rate: {df['Survived'].mean():.1%}")
print(f"   • Women had higher survival rate: {df[df['Sex']=='female']['Survived'].mean():.1%}")
print(f"   • Men had lower survival rate: {df[df['Sex']=='male']['Survived'].mean():.1%}")

print("\n2. CLASS INSIGHTS:")
for pclass in sorted(df['Pclass'].unique()):
    rate = df[df['Pclass']==pclass]['Survived'].mean()
    print(f"   • Class {pclass} survival rate: {rate:.1%}")

print("\n3. AGE INSIGHTS:")
child_survival = df[df['Age'] < 18]['Survived'].mean()
adult_survival = df[df['Age'] >= 18]['Survived'].mean()
print(f"   • Children (<18) survival rate: {child_survival:.1%}")
print(f"   • Adults (18+) survival rate: {adult_survival:.1%}")

print("\n4. FAMILY INSIGHTS:")
alone_survival = df[df['FamilySize'] == 1]['Survived'].mean()
with_family_survival = df[df['FamilySize'] > 1]['Survived'].mean()
print(f"   • Passengers alone survival rate: {alone_survival:.1%}")
print(f"   • Passengers with family survival rate: {with_family_survival:.1%}")

print("\n5. ECONOMIC INSIGHTS:")
avg_fare_survived = df[df['Survived'] == 1]['Fare'].mean()
avg_fare_died = df[df['Survived'] == 0]['Fare'].mean()
print(f"   • Average fare of survivors: ${avg_fare_survived:.2f}")
print(f"   • Average fare of non-survivors: ${avg_fare_died:.2f}")

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
