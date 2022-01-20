# Explore Plotting with Excel

For your first assignment, you’ll combine all the Excel concepts that the module covered today into a complete analysis workflow.

Specifically, you’ll summarize and visualize a dataset that contains Amazon product orders. The dataset contains order IDs, product names, categories, selling prices, shipping weights, shipping methods, and shipping prices. Note that the selling prices determine the shipping prices, as the following table shows:

| Selling Price | Shipping Price |
| --- | --- |
| $0.00 &ndash; $50.00 | $10.00 |
| $50.01 &ndash; $90.00 | $5.00 |
| $90.01 &ndash; $149.99 | $2.50 |
| $150.00 or more | $0.00 |


The data for this assignment is from the  [Amazon Product Dataset 2020 from data.world](https://data.world/promptcloud/amazon-product-dataset-2020) and has been modified by using Python and Pandas.

## Instructions
Open the `ProductionPivot_Unsolved.xlsx` file and complete the following steps:

1. Create a new column named Total Price that adds the Selling Price and Shipping Price columns together, as the following image shows:

    ![A screenshot depicts a Total Price column of sums in Column H.](Images/01-TotalPriceColumn.png)

2. Create the first pivot table as follows: use the data on the Orders sheet to calculate the total number of products (that is, the count) for each category in the Category column, and then order the number of products per category from highest to lowest.

    **Note:** You should get a grand total of 1501 products across all categories, as the following image shows:

    ![A screenshot depicts the first pivot table, which includes the counts of products per category.](Images/02-ProductsPerCategoryPivot.png)

3. Return to the original Orders sheet, and then create a second pivot table that calculates the total number of products for each shipping method, as the following image shows:

    ![A screenshot depicts the second pivot table, which includes the counts of products per shipping method.](Images/03-ProductsPerShippingMethodPivot.png)

4. Using the data from second pivot table that you just created, create a plot that visualizes the number of products by shipping method&mdash;specifically, by Standard, 2-day, and Prime, as the following image shows:

    ![A screenshot depicts a bar chart of products by shipping method.](Images/04-ProductsPerShippingMethodChart.png)

5. Return to the original Orders sheet, and then create a third pivot table that does the following:

    * Calculates the sum of the total prices for each combination of category and shipping method.

    * Orders the sum of the total prices for each category from highest to the lowest. Then, filters the pivot table to display only the top five categories based on the sums of the total prices, where a minimum of 10 products have been ordered, as the following image shows:

      ![A screenshot depicts the third pivot table.](Images/05-TotalPricePivot.png)

      **Hint:** Use the first pivot table that you created to determine which categories have a minimum of 10 products that have been ordered.

6. Using the data from the filtered pivot table that you just created, create a bar chart that visualizes the total price for each combination of category and shipping method, as the following image shows:

    ![A screenshot depicts this bar chart.](Images/06-TotalPriceChart.png)

7. Return to the original Orders sheet, and then create one last pivot table that does the following:

    * Calculates the average of the total prices for each combination of category and shipping method.

    * Orders the average of the total prices for each category from highest to the lowest. Then, filters the pivot table to display only the top five categories based on the average of the total prices, where a minimum of 10 products have been ordered, as the following image shows:

      ![A screenshot depicts the fourth pivot table.](Images/07-AvgPricePivot.png)

8. Using the data from the filtered pivot table that you just created, create a bar chart that visualizes the average price for each combination of category and shipping method, as the following image shows:

    ![A screenshot depicts this bar chart.](Images/08-AvgPriceChart.png)

## Grading Rubric

[Explore Plotting with Excel Rubric](Explore_Plotting_with_Excel_Rubric.pdf)

---

© 2022 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.
