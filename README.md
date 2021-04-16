# Excel: Kickstarter

## Goal:

Organize and analyze 4,000 past Kickstarter projects in order to discover trends and gain insight as to why some Kickstarters fail and others succeed.


## Process:
#### CONDITIONAL FORMATTING

Use conditional formatting to color-code the `state` column by the status of each campaign (successful, failed, cancelled, currently live), and color-code the `Percent Funded` column using a three-color scale.
![](https://github.com/lorijta92/excel-kickstarter-data/blob/master/Images/img_01.png?raw=true)

#### FORMULAS

Used different formulas to:
* Calculate the proportion a campaign was funded (`Percent Funded`) and average donation amount of each backer (`Average Donation`).
* Split the `Category and Sub-Category` column into two new columns based on the specified delimiter.
* Convert Unix timestamps in `deadline` and `launched_at` columns to normal dates in `Date_Created_Conversion` and `Date_Ended` columns.

![](https://github.com/lorijta92/excel-kickstarter-data/blob/master/Images/img_06.png?raw=true)

* Count (`COUNTIFS()`), sum, and calculate percentages of campaign states (successful, failed, cancelled) based on goal range. Create a line chart based on the table.
![](https://github.com/lorijta92/excel-kickstarter-data/blob/master/Images/img_05.png?raw=true)

#### PIVOT TABLES AND CHARTS
* Create pivot table and accompanying chart to count how many campaigns were successful, failed, canceled, or currently live per **category**.
![](https://github.com/lorijta92/excel-kickstarter-data/blob/master/Images/img_02.png?raw=true)
* Create pivot table and accompanying chart to count how many campaigns were successful, failed, canceled, or currently live per **sub-category**.
![](https://github.com/lorijta92/excel-kickstarter-data/blob/master/Images/img_03.png?raw=true)
* Create pivot table and accompanying chart based on count of `State` and `Date_Created_Conversion`, filterable by **parent-category** and **year**.
![](https://github.com/lorijta92/excel-kickstarter-data/blob/master/Images/img_04.png?raw=true)

#### STATISTICAL ANALYSIS

Compare the relationship between backers and campaign outcome (success or failure)
* Mean number of backers
* Median number of backers
* Minimum number of backers
* Maximum number of backers
* Variance of the number of backers
* Standard deviation of the number of backers 
![](https://github.com/lorijta92/excel-kickstarter-data/blob/master/Images/img_07.png?raw=true)

## Conclusions:
1. The parent category, “Theater” has the highest count of successful Kickstarters, and of that, “Plays” is the most successful sub-category. However, the parent category, “Music,” has the highest percentage rate of success. Based on this, one can conclude that arts-based Kickstarters are the most popular among backers and have the best chance of success.

2. Kickstarters had the highest count of success between April and June, which would suggest that the best time to launch a Kickstarter would be in the springtime. Conversely, there is a sharp from November to December, suggesting that the holiday season would be the worst time to launch a Kickstarter.

3. Campaigns with the highest success percentage had a lower fundraising goal. The higher the goal, the less success there was, with a sharp drop at the $45,000 mark. To increase the chances of a successful Kickstarter, one should set a goal of $4999 or less.

## Limitations:
This dataset does not give insight into individual backers, such as their motive for donating or not, annual income, and other living expenses. There could be a correlation between having more disposable income and the likelihood of donating, or between seasonal expenses (such as gift expenses during Christmas) and the lack of donating to Kickstarters.

This dataset also does not include information on the inherent qualities of each campaign. Did any campaigns provide reward programs? What sort of rewards were backers given and were there any commonalities between the rewards? For example, did campaigns that offered backers early access to a product have a higher rate of success? Or perhaps there was a correlation between the way a campaign was advertised that was particularly successful? Having information on how each campaign was presented would aid in more informative insights. 

Finally, I would have also liked to have seen information on the campaign starters themselves. Perhaps there was a correlations between the size of one’s network (family, friends, coworkers, acquaintances, etc.) and the success rate. I believe it is highly unlikely that every single backer of the 4000+ campaigns judged the campaigns solely on its merits alone, but there is no way to draw any informed conclusion on the matter.
