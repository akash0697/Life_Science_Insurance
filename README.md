# Life_Science_Insurance
The dataset belongs to a leading life insurance company. The company wants to predict the bonus for  its agents so that it may design appropriate engagement activity for their high performing agents and up-skill programs for low performing agents.

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

# Life Insurance Sales Prediction: Predictive Analytics

## Overview
This project leverages machine learning and statistical techniques to analyze and predict agent bonuses for a leading life insurance company in India. The goal is to identify key predictors for agent performance, optimize bonus distribution strategies, and improve overall sales efficiency.

## Objectives
- Build predictive models for agent bonuses.
- Use insights to design upskilling programs for low-performing agents.
- Develop strategies to increase company market share and profitability.

---

## Data Description
- **Dataset:** Life insurance company data with 4,520 observations and 20 features.
- **Data Types:**
  - Numerical: Age, Monthly Income, Sum Assured, Agent Bonus, etc.
  - Categorical: Channel, Occupation, Gender, Zone, Payment Method, etc.
- **Preprocessing Steps:**
  - Missing value imputation using median/mode.
  - Outliers retained as they represent genuine observations.
  - Categorical variables encoded into numerical values.
  - Data scaled using Z-score normalization.

---

## Exploratory Data Analysis (EDA)
### Key Findings
1. Sales dominated by agents over third-party and online channels.
2. Northern and Western regions outperform Eastern and Southern regions.
3. Married and divorced customers are key buyers, with salaried and small-business owners as major segments.
4. Significant predictors for bonuses:
   - Sum Assured
   - Customer Tenure
   - Age
   - Monthly Income

### Clustering Insights
- **Cluster 1:** Low bonuses, low income, short customer tenure.
- **Cluster 2:** Moderate bonuses, medium income, medium customer tenure.
- **Cluster 3:** High bonuses, high income, long customer tenure.

---

## Model Development and Tuning
### Models Built
1. **Linear Regression**: Base model for predicting bonuses.
2. **Decision Tree Regressor**: Decision support tool for conditional predictions.
3. **Random Forest Regressor**: Improved overfitting but computationally expensive.
4. **Artificial Neural Network (ANN)**: Captures complex non-linear relationships.

### Tuning Techniques
- **Linear Regression:**
  - Dropped insignificant predictors based on p-value (>0.05).
  - Final equation derived with adjusted R² to validate predictors.
- **Decision Tree and Random Forest:**
  - Hyperparameter tuning using Grid Search (e.g., max_depth, min_samples_split).
- **XGBoost:**
  - Objective: `reg:linear`.
  - Results showed slight overfitting but high accuracy.
- **ANN:**
  - Tuned using Grid Search (hidden_layer_sizes, activation, solver).

---

## Performance Metrics
| Model               | RMSE (Train) | RMSE (Test) | MAPE (Train) | MAPE (Test) |
|---------------------|--------------|-------------|--------------|-------------|
| Linear Regression   | 0.4400       | 0.4449      | 158.73       | 217.23      |
| Decision Tree       | 0.35         | 0.42        | 129.99       | 245.83      |
| Random Forest       | 0.24         | 0.38        | 87.00        | 193.40      |
| XGBoost             | 0.31         | 0.39        | 116.11       | 207.46      |
| ANN                 | 0.40         | 0.43        | 151.56       | 199.14      |

### Selected Model
**Linear Regression**:
- Best balance between simplicity and prediction consistency.
- Final equation:
AgentBonus = (-0.0022) * Intercept + (0.1419) * Age + (0.1484) * CustTenure + (0.121) * MonthlyIncome + (0.0861) * ExistingPolicyTenure + (0.5911) * SumAssured + (0.0752) * DesignationOrdinal

yaml
Copy code

---

## Business Implications
1. **Agent Incentivization:**
 - Design bonus structures prioritizing Sum Assured and Customer Tenure.
 - Focus on reselling policies to long-term customers.

2. **Regional Focus:**
 - Improve performance in Eastern and Southern regions using targeted market surveys.

3. **Channel Strategy:**
 - Offer better incentives to third-party and online channels to boost sales.

4. **Upskilling Plans:**
 - **Plan 1 (Product Knowledge):** Enhance product understanding and sales techniques.
 - **Plan 2 (Shadowing):** Low performers mirror high performers for on-the-job learning.

---

## Tools and Libraries
- **Programming Language:** Python
- **Libraries:** pandas, numpy, matplotlib, seaborn, sklearn, xgboost
- **Environment:** Jupyter Notebook

---

## Future Enhancements
- Incorporate advanced ensemble models to improve accuracy.
- Explore customer segmentation for personalized policy recommendations.
- Deploy the model into production using APIs for real-time bonus predictions.

---

For detailed analysis, refer to the project report.


