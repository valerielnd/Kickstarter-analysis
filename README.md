# Kickstarting with Excel

## Overview and purpose of the project

This project aims to analyze data from thousands of crowdfunding campaigns across different categories and countries to identify hidden trends and key factors that contribute to the success of crowdfunding projects. Specifically, the aim is to help someone seeking to fund a play through a crowdfunding campaign, make informed decisions about the timing and strategies to achieve a fundraising goal of $12,000.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
First, we examined the outcomes of campaigns based on their launch dates to assist in determining the impact of the launch timing on campaign performance. To proceed, we used the information in 
the column “launched_at” in the sheet "Kickstarters" of the file [Kickstarter_Challenge](https://github.com/valerielnd/Kickstarter-analysis/blob/main/Kickstarter_Challenge.xlsx) that we converted into dates to get the date each campaign was created. Then, using this new information, we built a pivot table filtered by year and project categories. In this table, we presented the months of the year in each row, the
number of campaigns undertaken during a month in each column, and how many failed, succeeded, or were canceled. Also, to have a visual summary of the results, 
we created a line chart to verify if there is a relationship between outcomes and the launch month.

![Pivot_table_outcome_based_launch_date](https://github.com/valerielnd/Kickstarter-analysis/blob/main/Pivot_table_outcome_based_launch_date.png)

![Chart_line_outcome_based_launch_date](https://github.com/valerielnd/Kickstarter-analysis/blob/main/Outcome_based_launch_date.png)

### Analysis of Outcomes Based on Goals
To continue, we analyzed the campaign's performance based on her goal amount. To find helpful information that can help her, 
we decided to compute the percentage of successful, failed, and canceled plays based on their funding goal amount. We created a new sheet, "Outcomes Based on Goals".
We gathered information about the goal amount and calculated the percentage of successful,  failed, and canceled campaigns for each range. 
To collect the values for the subcategory "plays" we used the function "COUNTIFS" where our first condition is 
the outcome of the campaign, then its goal amount, and finally, the subcategory must be "plays." 
As in our first analysis, we created a chart line to visualize the results and uncover a relationship between a play outcome and goal amount.

![Outome_vs_goal](https://github.com/valerielnd/Kickstarter-analysis/blob/main/Outcome_vs_Goals.png)


## Limitation of the Data set and possible analysis we could do
One drawback of the dataset is its time range, spanning from 2009 to 2017, which limits the accuracy of our analysis. A more precise assessment could be achieved with data from recent years. Additionally, while Kickstarter is a prominent platform for project funding, expanding our analysis to include data from other platforms catering to projects similar to the one analyzed would provide a more comprehensive understanding.

Additional analysis that we could do involves considering the play's characteristics, such as its purpose and overview, and comparing it with similar plays 
to find information such as the outcomes of those plays and what period of the year they were more successful.
