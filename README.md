# Churn_Analysis_ML_Project-Logistic_Regression-
## Business Objective:- 
'''Customer churn is a concerning problem for large companies (especially in the Telecom field) due to its direct effect on revenues. Companies often seek to know which customers are likely to churn in the recent future so that timely action can be taken to prevent it'''
### Problem Statement:-
'''Task is to perfom detail Analysis and build for this Telecom company a Logistic Regression Machine Learning model that predicts which of their customers are likely to churn (stop using their service in future)'''
'''- There are 3333 data instances distributed accross 11 variables.
- Variable datatypes
	- 5 variables are of float64 datatype
	- 6 variables are of int64 datatype
	
-The DataFrame is devoid of any missing values
- DataFrame does not have any duplicate instances
- There are some outliers in variable 
AccountWeeks,DataUsages,CostServCalls,DayMins,DayCalls,MonthlyCharge,AverageFree,RoamMins
   ** It is subject to investigate if these outliers are good outliers or bad outliers

- - - - - - - - - - - - UNIVARIATE ANALYSIS:-

- Churn
	- Churn is the target variable
	- Data is heavily imbalanced
	- 2580 data instances belongs to negative class{0} and 483 data instances belongs to positive class{1}.

- AccountWeeks
	- Most of the customers have duration of active account from 50 to 150 weeks
	- There is skewness of 1.09,it is subject to investigate if the skewness is occuring
	 because of outliers or it needs some transformation.

- ContractRenewal
	- 3010  customers has recent renewal of contract
	- 323 customers do not opt for contract renewal

- DataPlan
	- 922 customers have data plan
	- 2411 customers do not have data plan 

- DayMins
	- Most of the customers have Average DayTime minutes is in the range of 100 to 250 minutes
	
- DayCalls
	- Most of the customers have Average Number of DayTime calls are in the range of 60 to 125 times

- MonthlyCharge
	- Most of the customers have Average Monthly charges 35 to 80

- OverageFee
	- Most of the customers have largest overagefee for last 12 months ranges between 6 to 14

- MonthlyCharge
	- Most of the customers have Average Monthly charges 35 to 80



- - - - - - - - - - - - BIVARIATE ANALYSIS:-

	-Categorical Variables:- But they are LabelEncoded
		- Churn
		- ContractRenewal
		- DataPlan 

List of Important Variables
- DataUsages
- CustServCalls
- DayMins
- OverageFee
- RoamMins
- ContractRenewal
- DataPlan*


(A) Categorical vs Numeric

- (1) Churn Vs AccountWeeks
	- There does not exist  significant relation among them
	
	
- (2) Churn Vs DataUsage
	- There is a significant difference between the groups.

- (3) Churn Vs CustServCalls
	- There is a significant difference between the groups.

- (4) Churn Vs DayMins
	- There is a significant difference between the groups.

- (5) Churn Vs DayCalls 
	- There is no significant difference between the groups.

- (6) Churn Vs MonthlyIncome 
	- There is no significant difference between the groups.
	
- (7) Churn Vs OverageFee
	- There is significant difference between the groups.

- (8) Churn Vs RoamMins
	- There is significant difference between the groups.

(B) Categorical / Categorical

- (1) Churn Vs ContractRenewal
	- Chi-Squared Statistic: 222.56575664993764
	- P-value: 2.4931077033159204e-50
	- There is significant assosiation

- (2) Churn Vs DataPlan
	- Chi-Squared Statistic: 34.13166001075673  **  Value is not very high
	- P-value: 5.15063965903898e-09
	- There is significant assosiation

'''
