# Sales Performance Report Using Power-BI
This report provides an interactive analysis of sales data using **Power BI**  
The data for this report was sourced from **Kaggle**: [Sales in Saudi Arabia](https://www.kaggle.com/datasets/shilton123456/sales-in-saudi-arabia).  
![](Sales-Report.png)
<img src="Sales-Report.png" width="200">


## Steps Performed:

1. **Data Cleaning & Transformation**
- Cleaned and transformed data using **Power Query** to ensure accuracy and consistency.

2. **Data Modeling**
- Created a **Data Model** to define relationships between tables.
   ![](Modeling.png)

3. **Measures & DAX Calculations**
- Built **DAX measures** for key metrics and KPIs, such as:
     Total Sales = SUM('Fact Table'[Total Sales])
     AVG Sales Per Invoice = DIVIDE([Total Sales], [Invoices Count])
     Sales Growth % = DIVIDE([YTD] - [YTD Last Year], [YTD Last Year])
     Customer Satisfaction % = DIVIDE ( AVERAGE ( 'Fact Table'[Customer Satisfaction Score] ), 3 ) * 100

4. **Report Visualization**
   - Designed interactive **Line Charts with Area Shading** to show trends.
   - Added **Forecasting** to project future sales.
   - Applied filters and slicers for **dynamic exploration**, including a professionally formatted **Year filter**.
   - Displayed **Data Labels** only at key points for clarity.
