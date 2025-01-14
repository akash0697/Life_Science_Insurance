# Life_Science_Insurance
The dataset belongs to a leading life insurance company. The company wantsto predict the bonus for  its agents so that it may design appropriate engagement activity for their high performing agents and up-skill programs for low performing agents.

## Overview
This project focuses on analyzing and predicting agent bonuses for a leading life insurance company. By leveraging data analytics and predictive modeling, the project aims to improve agent incentivization, enhance performance, and optimize business outcomes.

## Objectives
- Predict agent bonuses based on customer and sales data.
- Identify key factors influencing agent performance.
- Design engagement and upskilling activities for agents.

## Data Summary
The dataset contains 20 features and 4,520 observations, with 12 numerical and 8 categorical variables. Data was collected monthly and sourced internally.

### Key Features
- **Numerical:** Age, Customer Tenure, Monthly Income, Sum Assured, Agent Bonus, etc.
- **Categorical:** Channel, Occupation, Gender, Zone, Payment Method, etc.

### Data Insights
- 1.29% of data has null values, addressed through imputation.
- Outliers in features like Monthly Income, Sum Assured, and Agent Bonus were retained as genuine observations.
- Categorical data was transformed into numerical formats for modeling.

## Exploratory Data Analysis (EDA)
### Univariate Analysis
- Continuous variables like Age and Monthly Income exhibit right-skewed distributions.
- Categorical variables show dominance of certain values, e.g., most sales are made by agents.

### Bivariate Analysis
- Positive correlations found between Agent Bonus and features like Age, Customer Tenure, and Sum Assured.
- No significant multicollinearity observed.

### Clustering Analysis
Hierarchical clustering identified 3 customer clusters based on agent bonus and other variables:
1. **Cluster 1:** Low bonuses, short tenure, low income.
2. **Cluster 2:** Moderate bonuses, medium tenure, moderate income.
3. **Cluster 3:** High bonuses, long tenure, high income.

## Key Business Insights
1. High agent bonuses are associated with long-tenured and older customers.
2. Regions like Northern and Western India perform better than Eastern and Southern regions.
3. Married or divorced customers purchase policies in higher volumes.

## Business Opportunities
- Enhance agent performance through better bonuses and upskilling.
- Improve sales in low-performing regions through targeted surveys and strategies.
- Increase market share and brand value by focusing on high-performing customer segments.

## Methodology
1. **Data Preparation:** Address missing values, transform categorical variables, and scale data using Z-score.
2. **EDA:** Understand data distribution, relationships, and insights.
3. **Model Building:** Use linear regression for bonus prediction.

## Tools and Techniques
- Python for data processing, visualization, and modeling.
- Libraries like pandas, matplotlib, and seaborn for analysis.

## Future Scope
- Explore advanced models for bonus prediction.
- Implement strategies to increase sales in underperforming regions.
- Design and monitor agent engagement programs.

---

For detailed analysis, refer to the project report.


