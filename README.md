# Sales Performance Report Using Power-BI
## Introduction:
This report provides an interactive analysis of sales data using **Power BI**
The data for this report was sourced from **Kaggle**: [Sales in Saudi Arabia](https://www.kaggle.com/datasets/shilton123456/sales-in-saudi-arabia).  

## Steps Performed:

1. **Data Cleaning & Transformation**
   - Cleaned and transformed data using **Power Query** to ensure accuracy and consistency.

2. **Data Modeling**
   - Created a **Data Model** to define relationships between tables.
   

3. **Measures & DAX Calculations**
   - Built **DAX measures** for key metrics and KPIs, such as:
     ```DAX
     Total Sales = SUM(Sales[Amount])
     Total Quantity = SUM(Sales[Quantity])
     Sales Growth % = DIVIDE([Total Sales] - [Previous Year Sales], [Previous Year Sales], 0)
     Previous Year Sales = CALCULATE([Total Sales], SAMEPERIODLASTYEAR(Date[Date]))
     ```

4. **Report Visualization**
   - Designed interactive **Line Charts with Area Shading** to show trends.
   - Added **Forecasting** to project future sales.
   - Applied filters and slicers for **dynamic exploration**, including a professionally formatted **Year filter**.
   - Displayed **Data Labels** only at key points for clarity.
