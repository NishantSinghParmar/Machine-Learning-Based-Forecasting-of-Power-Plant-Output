# PowerPredict: Machine Learning-Based Forecasting of Power Plant Output

## Project Overview
"PowerPredict" is a machine learning project focused on predicting the power output of a combined cycle power plant. Utilizing various environmental and operational parameters, this model aims to enhance the accuracy of power generation forecasting.

## Dataset Description
The dataset comprises 9568 data points collected from a Combined Cycle Power Plant over six years (2006-2011), under full load conditions. It includes hourly average ambient variables and operational parameters:

- **T (Temperature)**: Ambient temperature, affecting the performance of the gas turbines (GT).
- **AP (Ambient Pressure)**: Atmospheric pressure, influencing the efficiency of the GT.
- **RH (Relative Humidity)**: The moisture content in the air, impacting the GT operations.
- **V (Exhaust Vacuum)**: Vacuum level in the steam turbine (ST), which plays a crucial role in the ST's efficiency.

The dataset is aimed at predicting the net hourly electrical energy output (EP) of the plant. A Combined Cycle Power Plant (CCPP) integrates the operation of gas and steam turbines to generate electricity, making the interplay of these variables particularly significant for its efficiency.

## Objective
The goal of this project is to develop and compare multiple machine learning models to predict the power output of the plant based on these environmental and operational parameters. 

## Model Analysis and Results

### Models Employed
1. **Decision Tree Model**: 
   - **R² Score**: 0.922905874177941
   - Effective for capturing complex, non-linear relationships in the dataset.

2. **Multiple Linear Regression Model**: 
   - **R² Score**: 0.9325315554761303
   - Assumes a linear relationship between the variables, suitable for datasets with linear correlations.

3. **Polynomial Regression**: 
   - **R² Score**: 0.9458193347147237
   - Adds polynomial terms to linear models, allowing for more complex relationship modeling.

4. **Support Vector Regression (SVR)**: 
   - **R² Score**: 0.948078404998626
   - Known for its effectiveness in high-dimensional spaces, robust in various dataset types.

5. **Random Forest Regression**: 
   - **R² Score**: 0.9615908334363876
   - Combines multiple decision trees for better accuracy and stability.

### Evaluation
The performance of each model was assessed using the R² score, which reflects the proportion of variance in the dependent variable that is predictable from the independent variables. The Random Forest Regression model showed the highest R² score, indicating its superior predictive ability for this dataset.

## Conclusion
Through the comparative analysis of various machine learning models, significant insights were gained into their predictive performance. The Random Forest Regression model emerged as the most accurate, making it the most suitable for forecasting the power output of the CCPP.

## References
- UCI Machine Learning Repository
- https://archive.ics.uci.edu/dataset/294/combined+cycle+power+plant

---

