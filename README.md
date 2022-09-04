# Kickstarting with Excel

## Overview of Project

### Purpose

-The purpose of the analysis was to compare how different fundraising campaigns faired in relation to the launch dates and the funding goals.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

-The analysis of outcomes based on launch date was performed by creating a pivot table from the kickstarter dataset. A new 'year' column was added to the kickstarter sheet to allow the data to be filtered by Parent Category and Year. The columns were set to 'outcomes', the 'Data Created Conversion' was used for rows, and the values were set to 'Count of outcomes'. The column labels were adjusted to show only 'successful', 'failed' and 'cancelled' outcomes from the fundraising campaigns. Then the columns were sorted in descending order and the row labels were converted from years each campaign started to the month it started. From there, a pivot chart was created from the pivot table to display the data in a line chart to visualize the relationship between outcomes and launch month.The total outcomes from successful, failed and cancelled campaigns were shown on the y-axis, and the month the campaigns were started were shown on the x-axis.

### Analysis of Outcomes Based on Goals

- A new sheet was created to show the outcomes based on goals of the fundraising campaigns. A total of eight columns were added to the new sheet: goal, number successful, number failed, number canceled, total projects, percentage successful, percentage failed and percentage canceled. Dollar amount ranges were created in the goal column to group on their goal amount. The majority of the ranges covered a $5000 range except for the first and last ranges, which were set to less than $1000 and greater than $50000 respectively. From there countif() functions were used to populate the number successful, number failed and number canceled columns by filtering the outcome, goal and subcategory columns from the original kickstarter data set. The criteria 'plays' was used from the subcategory column. Next, the sum() function was used to populate the total project column by taking the sum of projects generated in the number successful, failed and canceled columns. Subsequently, the percentage of succesful, failed and canceled projects was calculated from the corresponding columns and the total projects column. From there, a line chart was created from the data generated to show the relationship between dollar-amount goals on the x-axis versus the percentage of successful, failed or canceled projects on the y-axis.

### Challenges and Difficulties Encountered

- One difficulty that was encountered during the analysis occurred when the parent category needed to be filtered by theater. Theater was not an option shown as a filter, so multiple filters were selected to include all the subcategories within the parent category of theater.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
    - One conclusion from the analysis is that the best probability to have a successful outcome for theater is to release the event during the months of February, May and June. My best guess for the success of theater events during those months is likely due to those time periods coinciding with spring and summer breaks for students or children. Parents would need to provide entertainment to their children during those months and would not have the restrictions of school night curfews, or family travel that occurs around the fall holidays.
    - The second conclusion is that canceled theater events remains nearly constant and at a low rate throughout the year. You can cancel at anytime!

- What can you conclude about the Outcomes based on Goals?
    - It can be concluded from the analysis that best chance for a play to be successful at the lowest cost occurs in the ranges of less than $1000 and $1000 to $4999. Essentially, set the top end of the budget for the play to $5000 and it has the best opportunity for a positive return on investment.

- What are some limitations of this dataset?
    - The limitations of the analysis is that it does not factor in the location or year the theater events were released. Both of those factors could be highly influential to the success of an event.

- What are some other possible tables and/or graphs that we could create?

    -  The theater outcomes could be separated into subcategories to analyze, which subcatergory from musicals, plays and spaces tended to be the most succesful from the theater category.
    - The location of the successful plays could be analyzed to determine if certain cities or metropolitan areas have higher success rates.