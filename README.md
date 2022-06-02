# kickstarter-analysis
Performing analysis on Kickstarter (crowdfunding) data to uncover trends


# Kickstarting with Excel

## Overview of Project

### Purpose
The purpose of this analysis is to determine how crowdfunding campaigns performed based off of their campaign launch date as well as their campaign fundraising goals. We are interested in looking at campaigns categorized specifically as theater and/or play due to our stakeholder's interest.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

![](Outcomes_vs_Launch_pivottable_fields.png)

In order to understand outcomes based on launch date I created a pivot table with the filters on "Parent Category" 
and "Years". The pivot table fields consisted of "Outcomes" in the columns, "Date Created Conversion" in the rows, 
and a count of the Outcomes as the values. I also filtered the column labels to show the campaigns that were
"successful," "failed," and "canceled." The pivot table provided a count of campaigns per month per Outcome.

Note: the "Years" column, was created by using the YEAR() function to extract the year from the “Date Created Conversion” column.



### Analysis of Outcomes Based on Goals

![](Outcomes_vs_Goal_formula.png)


In order to analyze the Outcomes based on Goals, I calculated the number of successful, failed, and canceled US campaigns that were subcategorized as plays by using the COUNTIFS statement displayed above. The formula adapted to account for the respective outcomes and Goal ranges.

Next, I used the SUM() function to total the number of campaigns per each Goal range. 


Then I calculated the percentages of successful, failed, and canceled projects based on the data from the "Total Projects," "Number Successful," "Number Failed," and "Number Canceled". I visualized this data with a line chart. 



### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

The most successful theater campaigns (111) were launched in May so May would be an ideal time to launch. However, May, June, July, August, and October had roughly the same number of failed theater campaigns (~50).

- What can you conclude about the Outcomes based on Goals?

From fundraising goals of $0-$29,999 the general trend of the successful campaigns is negative meaning that the the higher the fundraising goal is the 
lower the percentage of successful camppaigns. The highest percentage of successful campaigns were in the $0-$1000 campaign range.

- What are some limitations of this dataset?



- What are some other possible tables and/or graphs that we could create?

I would suggest creating a table and/or line chart to view the trend between Number of Backers, Average Donations, and Goals. 
It would be interesting to answer the question: Do lower fundraising goals have fewer backers but higher average donations?
I also would create a bar chart to display the average length of time campaigns ran based on Outcome.
