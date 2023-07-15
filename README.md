## Linear Regression to Predict MPG

The linear regression analysis was performed to predict the MPG (miles per gallon) values of MechaCar prototypes using multiple variables. The summary output from the linear regression model provides insights into the significance of the variables and the overall effectiveness of the model.

### Summary Output:

Please refer to the screenshot below for the summary output from the linear regression model:

[![Linear Regression Summary Output](https://github.com/Jeantherapy/MechaCar_Statistical_Analysis/blob/main/Images/Summary%20Model.png)

### Non-Random Amount of Variance:

From the summary output, we can determine which variables/coefficients provided a non-random amount of variance to the MPG values in the dataset by examining their corresponding p-values. Variables with p-values less than the chosen significance level (usually 0.05) are considered statistically significant and provide a non-random amount of variance to the response variable.

### Slope of the Linear Model:

The slope of the linear model is not considered to be zero. If the p-value for the coefficient of a variable is less than the significance level, it suggests that the variable has a significant linear relationship with the response variable. A non-zero slope indicates that the variable contributes to the prediction of the response variable.

### Effectiveness of the Linear Model:

The effectiveness of the linear model in predicting the MPG of MechaCar prototypes can be evaluated based on the coefficient of determination (R-squared value) and other metrics. The R-squared value represents the proportion of variance in the response variable that is explained by the model. A higher R-squared value indicates a better fit of the model to the data.

Additionally, the significance of individual variables (based on their p-values) and other diagnostic measures should be considered to assess the overall effectiveness of the model. If the model has significant variables, low p-values, and meets the assumptions of linear regression, it can be considered effective in predicting the MPG values.

It is recommended to thoroughly analyze the summary output, including the p-values, R-squared value, and diagnostic measures, to make a comprehensive assessment of the model's predictive capabilities for MechaCar prototypes.# MechaCar_Statistical_Analysis

## Summary Statistics on Suspension Coils

The summary statistics on the suspension coils provide insights into whether the manufacturing data meets the design specification of a variance not exceeding 100 pounds per square inch (PSI) for all manufacturing lots in total and each lot individually. We will examine both the `total_summary` and `lot_summary` dataframes to address this question.

### Total Summary:

Please refer to the screenshot below for the `total_summary` dataframe:

![Total Summary](https://github.com/Jeantherapy/MechaCar_Statistical_Analysis/blob/main/Images/Total%20Summary.png)

From the `total_summary` dataframe, we can observe the mean, median, variance, and standard deviation of the suspension coils' PSI values across all manufacturing lots. 

### Lot Summary:

Please refer to the screenshot below for the `lot_summary` dataframe:

![Lot Summary](https://github.com/Jeantherapy/MechaCar_Statistical_Analysis/blob/main/Images/Lot%20Summary.png)

The `lot_summary` dataframe provides the same summary statistics but grouped by each manufacturing lot. 

### Compliance with Design Specification:

To determine whether the manufacturing data meets the design specification of a variance not exceeding 100 PSI, we need to examine the variance values from both the `total_summary` and `lot_summary` dataframes.

If the variance of the suspension coils' PSI values is less than or equal to 100 PSI for both the `total_summary` and each individual lot in the `lot_summary`, then the manufacturing data meets the design specification.

However, if any of the variance values exceed 100 PSI, it indicates that the manufacturing process is not meeting the design specification for that particular manufacturing lot or in total.

By comparing the variance values from the summary statistics, we can determine whether the current manufacturing data meets the design specification for all manufacturing lots in total and each lot individually.

Please refer to the screenshots provided to examine the variance values in the `total_summary` and `lot_summary` dataframes and assess whether the manufacturing data meets the design specification.


## T-Tests on Suspension Coils

The t-tests on the suspension coils were performed to determine if the PSI (pounds per square inch) values across all manufacturing lots and for each manufacturing lot individually are statistically different from the population mean of 1,500 pounds per square inch. The following summary provides an interpretation of the t-test results:

### Summary of Interpretation and Findings:

Please refer to the screenshots below for the t-test results:

**T-Test for All Manufacturing Lots:**

![T-Test for All Lots](https://github.com/Jeantherapy/MechaCar_Statistical_Analysis/blob/main/Images/All%20Lots.png)

The t-test conducted on the PSI values across all manufacturing lots showed a p-value of 0.06. Since the p-value is above the significance level (e.g., 0.05), we fail to reject the null hypothesis. this suggests a marginally significant difference between the overall PSI values and the population mean of 1,500 PSI.

**T-Tests for Each Manufacturing Lot:**

* Manufacturing Lot 1:
![T-Test for Lot 1](path/to/t_test_lot1.png)

* Manufacturing Lot 2:
![T-Test for Lot 2](path/to/t_test_lot2.png)

* Manufacturing Lot 3:
![T-Test for Lot 3](path/to/t_test_lot3.png)

The t-tests conducted on each manufacturing lot individually showed the following results:

Lot 1: The p-value for Lot 1 is 1.00. This suggests that the PSI values for Lot 1 are not statistically different from the population mean of 1,500 PSI. There is no evidence to reject the null hypothesis that the mean PSI for Lot 1 is equal to 1,500 PSI.

Lot 2: The p-value for Lot 2 is 0.06. With a significance level of 0.05, this indicates a marginally significant difference between the PSI values for Lot 2 and the population mean of 1,500 PSI. However, additional analysis or consideration may be required to draw a definitive conclusion.

Lot 3: The p-value for Lot 3 is 0.04. With a significance level of 0.05, this suggests that the PSI values for Lot 3 are statistically different from the population mean of 1,500 PSI. There is evidence to reject the null hypothesis and conclude that the mean PSI for Lot 3 is not equal to 1,500 PSI.
### Summary:

Based on the t-test results, we can conclude the following:

The t-test results indicate that Lot 3 shows a statistically significant difference in the PSI values compared to the population mean of 1,500 PSI. Lot 2 and the overall dataset also show a marginal difference, suggesting the need for further investigation. However, Lot 1 does not exhibit a significant difference. These findings emphasize the importance of analyzing each lot separately to understand the variation in PSI values and their adherence to the design specification.

## Study Design: MechaCar vs Competition

In this study, we aim to quantify how the MechaCar performs against its competitors using various metrics that are of interest to consumers. We will focus on the metrics of cost, fuel efficiency (both city and highway), and safety rating.

### Metrics to Test:
1. Cost: The cost of the MechaCar compared to competitors' cars in a similar category.
2. Fuel Efficiency: Both city and highway fuel efficiency to assess the MechaCar's performance in terms of gas mileage compared to competitors.
3. Safety Rating: The safety rating of the MechaCar in comparison to competitors' vehicles to evaluate its safety features and performance.

### Hypotheses:
Null Hypothesis (H0): There is no significant difference between the MechaCar and competitors in terms of cost, fuel efficiency, and safety rating.
Alternative Hypothesis (HA): The MechaCar exhibits a significant difference compared to competitors in terms of cost, fuel efficiency, and safety rating.

### Statistical Test:
To test the hypotheses, we can use a combination of statistical tests depending on the nature of the data and the specific metrics being analyzed. 

1. Cost: A two-sample t-test or a non-parametric test (such as Mann-Whitney U test) can be used to compare the cost of the MechaCar with competitor vehicles. These tests will help determine if there is a statistically significant difference in cost between the MechaCar and its competitors.
 
2. Fuel Efficiency: For fuel efficiency, we can use a two-sample t-test or a non-parametric test to compare the average city and highway fuel efficiency of the MechaCar with competitors. These tests will provide insights into whether the MechaCar's fuel efficiency differs significantly from competitors' vehicles.

3. Safety Rating: To compare the safety ratings, we can use a chi-square test or Fisher's exact test to assess if there is a significant difference in safety ratings between the MechaCar and competitors.

The choice of statistical test will depend on the nature of the data and assumptions made about the distribution of the variables being analyzed.

### Data Needed:
To run the statistical tests, we would need data on the cost, fuel efficiency (city and highway), and safety ratings of the MechaCar as well as comparable data for competitors' vehicles. This data could be obtained from reliable sources such as industry reports, government safety ratings, or consumer reviews that provide standardized and comparable information on the metrics of interest.

By collecting and analyzing this data, we can perform the appropriate statistical tests to determine if the MechaCar performs significantly differently from its competitors in terms of cost, fuel efficiency, and safety rating. These findings would provide valuable insights to consumers and help assess the competitiveness of the MechaCar in the market.
