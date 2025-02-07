# Hotels Data Analysis Project

## Overview

The Hotels Data Analysis Project aims to analyze hotel bookings, occupancy rates, revenue generation, and trends across different hotel categories, cities, and booking platforms. This project uses datasets that include hotel details, room types, bookings, and aggregated booking statistics to provide valuable insights into the hospitality industry.

## Datasets

We are using five datasets for this project:

- dim_date.csv - Contains date-related information.

- dim_hotels.csv - Contains details of different hotels, including their category and location.

- dim_rooms.csv - Lists room categories and classifications.

- fact_aggregated_bookings.csv - Provides aggregate booking statistics per property.

- fact_bookings.csv - Includes detailed booking data.

## Project Workflow

### 1. Data Import and Exploration

  We start by loading the datasets and performing an initial exploration:

  - Checking dataset structures and dimensions.
    
  - Exploring unique values in key categorical variables such as room_category and booking_platform.
    
  - Analyzing distribution and trends in booking platforms using visualizations.
    
  - Understanding hotel distributions across different cities.

### Key Findings:

  - Identification of different booking platforms and their popularity.
    
  - Variability in hotel categories and room types.
    
  - Hotel distribution across various cities.

## 2. Data Cleaning

Data cleaning is performed to ensure accuracy and consistency in analysis:

  - Handling invalid guest entries: Removed records where the number of guests was less than or equal to zero.
  
  - Outlier removal: Identified and removed extreme values in revenue-related fields.
  
  - Null value handling: Kept missing ratings as filtering them would remove significant portions of the data.
  
  - Ensuring booking integrity: Removed records where successful_bookings exceeded capacity.

## 3. Data Transformation

To improve analytical insights, transformations were applied:

  - Created an occupancy percentage (occ_pct) column to analyze hotel occupancy.
  
  - Merged different datasets to facilitate city-based and category-based analyses.
  
  - Converted categorical codes (e.g., RT1, RT2) into meaningful room classification labels.

## 4. Insights Generation

Using the cleaned and transformed data, key insights were generated:

### 1. Average Occupancy Rate by Room Category
    
  - Computed the average occupancy rate for each room class (e.g., Standard, Premium, Elite).

### 2. City-wise Occupancy Rate

 - Determined which cities had the highest and lowest occupancy percentages.

### 3. Weekday vs. Weekend Occupancy

 - Analyzed whether hotels had better occupancy rates during weekends or weekdays.

### 4. Monthly Occupancy Trends

 - Focused on occupancy rates in specific months, such as June.

### 5. Revenue Analysis

  - Revenue Realized per City: Summed up total revenue generated in each city.
  
  - Revenue by Booking Platform: Visualized revenue distribution across different booking platforms.
  
  - Month-by-Month Revenue Trends: Analyzed how revenue fluctuates over different months.
  
  - Revenue per Hotel Type: Identified the most profitable hotel categories.

### 6. Ratings Analysis

  - Average Rating per City: Computed the mean rating given to hotels in each city.
  
  - Impact of Ratings on Revenue: Explored the correlation between guest ratings and revenue generated.

## Visualizations

Several visualizations were created to aid in better understanding:

 - Pie Chart: Distribution of bookings by platform.

 - Bar Charts: City-wise hotel counts and revenue realized per city.

 - Time Series Plots: Month-over-month revenue trends.

### New Data Integration

A new dataset for August was appended to the existing data to keep the analysis up-to-date.

## Conclusion

This project provides a detailed understanding of hotel bookings, occupancy trends, revenue generation, and key factors affecting the hospitality business. It allows stakeholders to make data-driven decisions regarding hotel operations, marketing strategies, and pricing policies.

## How to Run the Project

### Prerequisites

Ensure you have the following installed:

  - Python 3.x
  
  - Pandas
  
  - Matplotlib
