# Module 1 Challenge - An Analysis of Kickstarter Campaign Crowdfunding 

## Overview of Project

Louise, an up and coming playwright, launched a fundraising campaign for her new play titled Fever. Louise nearly met her fundraising goal in a short amount of time. Now, she needs to determine how her fundraising campaign results compared to others in relation to their launch dates and funding goals. This is an analysis of theatre outcomes based on launch date, and play fundraising campaign outcomes based on goals for comparison with Louise's fundraising for Fever.

### Purpose

The purpose of this project is to analyze the outcomes of similar fundraising campaigns for theatres and plays by launch date and fundraising goals for comparison against Louise's Fever. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

To compare the outcomes of similar theatre fundraising campaigns by their launch dates, I used a pivot table and line chart. In the pivot table and chart, I plotted the date (by month only) along the x-axis, and the count of the different outcomes along the y-axis. Further, I filtered for the campaigns by the "Theatre" category only. With these measures in place, the graphs displayed the "successful", "failed" and "canceled" campaigns by month to compare against Louise's. 


![Theatre_outcomes_vs_launch](https://user-images.githubusercontent.com/69849998/109581977-48026b80-7acb-11eb-8953-20d956766dca.png)


### Analysis of Outcomes Based on Goals

Comparing the outcomes of the fundraising campaigns for plays based on their fundraising goal was a multi-step process. Firstly, the goals were grouped in categories of less than $1,000, more than $50,000 and increments of $5,000 for all goals in between. The COUNTIFS function in Excel was used to determine the number of "successful", "failed, and "cancelled" plays based on their goal amount. From here, the sum function was used to calculate the number of total projects in each grouping of goal amount (ie. between $1000 - $4999). With these calculations mentioned, the percentages of successful, failed, and cancelled projects were determined. Lastly, I plotted the goals with the outcomes by percentage in a line graph. Since there were no cancelled plays, this line graph displayed a line for the successful projects and a line for the failed projects based on their project goals.


![Outcomes_vs_Goal](https://user-images.githubusercontent.com/69849998/109582071-7a13cd80-7acb-11eb-8aa1-9e0943d8b4e9.png)


### Challenges and Difficulties Encountered 

* The challenge I ran in to in this analysis had to do with being new to Excel. I left a filter on the kickstarter data worksheet, which impacted the COUNTIFS formula I was using to calculate the number of successful, failed and cancelled projects. This is a good lesson to check filters on data before developing formulas that could be impacted by these filters. 

* Another challenge I ran in to was that there is data missing specifically for the canceled campaigns in October. In future, I would try to get that data if it were possible, or remove the data if it was skewing the results. In this case, it was not, so I included it. 

* A possible challenge would have been the difference in the Canadian and American spellings of "canceled" vs. "cancelled". This may have caused difficulties when using the COUNTIFs function had it been spelled the canadian way, as it appears in the data in the American way. 

## Results

#### What are two conclusions you can draw about the Outcomes based on Launch Date?

The most successful Theatre fundraising campaigns were launched in May and June. Over 100 successful campaigns were launched in May, while 100 successful campaigns were launched in June. Therefore, it would be advisable to launch a theatre campaign in May or June, as it is likely to elicit similar results to those in the past.

#### What can you conclude about the Outcomes based on Goals?

The highest percentage of successful campaigns had goals under $4,999, followed closely by those with goals between $35,000 and $44,999. On the other hand, 80% of projects with goals between $25,000 and $29,999 failed, and 80-100% of goals greater than $45,000 failed. Louise had a goal of $10,000, which was close to but did not reach its fundraising goal. This outcome in line with past fundraising campaign results, of which 45% fail to meet the fundraising goal. Perhaps, if Louise had set a fundraising goal of under $4,999 or between $35,000 and $44,999, she would have been more likely to meet her goal.  

#### What are some limitations of this dataset?

* This dataset is dated, with the most recent data from 2017. More recent data would help to provide more relevant findings to Louise.
* Many of the campaigns are quite short in duration as well, lasting only a few months. With data from fundraising campaigns that were longer-lasting would provide more comparison for the duration Louise should have set for her campaign.  

#### What are some other possible tables and/or graphs that we could create?

* Plot the average donation by launch date (for theatre and plays) in a line graph to discover if the timing of the launch has an impact the amount people pledge. 
* Plot  the outcomes by country in a bar chart to determine if particular countries have a higher success rate of fundraising for plays/theatre. 
