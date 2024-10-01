# Tumor Volume Analysis for Drug Regimens in Mice

## Project Overview

This project focuses on analyzing tumor volume data from a study involving various mice treated with different drug regimens. The primary objective is to assess the effectiveness of these treatments by visualizing and analyzing key metrics such as tumor volume, mouse weight, and time points.

### Key Objectives:
- Merging datasets to create a single comprehensive DataFrame.
- Cleaning the data to remove duplicate entries based on Mouse ID and Timepoint.
- Generating summary statistics for tumor volumes (mean, median, variance, standard deviation, SEM).
- Creating bar charts, pie charts, line plots, scatter plots, and box plots.
- Identifying potential outliers using interquartile range (IQR).
- Performing correlation and regression analysis on mouse weight and tumor volume for the Capomulin regimen.

## Data Preparation

### Steps:
1. **Merge Datasets**: The datasets are merged to form a single DataFrame that includes information about the mice, their treatment regimens, and tumor volume over time.
2. **Clean the Data**: Duplicate data (mice with the same Mouse ID and Timepoint) are identified and removed, resulting in a clean DataFrame.
3. **Display Mice Count**: The number of unique mice is displayed before and after data cleaning.

## Summary Statistics

Using the `groupby()` function, the following summary statistics were generated for each drug regimen:
- Mean tumor volume.
- Median tumor volume.
- Variance of tumor volume.
- Standard deviation of tumor volume.
- Standard error of the mean (SEM) of tumor volume.

These statistics help in understanding the distribution of tumor volumes for each treatment group.

## Visualizations

### 1. **Bar and Pie Charts**:
- A **bar plot** is generated showing the total number of time points for all mice tested in each drug regimen.
- A **pie chart** shows the distribution of unique male vs. female mice across the study.

### 2. **Box Plot**:
- A **box plot** is created to show the distribution of the final tumor volume for all mice across four treatment groups: Capomulin, Ramicane, Infubinol, and Ceftamin.
- The interquartile range (IQR) and outliers are identified for each group.

### 3. **Line Plot**:
- A **line plot** is created for a single mouse treated with the Capomulin regimen, showing tumor volume over time.

### 4. **Scatter Plot**:
- A **scatter plot** is generated showing the relationship between average tumor volume and mouse weight for the Capomulin regimen.

## Correlation and Regression

- The **correlation coefficient** is calculated between mouse weight and average tumor volume for the Capomulin regimen.
- A **linear regression model** is applied, and the regression line is plotted on the scatter plot to visualize the relationship.

## Project Structure

```bash
📂 tumor-volume-analysis
├── data/
│   ├── Mouse_metadata.csv
│   ├── Study_results.csv
├── analysis.ipynb       # Jupyter notebook containing the full analysis
├── README.md            # Project documentation
└── output/              # Output charts and visualizations
