# Kickstarting with Excel - Challenge 1

## Overview of Excel Project
Louise is a playwright whose first play Fever recently fell short of its fundraising goal.
### Purpose
To use the Kickstarter dataset that contains multiple crowdfunding campaigns to provide Louise a visualization of campaign outcomes based on their launch dates and their funding goals.
This presentation of data will allow for effective analysis and reasonable conclusions to be drawn to help her be more likely to have successful campaigns in the future.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
A line chart was used to display the Outcomes Based on Launch Date. 
[Theater_Outcomes_vs_Launch.png](Resources/Theater_Outcomes_vs_Launch.png)
It provided a clear picture of the successful, failed and canceled campaigns. 
This chart was created by first inserting a pivot table into a new worksheet using the Kickstarter dataset.
Filters were utilized so the outcomes displayed only related to the parent category "Theater."
The launch date was grouped by month to show the relationship between outcomes and launch month.
[Kickstarter_Challenge.xlsx](Kickstarter_Challenge.zip)

### Analysis of Outcomes Based on Goals
A line chart was used to display Outcomes Based on Goals.
[Outcomes_vs_Goals.png](Resources/Outcomes_vs_Goals.png)
To have an effective visualization required creating dollar-amount ranges for Goals.
The countifs() function was used to populate the "Number Successful," "Number Failed," and the "Number Canceled" for each goals dollar range.
[Kickstarter_Challenge.xlsx](Kickstarter_Challenge.zip)

### Challenges and Difficulties Encountered
No challenges were encountered.
The Theater Outcomes Based on Launch Date required grouping the row labels in the pivot table for the Date Created Conversion.
That required using the Grouping Selection and the hint provided facilitated completing that step.
The Outcomes Based on Goals required using the countifs() function in 36 cells.
Using F4 in the countifs() function to lock the columns referenced on the Kickstarter worksheet allowed for the function to be copied from the "Number Successful" and used in the "Number Failed," and the "Number Canceled" columns.

## Results

### What are two conclusions you can draw about the Outcomes based on Launch Date?
There are more successful campaigns than failed and canceled campaigns combined.
Successful campaigns have the most variability by month. 
The highest number of successful campaigns were launched in May. 
It is likely that launching a campaign in May would lead to a higher likelihood of success. 
The number of canceled campaigns is fairly constant throughout the different months within a year, so the launch date has little impact on whether a campaign is canceled. 

### What can you conclude about the Outcomes based on Goals?
Plays typically had campaign goals under $5000. 
There were 720 total projects with goals under $5000.
Campaigns with goals under $5000 have the highest percentage of successful outcomes.   

### What are some limitations of this dataset?
This dataset does not have statistical components that would allow for more thorough analysis.

### What are some other possible tables and/or graphs that we could create?
A box and whiskers plot would provide the distribution of the data.
This chart would identify outliers that could skew data analysis results.
In addition it would show the mean which is a measure of central tendency and the interquartile range.