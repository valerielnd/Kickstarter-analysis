# Kickstarting with Excel

## Overview and purpose of the project
Louise, a play writer, wants to start a crowdfunding campaign to help fund her play, fever. She estimates that her project will cost $12000. 
To help her make key decisions about her project like when to start it and how to reach her goal amount, we have performed data analysis on 
several thousand crowdfunding campaigns for different categories of projects such as film and video, technology, and theater in several countries 
among which the US from 2009 to 2017. The goal is to find hidden trends to help determine factors capable of making her project successful. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
Knowing that Louise’s play came close to its fundraising goal, to help her determine how her campaign will perform in relation to a launch date 
and her funding goal, we carried out an analysis to visualize campaigns outcomes based on their launch date. To proceed, we used the information in 
the column “launched_at” in the sheet "Kickstarters" of the file [Kickstarter_Challenge](https://github.com/valerielnd/Kickstarter-analysis/blob/main/Kickstarter_Challenge.xlsx) that we converted into date to get the date each campaign was created. Using this new information, 
we built a pivot table  filtered by year and by project categories and in which we presented in the rows the months of the year and the columns the 
number of campaigns undertaken during each month, how many failed, succeeded or were cancelled. Also, to have a visual summary of the results, 
we created a line chart to verify if there is a relationship between outcomes and launch month.

![Pivot_table_outcome_based_launch_date](https://github.com/valerielnd/Kickstarter-analysis/blob/main/Pivot_table_outcome_based_launch_date.png)

![Chart_line_outcome_based_launch_date](https://github.com/valerielnd/Kickstarter-analysis/blob/main/Outcome_based_launch_date.png)

The challenges encountered while during this analysis was to find a way to select the rows and columns in the pivot table to just show the outcomes for 
each month from the original data wich is the creation date of the campaign. To find a solution, I consult an excel documentation provided by Microsoft 
wich gives instruction about grouping or ungrouping data in a PivotTable [Microsoft Documentation](https://support.microsoft.com/en-us/office/group-or-ungroup-data-in-a-pivottable-c9d1ddd0-6580-47d1-82bc-c84a5a340725?ui=en-us&rs=en-us&ad=us)

### Analysis of Outcomes Based on Goals

As we can see, plays where the goal amount in the range $1000 and less than $10000 and between $35000 and less than $50000s have a greater chance to succeed 
than fail. Between 5000 and 35000, they have a greater chance to fail than succeed. Also, between 10000 and 15000 they have about the same chance to fail and 
succeed. So, in Louise case, wich goal amount is 12000, her play has approximately the same chance to succeed and to fail. If she decides to increase her goal 
amount, it would be better to choose an amount between 35000 and 45000. Moreover, she must avoid ranges between 25000 to 30000 since her chance to fail is 
approximately 75% and 45000 to 50000.

![Outome_vs_goal(https://github.com/valerielnd/Kickstarter-analysis/blob/main/Outcome_vs_Goals.png)

The challenge that someone could encounter during this analysis could be how to use the function “COUNTIFS” with different criteria in different columns and to 
well define the goal amount ranges in the function to avoid overlapping.
