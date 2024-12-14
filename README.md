# Investment-Analysis

Problem Statement:

This project aims to provide actionable insights for identifying the most promising countries and the ideal investment types for an asset management company. The goal is to determine where the majority of investors are channeling their funds to make data-driven investment decisions. The dataset used in this analysis is sourced from Crunchbase, containing detailed records of funding rounds and company information.

Objectives:

1. Analyze funding data to identify patterns and trends in global investments.
2. Determine the top-performing countries based on investment volume.
3. Recommend the most suitable funding types (e.g., venture, angel, private equity) for optimal returns.

Technical Approach:

Data Preparation:

1. Data Loading: Imported and read data from multiple files including Rounds2 and Companies.txt.
2. Data Cleaning:
   1. Standardized data by converting key columns (e.g., permalink and company_permalink) to uppercase.
   2. Checked for and handled discrepancies between datasets, such as mismatched company records.
   3. Identified and removed redundant columns for streamlined analysis.
   4. Calculated and dropped columns with excessive missing values to ensure data quality.

Exploratory Data Analysis (EDA):

1. Pivot Table Analysis: Computed mean and median values of raised_amount_usd for different funding types to uncover trends.
2. Filtering: Applied range filters on raised_amount_usd to focus on investments between $4 million and $15 million.
3. Country Ranking: Identified the top 9 countries receiving the highest venture capital investments.
4. Category Segmentation: Created a main_category column using string extraction techniques to classify companies into broader sectors.

Feature Engineering:

1. Categorical Conversion:
  1. Transformed the raised_amount_usd column into categories (TypeA, TypeB, TypeC) using custom functions.
  2. Categories represent investment tiers for clearer segmentation.

Key Insights: 
  1. Top-performing countries in venture capital funding were ranked to prioritize investments.
  2. Main sectors were identified to align investments with industry trends.
  3. Funding types and amounts were analyzed to balance risk and opportunity..

Tools and Technologies:
  1. Python: Data analysis and manipulation using libraries like Pandas, NumPy, and Matplotlib.
  2. Data Visualization: Unveiled patterns through visualizations created with Matplotlib and Seaborn.
  3. Data Transformation: Applied advanced string and lambda functions for efficient feature creation.
