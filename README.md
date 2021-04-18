# Kickstarting with Excel

## Overview of Project

Louise is a playwright with an upcoming play titled "Fever". Louise has a budget of $10,000 and requires the help of crowdfunding in order to make the play possible. 

### Purpose

The purpose of this task is to organize, analyze, and visualize crowdfunding data in order to gain insights into what makes a crowdfunding campaign successful. 
Specifically, I will analyze past and present crowdfunding campaigns for theatre and plays campaigns using excel to determine what factors made them successful or unsuccessful. 

## Analysis and Challenges

The raw data was first organized in order to make analysis more efficient. The category and subcategory data were parsed into two new columns: a parent category and subcategory.
An average donation column was created and calculated by dividing the pledged data by the number of backers or number of people that donated to the campaign. 
The deadline and launched at data was displayed in Unix timestamps and were converted to date data. In addition, the year was extracted from the Date Created data. 
I also visualized the outcomes data by colour coding each outcome to make it easy and more efficiently readable. 

### Analysis of Outcomes Based on Launch Date

In order to determine whether the Launch Date affects the outcome of a crowdfunding campaign, I analyzed theatre campaign data relative to their launch date. I generated a pivot table comparing 
the date launched to the outcome, filtering by parent category and year. The main value outcome was the number of outcomes within each filter. I then generated a line chart to visually display 
this data.
The line chart can be found here: https://github.com/fadlnabbouh/kickstarter-analysis/blob/main/Resources/Theatre_Outcomes_vs_Launch.png. 

### Analysis of Outcomes Based on Goals

In order to determine whether the campaign's goal affected the outcome of the crowdfunding campaign, I analyzed play data relative to their original goal. I generated a new sheet that split the goals data 
by incremants of $5000 and used the COUNTIFS function to generate the number of campaigns by goal and outcome. I then generated the percentage of each outcome by the goal increment and visualized this data
in a line chart. 
The line chart can be found here: https://github.com/fadlnabbouh/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png. 

### Challenges and Difficulties Encountered

The greatest challenge I faced was using learning and using the functions required in this data analysis task. In particular, I experienced difficulty with the COUNTIFS function. I overcame the challenge by
better understanding the different parts of the function and through trial and error. I ran into errors when I inputted "Successful" instead of "successful", learning that the capitalization of the column 
values can be a potential issue when running a function. In addition, the use of "$" in front of the column letters when choosing a range made it helpful to copy the functions over to different columns without
changing the range. Finally, I ran into difficulty when inputting the goal increments into the function. I'd originally been using, as an example, "1000>" to incidate less than 1000, but I've learned that Excel
reads functions like a book and that the appropriate way to write this out is "<1000"- read as "less than 1000". 

Further challenges that may have been faced could be the effective use of graphic visualization to present the data. In the Outcomes by Launch Date graph, I used a line chart to display the change in number of 
outcomes over time. This would not have been as effective had it been a bar graph. The appropriate use of data visualization is extremely important to data analysis. 

## Results

### Outcomes vs. Launch Date

From the outcomes based on launch date data, I can see that while failed campaigns are relatively consistent over the year, successful campaigns fluctuate in total number. More specifically, the number of 
successful campaigns peaks in May, and is at its lowest in the winter months. This seems to suggest that the more successful campaigns for theatre occur during the spring and summer, namely in May, June, and July.
In addition, canceled campaigns and failed campaigns are consistent across the year in terms of total numbers. One limiation to this analysis is that data is analyzed as total number rather than as a percentage,
such as in the next graph. This limits my ability to conclude whether a greater proportion of campaigns are successful in May, or if there were just more campaigns during that month that lead to the heightened 
numbers.  

### Outcomes vs. Goals?

From the outcomes based on goals data, I can see that the percentage of successful campaigns, relative to the failed and canceled campaigns, is high when the goal amount is low. Success seems to drop when the 
goal is extremely high, above $45000. This would suggest that a lower goal results in a successful campaign. However, it is also noteworthy that there are more successful campaigns than failed campaigns when
the goal is $35000-$45000, while there are more failed campaigns when the goal is $20000 to $35000. This is inconsistent with my initial finding that the lower the goal, the more successful a campaign will be. 
This suggests that the goal itself doesn't play a role in the outcome of the campaign, and other factors are at play.  

### Limitations to the Dataset

One limitation to the dataset may be that there aren't enough data points within some filters. For example, with the data in Outcomes vs. Launch Date, there were more theatre campaigns during the summer, than
there are during other months, making it difficult to conclude whether time of year impacts success rate. In addition, in the Outcomes vs. Goals data, most data points lie below $10,000. In the future, more data
points for campaigns above $10,000 would be beneficial, or using smaller increments for campaigns under $10,000 when analyzing this data. 

### Other Possible Tables/ Graphs

Other possible graphs or tables can be generated to find new insights into what makes a campaign successful. First, using the graphs I've already generated above, I can broaden or specify each analysis to 
include theatre data or plays-specific data. For example, with the Outcomes vs. Launch Date data, I can specify plays instead of theatre to determine if there are any insights into play-specific campaigns. 
I can also generate this graph with percentage as the outcome rather than total to determine if a greater proportion of successful campaigns happen in the summer, rather than just total number. With the Outcomes
vs. Goals data, I can broaden the search to theatre data or compare it to other subcategories to determine if there are any insights there. 

Another graph I would have generated is comparing plays-specific data in different countries to determine whether the country of origin can determine success rate. 

Finally, I'd have generate a graph to analyze the average donation per campaign relative to success rate. Although it is difficult to control the amount of donation a person gives, it could potentially generate
some insight. 


