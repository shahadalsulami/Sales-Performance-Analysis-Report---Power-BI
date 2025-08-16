## **Sales Performance Report Using Power BI**  
This report provides an interactive analysis of sales data using **Power BI**.  
The dataset was sourced from **Kaggle**: [Sales in Saudi Arabia](https://www.kaggle.com/datasets/shilton123456/sales-in-saudi-arabia).  

<img src="Sales-Report.png" width="600">

### **Steps Performed**

### **1. Data Cleaning & Transformation**  
- Cleaned and transformed the data using **Power Query** to ensure accuracy and consistency

### **2. Data Modeling**  
- Created a **Data Model** to define relationships between tables  


### **3. Measures & DAX**  
Built **DAX measures** for key metrics and KPIs, such as:  

- Total Sales = SUM('Fact Table'[Total Sales])  
- AVG Sales Per Invoice = DIVIDE([Total Sales], [Invoices Count])  
- Sales Growth % = DIVIDE([YTD] - [YTD Last Year], [YTD Last Year])  
- Sales Target = [Total Sales] * 1.1
- Customer Satisfaction % = DIVIDE(AVERAGE('Fact Table'[Customer Satisfaction Score]), 3) * 100  

### **4. Report Visualization**
Created interactive visuals with forecasting to highlight trends and support data-driven insights
