# Kickstarting with Excel
    ** This is a repository to store the Module 1 Excel Challenge **

## Overview of Project
Louise wants to know how different campaigns fared in relation to their launch dates and their funding goals.

### Purpose
Using the Kickstarter dataset to visualize campaign outcomes (especially for parent category theater) based on their launch dates and visualize the percentage of successful, failed, and canceled plays based on the funding goal amount (especially for subcategory plays).

## Analysis and Challenges
Deliverable 1: Outcomes Based on Launch Date Chart
    
    1. Using the Kickstarter dataset, Create a pivot tables and graphing in Excel to visualize   campaign outcomes ("successful," "failed," and "canceled") based on launch date.
    
    2. Create a new column labeled "Years." and use the YEAR() function to extract the year from the "Date Created Conversion" column.
    
    3. Create new pivot table sheet "Theater Outcomes by Launch Date." from the KickStarter worksheet
    
    4. Filter the pivot table based on "Parent Category" and "Years."
    
    5. Place the pivot table fileds "outcomes" on columns, "months" on rows, and "Count of 
       outcomes" on values.
    
    6. Filter the column labels to show only "successful," "failed," and "canceled."
    
    7. Filter the "Parent Category" to show only the data for "theater."
    
    8. Sort the campaign outcomes in descending order so "successful" is first.
    
    9. Create a line chart from the pivot table to visualize the relationship between outcomes  
       and launch month.


Deliverable 2: Outcomes Based on Goal Chart
    
    1. Create a new sheet and label it "Outcomes Based on Goals." in the KickStarter Sheet.
    
    2.  Create a new sheet "Outcomes Based on Goals" with following columns 
        
        Goal
        Number Successful
        Number Failed
        Number Canceled
        Total Projects
        Percentage Successful
        Percentage Failed
        Percentage Canceled
    
    3. In the Goal column, create the following dollar-amount ranges so projects can be 
       grouped based on their goal amount.

        Less than 1000
        1000 to 4999
        5000 to 9999
        10000 to 14999
        15000 to 19999
        20000 to 24999
        25000 to 29999
        30000 to 34999
        35000 to 39999
        40000 to 44999
        45000 to 49999
        50000 or more

    4. Use COUNTIFS() functions to populate the "Number Successful," "Number Failed," and "Number Canceled" columns by filtering on the Kickstarter "outcome" column, on the "goal" amount column using the ranges created in Step 3, and on the "Subcategory" column using "plays" as the criteria.
    
    5. Use the SUM() function to populate the "Total Projects" column with the number of successful, failed, and canceled projects for each row.
    
    6. Calculate the percentage of successful, failed, and canceled projects for each row.

    7. Create a line chart titled "Outcomes Based on Goal" to visualize the relationship between the goal-amount ranges on the x-axis and the percentage of successful, failed, or canceled projects on the y-axis.

### Analysis of Outcomes Based on Launch Date
![image_name](https://github.com/raneymjohnGit/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png)


### Analysis of Outcomes Based on Goals
![image_name](https://github.com/raneymjohnGit/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png)


### Challenges and Difficulties Encountered

Deliverable 2: Outcomes Based on Goal Chart
    1. When we format the "Sum of Percenatge Sucessful", "Sum of Percenatge Failed", "Sum of Percenatge Canceled" to "Percentage",  the Y-axis on the chart becomes multiplied by 100.
    So inorder to avoid that, I kept the format of the "Sum of Percenatge Sucessful", "Sum of Percenatge Failed", "Sum of Percenatge Canceled" to "Number" and created the chart then changed the format of the fields in the Pivot table

Reference documents:
1.  Module 1 from our Boot Camp
2.  COUNTIFS: https://support.microsoft.com/en-us/office/countifs-function-dda3dc6e-f74e-4aee-88bc-aa8c2a866842



## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
   1. Campaigns started in the month of May and June have more successful outcomes
   2. December less number of campaigns compared to other months.


- What can you conclude about the Outcomes based on Goals?
    1.  Lesser the goal amount, chances of success are high.

- What are some limitations of this dataset?
    1. This data set has no information on the cities, or age group that they are targeting. 

- What are some other possible tables and/or graphs that we could create?
    1. We could create another chart Outcome based on number of backers
