# Tech Layoffs Data Cleaning Project (2019-Present)

## Project Overview
This project focuses on cleaning, standardizing, and preparing a real-world tech layoffs dataset sourced from Kaggle: “Layoffs Dataset: Tech layoffs from COVID-19 (2019) to present.” The dataset captures layoffs across global technology companies during one of the most volatile periods in modern economic history. The primary goal of this project was to transform raw, messy data into high-quality, analysis-ready data using SQL-based data cleaning techniques.

## Objectives
* Ensure data accuracy, consistency, and reliability
* Eliminate duplicate records
* Standardize categorical fields (company names, industries, locations)
* Handle missing and null values appropriately
* Prepare the dataset for exploratory analysis, visualization, and modeling

## Data Cleaning Process
1. Removing Duplicates
* Used ROW_NUMBER() with PARTITION BY to identify duplicate records
* Retained only the most relevant entries to ensure record uniqueness

2. Standardizing Text Fields
* Applied TRIM() to remove leading/trailing whitespaces
* Standardized company names, industries, and locations to avoid false category splits
* Corrected inconsistent capitalization and naming variations

3. Handling Missing & Null Values
* Identified incomplete records using IS NULL
* Removed rows with insufficient critical information where appropriate
* Ensured numerical fields (e.g., layoffs count) were logically valid

4. Validating Data Relationships
* Used JOINs to verify consistency across related fields and records
* Cross-checked company, industry, and location values to detect mismatches

## Outcome
The final dataset is:
* Clean and standardized
* Free of duplicates and structural inconsistencies
* Ready for EDA, dashboards, and predictive modeling
* Suitable for real-world business and economic analysis

This cleaned dataset can now be confidently used to analyze:
* Layoff trends over time
* Industry-specific impacts
* Geographic distribution of layoffs
* Company-level workforce volatility
