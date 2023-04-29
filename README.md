# *Data Cleaning using Excel*

This project is a guide for data cleaning using Microsoft Excel. It covers basic data-cleaning techniques that can be applied to any dataset using Excel.

## Table of Contents
- Introduction
- Task performed
- Prerequisites
- Data Cleaning Techniques:
  - Remove rows with condition
  - Clean and format columns
  - Fill in Blank Cells:
- Highlighting Rows with the Top 10 Highest Salary

  
## Introduction

Data cleaning is the process of identifying, correcting, and removing errors, inconsistencies, and inaccuracies in datasets. It involves a series of steps such as data validation, data transformation, data normalization, and data enrichment to ensure that the data is accurate, complete, and consistent. The purpose of data cleaning is to improve the quality and reliability of data, making it more suitable for analysis, reporting, and decision-making. Data cleaning is a critical step in data preprocessing and is often performed before data analysis or machine learning algorithms are applied to the data.


## Task performed

The following assignment is given by `Unmassenger`. To perform the data-cleaning following tasks are given:

**Task 1:** Where **Name and Email-Id** is missing delete the entire row.

**Task 2:** Where **Name** is missing fill the value in place by extracting the name from the **Email-id column**.

**Task 3:** Fill the Missing Age value with the **mean of the Age column**.

**Task 4:** Clean and Format the Phone number column and it should show like (**91-xxxxxxxx**).

**Task 5:** Where the Name is there but no Email-Id then fill the blank with (**support@dataisgood.com**).

**Task 6:** Where address is not there fill it with (**Address not Available**).

**Task 7:** In the **Department column** make the data proper with the useful functions and rename the Wrong-spelled words in the department column.

**Task 8:** Highlight the **Top 10 Employees** with the highest salary in the dataset.

**`These tasks are recorded in macro and can be checked within the Excel file attached to this repository.`**


## Prerequisites

To follow along with this project, you will need:

- Microsoft Excel installed on your computer
- A dataset to clean

## **Data Cleaning Techniques**

### Remove rows with condition

There are some data in the dataset where we are unable to identify the actual relationship with other data so it is better to remove those data from the dataset. In the dataset where Name and Email ID are missing, we will remove those entire rows. 

We can use the filter function in Excel to remove rows where two columns data are missing. Here are the steps:

- Select the dataset in Excel.
- Click on the "Data" tab in the top menu.
- Click on the "Filter" button.
- Click on the filter arrow in the column header of the first column with missing data.
- Deselect the checkbox for the (Blanks) option.
- Click on the filter arrow in the column header of the second column with missing data.
- Deselect the checkbox for the (Blanks) option.
- Excel will now filter the dataset and remove all rows where either of the two columns has missing data.

### Clean and format columns

Cleaning and formatting columns can make data to easy to understand, sometimes the data is not in the proper format, which will make analysis critical. 

We can make the data easy to understand by correcting the data and wrong-spelled words in a column. To uppercase a column in Excel using `UPPER` function and then find and replace the incorrect spelling, follow these steps:

- Select the sheet containing the column you want to convert to uppercase.
- Click on the cell in the column where you want to start the uppercase conversion.
- In the formula bar at the top of the screen, enter the UPPER function and the cell reference of the first cell in the column. For example, if you want to convert the "A" column to uppercase and you want to start with cell A2, enter `"=UPPER(A2)"` in the formula bar.
- Press Enter to apply the UPPER function to the first cell in the column.
- Excel will convert the text in the cell to uppercase. To apply the UPPER function to the rest of the cells in the column, click on the cell where you applied the function and drag the fill handle (the small square at the bottom-right corner of the cell) down to the last cell in the column that you want to convert.
- Release the mouse button to apply the UPPER function to all selected cells.
- The entire column should now be in uppercase.
- Now, to find and replace the incorrect spelling, click on the "Find & Select" button in the "Editing" group on the "Home" tab.
- Select "Replace" from the drop-down menu.
- In the "Find what" field, enter the incorrect spelling that you want to replace. For example, if "Marketing" was misspelled as "Marketting," enter "Marketting" in this field.
- In the "Replace with" field, enter the correct spelling. In our example, enter "Marketing" in this field.
- Click on the "Replace All" button to replace all instances of the incorrect spelling with the correct spelling. If you want to review each instance before replacing, click on "Find Next" and then "Replace" for each instance.
- Once you have reviewed and replaced all incorrect spellings, you can save the changes to the worksheet.

### Fill in Blank Cells

Blank cells can cause errors in analysis. You can fill in blank cells with the following steps:

- Select the data range.
- Go to the Home tab in the ribbon.
- Click on the Find & Select button.
- Click on the Go To Special option.
- Select the Blanks option.
- Click OK.
- Type in the value to fill in the blank cells.
- Press Ctrl + Enter.

### Highlighting Rows with the Top 10 Highest Salary

To highlight the Top 10 Employee rows with the highest salary in the dataset, the following steps been followed:

- Select the dataset in Excel.
- Click on the "Home" tab in the ribbon and then click on "Conditional Formatting" in the "Styles" group.
- Select "New Rule" from the drop-down menu.
- In the "New Formatting Rule" dialog box, select "Use a formula to determine which cells to format."
- In the "Format values where this formula is true" field, enter the following formula: =RANK.EQ($M7,$M:$M)<=10
- This formula will highlight rows where the value in the Salary column is less than or equal to the 10th Rank in the column.
- Click on the "Format" button and select the formatting style that you want to use to highlight the rows that match the criteria.
- Click on "OK" to close the "New Formatting Rule" dialog box.
- Now, all the 10 rows will be highlighted which have highest salary.

___________________________________________________________________________________________________
