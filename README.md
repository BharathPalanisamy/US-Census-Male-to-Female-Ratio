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

### Prerequisites
- Python 3.7 or higher
- Required packages: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `requests`

### Setup Instructions

1. **Clone or Download This Repository**
   ```bash
   git clone <repository-url>
   cd US-Census-Male-to-Female-Ratio
   ```

2. **Install Required Packages**
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn requests jupyter
   ```

3. **Get Your Census API Key** (Required)
   - Visit: [US Census Bureau API Key Signup](https://api.census.gov/data/key_signup.html)
   - Fill out the form with your organization name and email
   - You'll receive your API key via email (usually within a few minutes)

4. **Configure Your API Key** (Choose ONE method)

   **Option A: Environment Variable (Recommended)**
   ```bash
   export CENSUS_API_KEY="your_api_key_here"
   ```
   
   **Option B: .env File (Persistent)**
   ```bash
   # Copy the example file
   cp .env.example .env
   
   # Edit .env and replace YOUR_API_KEY_HERE with your actual key
   ```
   
   **Option C: Direct in Notebook (Not recommended for sharing)**
   - Open the notebook and uncomment the line in the first code cell
   - Replace `your_key_here` with your actual API key

5. **Run the Jupyter Notebook**
   ```bash
   jupyter notebook US_CENSUS_POPULATION_PREDICTIONS.ipynb
   ```
   
   Or in VS Code:
   - Open the notebook file
   - Select a Python kernel
   - Click "Run All" or run cells individually

6. **View Results**
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
   **Application:** If data indicates a growing female population in a specific area, automotive companies can focus marketing efforts       on vehicles that appeal to this demographic. For instance, promoting family-oriented or eco-friendly cars like electric vehicles and     SUVs.

**Product Development and Regional Sales Strategies:** Demographic trends allow automotive companies to plan their product development and regional sales strategies more effectively. Understanding shifts in gender ratios can guide the design and release of new models that cater to market demand.

2. #### Example:
   **Data:** Predicted demographic trends over the next five years can inform strategic planning.<br>
   **Application:** If the data predicts a balanced or increasing male-to-female ratio, companies can develop a product lineup that          appeals to a wider audience. By prioritizing the production of versatile, fuel-efficient models, they can ensure better alignment        with market needs.

## Conclusion
This analysis provides valuable insights that can help businesses make informed decisions based on demographic trends. Whether it's for targeted marketing or strategic product development, understanding male-to-female population ratios is crucial for industries, including automotive, to adapt to changing market dynamics.

## Acknowledgments

Special thanks to:
- **Santhosh Kanala**: For his guidance and mentoring throughout the development of this project.
- **Chandran Palanisamy**: For his advice on simplifying graphing techniques and visualization.
