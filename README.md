# Auto Price Prediction (PRCP-1017)

## Problem Statement
The objective of this project is to model car prices to help management understand how different specifications and features affect market value. This allows businesses to manipulate car designs and marketing strategies to meet specific price levels effectively.

## Dataset Overview
The dataset consists of 201 records with 26 unique attributes. Below is the detailed breakdown of the features analyzed:
  - **Symboling:** A risk rating assigned to the car (-3 to +3). Higher values indicate a riskier vehicle for insurance.
  - **Normalized-losses:** The relative average loss payment per insured vehicle year.
  - **Make/Fuel-Type/Aspiration:** Categorical data identifying the manufacturer, fuel (gas/diesel), and engine induction (standard/turbo).
  - **Body-style/Drive-wheels/Engine-location:** Structural details that impact aerodynamics and handling.
  - **Wheel-base/Length/Width/Height/Curb-weight:** Physical dimensions; Curb-weight was identified as a primary price driver.
  - **Engine-type/Cylinders/Engine-size:** Mechanical specs; Engine-size showed the highest correlation with market value
  - **Fuel-system/Bore/Stroke/Compression-ratio:** Internal combustion parameters.
  - **Horsepower/Peak-rpm:** Measures of engine performance and power output.
  - **City-mpg/Highway-mpg:** Fuel efficiency metrics; typically inversely correlated with price and performance.
  - **Price (Target):** The final valuation of the vehicle.
    
## Methodology
- **Data Preprocessing:** Handled non-standard null values (e.g., '?') and reduced price skewness.
- **Feature Engineering:** Identified critical drivers of valuation like curb-weight.
- **Modeling:** Utilized Random Forest algorithms to establish a reliable predictive baseline.

## Results
- Achieved a high predictive accuracy with an **R2 score of 0.94**.

## Technologies Used
- Python (Pandas, NumPy)
- Scikit-learn (Random Forest)
- Matplotlib & Seaborn
