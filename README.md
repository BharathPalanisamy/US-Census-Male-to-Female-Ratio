# US-Census-Male-to-Female-Ratio

## Project Overview

This project analyzes the male-to-female population ratio in the United States using data from the US Census Bureau over the past 10 years (2013-2022) and predicts trends for the next 5 years (2023-2027). The project visualizes gender population distributions, ratios, and overall population trends, offering insights into gender demographics across a 15-year span.

The goal is to highlight trends in population distribution between genders, display the overall population in millions, and predict future ratios using linear regression.

## Technologies Used

- **Python**: Core programming language for data retrieval, processing, and analysis.
- **Pandas**: Used for data manipulation, organization, and analysis.
- **Matplotlib**: Library for data visualization, creating graphs that represent population trends and gender ratios.
- **US Census Bureau API**: Source for historical population data (2013-2022).
- **Linear Regression (scikit-learn)**: Predicts future population trends and gender ratios.

## How to Run This Project

1. **Install Jupyter Notebook**
   - Use the following command to install Jupyter Lab, which will serve as the workspace:
     ```bash
     pip install jupyterlab
     ```

2. **Set Up Environment Variable for the Census API Key**
   - Request an API key from the [US Census Bureau](https://api.census.gov/data/key_signup.html).
   - Set the key as an environment variable:
     ```bash
     export CENSUS_API_KEY=your_api_key_here
     ```

3. **Run the Jupyter Notebook**
   - Open the project in Jupyter Lab.
   - Click on the kernel menu and select "Restart and Run All" to execute the entire project script.

4. **Generate and View Results**
   - The script will automatically fetch data, process it, and generate visualizations.
   - The graph will display:
     - Historical trends for male and female populations (2013-2022).
     - Predicted trends for the next 5 years (2023-2027) using linear regression.
     - Male-to-female ratios as a percentage, showing shifts in population dominance over time.
     - Background shading indicates historical data (green) and future predictions (blue).

## Project Breakdown

### Data Retrieval and Processing
- Data is fetched from the US Census Bureau API for the last 10 years.
- Male and female population data is extracted, cleaned, and stored in pandas DataFrames.
- Male-to-female ratios are calculated, expressed as a percentage.

### Predictive Modeling
- Linear regression models are trained using historical data to predict male and female populations for the next 5 years.
- Predictions are used to estimate future male-to-female ratios.

### Visualization
- A detailed graph is generated showing historical and predicted data:
  - Lines represent actual and predicted trends for male and female populations.
  - Percentage lines show male-to-female ratios.
  - Background colors visually separate past data from future predictions.

## Acknowledgments

Special thanks to:
- **Santhosh Kanala**: For his guidance and mentoring throughout the development of this project.
- **Chandran Palanisamy**: For his advice on simplifying graphing techniques and visualization.
