# Kickstarter Analysis
Challenge 1 by Dan Nyhan!

# Kickstarting with Excel

## Overview of Project

### Purpose

The purpose of this analysis is to discover how some playwrights' crowdfunding campaigns raise more money than others' campaigns, based on their launching date and their funding goals. Louise, a playwright, has requested this analysis in order to increase the crowdfunding her play recieves. This analysis, performed through Microsoft Excel, will optimize Louise's future crowdfunding campaigns, in relation to the variables of the launch date and funding goal. The dataset used in this analysis has consists of 1043 plays.

## Analysis and Challenges
There were two analyses for this projected; there was one analysis completed for each variable Louise had requested. The one for the launch date analysis is titled "Outcomes based on Launch Date." The one for the crowdfunding goal variable is titled "Outcomes Based on Goals." 

### Analysis of Outcomes Based on Launch Date
This analysis was performed by using a Pivot Table in Microsoft Excel. I used months of the year as the input variable. Thus, for each month I listed the number of successful, failed, and canceled crowdfunding campaigns in the "theater" parent cateogory (plays are a subcategory). Under the "Challenges and Difficulties Encountered" subheading, I will explain the significance of using this parent category, instead of the primary subcategory. Anyways, this dataset had Unix timestamps instead of identifiable dates, so I used [this code](https://courses.bootcampspot.com/courses/1018/pages/1-dot-3-3-timing-success?module_item_id=395347) to convert the timestamp to a readable date. Here is an image of the pivot table: ![Here](https://github.com/nyhandan/Kickstarter-Analysis/blob/main/Outcomes%20based%20on%20launch%20date%20pivot%20table.png)

Here is a graphical depiction of the pivot table: 
![here](https://github.com/nyhandan/Kickstarter-Analysis/blob/main/Challenge%201%20Resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
The second analysis was done using the [COUNTIFS](https://support.office.com/en-us/article/countifs-function-dda3dc6e-f74e-4aee-88bc-aa8c2a866842) function in Mircosoft Excel. I counted the number of successful, failed, and canceled crowdfunding campaigns for just the "plays" subcategory. I categorized my counts based on uniform, incremental ranges of goals. Then I took the percentage of successful, failed, and canceled plays from the total amount of plays. Here is a screenshot of the table:
![here](https://github.com/nyhandan/Kickstarter-Analysis/blob/main/Outcomes%20Based%20on%20Goals.png)

Here is the graphical depiction of my analysis:
![here](https://github.com/nyhandan/Kickstarter-Analysis/blob/main/Challenge%201%20Resources/Outcomes%20Based%20on%20Goals.png) 

### Challenges and Difficulties Encountered

One challenge I encountered was that the COUNTIFS function is tricky to navigate, because the syntax for the function is generic. I had to enter 4 arrays to specify what I was counting, which proved confusing as there were essentially no nuances between the arrays I used. This was overcome by strict organizational standards of the COUNTIF function to maintain efficiency in the analysis. 

A difficulty I encountered was that I was instructed to use a parent category instead of the subcategory in question for the "Analysis of Outcomes By Date." This makes the analysis scientifically invalid, as it is not logical to use this excess data. It may or may not have a significant effect on the results. 

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

Two conclusions I can draw from the Outcomes based on Launch Date are that the month of May is likely the best time to start a campaign, and the fall months will likely have the most unpredictable results. 

- What can you conclude about the Outcomes based on Goals?

A conclusion of the Outcomes Based on Goals I will make is that after about a $15000 goal, the volatility of the success rate is quite high. The higher goals are quite unpredictable.

- What are some limitations of this dataset?

A limitation of this dataset is that there aren't any canceled campaigns for the plays, and there are relatively few campaigns with the goal amount exceeding $30000. So it is hard to analyze the upper echelon of campaign goals, as the data becomes much more sparse. 

- What are some other possible tables and/or graphs that we could create?

We could create a graph describing the relationship between the timeframe length of the campaign, and the amount of money pledged. We could also use the Pivot table to see a year-by-year breakdown. 
