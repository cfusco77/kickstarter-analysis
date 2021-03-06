# An Analysis of Kickstarter Campaigns 
---
## Overview of Project
Perform analysis using a dataset of several thousand crowdfunding projects to uncover any hidden trends

### Purpose
The purpose of this invetigation is to provide our client, Louise, a visual analysis of campaign outcomes based on their launch dates and their funding goals. Louise is a an up and coming playright looking to get her next project, Fever, funded via a crowdfunding campaign. Upon analysis we will provide Louise a recommendation so that her first crowdfunding campaign is a success. 

## Analysis and Challenges
*Possible challenge* : Please note that when I recieved the raw data both the Deadline and Launched_at columns contained dates formatted as Unix timestamps. I have converted that data into short form dates to aid in our analysis and provide Louise a readable output. 

### Analysis of Outcomes Based on Launch Date
Of the 4113 crowdfunding campaigns 1369 are categorized under the Parent Category: Theater. I have filted the dataset to include only Theater campaigns in the following analysis.

Having sorted the data and grouped by month, my initial observations are that not all months have the same number of campaigns. May and June have the highest count of total campaigns. The number of successful campaigns in a given month ranges from [37, 111] while the number of failed camapigns has a much smaller spread, [31, 52.] 

The table, pictured below, illustrates the count of campaign outcomes by month. It appears May is an exceptionally good time to launch a campaign, followed by June and then July. 

![Theater_Outcomes_vs_Launch](https://github.com/cfusco77/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png)

I want to point out a limitation of this table: Here I have shown the count of each type of outcome throughout the year. Perhaps instead we should plot the outcome rates which would control for the number of campaigns launched each month. I have performed this secondary analysis to confirm that success rate is in fact the highest in May and June. An additional finding, which may be harder to ascertain from the table, is that May and June also have the lowest failure rates. 

---
### Analysis of Outcomes Based on Goals
The table, pictured below, illustrates the effect campaign goal amount has on campaign outcome specifically for campigns with the subcategory: Plays. I have chosen to plot percent outcomes. There were no canceled fundraising campaigns for plays and so the two possible outcomes are success or failure. With only two possible outcomes the lines will be mirror images of one another which we see here. If we were to draw a trend line we would find that generally the larger the campaign goal the greater chance of failure. However campaigns with goals between $25K - $40k are not consistent with that finding. 

![Outcomes_vs_Goals](https://github.com/cfusco77/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png) 

When Louise came to us, she had a $10,000 goal in mind, based on my analysis I would predict a 54% chance of success based on other plays with similiar sized goals.

### Limitations of the Dataset
The dataset only holds data up to 2017, ideally we would have data up to date, 2021, to feel more confident in our analysis and predictions of future outcomes.  

The outcome of the play is a categorical attribute determined based on whether the goal was met but does not take into condsideration how far off failed campaigns were from their goal. This might be an interesting addtional measure for further analysis. 


