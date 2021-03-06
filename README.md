# Kickstarting with Excel

## Overview and purpose of the project
Louise, a play writer, wants to start a crowdfunding campaign to help fund her play, Fever. She estimates that her project will cost $12000. 
To help her make critical decisions about her project like when to start it and how to reach her goal amount, we have performed data analysis on 
several thousand crowdfunding campaigns for different categories of projects such as film and video, technology, and theater in several countries 
among which the US from 2009 to 2017. The goal is to find hidden trends to help determine factors capable of making her project successful. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
Knowing that Louise’s play came close to its fundraising goal, to help her determine how her campaign will perform in relation to a launch date,
we analyzed campaigns' outcomes based on their launch date. To proceed, we used the information in 
the column “launched_at” in the sheet "Kickstarters" of the file [Kickstarter_Challenge](https://github.com/valerielnd/Kickstarter-analysis/blob/main/Kickstarter_Challenge.xlsx) that we converted into dates to get the date each campaign was created. Then, using this new information, 
we built a pivot table filtered by year and by project categories. In this table, we presented in each row the months of the year and each column the 
number of campaigns undertaken during a month, how many failed, succeeded or were cancelled. Also, to have a visual summary of the results, 
we created a line chart to verify if there is a relationship between outcomes and launch month.

![Pivot_table_outcome_based_launch_date](https://github.com/valerielnd/Kickstarter-analysis/blob/main/Pivot_table_outcome_based_launch_date.png)

![Chart_line_outcome_based_launch_date](https://github.com/valerielnd/Kickstarter-analysis/blob/main/Outcome_based_launch_date.png)

The challenge encountered during this analysis was to find a way to select the rows and columns in the pivot table to show the outcomes for 
each month. To find a solution, I consulted an excel documentation provided by Microsoft 
which gives instruction about grouping or ungrouping data in a PivotTable [Microsoft Documentation](https://support.microsoft.com/en-us/office/group-or-ungroup-data-in-a-pivottable-c9d1ddd0-6580-47d1-82bc-c84a5a340725?ui=en-us&rs=en-us&ad=us)

### Analysis of Outcomes Based on Goals
To continue, we performed an analysis to determine how Louise's campaign will perform based on her goal amount. To find useful information that can help her, 
we decided to compute the percentage of successful, failed, and canceled plays based on their funding goal amount. We created a new sheet, "Outcomes Based on Goals" 
in the "Kickstarter" excel file in which we gathered information about the goal amount specified in several ranges and we calculated the percentage of successful, 
failed, and canceled campaigns for each range. To collect the values for the subcategory "plays" we used the function "COUNTIFS" where our first condition is 
the outcome of the campaign, then its goal amount, and finally the subcategory which must be "plays". As in our first analysis, we created a chart line to visualize the 
results and uncover a relationship between a play outcome and goal amount.

![Outome_vs_goal](https://github.com/valerielnd/Kickstarter-analysis/blob/main/Outcome_vs_Goals.png)

The challenge that someone could encounter during this analysis is about using the function “COUNTIFS” and defining the criteria residing in different columns and also 
how to enter the goal amount ranges to avoid overlapping.

## Limitation of the Data set and possible and possible analysis we could do
One limitation of the data set is that it provides information about campaigns undertaken from the year 2009 to 2017. We could do a more accurate analysis 
with data from more recent years. 
Also, even though Kickstarter is one of the best platforms where projects can find support, it would be good to analyze information from other platforms where projects like Louise's will be funded.

Additional analysis that we could do involve considering Louise's play characteristics such as its purpose and overview and comparing it with similar plays 
to find information such as the outcomes of those plays and what period of the year they were more successful.
