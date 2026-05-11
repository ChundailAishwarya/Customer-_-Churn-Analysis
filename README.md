# Customer-_-Churn-Analysis
CUSTOMER CHURN ANALYSIS DASHBOARD USING POWER BI

*PROJECT OVERVIEW

This project focuses on analyzing customer churn data using Microsoft Power BI.
The dashboard provides interactive visual insights into customer behavior, churn patterns, contract types, payment methods, customer satisfaction, support calls, and revenue-related metrics.
The objective of this project is to:
Identify factors contributing to customer churn
Track important customer KPIs
Build an interactive business intelligence dashboard
Generate actionable insights for retention strategies
*DATASET

The dataset contains customer-related information such as:
Customer demographics
Gender
Age
Contract type
Internet service
Payment method
Monthly charges
Total charges
Satisfaction score
Support calls
Tenure
Churn status
*TOOLS & TECHNOLOGIES

Microsoft Power BI
DAX (Data Analysis Expressions)
Power Query
CSV Dataset
*STEPS PERFORMED

1. Import Dataset into Power BI
Open Microsoft Power BI Desktop
Click Home → Get Data → Text/CSV
Select the customer churn dataset
Load the dataset into Power BI
*DASHBOARD VISUALIZATION

3. Table Visual – Customer Details
Created a Table Visual to display:
Customer ID
Gender
Age
Contract Type
Internet Service
Payment Method
Monthly Charges
Tenure
Satisfaction Score
Churn Status
4. Card Visual – Total Customers
Created a KPI card showing the total number of customers.
DAX Measure
DAX
Total Customers =
COUNTROWS('customer_churn_dataset')
5. Card Visual – Churn Customers
Created a KPI card showing total churned customers.
DAX Measure
DAX
Churn Customers =
CALCULATE(
    COUNTROWS('customer_churn_dataset'),
    'customer_churn_dataset'[Churn] = "Yes"
)
6. Card Visual – Average Monthly Charges
Created a KPI card showing average monthly charges.
DAX Measure
DAX
Average Monthly Charges =
AVERAGE('customer_churn_dataset'[MonthlyCharges])
7. Pie Chart – Churn Status
Created a pie chart to visualize:
Churn = Yes
Churn = No
This helps understand the overall churn distribution.
8. Bar Chart – Churn by Contract Type
Created a bar chart comparing churn customers across:
Month-to-Month
One Year
Two Year contracts
Insight
Month-to-Month contracts usually show higher churn rates.
9. Column Chart – Internet Service vs Total Customers
Created a column chart displaying total customers by:
Fiber Optic
DSL
No Internet Service
10. Line Chart – Tenure vs Total Charges
Created a line chart to analyze:
Customer tenure
Total revenue contribution
Insight
Customers with higher tenure generally contribute more revenue.
*INTERACTIVE SILCERS
11. Gender Slicer
Added a slicer for:
Male
Female
12. Contract Type Slicer
Added slicer for:
Month-to-Month
One Year
Two Year
13. Internet Service Slicer
Added slicer for:
DSL
Fiber Optic
No Service
*BUSINESS ANALYSIS QUESTIONS
14. Which Payment Method Has the Highest Churn?
Analyzed churn across payment methods.
Insight
Electronic Check customers generally have the highest churn rate.
15. Do Support Calls Affect Churn?
Compared:
Number of support calls
Churn behavior
Insight
Customers with higher support calls tend to churn more frequently.
16. Does Satisfaction Score Affect Churn?
Analyzed satisfaction score against churn.
Insight
Lower satisfaction scores are strongly associated with higher churn.
17. Average Tenure of Churned Customers
DAX Measure
DAX
Average Tenure Churned =
CALCULATE(
    AVERAGE('customer_churn_dataset'[Tenure]),
    'customer_churn_dataset'[Churn] = "Yes"
)
18. Highest Monthly Charge
DAX Measure
DAX
Highest Monthly Charge =
MAX('customer_churn_dataset'[MonthlyCharges])
19. Lowest Satisfaction Score
DAX Measure
DAX
Lowest Satisfaction Score =
MIN('customer_churn_dataset'[SatisfactionScore])
20. Churn Rate Percentage
DAX Measure
DAX
Churn Rate % =
DIVIDE(
    [Churn Customers],
    [Total Customers],
    0
) * 100
21. Which Age Group Has the Highest Churn?
Created age groups such as:
18–25
26–35
36–45
46–60
60+
Insight
Young and middle-aged customers often show higher churn rates.
*FINAL DASHBOARD FEATURES
The final interactive dashboard includes:
KPI Cards
Pie Charts
Bar Charts
Column Charts
Line Charts
Interactive Slicers
Customer Segmentation
Churn Analysis
Revenue Insights
*KEY INSIGHTS
Month-to-Month contracts have the highest churn
Electronic Check payment users churn more
Low satisfaction scores increase churn probability
More support calls indicate dissatisfaction
Long-term customers generate higher revenue
Fiber Optic users may show higher churn depending on pricing
*CONCLUSION
This Power BI dashboard provides a complete customer churn analysis solution that helps businesses:
Understand customer behavior
Improve retention strategies
Identify high-risk customers
Monitor revenue impact
Make data-driven decisions
*FUTURE IMPROVEMENTS
Possible future enhancements:
Predictive churn modeling using Machine Learning
Real-time dashboard updates
Customer lifetime value analysis
Advanced segmentation
Automated reporting
AISHWARYA
Customer Churn Analysis Dashboard Project using Microsoft Power BI and DAX.
