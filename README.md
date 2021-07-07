# Kickstarting with Excel

## Overview of Project

### Purpose
Louise, who wrote a play and launched a successful Kickstarter campaign for it, has asked for an analysis of how campaigns for other plays fared based on the month in which their Kickstarter campaigns launched, and based on the dollar amount of their campaign goals.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
Using the large Kickstarter dataset, I created a pivot table filtered by parent categories and years. The columns contain the outcomes of the Kickstarter campaigns, and the rows contain the date the campaigns were created (that is, launched). I deleted the contents of the rows that Excel generated automatically, and that revealed the months of the year, which was the degree of specificity I needed. The result was a table containing three columns, showing the number of successful, failed, and canceled campaigns that had been launched in each of the twelve months of the year. Then I created a line chart whose three lines provide a visual analysis of the number of campaigns that were successful, that failed, or that were canceled (the x-axis) based on the month of the year in which they were launched (the y-axis). It is clear that the largest number of successful theatrical production Kickstarter campaigns were launched in May, and the smallest number of successful campaigns were launched in December. The largest number of failed campaigns were also launched in May, while the smallest number of failed campaigns were launched in November. The number of campaigns that were canceled is minimal and shows little variation based on the months in which they were launched.

### Analysis of Outcomes Based on Goals
Louise also wanted to know how successful various Kickstarter campaigns for plays were based on how much money the campaign for each project hope to raise (that is, its goal). She specified various dollar amount ranges, so I used Excel's COUNTIFS function to populate a table showing the number of campaigns that were successful, that failed, or that were canceled in each goal dollar amount range. COUNTIFS was the function to use because it supplies a count of campaigns which, to use an example, were successful and had a goal of greater than or equal to $1000 and were plays, and had a goal or less that $4999. Once I had a working formula I altered it to count the number of productions in each goal dollar amount range. Then I used the SUM function to add the number of successful, failed, and canceled campaigns to produce a column of the toal number of projects in each range. Then I could easily create columns showing the percentages of campaigns in each goal range that were successful, failed, or canceled by dividing, for example, the number of successful projects in a given range by the total number of projects in that range. Finally, I created a line chart that provides a visual analysis of the percentage of campaigns that were successful, failed, or canceled.

### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
![mypic1](https://github.com/JGGall/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png)
![mypic2](https://github.com/JGGall/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png)
