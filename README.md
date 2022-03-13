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
wich gives instruction about grouping or ungrouping data in a PivotTable
