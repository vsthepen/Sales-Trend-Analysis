# [Project 2: Sales Trend, Product Sales & Sales Team Performance Analysis]

The executive management of Mark Up Foods and Beverages requested for a sales trend and product sales analysis report to enable them gain insights into the top performing and underperforming products, also to evaluate sales team performance between 2019 and 2021. The data was collected in 3 separate excel workbooks for each year. Each workbook contained similar columns such as salesperson, orders, order Date, product group, quantity, unit price, etc. The sales budget data for each year was equally provided. The data was then extracted and transformed using the power query editor.

First Step: I ensured that totals, subtotals, empty rows, and columns were removed from the tables. I also checked that all columns had a first row of descriptive heading. Furthermore, data types for each column were validated to ensure correctness.

Second Step: After the data cleaning process, the three separate tables for each year were appended into one since they had the same exact headers and contained similar information. Thereafter, tables not needed in the model were disabled leaving only one big fact table.

Third step: The data in the fact table was normalized. This resulted in the creation of 2 dimension tables which includes the Product and Salesperson table. I ensured that the dimension tables only contained unique values i.e., duplicates were removed.

Fourth step: The fact and dimension tables were loaded onto the power bi report page. Relationships were created between the tables with the help of unique keys i.e., Salesperson key and Product ID.

Measures such as Total Budgeted Sales, Total Actual Sales, Total Quantity Sold, Rank for Salesperson, % Budgeted sales vs Actual were calculated by using DAX.

Fifth Step:  A sales trend dashboard was built showing the total sales by product group, quarterly & yearly sales trend. This was visualized with the aid of a clustered bar chart and an area chart respectively.

## Sales Trend Dashboard
![MARK UP FOODS AND BEVERAGE-2](https://user-images.githubusercontent.com/115559534/199511693-d1d90215-8f3d-499f-a4ce-02629ca5b818.png)

## INSIGHTS

- Over the past two years, the month of **October** has seen the highest sales revenue.

- **Wheat flour, oil, and yeasts** are the top 3 bestselling products. More than half **(53%)** of the company's sales revenue and **81%** of the total number of products sold come from these three categories.

- **Cassava starch, tea, and tomato sauce** are the three products that performed poorly. **Red wine and energy drinks** round out the list.

## RECOMMENDATIONS

- Since October consistently sees the highest sales revenue, the company should prepare for this peak in demand. This could be in terms of increasing production capacity, launching special promotions, or running targeted marketing campaigns in the lead-up to October.

- Since **Wheat flour, oil, and yeasts** contribute significantly to sales revenue and the total number of products sold, the company should continue to emphasize and invest in these product categories. e.g, expanding product lines by selling multiple variants of these products with varied price ranges or enhancing marketing efforts.

- It's important to understand why **Cassava starch, tea, and tomato sauce** are not performing well. We can investigate other factors such as demand, pricing, quality, and competition. In addition, we can consider if there are opportunities for improvement, price adjustments or marketing efforts to boost sales.

- If **Red wine and energy drinks** continue to underperform, it may be worthwhile to reassess whether they align with the company's customer base. We should consider discontinuing these products if they are not contributing to the company's overall profitability.


A Sales Team dashboard was additionally created to display the Quantity sold by Salesperson, Actual vs Budgeted sales for each person and the Top 3 Salespersons by Sales Amount. A bar chart, line chart and a multi row card were used respectively.

## Sales Team Performance Dashboard
![MARK UP FOODS AND BEVERAGE-3](https://user-images.githubusercontent.com/115559534/199512100-9892749d-2297-41f6-954b-df6cf4f4bc24.png)

## INSIGHTS

- For the past two consecutive years, **Carla Feirrera, Julio Lima, and Gustavo Gomes** have earned the most in sales (based on revenue and quantity of products). They have consistently generated at least 50% of the company's annual revenue.

- **Isabella Souza** has been noted as one of the three lowest underperforming salespersons (based on revenue and target goals).

- At least 3-5 employees surpass their sales target each year.
