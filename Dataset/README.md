# Job Dataset - Scraped & Cleaned

## Overview
This dataset contains job listings scraped from various job websites, including **Indeed**, **Glassdoor**, and **LinkedIn**. The data includes job titles, salaries, company names, locations, and other relevant details. It has been cleaned and preprocessed to be ready for analysis and model building.

## Files Description

- **Raw Data**:
  - `job_listings_indeed.csv`: Raw job data from Indeed.
  - `job_listings_glassdoor.csv`: Raw job data from Glassdoor.
  - `job_listings_linkedin.csv`: Raw job data from LinkedIn.

- **Cleaned Data**:
  - `job_listings_cleaned.csv`: Cleaned job listings with missing values and duplicates removed.
  - `salary_data_cleaned.csv`: Cleaned salary data after handling outliers and inconsistencies.
  - `location_data_cleaned.csv`: Standardized location data.

- **Data Preprocessing Scripts**:
  - `data_cleaning.py`: Data cleaning steps, including handling missing values and normalization.
  - `feature_transformation.py`: Encoding categorical variables and scaling numerical data.

## Data Science Steps Performed
1. **Data Scraping**: Scraped job-related data from **Indeed**, **Glassdoor**, and **LinkedIn**.
2. **Data Cleaning**: Removed duplicates, handled missing values, and standardized formats.
3. **Feature Engineering**: Transformed categorical data and scaled numerical features for model use.
4. **Ready for Modeling**: The cleaned data is prepared for building predictive models like salary prediction or job trend analysis.

## Usage
The dataset is ready for predictive modeling or data analysis tasks. Use the cleaned data for salary prediction, job trend forecasting, or other related tasks.
