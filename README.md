
#Module 5 Challenge 

---

## Data Analysis Summary

This document outlines the steps taken and insights gained from analyzing athletic sales data spanning 2020 and 2021.

### Step 1: Data Preparation

The analysis began with preparing the data through the following steps:

- **Data Consolidation**: Merged `athletic_sales_2020.csv` and `athletic_sales_2021.csv` into a single file using the `pd.concat()` method. This approach was chosen due to the identical column headers, variables, and data types across both files.
- **Null Value Check**: Employed `.isna()` to scan for any null values within the dataset. The inspection confirmed the absence of null values.
- **Date Conversion**: Transformed the `invoice date` from an object to a `datetime` format to facilitate further analysis. Verification via a print statement confirmed the successful conversion to `datetime64`.

### Step 2: Broad Analysis

A series of questions related to the sales data were addressed as follows:

1. Generated a pivot table to display total products sold by region, employing a multi-index and `aggfunc='sum'`. The table was sorted to highlight the top 5 regions by total products sold.
2. Grouped data by retailer and product line using the pivot table method to analyze sales distribution.
3. Identified the top 5 regions with the highest number of products sold and the most total sales, respectively.
4. Determined the top 5 retailers contributing the most to total sales, showcasing their performance.

### Step 3: Focused Analysis on Women’s Athletic Footwear

The analysis then narrowed down to examine sales of Women’s Athletic Footwear specifically:

1. Filtered the dataset to include only Women’s Athletic Footwear sales.
2. Utilized pivot tables to find the top 5 regions by the number of units sold and total sales of Women’s Athletic Footwear.
3. Set the `invoice date` as the index in a pivot table to observe sales trends, followed by printing the table for confirmation.
4. Resampled the data by days (`D`) and weeks (`W`) to identify peak sales periods, using `.resample()` and summarizing the highest sales by day and week.

Certainly! Here's how you can format the resources section for a Markdown document, such as a README.md file:

---

## Resources

For this assignment, I relied on the following resources to complete the work:

1. 04-Pandas-Data-Preparation-1
2. 05-Pandas-Data-Preparation-2
3. [Pandas Merging Guide](https://pandas.pydata.org/docs/user_guide/merging.html)
4. [Pandas Reshaping Guide](https://pandas.pydata.org/docs/user_guide/reshaping.html)
5. Coursera and DataCamp

---
---

