# An Analysis of Kickstarter Campaigns
Performing analysis on global Kickstarter data to uncover trends in successful theather campaign 
## Overview 
Kickstart campaigns fund independent projects. To run a succesful kickstarter campaign one should take into consideration importnant variables like the donation goal and the best time of year to run a campaign. Using global kickstarter data [Kickstarter_Challenge.xlsx](https://github.com/godak9/kickstarter-analysis/files/8904230/Kickstarter_Challenge.xlsx) I narrowed my search down to theather/play campaigns and performed analyses on successful and unsuccessful campaigns that revealed trends on donation goals and launch times. 
## Analysis
I used Excel to create the following graphs via pivot tables and formulas using data from the "Kickstarter" worksheet.
### Theather Outcomes Based on Launch Date
First, I created a line graph that showed the number of successful, failed, and canceled theater campaigns based on the month of the year the campaign was launched. This line graph displayed patterns about what month of the year would be best to start a kickstarter campaign for theater production. To create this graph, I first created a pivot table using the Kickstarter data. In the pivot table fields I entered "Parent Category" and "Year" in the Filters field, "Outcomes" in the Columns field, "Date Created Conversion" in the rows field, and "Outcomes" in the Values field. I narrowed down the date to only the months of the year by removing "Quarters" and "Years" from the Rows field, but set the "Year" filer to "All" to show data from across the years. Lastly, I set the "Parent Category" filter to "Theater" and created this line graph. Both aforementioned pivot table and graph can be found in the "Theater Outcomes Based on Date" worksheet.
![Theater_Outcomes_vs_Launch ](https://user-images.githubusercontent.com/104794100/173905082-b5763cda-8f1b-4f2a-98bb-0d20cfc6d1c9.png)
### Play Outcomes Based on Goals
Second, I created a line graph that showed the pecentage of successful, failed, and canceled play campaigns based on the donation goal set by the campaign. This line graph displayed patterns about what goal range to aim for when running a kickstarter campaign for play production. To create this graph, I first created a filtered set of data from the "Kickstarter" worksheet which can be found in a new worksheet titled "Outcomes Based on Goals". I created a "Goals" column that grouped goals into goal ranges. Then I found the number of successul, failed, and canceled campaigns that were included in each goal range using the "COUNTIFS" formula. Below is an example of the  "COUNTIFS" formula used to find the number of succesful play kickstarter campaigns that set their goal between $1,000 and $4,999.
```
=COUNTIFS(Kickstarter!F:F, "Successful", Kickstarter!D:D, ">=1000", Kickstarter!D:D, "<=4999",  Kickstarter!R:R, "plays")
```
Next, I totaled amount of projects for each goal range in a new column titled "Total Projects" using the "SUM" formula. Below is an example of the "SUM" formula used to find the total number of projects for goals set between $1,000 and $4,999.
```
=SUM(B3,C3,D3)
```
Finally, I found the percentage of successful, failed, and canceled kickstarter campaigns using the "ROUND" formula and dividing the number of succesful, failed, or canceled kickstarter campigns for each goal range and dividng it by the toal amount of projects for each goal range. Below is an example of the "ROUND" formula used to find the percentage of successful play kickstarter campaigns that set their goal between $1,000 and $4,999.
```
=ROUND(B3/E3*100, 0)
```
With the data in the "Outcomes Based on Goals" worksheet, I created the line graph below by selecting what data I wanted to be included in the "Select Data" section in the "Chart Design" Ribbon. 
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/104794100/173917237-87ff7485-971e-469b-b04a-5691bf52953f.png)

### Challenges 
## Conclusions 
