# Health Partners Group (HPG) Analysis Project

## Overview
This project analyzes funding, funding partners, and implementing partners in Mozambique from 2016 to 2024. The Health Partners Group (HPG) in Mozambique compiled this dataset to facilitate communication and collaboration among stakeholders in the health sector.

## Data Source
The dataset was sourced from the Health Partners Group and includes information on:
- Project names
- Funding partners
- Implementing partners
- Project values (in various currencies)
- Project timelines
- Geographical coverage (provinces and districts)

**Note**: This analysis includes only current projects and excludes humanitarian projects.

## Data Cleaning and Preparation
The following data cleaning steps were performed:

1. **Data Import and Inspection**
   - Imported necessary libraries: pandas, numpy, matplotlib, seaborn, forex-python
   - Loaded the dataset from CSV format
   - Examined data structure and statistics

2. **Data Type Standardization**
   - Converted years to datetime format
   - Standardized funding amounts by converting all currencies to USD
   - Filled missing start dates with the mean start date (2021)

3. **Missing Value Handling**
   - Identified and visualized missing values percentages
   - Addressed missing data in geographical information
   - Created a "Not Specified" category for missing district data

4. **Data Reshaping**
   - Created a melted dataset to better represent geographical coverage
   - Created unique project identifiers to avoid confusion with duplicate project names
   - Exported cleaned dataset for analysis

## Exploratory Analysis
The analysis explores several key aspects of health project funding in Mozambique:

1. **Funding Partner Analysis**
   - Top 10 funding partners by number of projects
   - Treemap displaying funding partners proportional to total project value
   - Top 10 partners by total funding amount in USD

2. **Temporal Analysis**
   - Line chart showing total project value over time (by start year)
   - Analysis of funding changes during and after the COVID-19 pandemic (2020-2023)

3. **Project Value Analysis**
   - Total funding allocated across all projects ($3.65B)
   - Identification of highest funded project: Global Health Supply Chain Procurement and Supply Management (PSM) - $541,730,004
   - Identification of lowest funded project: Malaria - $42,000

4. **Collaboration Analysis**
   - Identification of collaboration patterns between funding partners and implementing partners
   - Heatmap visualization of key partnerships
   - Analysis of funding distribution strategies

5. **Geographical Analysis**
   - Distribution of projects across provinces in Mozambique
   - Focus areas for different funding partners

## Key Insights

- **Total Funding**: The total funding allocated across all projects is approximately $3.65 billion.

- **Funding Trends**: The highest project funding occurred in 2024, indicating a significant increase in investment compared to previous years. This suggests a growing emphasis on project development, possibly due to increased budget allocations, economic growth, or strategic priorities.

- **Collaboration Patterns**: 
  - Bill and Melinda Gates Foundation collaborates with multiple implementing partners, including CHAI, Fundação Manhiça, Instituto Nacional de Saúde, The Global Fund, and WHO, suggesting a broad investment strategy.
  - Some funding partners like Canada maintain exclusive collaborations with specific implementing partners, indicating a selective partnership approach.
  - Other funding partners like the Arab Bank for Economic Development in Africa have limited engagement with implementing partners.

- **Project Value Distribution**: There is a wide range in project funding, from as little as $42,000 to as much as $541.7 million, highlighting the diversity of project scales within the health sector in Mozambique.

## Technologies Used
- Python 3
- pandas for data manipulation
- NumPy for numerical operations
- Matplotlib and Seaborn for visualization
- Plotly for interactive visualizations
- forex-python for currency conversion

## Future Work
Potential areas for further analysis include:
- Impact assessment of funded projects
- Correlation between funding amounts and health outcomes
- Sustainability analysis of projects after funding periods
- Geographical gap analysis to identify underserved regions
- Temporal trends in funding focus areas

## Limitations
- The dataset only includes current projects and excludes humanitarian projects
- Some projects had missing start dates and geographical information
- Currency conversion rates may fluctuate over time, potentially affecting the accuracy of USD conversions

## Acknowledgements
The Health Partners Group (HPG) in Mozambique for compiling and providing access to this valuable dataset.