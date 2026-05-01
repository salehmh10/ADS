# Applied Data Science - Assignment 1

## Overview
This repository contains my first assignment for the Applied Data Science course.  
It includes one main data analysis notebook and one bonus web scraping notebook.

## Files
- `assignment1.ipynb`: Main assignment notebook
- `HW1_BONUS.ipynb`: Bonus web scraping notebook
- `Data.csv`: Tehran housing dataset
- `samand_bama_bonus.xlsx`: Final scraped Samand car dataset

## Part 1: Main Assignment - Tehran Housing Analysis
The main notebook analyzes a Tehran housing dataset with 12,383 rows and 9 columns.

Main steps:
- Loaded and inspected the dataset
- Checked missing values and duplicate rows
- Cleaned invalid and unrealistic values
- Converted and validated numerical columns
- Created `price_per_meter`
- Encoded neighborhoods based on average price per meter
- Created new features such as `age`, `quality_score`, `compare_to_mean`, and `neighborhood_price_category`
- Used different visualizations, including histogram, scatter plot, pie chart, bar chart, line chart, multi-line chart, and an interactive Plotly chart
- Applied feature transformations
- Used Mutual Information for feature selection
- Standardized numerical features and applied PCA
- Answered the feature engineering reflection question

After cleaning and outlier removal, the dataset was reduced to 10,307 rows.

## Part 2: Bonus - Web Scraping
The bonus notebook collects data for 50 Samand cars manufactured after 1385 from bama.ir.

Extracted fields:
- price
- mileage
- color
- production year
- transmission type
- description
- title
- url

There was a problem because the main bama.ir link returned only about 30 ads.  
To solve this, I divided prices into 5 ranges and used 5 different links:

- 300M to 500M
- 500M to 700M
- 700M to 1B
- 1B to 1.5B
- 1.5B to 3B

In total, 272 ad links were collected, and the final dataset contains 50 valid Samand car records.

## Tools
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly
- Scikit-learn
- Selenium

