# An Analysis of Kickstarter Campaigns
Performing analysis on global Kickstarter data to uncover trends in successful theather campaign 
## Overview 
Kickstart campaigns fund independent projects. To run a succesful kickstarter campaign one should take into consideration importnant variables like the number of donors, the donation goal, and the best time of year to run a campaign. Using global kickstarter data [Kickstarter_Challenge.xlsx](https://github.com/godak9/kickstarter-analysis/files/8904230/Kickstarter_Challenge.xlsx) I narrowed my search down to theather/play campaigns and performed analyses on successful and unsuccessful campaigns that revealed trends on donation goals and launch times. 
## Analysis
I used Excel to create the following graphs by filtering data from the "Kickstarter" worksheet. Pivot tables 
### Theather Outcomes Based on Launch Date
I wanted to create a line graph that would show the number of successful, failed, and canceled cmapaigns based on the month of the year the campaign was launched. This line graph displays patterns about what month of the year would be best to start a kickstarter campaign for theater production. To create this graph, I first created a pivot table using the Kickstarter data. In the pivot table fields I put "Parent Category" and "Year" in the Filters field, "Outcomes" in the Columns field, "Date Created Conversion" in the rows field, and "Outcomes" in the Values field. I narrowed down the date to only the months of the year by removing "Quarters" and "Years" from the Rows field, but set the "Year" filer to "All" to show data from across the years. Lastly, I set the "Parent Category" filter to "Theater" and created the the line graph below":
![Theater_Outcomes_vs_Launch ](https://user-images.githubusercontent.com/104794100/173905082-b5763cda-8f1b-4f2a-98bb-0d20cfc6d1c9.png)

### Play Outcomes Based on Goals
##Conclusions 
