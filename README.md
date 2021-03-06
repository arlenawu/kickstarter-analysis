# kickstarter-analysis
Analyzing Kickstarter campaign trends for playwright Louise

## Overview of Project
This project examines the outcomes of Kickstarter campaigns for plays by analyzing the campaigns' successes or failures based on the time of year they were launched, and how high their fundraising goals were. The dataset includes Kickstarter campaigns ranging from 2009 to 2017.

### Purpose
This purpose of this project is to see whether the launch date or the fundraising goals for plays on Kickstarter has any relation to whether or not a campaign is successfully funded.

## Analysis and Challenges
The analysis can be broken down into two sections -- analysis of campaign outcomes based on launch date, and analysis of campaign outcomes based on fundraising goals. Before tackling either of these sections, however, a few adjustments needed to be made to the raw dataset first.

First, the Category of the types of Kickstarter campaigns there were (music, publishing, theater, etc.) needed to be split into two columns, the Parent Category, and the Subcategory, so that the analysis could specifically focus on Plays, a subcategory of the parent category, Theater. This was done using the "Convert Text to Columns Wizard" in the Data tab of Excel. Next, because the calendar dates of the raw data were written in Unix timestamps, they were converted into the standard mm/dd/yyyy format so that the campaigns could be more easily analyzed by their launch dates.

### Analysis of Theater Outcomes Based on Launch Date
In order to examine the relationship between the campaigns' outcomes and their launch date, and to see what time of year has been best to launch Kickstarter campaigns, a pivot table was created from the dataset. The table was filtered to only show campaigns from the parent category Theater. The rows of the table showed the month each campaign was launched, and the columns displayed their outcomes. This provided a quick count of how many successful, failed, and canceled Theater campaigns there were that launched each month from 2009 to 2017. Any ongoing, live campaigns were omitted from the data in order to focus on the outcomes of campaigns that had already finished. A line graph was created in order to better visualize the data, which can be seen here: [Theater Outcomes vs_Launch](Resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
The next step was to see what percentage of campaigns succeeded, failed, or were canceled in relation to how high their fundraising goals were. Goals were divided into twelve tiers from less than $1,000 USD to $50,000 USD or higher. The number of successful, failed, and canceled plays were counted for each tier using Excel's built-in count functions, and from there the percentages of successful, failed, and canceled plays were calculated. A line chart was then produced from the results, which can be seen here: [Outcomes_vs_Goals](Resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered
There weren't any overt difficulties in the analysis, but there was some tedium when creating the table in the Outcomes Based on Goals tab of the .xlsx file. The formulas needed in the first few columns couldn't easily be copied to fill out every cell with Excel's built-in quick-fill functions. Every cell needed a little bit of manual editing to ensure they had the correct formula, and because of this, special care had to be taken to ensure that there were no mistakes or typos in any of them.

## Results

- Outcomes based on Launch Date

It appears that most of the successful Kickstarter campaigns launched in May through July. Although there was also a greater total number of campaigns launched during this time, a greater percentage of them were still successful compared to most other times of year. The least successful launch period for Kickstarter campaigns is December, which is most likely due to the holiday season, so it would be best to avoid launching a new campaign during that time.

- Outcomes based on Goals

A majority of campaigns with goals that were less than $5,000 USD were successful in raising funds, but for campaigns with goals of $5,000 USD or more, chances of success drop significantly. Any campaigns with goals at $45,000 USD or above are highly likely to fail to raise enough funds. Based on this, it seems that it may be best to keep budget goals under $5,000 USD.

- Limitations

This data set doesn't take into account other factors that could influence the outcomes of the Kickstarter campaigns, such as advertisement strategies, genre of the plays, duration of the campaign, or whether or not the campaign was highlighted by Kickstarter as a staff pick.

- Potential Avenues for Additional Analysis

It would be quite interesting to see if there are any correlations between campaign outcomes, their fundraising goals, and the duration for how long the campaigns lasted. It may also be useful to know how many backers each campaign had, and how much each campaign raised, to see on average approximately how much each backer would pledge -- this information would be useful to gather an idea of how many people would need to be attracted in advertising campaigns.
