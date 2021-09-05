# An Analysis of Kickstarter Campaign

## Overview of Project
Louise has recently successfully concluded crowdfunding campaign for the play "Fever". The estimated cost of the play is $10,000. 

Post the campaign Louise wanted to analyze historical Kickstarter campaign data in order to better understand what were the factors, if any, that contributed towards success or failure of a crowdfunding campaign

### Purpose
This report aim to review the historical data of the Kickstarter campaigns and analyse if:
- The launch date of the campaigns was contributing factor in campaign being failed vs successful
- The target goal of the campaigns contributed in success or failure of the campaigns

## Analysis and Challenges
From the Kickstarter data, the campaigns with similar sub category as to play "Fever" were selected to be analyzed. Further, outcomes based on launch date and campaign goal size were analysed.

### Analysis of Outcomes Based on Launch Date
In the theater category total of 1369 campaigns were launched, out of those 61% or 839 campaigns were successful. Most of the campaigns were launched during the months of May to August (Please refer to line graph below)

![Theater Outcomes Based on Launch Date](https://github.com/div1085/kickstarter-analysis/blob/65ace00083f249d75a65286b3306f5b7a156d701/Resources/Theater_Outcomes_vs_Launch.png)

Based on the graph above, most successful campaigns (111) were launched in the month of May, followed by month of June in which 100 successful campaigns were launched. However, corresponding to it, most failed campaigns were also launched in the months of May and June with 166 and 153 failed campaign respectively.

### Analysis of Outcomes Based on Goals
As per the line chart below, in the theater category campaigns below 5000 dollars are most successful, whereas campaigns above 25000 dollars are most likely to fail.

![Outcomes Based on Goals](https://github.com/div1085/kickstarter-analysis/blob/387f2081dce55527f9c6ca046fe356595ddceae7/Resources/Outcomes_vs_Goals.png)

Although campaigns between 35000 to 45000 dollars have success rate of 67%, they do not truly reflect the trend as number of campaigns are very less, only 9, out of 1047 total campaigns. If we ignore these outlier, we can observe the 'failed' line trending downwards are the campaign goals are increasing almost reaching to 100% failure rate in campaigns greater than 45000 dollars.
  
### Challenges and Difficulties Encountered
Few of the challenges faced during the analysis were:
1. The sheer quantity of data can be overwhelming. The problem can be overcome by utilizing excel functions such as pivot table to sort and refine, and ifs function to extract data frequency to be analyzed.
2. Representing information in graphical form and using graphs and charts to interpret the data.
3. Prior to utilizing the data it needs to be sanitized for use. For example, while doing the analysis above, only data from theater subcategory was selected, and then further information was extracted such as converting time stamps to date.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
	1. The best months to launch the campaigns are from May to August, with May being the best month over the years.
	2. The 'successful' and 'failed' lines in the graph have similar trajectory. Both lines follow the similar upward trend in months on February, May, and October and downward trend in months of March, July, August and September. Both lines almost converge in the month of December. Biggest distance between the two lines are in the months of May, June, and July where successful is trending downwards and failed category has plateau a bit.

- What can you conclude about the Outcomes based on Goals?
As the campaign goal increase the probability of failure also increases based on historical data. Campaigns under 5000 have best chance of success.

- What are some limitations of this dataset?
The dataset doesn’t include characteristics of the campaigns such as:
	- Locations of the plays, were they organized in big cities or small towns
	- How the campaigners reached their target audience, any use of social or digital media?
As information such as these may provide clues as what type of campaigns are successful 

- What are some other possible tables and/or graphs that we could create?

We can create table and graph similar to Outcome based on Goals. Where we can create a table with ranges of goal (0-5000, 5000-10000, so on), number of campaigns under each goal range and average backers for these campaigns. When we plot this, it will show us where the interest of backers lies based on size of campaign.
