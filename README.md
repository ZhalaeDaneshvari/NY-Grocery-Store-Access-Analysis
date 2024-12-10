# INFO 2950 Final Project - Grocery Store Access Analysis in New York State

## Overview
This project analyzes the relationship between grocery store accessibility and socioeconomic factors across New York State census tracts. We investigate how median income levels and racial composition correlate with access to grocery stores, providing insights into potential food access disparities.

## Research Questions
1. How does the socioeconomic status of census tracts in New York State, as measured by median income levels, correlate with access to grocery stores, and to what extent does this relationship vary across different income brackets?

2. What is the relationship between the racial composition of census tracts in New York State and the accessibility of grocery stores, and are there significant disparities in store access among different racial groups?

## Key Findings
- Geographic location, rather than demographics alone, is the primary driver of grocery store access
- Higher-income areas surprisingly show greater distances to stores
- Urban-rural divide explains many apparent racial and income-based patterns
- County-level variations suggest need for locally-tailored solutions
- Transportation infrastructure may be as important as store location

## Repository Structure
- `data_cleaning.ipynb`: Jupyter notebook containing data cleaning procedures
- `exploratory_analysis.ipynb`: Initial data exploration and analysis
- `complete_analysis.ipynb`: Complete comprehensive analysis and conclusions
- `merged_census_store_data.csv`: Final cleaned dataset combining census and store location data
- Various supporting files for census tract data (.cpg, .dbf, .prj, .shp, .xml)

## Data Sources
- US Census tract data
- Grocery store location data
- Demographic and income data from census tracts

## Methodology
1. Data Collection and Cleaning
   - Matched grocery store locations with census tract data
   - Extracted socioeconomic and demographic information
   - Calculated distances between tract centers and nearest stores

2. Analysis
   - Statistical analysis of income-access relationships
   - Investigation of racial composition impacts
   - Geographic variation study
   - Model development and validation

## Results
### Income Analysis
- Positive correlation between income and store distance (β = 0.5461, p < 0.001)
- Strong county-level variations (R² ranging from 0.00 to 0.73)
- Urban-rural differences in relationship strength

### Racial Composition Analysis
- White population: Positive correlation (β = 0.3175)
- Black population: Slight negative (β = -0.0634)
- Hispanic population: Strong negative (β = -0.2983)
- Asian population: Moderate negative (β = -0.1718)

## Limitations
- Straight-line distance measurements may oversimplify access
- County-level analysis may mask local variations
- Limited store quality and selection data
- Challenge in separating urban-rural effects from demographic effects

## Future Work
- Include transportation accessibility analysis
- Study store quality and selection
- Examine temporal changes
- Analyze price variations
- Consider interaction effects

## Requirements
- Python 3.12.1
- Required packages listed in `complete_analysis.ipynb`

## Usage
1. Clone the repository
2. Install required packages:
3. Run notebooks in order:
   - `data_cleaning.ipynb`
   - `exploratory_analysis.ipynb`
   - `complete_analysis.ipynb`

## Contributors
- Zhalae Daneshvari - @ZhaLaeDaneshvari
- Peyton Smith - @peytonrsmith
- Sunny Liu @sl-013

## Acknowledgments
- USDA Food Access Research Atlas
- New York State Department of Health
- US Census Bureau