# Data Analysis Report: Used Cars Dataset

## Overview

This report provides an analysis of the **Used Cars Dataset**. The dataset contains information about used cars listed on Craigslist, including features such as car price, year, mileage, manufacturer, condition, fuel type, and more. The analysis includes cleaning the data, handling missing values, and answering various business questions using the dataset.

## Data Overview

The dataset consists of the following columns:
- `price`: Price of the car
- `year`: Model year of the car
- `odometer`: Mileage of the car (in miles)
- `manufacturer`: The manufacturer of the car
- `model`: The model of the car
- `condition`: Condition of the car (e.g., new, like new, excellent, etc.)
- `fuel`: Type of fuel used by the car
- `transmission`: Type of transmission (automatic/manual)
- `drive`: Drivetrain (e.g., FWD, RWD, 4WD)
- `type`: Type of car (e.g., sedan, SUV, truck)
- `paint_color`: The color of the car
- `region`: Region where the car is listed
- `state`: State where the car is listed
- `lat`: Latitude of the car's location
- `long`: Longitude of the car's location

## Data Cleaning

We started by assessing the dataset and identifying columns with missing values. Rows containing any missing values were removed to ensure a clean dataset for analysis.

```python
# Drop all rows with any missing values
df.dropna(inplace=True)

# Verify if any missing values remain
df.isnull().sum()
# vechiles-dataset-EDA
