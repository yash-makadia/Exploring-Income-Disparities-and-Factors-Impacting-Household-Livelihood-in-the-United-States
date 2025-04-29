# Exploring Income Disparities and Factors Impacting Household Livelihood in the United States
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

## Overview

This data analysis project investigates income disparities across the United States using 2020 US Census data, developed as a group project for BUDT704: Data Processing and Analysis in Python (Fall 2022, taught by Professor John Bono) at the Robert H. Smith School of Business, University of Maryland, College Park. Leveraging Python, we conducted exploratory data analysis (EDA), visualized socio-economic factors, and built a predictive model to estimate household income based on education, employment, and demographic characteristics. The project aims to uncover insights into income variations and provide actionable recommendations for addressing disparities.

**Primary Objectives**:
- Analyze median household income variations across US states.
- Explore relationships between income, education, and employment types.
- Develop a predictive model to estimate income and identify key influencing factors.
- Recommend strategies for states to improve median household income.

## Features

- **Exploratory Data Analysis**: Visualizes income distributions, employment types, and education levels across states.
- **Data Preprocessing**: Consolidates and cleans US Census data using zip codes as the primary key.
- **Predictive Modeling**: Builds a model to estimate household income based on socio-economic factors.
- **Actionable Insights**: Identifies opportunities for states to enhance income through targeted interventions.

## Dataset

The dataset, sourced from the [US Census Data website](https://data.census.gov/) for 2020, includes:
- **Economic Characteristics**: Income, employment types (from table DP03).
- **Demographic and Housing**: Age, race, housing estimates (DP05).
- **Educational Attainment**: Education levels (S1501).
- **Financial Characteristics**: Housing unit finances (S2506).

**Access**: Data is publicly available at [https://data.census.gov/](https://data.census.gov/). Due to size, the consolidated dataset is not hosted in the repository but can be recreated using the provided code.

## Methodology

### Data Preparation
- **Data Collection**: Combined tables DP03, DP05, S1501, and S2506 using zip codes as the primary key.
- **Preprocessing**:
  - Cleaned missing values and standardized formats.
  - Merged datasets to create a comprehensive analysis-ready dataset.
- **Exploratory Data Analysis (EDA)**:
  - Analyzed median household income by state, identifying disparities.
  - Visualized distributions of employment types and education levels.
  - Compared high- and low-income states to assess education’s impact on income.

### Modeling
- **Predictive Model**: Developed a regression model (e.g., Linear Regression or Random Forest) to estimate household income based on features like education level, employment type, and demographic factors.
- **Feature Selection**: Identified key predictors (e.g., education attainment, employment status) through correlation analysis and feature importance.
- **Evaluation**: Assessed model performance using metrics like Mean Squared Error (MSE) and R-squared.

### Visualizations
- Created plots (e.g., histograms, bar charts, scatter plots) to illustrate income variations, employment distributions, and education-income relationships.
- Used libraries like Matplotlib and Seaborn for clear, informative graphics.

### Libraries
- Python libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`.

## Setup Instructions

### Prerequisites
- Python (version 3.8 or higher).
- Jupyter Notebook or any Python IDE (e.g., VS Code, PyCharm).
- Install required libraries:
  ```bash
  pip install pandas numpy matplotlib seaborn scikit-learn
  ```

### Installation
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yash-makadia/Exploring-Income-Disparities-and-Factors-Impacting-Household-Livelihood-in-the-United-States.git
   cd Exploring-Income-Disparities-and-Factors-Impacting-Household-Livelihood-in-the-United-States
   ```
2. **Download the Dataset**:
   - Access raw data from [https://data.census.gov/](https://data.census.gov/) (tables DP03, DP05, S1501, S2506).
   - Place CSV files in the repository root or update file paths in `census_income_analysis.py`.
3. **Run the Code**:
   - Open `census_income_analysis.py` in a Python IDE or Jupyter Notebook.
   - Update dataset paths in the script as needed.
   - Execute the script to preprocess data, generate visualizations, and train the predictive model.

## Key Findings

- **Income Disparities**: Significant variations in median household income across states, with some states consistently below the national average.
- **Education Impact**: Higher education levels correlate with increased income, particularly in high-income states.
- **Employment Types**: States with diverse employment structures (e.g., professional, technical jobs) tend to have higher median incomes.
- **Model Insights**: The predictive model identified education and employment as top factors influencing income, enabling targeted policy recommendations.

## Impact and Recommendations

- **For Policymakers**: Focus on improving education access and job training in low-income states to reduce disparities.
- **For Organizations**: Invest in workforce development programs targeting high-impact sectors identified by the model.
- **Actionable Insights**:
  - Prioritize educational attainment to boost income potential.
  - Promote diverse employment opportunities in underperforming states.
  - Use model predictions to identify states with the greatest improvement potential.

## Project Files

- `census_income_analysis.py`: Python script for data preprocessing, EDA, visualization, and predictive modeling.
- `docs/US_Census_Data_Analysis_Python_Project.pdf`: Comprehensive project report detailing methodology, findings, and recommendations.
- `LICENSE`: GNU General Public License v3.0.

## Course Information

- **Course**: BUDT704: Data Processing and Analysis in Python
- **Professor**: John Bono
- **Semester**: Fall 2022
- **Institution**: Robert H. Smith School of Business, University of Maryland, College Park

## Challenges and Lessons Learned

- **Data Integration**: Merging multiple Census tables required careful preprocessing to align zip codes and handle missing data.
- **Feature Selection**: Identifying the most impactful features for income prediction involved iterative analysis.
- **Key Takeaways**:
  - Robust data cleaning is essential for reliable analysis.
  - Visualizations enhance understanding of complex socio-economic trends.
  - Predictive models provide actionable insights for policy decisions.

## Future Scope

- Incorporate additional Census years for temporal analysis.
- Explore advanced models (e.g., Gradient Boosting, Neural Networks) for improved accuracy.
- Analyze regional disparities within states for more granular insights.
- Develop an interactive dashboard for real-time income analysis.

## References

- [US Census Data](https://data.census.gov/)
- Python Documentation: [pandas](https://pandas.pydata.org/), [numpy](https://numpy.org/), [matplotlib](https://matplotlib.org/), [seaborn](https://seaborn.pydata.org/), [scikit-learn](https://scikit-learn.org/)

## License

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please fork the repository, create a new branch, and submit a pull request with your changes. Ensure compliance with the GPL-3.0 license.

## Contact

For questions or feedback, please open an issue on GitHub or contact the project maintainer at [yashmakadia1908@gmail.com](mailto:yashmakadia1908@gmail.com).

## Acknowledgments

Special thanks to my team for their dedication and collaborative spirit. I express gratitude to Professor John Bono for his guidance and support throughout the project.
