# Sales Dashboard
### Sales Analysis by Product Color & Category Dashboard using **Power BI**
![dashboard1](https://github.com/ThuyTran102/Sales-Analysis-by-Color-and-Product-Category_Dashboard/blob/main/images/Sales%20Analysis%20by%20Color%20and%20Product%20Category%20(Power%20BI).png)

## Table of Contents:
- [Project Objectives](https://github.com/ThuyTran102/Sales-Analysis-by-Color-and-Product-Category_Dashboard?tab=readme-ov-file#project-objectives)
- [Data Preparation](https://github.com/ThuyTran102/Sales-Analysis-by-Color-and-Product-Category_Dashboard?tab=readme-ov-file#data-preparation)
- [Data Modeling](https://github.com/ThuyTran102/Sales-Analysis-by-Color-and-Product-Category_Dashboard?tab=readme-ov-file#data-modeling)
- [Data Analysis (DAX)](https://github.com/ThuyTran102/Sales-Analysis-by-Color-and-Product-Category_Dashboard?tab=readme-ov-file#data-analysis-dax)
- [Data Visualization (Dashboard)](https://github.com/ThuyTran102/Sales-Analysis-by-Color-and-Product-Category_Dashboard?tab=readme-ov-file#data-visualization-dashboard)
- [Insights](https://https://github.com/ThuyTran102/Sales-Analysis-by-Color-and-Product-Category_Dashboard?tab=readme-ov-file#insights)
- [Recommendations](https://https://github.com/ThuyTran102/Sales-Analysis-by-Color-and-Product-Category_Dashboard?tab=readme-ov-file#recommendations)
- [Interpretation of each charts](https://github.com/ThuyTran102/Sales-Analysis-by-Color-and-Product-Category_Dashboard?tab=readme-ov-file#interpretation-and-basic-analysis-of-each-charts)


## Project Objectives:
- Analyze sales performance across product colors and categories over time periods.  
- Identify key revenue drivers and profitability trends.  
- Support strategic decision-making through data-driven insights.  
- Improve inventory management and marketing strategies by understanding sales patterns.


## Data Preparation:
Data transformation was done in Power Query and the dataset was loaded into Microsoft Power BI Desktop for modeling.
- Ensure all columns are formatted correctly (e.g., numeric data as decimals, dates as date types).
- Handle missing or incorrect data using Power Query (replace, remove, or impute values).

## Data Modeling:
After the dataset was cleaned and transformed, it was ready to be modeled.
A star schema data model with the following relationships is shown below:

| Model view |
| ----------- |
|![model](https://github.com/ThuyTran102/Sales-Analysis-by-Color-and-Product-Category_Dashboard/blob/main/images/model.png)|

#### Purpose of the Model
This structure supports analytics by combining sales with product, customer, geographic, and time dimensions.

#### Relationships in the Data Model

1. **Products Table ↔ Sales Table**  
   - The `ProductKey` in the **Products** table is linked to the `ProductKey` in the **Sales** table.  
   - This relationship allows tracking of sales data for each product, such as `SalesAmount`, `OrderQuantity`, and `UnitPrice`.

2. **Customers Table ↔ Sales Table**  
   - The `CustomerKey` in the **Customers** table is linked to the `CustomerKey` in the **Sales** table.  
   - This relationship provides customer details, like `YearlyIncome`, `MaritalStatus`, and `Gender`, associated with specific sales.

3. **Territory Table ↔ Sales Table**  
   - The `SalesTerritoryKey` in the **Sales** table is linked to the `TerritoryKey` in the **Territory** table.  
   - This connection helps identify the geographic or regional details of sales, such as `Country`, `Region`, and `Group`.

4. **Calendar Table ↔ Sales Table**  
   - The `OrderDate` in the **Sales** table is linked to the `Date` in the **Calendar** table.  
   - This allows for time-based analysis of sales, including metrics by `MonthName`, `FiscalYear`, or `CalendarQuarter`.




## Data Analysis (DAX):
Measures used in all visualization are:
<p align="center" style="margin-top: 20px; margin-bottom: 20px;">
<img width="20%" src="https://github.com/ThuyTran102/Sales-Analysis-by-Color-and-Product-Category_Dashboard/blob/main/images/key_measures.png" alt="Outcome"></img>
</p>


## Data Visualization (Dashboard):
Data visualization for the data analysis (DAX) was done in Microsoft Power BI Desktop:

| Dashboard |
| ----------- |
|![dashboard1](https://github.com/ThuyTran102/Sales-Analysis-by-Color-and-Product-Category_Dashboard/blob/main/images/Sales%20Analysis%20by%20Color%20and%20Product%20Category%20(Power%20BI).png)|


## Insights:
1.	 **Bikes** account for the majority of the total revenue (96.46%), while **Accessories** and **Clothing** contribute only marginally.
2.	Product colors show significant differences in revenue contribution: **black** and **red** **dominate** **but** recorded **declines in 2019**.
3.	Overall revenue grew strongly from 2016 to 2018 but plateaued in 2019, primarily due to a decline in sales growth of **Bikes in black and red** (This was the company's super-star product before).


## Recommendations:
1.	**Diversify the product portfolio**: Develop "Accessories" and "Clothing" categories to reduce reliance on "Bikes."
2.	**Analyze color demand**: Focus on trending colors like **yellow** and **blue** instead of over-relying on **black** and **red**.
3.	**Investigate the 2019 decline**: Conduct an in-depth analysis of causes and propose strategies for recovery in subsequent years.


## Interpretation and Basic Analysis of each Charts 
<p align="center" style="margin-top: 20px; margin-bottom: 20px;">
<img width="75%" src="https://github.com/ThuyTran102/Sales-Analysis-by-Color-and-Product-Category_Dashboard/blob/main/images/Interpretation1.png" alt="Outcome"></img>
</p>
<p align="center" style="margin-top: 20px; margin-bottom: 20px;">
<img width="75%" src="https://github.com/ThuyTran102/Sales-Analysis-by-Color-and-Product-Category_Dashboard/blob/main/images/Interpretation2.png" alt="Outcome"></img>
</p>
<p align="center" style="margin-top: 20px; margin-bottom: 20px;">
<img width="75%" src="https://github.com/ThuyTran102/Sales-Analysis-by-Color-and-Product-Category_Dashboard/blob/main/images/Interpretation3.png" alt="Outcome"></img>
</p>
<p align="center" style="margin-top: 20px; margin-bottom: 20px;">
<img width="75%" src="https://github.com/ThuyTran102/Sales-Analysis-by-Color-and-Product-Category_Dashboard/blob/main/images/Interpretation4.png" alt="Outcome"></img>
</p>
<p align="center" style="margin-top: 20px; margin-bottom: 20px;">
<img width="75%" src="https://github.com/ThuyTran102/Sales-Analysis-by-Color-and-Product-Category_Dashboard/blob/main/images/Interpretation5.png" alt="Outcome"></img>
</p>

