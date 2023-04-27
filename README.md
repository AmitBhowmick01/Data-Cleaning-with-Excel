# *Data Cleaning using Excel*

This project is a guide for data cleaning using Microsoft Excel. It covers basic data-cleaning techniques that can be applied to any dataset using Excel.

## Table of Contents
- Introduction
- Prerequisites
- Data Cleaning Techniques:
  - Remove rows with condition
  - Clean and format columns
  - Fill in Blank Cells:
  
  
## Introduction

Data cleaning is the process of identifying, correcting, and removing errors, inconsistencies, and inaccuracies in datasets. It involves a series of steps such as data validation, data transformation, data normalization, and data enrichment to ensure that the data is accurate, complete, and consistent. The purpose of data cleaning is to improve the quality and reliability of data, making it more suitable for analysis, reporting, and decision-making. Data cleaning is a critical step in data preprocessing and is often performed before data analysis or machine learning algorithms are applied to the data.


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

