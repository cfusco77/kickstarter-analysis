# An Analysis of Kickstarter Campaigns 
---
## Overview of Project
Perform analysis using a dataset of several thousand crowdfunding projects to uncover any hidden trends

### Purpose
The purpose of this invetigation is to provide our client, Louise, a visual analysis of campaign outcomes based on their launch dates and their funding goals. Louise is a an up and coming playright looking to get her next project, Fever, funded via a crowdfunding campaign. Upon analysis we will provide Louise a recommendation so that her first crowdfunding campaign is a success. 

## Analysis and Challenges
Please note that when I recieved the raw data both the Deadline and Launched_at columns contained dates formatted as Unix timestamps. I have converted that data into short form dates to aid in our analysis and provide Louise a readable output. 

### Analysis of Outcomes Based on Launch Date

Of the 4113 crowdfunding campaigns 1393 are categorized under the Parent Category: Theater. I have filted the dataset to include only Theater campaigns in the following analysis. The table, pictured below, illustrates the count of campaign outcomes by month. It appears May is an exceptionally good time to launch a campaign, followed by June and then July. 

![Theater_Outcomes_vs_Launch](https://github.com/cfusco77/kickstarter-analysis/blob/main/Theater_Outcomes_vs_Launch.png)

I want to point out a limitation of this table: Here I have shown the count of each type of outcome throughout the year. Perhaps instead we should plot the outcome rates which would control for the number of campaigns launched each month. I have performed this secondary analysis to confirm that success rate is in fact the highest in May and June. An additional finding, which may be harder to ascertain from the table, is that May and June also have the lowest failure rates. 

---
### Analysis of Outcomes Based on Goals
![Outcomes_vs_Goals](https://github.com/cfusco77/kickstarter-analysis/blob/main/Outcomes_vs_Goals.png) 

### Challenges and Difficulties Encountered

## Next Steps 

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?

