# Kickstarting with Excel

## Overview of Project

### Purpose

Louise has been hard at work on her campaign. This project aims to help Louise with her campaign and timeline. She is now interested in understanding how different campaigns performed in relation to their launch dates and their funding goals. The analysis for outcomes based on launch date will specifically look at the “theater” category, and the analysis for outcomes based on funding goals will look at the “plays” subcategory.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

To discover any trends in theater outcomes based on launch date, a pivot table was created to customize all of the Kickstarter data to only show outcomes and launch date by month with filters for the parent category and years. The parent category was filtered to only show theater. Using the pivot table, a line chart was generated to visualize the relationship between campaign outcomes and the month they were launched. The chart below revealed that the month that launched the most successful Kickstarter campaigns (111) for theater was May. March, and September had roughly the same number of successful campaigns launched (high 50s). Campaigns launched in December were least likely to perform well and succeed. As for failed campaigns, the months May, June, July, August, and October all had roughly the same number of campaigns launched (50).

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/90656004/136834719-37854c74-ec57-467e-add3-b1c040048b89.png)

### Analysis of Outcomes Based on Goals

The following analysis of outcomes based on funding goals provides Louise with a visual representation of successful, failed, and canceled plays based on the funding goal amount. The goals indicate how much money each campaign need to succeed, and the outcomes convey whether the campaign met its goal. For the purposes of this analysis, the funding goals were grouped into dollar-amount ranges. The COUNTIFS function was used to determine the number successful, failed, and canceled plays. For example, the formula used to find the number of successful campaigns with funding goals of less than $1,000 was =COUNTIFS(Kickstarter!$D:$D,"<1000",Kickstarter!$F:$F,"successful",Kickstarter!$R:$R,"plays"). In the Kickstarter data sheet, column D consisted of the goals, column F was the outcome, and column R contained the subcategory. After filtering to only show the “plays” subcategory and finding the number of each outcome, total projects for each goal-amount range were calculated. The final step consisted of calculating the percentages of each outcome type by goal-amount range and creating a line chart based on the resulting percentages. 

This analysis revealed that most successful campaigns had goals less than $1,000, between $35,000 to $39,999, and between 40,000 to $44,999. Most failed campaigns had goals between $45,000 to $49,999.

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/90656004/136834734-eca41551-237e-4db0-9b69-70f9184d4e16.png)

### Challenges and Difficulties Encountered

A challenge encountered was not using the proper formulas to determine the outcomes based on goals. Initially, the data was filtered in the Kickstarter tab of the Excel workbook. The outcome column was filtered to only show one outcome type at a time and to only show plays in the subcategory column. The resulting outcome percentages for each goal-amount range did not make mathematical sense. It became clear that the formulas needed to reflect the filters for the outcome types and the plays subcategory instead of relying on the filter tool. Once the filters for outcome and subcategory were included in the formulas, the data was able to be properly customized to reveal the number of successful, failed, and canceled outcomes by goal range as well as the percentage of each outcome by goal range. 

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

  As discussed in a previous section, campaigns for plays launched in May were more successful than those launched in any other month. The month of December experienced the least number of successful campaign outcomes for plays. 

- What can you conclude about the Outcomes based on Goals?

  Plays with higher funding goals (greater than $45,000) were less successful than those with lower funding goals.

- What are some limitations of this dataset?

  Based on this dataset, it cannot be determined how many individuals pledged to each campaign. This can make a big difference in understanding why some campaigns had such high or low goal amounts and such high or low pledge amounts. Some successful campaigns required less money to reach their goals whereas many failed campaigns had some of the highest funding goals. Another limitation was that outliers were not identified and eliminated since they may not have been representative of the data as a whole and for the purposes of our analysis. Lastly, the funding goals and pledges do not indicate what the money would go towards, like infrastructure building, marketing, or payroll. This breakdown would allow for us to analyze the data on a more granular level if we wanted.

- What are some other possible tables and/or graphs that we could create?

  An additional chart that could be created with this dataset would be a line chart that looks at a different category and a specific year or compare different years with a chart for each year. For example, we could choose the “film & video” category and see how it performs in 2009 compared to 2017. Also, if it were possible to get the data on how many people were pledged to each campaign, it would be interesting to see funding goals in relation to the number of individuals pledging money toward them. This could be shown in either a line or bar chart depending on which provides the best visual representation. 
