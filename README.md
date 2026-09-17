# Online Retail II - Data Cleaning and Feature Engineering

## Overview

This project focuses on data cleaning, preprocessing, exploratory data analysis, and feature engineering using the Online Retail II dataset.

The main goal is to prepare the raw retail transaction data for further analysis by identifying and handling data quality issues, creating useful features, and exploring sales patterns through visualizations.

## Dataset

The project uses the [UCI Online Retail II Dataset](https://archive.ics.uci.edu/dataset/502/online+retail+ii).

The dataset contains transactional data from a UK-based online retail company covering transactions between 2009 and 2011.

The original dataset is provided as an Excel file:

```text
online_retail_II.xlsx
```

The dataset itself is not included in this repository because it is a relatively large raw data file.

To run the notebook, download the dataset and place it in the project root directory.

## Project Objectives

The main objectives of this project are:

* Inspect the structure and quality of the raw dataset
* Identify missing values and duplicate records
* Clean invalid and inconsistent transaction records
* Handle canceled invoices
* Handle negative quantities and prices
* Address missing Customer IDs
* Create new features for analysis
* Explore sales trends and customer transactions
* Visualize important patterns in the data

## Data Cleaning

The following data cleaning steps were performed:

1. Loaded the raw Excel dataset.
2. Examined the dataset shape, data types, missing values, and duplicate records.
3. Removed duplicate rows.
4. Identified canceled invoices using invoice numbers starting with `C`.
5. Removed canceled transactions from the analysis.
6. Removed transactions with negative quantities.
7. Removed transactions with negative prices, including records identified as "Adjust bad debt".
8. Handled missing Customer IDs using the project's invoice-based imputation approach.

## Feature Engineering

Several new features were created to make the dataset more useful for analysis.

### Sales

Calculated the total sales value for each transaction:

```text
Sales = Quantity × Price
```

### Date and Time Features

Additional features were extracted from the transaction date:

* Year
* Month
* Day of Week
* Hour

These features allow the analysis of sales patterns over time.

## Exploratory Data Analysis

The notebook includes visualizations and analysis of:

* Sales by day of the week
* Number of orders by hour
* Monthly sales trends
* Revenue by country

These visualizations help identify patterns in customer transactions and sales performance.

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook
* Google Colab


## Proje
