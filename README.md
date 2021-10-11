# Kickstarting with Excel

## Overview of Project

### Purpose

Louise has been hard at work on her campaign. This project aims to help Louise with her campaign and timeline. She is now interested in understanding how different campaigns performed in relation to their launch dates and their funding goals. The analysis for outcomes based on launch date will specifically look at the “theater” category, and the analysis for outcomes based on funding goals will look at the “plays” subcategory.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

To discover any trends in theater outcomes based on launch date, a pivot table was created to customize all of the Kickstarter data to only show outcomes and launch date by month with filters for the parent category and years. The parent category was filtered to only show theater. Using the pivot table, a line chart was generated to visualize the relationship between campaign outcomes and the month they were launched. The chart below revealed that the month that launched the most successful Kickstarter campaigns (111) for theater was May. March, and September had roughly the same number of successful campaigns launched (high 50s). Campaigns launched in December were least likely to perform well and succeed. As for failed campaigns, the months May, June, July, August, and October all had roughly the same number of campaigns launched (50).

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/90656004/136834719-37854c74-ec57-467e-add3-b1c040048b89.png)

### Analysis of Outcomes Based on Goals

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/90656004/136834734-eca41551-237e-4db0-9b69-70f9184d4e16.png)

### Challenges and Difficulties Encountered

A challenge encountered was not using the proper formulas to determine the outcomes based on goals. Initially, the data was filtered in the Kickstarter tab of the Excel workbook. The outcome column was filtered to only show one outcome type at a time and to only show plays in the subcategory column. The resulting outcome percentages for each goal-amount range did not make mathematical sense. It became clear that the formulas needed to reflect the filters for the outcome types and the plays subcategory instead of relying on the filter tool. Once the filters for outcome and subcategory were included in the formulas, the data was able to be properly customized to reveal the number of successful, failed, and canceled outcomes by goal range as well as the percentage of each outcome by goal range. 

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

    Campaigns for plays launched in May were more successful than those launched in any other month.
    The month of December experienced the least number of successful campaign outcomes for plays. 

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
