# kickstarter-analysis
Analyzing Kickstarter campaign trends for playwright Louise

## Overview of Project
This project examines the outcomes of kickstarter campaigns for plays by analyzing the campaigns' successes or failures based on the time of year they were launched, and how high their fundraising goals were. The dataset includes kickstarter campaigns ranging from 2009 to 2017.

### Purpose
This purpose of this project is to see whether the launch date or the fundraising goals for plays on Kickstarter has any relation to whether or not a campaign is successfully funded.

## Analysis and Challenges
The analysis can be broken down into two sections -- analysis of campaign outcomes based on launch date, and analysis of campaign outcomes based on fundraising goals. Before tackling either of these sections, however, a few adjustments needed to be made to the raw dataset first.

First, the Category of the types of kickstarters there were (music, publishing, theater, etc.) needed to be split into two columns, the Parent Category, and the Subcategory, so that the analysis could specifically focus on Plays, a subcategory of the parent category, Theater. This was done using the "Convert Text to Columns Wizard" in the Data tab of Excel. Next, because the calendar dates of the raw data were written in Unix timestamps, they were converted into the standard mm/dd/yyyy format so that the campaigns could be more easily analyzed by their launch dates.

### Analysis of Outcomes Based on Launch Date


### Analysis of Outcomes Based on Goals


### Challenges and Difficulties Encountered
There weren't any overt difficulties in the analysis, but there was some tedium when creating the table in the Outcomes Based on Goals tab of the xlsx file. The formulas needed in the first few columns couldn't easily be copied to fill out every cell with Excel's built-in quick-fill functions. Every cell needed a little bit of manual editing to ensure they had the correct formula, and because of this, special care had to be taken to ensure that there were no mistakes or typos in any of them.

## Results

- Outcomes based on Launch Date

It appears that most of the successful kickstarter campaigns for plays occurrs in May through July. Although there was also a greater total number of kickstarters run during this time, a greater percentage of them were still successful compared to most other times of year. The least successful period for kickstarter campaigns is December, which is most likely due to the holiday season, so it would be best to avoid running a kickstarter campaign during this time.

- Outcomes based on Goals

A majority of campaigns with goals that were less than $5000 USD were successful in raising funds, but for campaigns with goals of $5000 USD or more, chances of success drop significantly. Any campaigns with goals at $45,000 USD or above are highly likely to fail to raise enough funds. Based on this, it seems that it may be best to keep budget goals under $5000 USD.

- Limitations

This data set doesn't take into account other factors that could influence the outcomes of the kickstarter campaigns, such as advertisement strategies, genre of the plays, duration of the campaign, or whether or not the a campaign was highlighted by kickstarter as a staff pick.

- Potential Avenues for Future Analysis

It would be quite interesting to see if there are any correlations between campaign outcomes, their fundraising goals, and the duration for how long the campaigns lasted. It may also be useful to know how many backers each campaign had, and how much each campaign raised, to see on average approximately how much each backer would pledge -- this information would be useful to to gather an idea of how many people would need to be attracted in advertising campaigns.
