# Life_Science_Insurance
The dataset belongs to a leading life insurance company. The company wantsto predict the bonus for  its agents so that it may design appropriate engagement activity for their high performing agents and up-skill programs for low performing agents.

Introduction to problem statement
The data given is a company's internally acquired data, which is provided tous by a leading Life
Insurance organization located in India.
We have been provided with the data with the objective of establishing a model for the
organization which helps us in predicting the Bonus given tothe agents when they sell policies and
onboard customers (with or withouttheir families) with one/multiple Life Insurance Policies.
Idea behind making a model isto understand the most important predictors in deciding the agent 
bonuses. With the help of this knowledge, we will be able to motivate higher performing agents by
better incentivisation and also help their underperforming peers with strategies that may involve up￾skilling.It may also involve the process of auditing their sales meets and calls to better their
performance from a selling perspective.
Need of the Study
Understanding what type of bonuses should be allotted with appropriatesales is an important
step towards building a high performance - high rewarding sales team.
A high performance - high reward environment also builds a strong internal team, which has a
higher chance of retention, mainly due to the growth andrecognition an Agent or Employee receives
for his/ her performance. Properrecognition of agent's contribution leads to agent feeling more
satisfied andmotivated to work harder and better.
Better incentivisation leads to creating performance oriented employees andfuture leaders within the
organization.
Good Performance also leads to internal appraisals and for a sales team, agood internal growth story
is a benchmark which low-medium sales performers can strive for growth and thus seek 
improvement.
As for the low performing counterparts, up-skilling plans, call/visit shadowingplans (Where a low 
performing employee is grouped with the higher performing employee, with the desired objective of 
mirroring things like a solid sales pitch, asking the right questions to the customer, building an
understanding of customer profile, ideal conversion atmospheres, even prospecting and pursuing the
more likely customer, or evensimply - effective time management).
At the end of the day Sales is about providing an effective solution to customer’s problem in
the best possible way.
Business Opportunities:
1. Better Bonuses, Higher Performance, more sales which in turn wouldmean more business to
the organization.
2. A better Brand value can be expected considering higher volumes of sales being good and
Ideal outcome would be the company's name becoming a household name in India for Life
Insurance.
3. Higher Profits can be expected with increase in sales.
4. Increase in market share of the Life insurance company.
Social opportunities:
1. Increase in awareness of the benefits of Life Insurances.
2. Ideal outcome from a social perspective, would mean that more and more lives getting insured 
leading to financial security in case of an unfortunate mishappening
3. Life Insurance policies is the only security families have, when there is asingle bread winner in
the household
Data Dictionary
Fig 1: Data Dictionary
4 | P a g e 
Fig 2: Head of the data
Fig 3: Tail of the data
5 | P a g e 
6 | P a g e 
2. Data Report
Non-Visual understanding of the data
First, we understand how the data was collected in terms of time, frequencyand methodology.
Methodology: In the initial inspection, the data seems to be collected after the Customer/ 
Customer’s Family has purchased the Life insurance Plan or after the acquisition of the customer has
been done.
Source: The source of the data is internal, and is given by the organization(Primary Data Source).
Time and Frequency: Data is collected at a monthly frequency after customer is on boarded
with at least one insurance policy.
Approach for Exploratory Data Analysis:
1. We load the data dictionary and understand it thoroughly.
2. We then check if the data is loaded correctly using head and tail function.
3. We check the shape using the shape function.
4. Using the info function, we gather information around the Data Impurities(specifically Null
Values) and the data type of each column.
5. We check the null values column wise and their total.
6. Check for duplicate values using duplicated function.
7. Describe function is used to understand the statistical side of our data inpertinence to
distribution and count of the data.
Visual inspection of data (rows, columns, descriptive details):
Fig 4: Basic data description
7 | P a g e 
Insights from Visual Inspection:
1. The data has a total of 20 Features (Columns) and 4520 Observations inthe form of Customer
Data points (Rows)
2. We have 12 Numeric Data Features and 8 Object Data Type Featuresin ourdata. We will have to
convert data of object type to numeric considering this being a predictive problem statement.
However, we will explore the data more in depth before doing so.
3. 1.29% of our data is with null values which we will explore in the dataanalysis segment.
4. There are no duplicate values in the data.
Understanding of attributes(variable info, renaming if required):
 
Fig 5: General Information about the data Fig 6: Null values in the dataset
There are a total of 1166 Null Values in our data as shown above:
1. Age has 269 Null Values
2. CustTenure has 226 NullValues
3. NumberOfPolicy has 45 NullValues
4. MonthlyIncome has 236 NullValues
5. ExistingPolicyTenure has 184Null Values
6. SumAssured has 154 NullValues
7. CustCareScore has 52 NullValues
Numerical Features total – 12
'CustID', 'AgentBonus', 'Age', ‘CustTenure’, 'ExistingProdType', ‘NumberOfPolicy’, 'MonthlyIncome',
'Complaint', 'ExistingPolicyTenure', 'SumAssured', 'LastMonthCalls', and ‘CustCareScore' are Numerical.
Categorical Featurestotal – 7
Channel', 'Occupation', 'EducationField', 'Gender', 'Designation',‘MaritalStatus', ‘Zone’
8 | P a g e 
and ‘PaymentMethod' are Categorical.
Renaming:
1. We observed that there is a data entry error in the Gender column where'Female' is mis-spelled as
'Fe male'.
2. We also observe that in the case of Designation, 'Exe' seems to be equivalent to 'Executive' -
given that the Monthly Income also falls in the same bucket. We will go ahead and change 'Exe'
to 'Executive'.
3. In column EducationField 'UG' and 'Undergraduate' are the same meaning.We will go ahead and
change UG to Undergraduate.
3. EXPLORATORY DATA ANALYSIS
Univariate analysis (distribution and spread for every continuous
attribute, distribution of data incategories for categorical ones)
Presence of Outliers:
These are the following variables with outliers and we check them visuallywith the Boxplot
visualization:
1. Monthly Income
2. Existing Policy Tenure
3. Existing Product Type
4. Sum Assured
5. Age
6. Agent Bonus
7. Customer Tenure
8. Last Month Calls
Skewness:
In statistics, skewness is a measure of the asymmetry of the probability distribution of a random
variable about its mean. In other words, skewness tells you the amount and direction of skew
(departure from horizontal symmetry). The skewness value can be positive or negative, or even
undefined. If skewness is 0, the data are perfectly symmetrical, although it isquite unlikely for real￾world data. As a general rule of thumb:
9 | P a g e 
Fig 7: Advance data description
Convention:
Positive Skewness - Right Skewed
Negative Skewness - Left Skewed
If skewness is less than -1 or greater than 1, the distribution is highly skewed.
If skewness is between -1 and -0.5 or between 0.5 and 1, the distribution is moderately skewed.
If skewness is between -0.5 and 0.5, the distribution is approximately symmetric.
Boxplot:
 
 
10 | P a g e 
Fig 8: Boxplot of all the numeric variables
Distribution Plot
 
 
 
Fig 9: Distribution plot for all the numeric variables
11 | P a g e 
Inferences:
We can make the following observations with the help of the above table and
boxplot/distributiongraphs below (Figure 2 and Figure 3):
1. The distribution of the variable 'Agent Bonus' is moderately right skewed.
2. The distribution of the variable 'Age' is moderately right skewed.
3. The distribution of the variable 'Customer Tenure' is moderately right skewed.
4. The distribution of the variable 'Existing Prod Type' is approximately symmetric.
5. The distribution of the variable 'Number Of Policy' is approximately symmetric.
6. The distribution of the variable 'Monthly Income' is highly right skewed.
7. The distribution of the variable 'Complaint' is moderately right skewed.
8. The distribution of the variable 'Existing Policy Tenure' is highly right skewed.
9. The distribution of the variable 'Sum Assured' is moderately right skewed.
10.The distribution of the variable 'Last Month Calls' is moderately right skewed.
11.The distribution of the variable 'Customer Care Score' is approximately symmetric.
12. There are no negative values in our data.
Univariate Analysis for categorical variables:
 
12 | P a g e 
 
Fig 10: Categorical Variables count plot
Fig 11: Count for categorical variables
Inferences for Visual Analysis of Categorical Variables:
1. Sales made by Agents dominate the other two channels (i.e. Third Party Partner and Online Channels).
2. Major Customers are from families where the main source of income is Salaried and Customers who operate 
a small business.
3. Major chunk of the Customers have an educational qualification of Graduate followed by Under Graduate.
4. The observations for the gender Male is about 2500 and Female is about 1800.
5. Most of the customers are Manger, Executive and Senior Manger Level.
6. Most of the people are working in Managerial or Executive level positions, followed by people working as 
Senior Managers.
7. More than half of the customers who have purchased life insurance plans are married or divorced.
8. There is a higher company presence in Northern and Western India, where as sales numbers in the Eastern 
and Southern India is very poor .
9. Most of the people opt for Half Yearly and Yearly plans.
Bivariate Analysis
Correlation is a statistical measure that expresses the extent to which two variables are linearly 
related (meaning they change together at a constant rate).
Convention:
Correlation coefficients whose magnitude are between 0.7 and 1 indicatevariables which can be
considered highly correlated.
Correlation coefficients whose magnitude are between 0.5 and 0.7 indicatevariables which can be
considered moderately correlated.
Correlation coefficients whose magnitude are between 0.3 and 0.5 indicatevariables which have a
low correlation.
Correlation coefficients whose magnitude are less than 0.3 have little if any(linear) correlation.
Fig 12: Heatmap
13 | P a g e 
Fig 13: Pairplot
We can clearly draw the following inferences from the above heatmap and the following table
(printed correlation higher than 0.7 that the Sum assuredis highly correlated to Agent Bonus
(Target Variable).
Multicollinearity is a statistical concept where several independent variablesin a model are 
correlated. Two variables are considered to be perfectly collinear if their correlation coefficient
is +/- 1.0. Multicollinearity amongindependent variables will result in less reliable statistical
inferences.
In our data, we do not have any highly correlated independent variables.
We can also see how two continuous variables are associated with eachother with the help of the
following pair plot below.
We can clearly see that Agent Bonus (our target variable) is positively correlated with Age, Customer
Tenure, Monthly Income and Sum Assured.
14 | P a g e 
15 | P a g e 
Removal of unwanted variables
We see that the Customer ID cannot be a significant predictor since it is a unique identifier. Unique
observations in general are not significant when itcomes to predictive modeling. We go ahead and
remove it using the drop function.
Missing Value treatment
Approach:
If there are several or large numbers of data points that act as outliers. Outliers data points will have a 
significant impact on the mean and hence, in such cases, it is not recommended to use the mean for 
replacing the missing values. Using mean values for replacing missing values may not create a great model 
and hence gets ruled out. For symmetric data distribution, one can use the mean value for imputing missing 
values. Since we don’t have a large (> 15% of missing values) in our data, we will go ahead and impute 
missing values in the following manner:
For Age, MonthlyIncome, SumAssured, CustomerTenure have Outliers, we will impute using Median.
For ExistingPolicyTenure, CustCarescore and Number of policy do not have Outliers; we will impute using 
the Mode since they are taking whole values.
Outlier treatment
Approach:
For Outlier Treatment We usually have 3 ways we can approach them:
1) Retain the outliers if data occurrence seems to be genuine.
2) Drop or remove the outliers.
3) Capping these data points to the upper and lower limit of the distribution,to ensure they lie
within range of data points.
After carefully examining the features with outliers present, we reach a conclusion of not
removing/treating these outliers as they seem to be genuine observations. All of these data points
existing as outliers hold high importance for analysis.
Fig 14: Features with outliers (in %)
16 | P a g e 
Monthly Income: Income is subjective and different for different individuals and is a genuine observation. 
We should not treat these outliers with high Monthly Income. 
Existing Policy Tenure: Tenure can be dependent on multiple factors. Though most individuals lie between 
1-5, there are customers on boarding for policies with higher tenures as well.
Existing Product Type: The type of products are categorized into 6 Categories. This is a data point which 
exists in numeric format however is categorical and need not be treated for outliers.
Sum Assured: Sum Assured may be different for different policies within the system and again, should not be 
dropped as they hold high importance in the analysis.
Age: In this case there are people with above 35 Age onboard with the insurance company which could be a 
part of a family package or even would have on boarded at a younger age and have been in the system. 
Agent Bonus: Higher sales performers may receive higher bonus and since this is the target variable, this 
information of higher performing agents getting higher bonuses, is of utmost importance to us.
Customer Tenure: Again, similar to age, this can be a data point which indicates customers tenure with the 
company in the system, and completely normal.
Last Month Calls: Total calls attempted by company to a customer for cross sell can be high in case of a 
follow-up attempt made by an agent. This can be analyzed further. If done by high performing agent then 
deduction can be made that more number of follow ups usually lead to more cross selling.
Variable transformation
CategoricalVariableTransformations:
Linear Regression models can only handle numeric variables. Therefore, if a column has categorical
variable, models will only work when it is encoded tonumeric variable.
There are two types of categorical data:
Ordinal: Order based Payment Method
Nominal: Without any order or ranks like city Channel, Marital Status, Zone
Designation - Order can be on the basis from customers with higher designation to lower designation 
conventionally (i.e. VP > AVP > Senior Manger > Manager > Executive). All other features (Channel,
Occupation, Education Field, Gender, Marital Status, Zone and Payment Method) will be considered as 
nominal for further steps.
In the case of Educational field we can do so too, however we see separate classes of information.
For example Post Graduation and MBA.
MBA is a Post Graduation however not all customers may have done an MBA. Hence, ranking them according 
to order may become difficult.
17 | P a g e 
Fig 15: Variable after transformation
All features have been successfully converted to numeric data types.
The scales of each x-variable need to be specified, because linear regression is heavily dependent on 
scale. If we were to train on a dataset where length is measured in feet and another measured in miles, 
the performance of both will be the same but the coefficients will differ.
We will go ahead and scale the entire data using Z score.
Z-score is a variation of scaling that represents the number of standard deviations away from the mean. 
You would use z-score to ensure your feature distributions have mean = 0 and std = 1. It's useful when 
there are a few outliers, but not so extreme that you need clipping.
Addition of new variables
At this moment we do not see the need to add a New Variable given theexisting features provided
to us in the data set.
4. Business insights from EDA
Before we jump onto the insights, we need to check if the data and predictorvariables are balanced?
In this case since our target variable is continuous and our predictor variables are a mix of 
continuous and categorical, we will use Linear Regression for our model building exercise.
Linear regression being a model which predicts continuous variables, doesnot require data balancing
(which is usually required by models which are based on classification).
Hence, we do not have a need of processing the data through a databalancing methodology.
Data Balancing:
In this case, since our target variable is continuous and our predictor variables are a mix of continuous and 
categorical. 
We will use Linear Regression for our model building exercise.
Linear regression being a model which predicts continuous variables does not require data balancing (which is 
usually required by models which are based on classification).
Hence, we do not have a need of processing the data through a data balancing methodology.
Here are data imbalance observations for categorical variables. We need to keep these in mind when these 
variables come up as important predictors as there will be some features (eg: in Zone- there is very less data in 
Eastern and Southern Zone).
1. Sales made by Agents dominate the other two channels (i.e. Third Party Partner and Online Channels).
2. Majority Customers are from families where the main source of income is Salaried and people who operate 
a small business
3. Majority of the Customers have an educational qualificaiton of Graduate followed by Under Graduate
4. The obsevations for the gender Male is about 2500 and Female is about 1800
5. Most of the customers are Manger, Execective and Senior Manger Level
6. Most of the people are working in Managerial or Executive level positions, followed by people working as 
Senior Managers
7. More than half of the customers who have purchased life insurance plans are Married or Divorced
8. There is a higher company presence in Northern and Western India, where as sales numbers in the Eastern 
and Southern India is very poor.
9. Most of the people opted for Half Yearly and Yearly plan.
Business Insights Using Clustering:
We have performed Hierarchical Clustering.
Parameter used for Linkage is Average Linkage.
In average linkage, we define the distance between two clusters to be the average distance between 
data points in the first cluster and data points in the second cluster. On the basis of this definition of 
distance between clusters, at each stage of the process we combine the two clusters that have the 
smallest average linkage distance.
fcluster:
It is a methodology used to flatten the clusters.
We have used number of Clusters as 3 and the criterion as maxclust.
Maxclust: The maxclust criterion is a distance threshold; it rejects far points from being in the same 
cluster.
18 | P a g e 
Insights:
Before we move onto insights from clustering, we have used the mean values to understand how each 
numerical continuous feature is in the Cluster.
For the categorical (Nominal and Ordinal), since we have encoded them, it is better if we look at the 
mode as it will give us the variable that has occured the most in each cluster.
Fig 16: Dendogram for clustering
Number of Clusters - 3:
Using Number of Clusters as 3
Since, we can see from the above dendogram that major chunk of data can be bucketed into 6 such 
categories where we can segment the customer bucket.
We can also see that the distance between each of these 3 i.e. the volume of customers in each bucket 
is similar and 3 look optimal visually as well.
The number of clusters is the number of vertical lines in the dendogram cut by a horizontal line that 
can transverse the maximum distance vertically without intersecting a cluster.
In this case, we cut the model where we get 3 clusters.
Fig 17: Clustering Result
19 | P a g e 
Insights for Cluster 1 (Number of Customers in Cluster 1 - 4480):
Target Variable: Average Agent Bonus given for this cluster of customers is almost half of what is to 
the other 2 clusters (Average Agent Bonus of 4040.94)
Average Age of customer is 14 
Average Tenure of Customer is the least amongst all 3 (around 14)
Existing Product Type (rounded off since original values are integers) - 4 
Number of Policy (rounded off since original values are integers) - 4
Average Monthly Income of customers is lowest amongst the 3 clusters (22711.33)
Average number of Complaints is lowest of all (0 and 1)
Average Existing Policy Tenure is 4 which is on the lower side (Range 1-21)
Average Sum Assured is the least as compared to all 3 clusters (613056.77)
Average of Last Month Calls is the least to these customers in cluster 1 - 5 (Range of calls is 0 - 16)
Average Customer Care Score is 3 out of 5 which is average (Range is 1-5)
Insights for Cluster 2 (Number of Customers in Cluster 2 - 11):
Target Variable: Average Agent Bonus given for this cluster of customers is on the higher side 
(Average Agent Bonus of 7059.82)
Average Age of customer is 20
Average Tenure of Customer is the in the middle amongst all 3 (around 28)
Existing Product Type (rounded off since original values are integers) - 3
Number of Policy (rounded off since original values are integers) - 3
Average Monthly Income of customers is in between cluster 1 and cluster 3 (31654.36)
Average number of Complaints is highest of all 3 clusters (0 and 1)
Average Existing Policy Tenure is 19 and is the highest in cluster 2 (Range 1-21)
Average Sum Assured is in between cluster 1 and cluster 2 (997513.27)
Average of Last Month Calls is the least to these customers in cluster 2 - 5 (Range of calls is 0 - 16)
Average Customer Care Score is 3 out of 5 which is average (Range is 1-5)
Insights for Cluster 3 (Number of Customers in Cluster 3 - 29):
20 | P a g e 
21 | P a g e 
Target Variable: Average Agent Bonus given for this cluster of customers is on the highest amongst 
the 3 clusters (Average Agent Bonus of 8646.52)
Average Age of customer is 35
Average Tenure of Customer is the highest amongst all 3 (around 38) 
Existing Product Type (rounded off since original values are integers) - 5
Number of Policy (rounded off since original values are integers) - 4
Average Monthly Income of customers is highest amongst the 3 clusters (22711.33)
Average number of Complaints is between cluster 1 and cluster 2 (0 and 1)
Average Existing Policy Tenure is 9 (Range 1-21)
Average Sum Assured is the highest as compared to all 3 clusters (1331521.10)
Average of Last Month Calls is the least to these customers in cluster 3 - 7 (Range of calls is 0 - 16)
 Average Customer Care Score is 3 out of 5 which is average (Range is 1-5)
Business Implications
1. Agent Bonus is highest for cluster where average tenure of customer is highest indicating that
reselling policy is strong for these customers. Thisalso is confirmed by the average number of 
calls made by agents as it is highest across all 3 customers.
2. Agent Bonus is highest for customer policies where average age of customer is higher. Long
term customers are bringing in a good policy/reselling.
3. Sum Assured is also higher to customers who have a higher average age indicating trend. Higher
age customers can be pursued more rigorously to up sell policies.
4. Monthly income is highest for customers where the sum assured is higherindicating right kind of
follow-up done on cream customers which is good time management. Lower performing sales
agents can learn this to maximize company realization.
Insights from EDA
1. Sales made by Agents dominate the other two channels (i.e. Third PartyPartner and Online
Channels).
2. Majority Customers are from families where the main source of income isSalaried and people
who operate a small business.
3. Majority of the Customers have an educational qualification of Graduatefollowed by Under
Graduate.
4. The observations for the gender Male is about 2500 and Female is about1800.
5. More than half of the customers who have purchased life insurance plansare Married or Divorced
indicating family members purchasing plans in higher volumes than independent people.
6. There is a higher company presence in Northern and Western India, whereas sales numbers in the 
Eastern and Southern India is very poor. Surveys can be done and improvements can be thought 
of for low performing regions.
