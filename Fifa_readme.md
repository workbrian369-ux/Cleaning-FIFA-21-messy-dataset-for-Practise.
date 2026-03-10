# FIFA 21 Data Cleaning & Exploratory Analysis

## Project Overview
This project focuses on the end-to-end processing of the "messy" FIFA 21 dataset. The goal was to transform raw, unformatted player data into a clean, analysis-ready format to uncover insights into player potential, valuation, and skill correlations.

## Data Engineering & Cleaning
The primary challenge of this dataset was its "dirtiness." Key cleaning steps included:
* **Currency Conversion:** Transformed player `Value`, `Wage`, and `Release Clause` from strings (e.g., €100M, €10K) into numeric floats for calculation.
* **Height & Weight Normalization:** Converted various units (lbs/kg and feet-inches/cm) into standard metric values.
* **Date Processing:** Cleaned `Joined` dates to analyze player longevity and loyalty.
* **Star Rating Stripping:** Removed special characters from `W/F`, `SM`, and `IR` columns to make them quantifiable.

## Key Insights
* **Undervalued Potential:** Identified a segment of young players with high potential-to-overall gaps who are currently undervalued in the market.
* **Skill Synergy:** High correlations found between `Dribbling` and `Ball Control`, as well as `Vision` and `Passing`, helping define specific player archetypes.
* **Physical Bias:** Analyzed the distribution of "Preferred Foot" and its impact on overall ratings (OVA), finding a slight median advantage for right-footed players in certain positions.

## Technical Stack
* **Language:** Python 3.x
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
* **Methodologies:** Descriptive Statistics, Diagnostic Analysis, Data Visualization (Heatmaps, Scatter Plots).

## How to Use
1. Clone the repository.
2. Ensure you have the dependencies installed: `pip install pandas numpy matplotlib seaborn`.
3. Open `fifa21_analysis.ipynb` in Jupyter Notebook or VS Code to view the full pipeline.

## Future Work
* Implement **K-Means Clustering** to group players by playstyle rather than just position.
* Build a **Linear Regression** model to predict player market value based on skill sets.