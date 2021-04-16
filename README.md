# Excel: Kickstart My Chart

## Goal:

Organize and analyze 4,000 past Kickstarter projects in order to discover trends and gain insight as to why some Kickstarters fail and others succeed.


## Process:
#### CONDITIONAL FORMATTING

Use conditional formatting to color-code the `state` column by the status of each campaign (successful, failed, cancelled, currently live), and color-code the `Percent Funded` column using a three-color scale.

#### FORMULAS

Used different formulas to:
* Calculate the proportion a campaign was funded (`Percent Funded`) and average donation amount of each backer (`Average Donation`).
* Split the `Category and Sub-Category` column into two new columns based on the specified delimiter.
* Convert Unix timestamps in `deadline` and `launched_at` columns to normal dates in `Date_Created_Conversion` and `Date_Ended` columns.
* Count (`COUNTIFS()`), sum, and calculate percentages of campaign states (successful, failed, cancelled) based on goal range. Create a line chart based on the table.

#### PIVOT TABLES AND CHARTS
* Create pivot table and accompanying chart to count how many campaigns were successful, failed, canceled, or currently live per **category**.
* Create pivot table and accompanying chart to count how many campaigns were successful, failed, canceled, or currently live per **sub-category**.
* Create pivot table and accompanying chart based on count of `State` and `Date_Created_Conversion`, filterable by **parent-category** and **year**.

#### STATISTICAL ANALYSIS

Compare the relationship between backers and campaign outcome (success or failure)
* Mean number of backers
* Median number of backers
* Minimum number of backers
* Maximum number of backers
* Variance of the number of backers
* Standard deviation of the number of backers 
