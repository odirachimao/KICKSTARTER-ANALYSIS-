# Kickstarting with Excel

## Overview of Project


### Purpose
This project provides a global analysis of the Kickstarter campaigns from 2009 to 2017. It dives deeper into the ‘theater and plays’ category to uncover the different trends that led to its success and failure based on their launch dates and funding goals. 

## Analysis and Challenges
Analysis:
•	I performed my analysis for the “Theater outcomes based on launch date” by first creating a pivot table to filter out the successful, failed and canceled dataset I needed to analyze the theater category. This way I was able to add a line graph through the insert tab to track the changes among all 3 outcomes during in the span of 12 months. 
 
•	The “Outcomes based on Goals” was examined using the CountIf function to determine the number of successful, failed and canceled based on the goal ranges and the “play” subcategory. 
The sample code used was:
> =COUNTIFS(KICKSTARTER!$F$2:$F$4115,"successful",KICKSTARTER!$D$2:$D$4115,"<1000",KICKSTARTER!$R$2:$R$4115,"plays").

Once I was able to determine the value for each outcome per range, I used the SUM function to find the total number projects for each given range. 
The sample code used was: 
> =SUM(B2:D2)
Then I was able to find the percentage of each outcome by dividing the number of each outcome per range by the sum of the total projects per range.
The sample code used was: 
> =B2/E2

This way I was able to insert a line graph to show the trends of each outcome based on the given range values.

Challenges: 
One of the major challenges I faced doing this project was having to breakdown down datasets into subsets. For example, the dataset needed to be further organized by fragmenting the “category and subcategory” column into “parent category and “subcategory” for a more detailed analysis to be conducted.

Another big challenge that came along the way was having to create “the outcomes based on goals” line graph. There was an issue with the version of excel I had installed that limited me to only 255 data series per chart. After researching this, it seemed to be a problem that came with the 2010 excel version on MacBook. This way I had to copy and paste the values into new separate in order for the chart to populate. This was a challenge because it became very time consuming and required extra research in trying to figure out what the problem was. 

 
The link to the issue: 
https://techcommunity.microsoft.com/t5/excel/excel-2010-the-maximum-number-of-data-series-per-chart-is-255/m-p/2229562



### Analysis of Outcomes Based on Launch Date:
•	It can be concluded that May had the highest success rate of launching a theater campaign with a total of 111 successful campaigns launched, followed by June with 100 successful campaigns launched.
•	There is also so significant amount of decline in the overall success rate of the launching campaigns in the last few months of the year, September, October, November and December, with a high increase in failed campaigns during that period. December being the lowest with only 37 successful campaigns launched.


### Analysis of Outcomes Based on Goals:
•	It can be concluded that the higher the funding goal does not necessarily have a positive effect on the successful rate of the campaigns. The analysis draws that the success rate is even higher for campaigns with a funding goal that is less than $5,000. Campaigns with a funding goal between <$1,000 too $4,999 had the highest success rate ranging between 76% - 73%, while the opposite reflected on the rest. 

## Results

- What are some limitations of this dataset?
•	I feel like the dataset is only limited to one crowdsourcing company; we may need to analyze more crowdsourcing companies to be able to bring in more significant findings. 
•	Lack of metrics that describe the success and failures of each category or industry during the listed time period. We would have been able to provide a more detailed analysis if the data showed whether each category succeeds or fails during certain time periods. This will help in accounting for external factors.

- What are some other possible tables and/or graphs that we could create?
•	Box plots that display significant funding goal outliers.
•	A scatter plot will be effective in measuring the relationship between the number of backers and how it affects the success of each category in the project. 
•	A bar chart would have been helpful in comparing the number of projects per year to see how much it peaked and in what year and how bad it declined. 


