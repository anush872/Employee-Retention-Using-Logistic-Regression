**Employee Retention Analysis**
**Overview**
This analysis explores the factors influencing employee retention and builds a machine learning model (logistic regression) to predict whether employees are likely to leave the organization. Key steps include exploratory data analysis (EDA), feature selection, and model evaluation.
________________________________________________________________________________________________________________________________________________________________________
**Objectives**
1.	Identify variables that directly impact employee retention (i.e., whether they leave or stay).
2.	Visualize the relationships between employee attributes (e.g., salary, department) and retention.
3.	Build and evaluate a logistic regression model for prediction.
4.	Analyse the accuracy of the model
___________________________________________________________________________________________________________________________________________________________________
**Data Exploration and Key Insights**
1. Data Overview
The dataset includes features such as:
•	Satisfaction Level
•	Last Evaluation
•	Number of Projects
•	Average Monthly Hours
•	Time Spent in Company
•	Work Accidents
•	Promotion in the Last 5 Years
•	Department
•	Salary
•	Retention Status (left - 1 for employees who left, 0 for those who stayed)
2. Exploratory Data Analysis (EDA)
Bar Chart: Salary vs Retention
•	Employees with low salaries are significantly more likely to leave compared to those with medium or high salaries.
Bar Chart: Department vs Retention
•	Retention rates vary across departments. For example, technical roles may have different retention rates compared to sales roles.
Average Metrics Grouped by Retention
Using df.groupby('left').mean(), the following patterns were observed:
•	Satisfaction Level: Lower among employees who left (0.44) compared to those who stayed (0.66).
•	Average Monthly Hours: Higher for employees who left (207) compared to those who stayed (199).
•	Promotions in the Last 5 Years: Employees who received promotions are more likely to stay.
___________________________________________________________________________________________________________________________________________________________
**Logistic Regression Model**
1. Feature Selection
Based on EDA, key features used for the model include:
•	Satisfaction Level
•	Average Monthly Hours
•	Time Spent in Company
•	Salary
2. Model Building
The logistic regression model was built using scikit-learn with the selected features.
3. Model Evaluation
•	The model's accuracy was measured to evaluate its performance.
•	Further metrics such as precision, recall, and F1-score can also be calculated for better assessment.
__________________________________________________________________________________________________________________________________________________________________
**Conclusion**
This project has provided a comprehensive understanding of employee retention through machine learning. By applying a logistic regression model, I have learned how to:
•	Select relevant features based on exploratory data analysis.
•	Train and evaluate a predictive model to identify factors contributing to employee attrition.
The analysis revealed that low satisfaction levels, excessive working hours, and lack of promotions are significant factors affecting retention. Implementing the recommendations can help organizations make data-driven decisions to improve employee satisfaction and reduce turnover. Additionally, the machine learning approach demonstrated the importance of feature selection and model evaluation in deriving actionable insights from data and found out the accuracy of the model.

