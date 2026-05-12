Customer Churn Analysis Dashboard – Power BI

📌 Project Overview

This project focuses on analyzing customer churn data using Microsoft Power BI.
The dashboard provides interactive visual insights into customer behavior, churn trends, payment methods, customer satisfaction, support calls, tenure, and service usage.
The main objective of this project is to help businesses identify the major factors contributing to customer churn and support data-driven decision-making.

📂 Dataset Information

The dataset contains customer-related information such as:

•Customer ID

•Gender

•Age Group

•Contract Type

•Internet Service

•Monthly Charges

•Total Charges

•Tenure

•Payment Method

•Support Calls

•Satisfaction Score

•Churn Status

🛠 Tools & Technologies Used
Microsoft Power BI

Power Query
DAX (Data Analysis Expressions)

•Microsoft Power BI

•Power Query

•DAX (Data Analysis Expressions) 


📊 Dashboard Features
✅ Visualizations Created

Table Visual

Displays all customer details including:

•Customer ID

•Gender

•Contract Type

•Internet Service

•Monthly Charges

•Total Charges

•Tenure

•Churn Status


1)KPI Cards

The dashboard contains KPI cards for:
•Total Customers

•Churn Customers

•Average Monthly Charges

•Churn Rate %


2)Charts & Visuals

 Pie Chart

    •Churn Status (Yes / No)


Bar Chart

    •Churn by Contract Type
 Column Chart

    •Internet Service vs Total Customers

 Line Chart

    •Tenure vs Total Charges

3)Slicers Added

Interactive slicers were created for:
•Gender

•Contract Type

•Internet Service

These slicers allow dynamic filtering across all dashboard visuals.


📈 Business Analysis Performed

🔹 Payment Method with Highest Churn:
Analyzed which payment method contributes to the highest customer churn.

🔹 Support Calls vs Churn:
Studied whether customers making more support calls are more likely to churn.

🔹 Satisfaction Score vs Churn:
Analyzed how customer satisfaction impacts churn behavior.

🔹 Average Tenure of Churned Customers:
Calculated the average duration customers stay before churning.

🔹 Highest Monthly Charge:
Identified the maximum monthly charge among all customers.

🔹 Lowest Satisfaction Score:
Identified the minimum customer satisfaction score.

🔹 Age Group with Highest Churn:
Analyzed which customer age category has the highest churn percentage.


🧮 DAX Measures Used

*Total Customers:
     Total Customers = COUNT(CustomerChurn[CustomerID])

*Churn Customers:
     Churn Customers =
CALCULATE(
    COUNT(CustomerChurn[CustomerID]),
    CustomerChurn[Churn] = "Yes"
)

*Churn Rate %:
     Churn Rate % =
DIVIDE([Churn Customers], [Total Customers], 0) * 100

*Average Monthly Charges:
     Average Monthly Charges =
AVERAGE(CustomerChurn[MonthlyCharges])


📌 Key Insights

•Customers with month-to-month contracts showed higher churn rates.

•Certain payment methods experienced significantly higher churn.

•Lower satisfaction scores were strongly associated with churned customers.

•Customers with frequent support calls had a greater tendency to churn.

•Specific age groups showed higher churn percentages compared to others.



🎯 Project Outcome

The interactive dashboard enables businesses to:

•Monitor customer churn trends

•Understand customer behavior

•Improve customer retention strategies

•Identify high-risk customer segments

•Make data-driven business decisions


🚀 How to Use

1)Download the .pbix file.

2)Open it using Microsoft Power BI Desktop.

3)Refresh the dataset if needed.

4)Use slicers to interact with dashboard visuals.



📁 Project Structure

  Customer-Churn-Analysis/
│
├── Customer_Churn_Dashboard.pdf
├── customer_churn_dataset.csv
├── dashboard.png
└── README.md


📚 Learning Outcomes

Through this project, I learned:

•Data cleaning and transformation in Power BI

•Creating interactive dashboards

•Writing DAX measures

•Performing customer churn analysis

•Building business intelligence reports


⭐ Conclusion

This Power BI Customer Churn Analysis Dashboard provides meaningful insights into customer retention and churn behavior.
The project demonstrates how business intelligence tools can transform raw data into actionable insights for organizations.





