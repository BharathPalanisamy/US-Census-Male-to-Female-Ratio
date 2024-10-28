# US Census Male to Female Ratio for automotive industries

## Project Overview

This project analyzes the male-to-female population ratio in the United States using data from the US Census Bureau over the past 10 years (2013-2022) and predicts trends for the next 5 years (2023-2027). The project visualizes gender population distributions, ratios, and overall population trends, offering insights into gender demographics across a 15-year span. 

The goal is to highlight trends in population distribution between genders, display the overall population in millions, and predict future ratios using linear regression.

## Technologies Used

- **Python**: Core programming language for data retrieval, processing, and analysis.
- **Pandas**: Used for data manipulation, organization, and analysis.
- **Matplotlib**: Library for data visualization, creating graphs that represent population trends and gender ratios.
- **US Census Bureau API**: Source for historical population data (2013-2022). (Can be worked for any county or state just have to change the API code).
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

## Automotive Industry Use Cases
**Targeted Marketing for Automotive Sales:** Automotive companies can use the male-to-female population ratios to enhance their marketing campaigns. By analyzing demographic data, manufacturers can identify which regions have a higher concentration of males or females and tailor their advertising accordingly.

1. #### Example:
   **Data:** Historical and predicted population ratios provide insight into gender trends.<br>
   **Application:** If data indicates a growing female population in a specific area, automotive companies can focus marketing efforts on vehicles that appeal to this demographic.       For instance, promoting family-oriented or eco-friendly cars like electric vehicles and SUVs.

**Product Development and Regional Sales Strategies:** Demographic trends allow automotive companies to plan their product development and regional sales strategies more effectively. Understanding shifts in gender ratios can guide the design and release of new models that cater to market demand.

2. #### Example:
   **Data:** Predicted demographic trends over the next five years can inform strategic planning.<br>
   **Application:** If the data predicts a balanced or increasing male-to-female ratio, companies can develop a product lineup that appeals to a wider audience. By prioritizing the       production of versatile, fuel-efficient models, they can ensure better alignment with market needs.

## Acknowledgments

Special thanks to:
- **Santhosh Kanala**: For his guidance and mentoring throughout the development of this project.
- **Chandran Palanisamy**: For his advice on simplifying graphing techniques and visualization.
