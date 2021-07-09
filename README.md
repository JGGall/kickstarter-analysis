# Kickstarting with Excel

## Overview of Project

### Purpose
Louise, who wrote a play and launched a successful Kickstarter campaign for it, has asked for an analysis of how campaigns for other plays fared based on the month in which their Kickstarter campaigns launched, and based on the dollar amount of their campaign goals.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
Using the large Kickstarter dataset, I created a pivot table filtered by parent categories and years. The columns contain the outcomes of the Kickstarter campaigns, and the rows contain the date the campaigns were created (that is, launched). I deleted the contents of the rows that Excel generated automatically, and that revealed the months of the year, which was the degree of specificity I needed. The result was a table containing three columns, showing the number of successful, failed, and canceled campaigns that had been launched in each of the twelve months of the year. 
![mypic2](https://github.com/JGGall/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png)

Then I created a line chart whose three lines provide a visual analysis of the number of campaigns that were successful, that failed, or that were canceled (the x-axis) based on the month of the year in which they were launched (the y-axis). It is clear that the largest number of successful theatrical production Kickstarter campaigns were launched in May, and the smallest number of successful campaigns were launched in December. The largest number of failed campaigns were also launched in May, while the smallest number of failed campaigns were launched in November. The number of campaigns that were canceled is minimal and shows little variation based on the months in which they were launched.

### Analysis of Outcomes Based on Goals
Louise also wanted to know how successful various Kickstarter campaigns for plays were based on how much money the campaign for each project hope to raise (that is, its goal). She specified various dollar amount ranges, so I used Excel's COUNTIFS function to populate a table showing the number of campaigns that were successful, that failed, or that were canceled in each goal dollar amount range. COUNTIFS was the function to use because it supplies a count of campaigns which, to use an example, were successful and had a goal of greater than or equal to $1000 and were plays, and had a goal or less that $4999. Once I had a working formula I altered it to count the number of productions in each goal dollar amount range. Then I used the SUM function to add the number of successful, failed, and canceled campaigns to produce a column of the toal number of projects in each range. Then I could easily create columns showing the percentages of campaigns in each goal range that were successful, failed, or canceled by dividing, for example, the number of successful projects in a given range by the total number of projects in that range. 
![mypic1](https://github.com/JGGall/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png)
Finally, I created a line chart that provides a visual analysis of the percentage of campaigns that were successful, failed, or canceled.

### Challenges and Difficulties Encountered
I had trouble creating my first pivot table as part of this analysis, but with some advice from a classmate I could see what I had done wrong. I believe that with practice the creation of pivot tables will become second nature. The instructions were clear enough so that I could extract the necessary information from the parent category, but that process would be complicated if I had needed to figure it out on my own. Regarding the outcomes based on goals, I found it very challenging to write the COUNTIFS formula for the first and second cells. Once I could verify that the formula worked, I found it easy (although time consuming) to modify the formula for the remainder of the first three columns.

## Results

###### What are two conclusions you can draw about the Outcomes based on Launch Date?
- First, it is clear that campaigns launched in May were more likely to be successful than in any other month of the year, followed by campaigns launched in June and July. A campaign with a December launch date was less likely to succeed than one launched in any other month. Naturally, I would recommend a May launch for any future campaign.
- Second, the line chart shows that successful campaigns and failed campaigns follow roughly the same pattern when it comes to the percentage that were successful based on the month of the year in which they were launched. The lines are not mirror images of one another, so the notion that May launches are successful while December launches are unsuccessful needs to be set aside as too simplisitic. More important factors are likely at work when it comes to how successful a theater Kickstarter campaign is likely to be.

###### What can you conclude about the Outcomes based on Goals?
- The line chart for outcomes based on the goal of each campaign does show patterns that are roughly mirror images of one another. Campaigns with goals of less than $1000 had a high success rate, as did campaigns with goals between $1000 and $4999. The percentage of successful campaigns dropped as the goals increased--with the exception of a very small absolute number of campaigns with high goals between $35,000 and $44,999 that had a high success rate. In general, campaigns with high goals were more likely to fail. It would seem wise for someone intending to conduct a Kickstarter campaign for a theatrical production to keep the goal modest, as the goal is more liely to be achieved that way.

###### What are some limitations of this dataset?
- The user of this dataset does not know anything about those who contributed to the Kickstarter campaigns, nor about their motivations. More data could allow us to understand whether a potential contributor was discouraged by a large campaign goal or encouraged by the small size of another goal. A contributor could be motivated by the idea that he or she could make a real difference with a small dollar amount. We also don't know whether corporations or foundations made contributions towards campaigns with very high goals, allowing them to attain a high-dollar goal with a few large contributions while other exciting projects with middle-sized goals failed beacuse they didn't attract similar large contributions.

###### What are some other possible tables and/or graphs that we could create?
The number of successful and failed projects are heavily clustered in the three dollar ranges that are less than $10,000. It would be a good idea to alter the table in a way that explores the success rate of projects with smaller goals by adding ranges of smaller dollar amounts. I would make the ranges in $500 increments up to $3000, and than in $1000 increments up to $10,000. This would give much more information about the projects whose campaigns had small goals. 
While the chart that shows the percentage of successful, failed, or canceled campaigns is a useful one, I think our understanding of trends would be enhanced by the addition of a chart based on the absolute number of project campaigns. This would balance the conclusions a user might draw from a chart based on percentage of success or failure, since a large spike or drop can be based on only a handful of campaigns.

