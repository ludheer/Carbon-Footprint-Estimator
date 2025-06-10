# Carbon-Footprint-Estimator
Final impression :The models did a pretty good job, considering we used just basic lifestyle inputs.
Carbon emissions can vary a lot due to many hidden factors we didn’t capture.
Even then, our predictions stayed fairly close to real values across a wide range.
With more detailed inputs, the accuracy can improve even further


##  Objective

To build a lightweight, functional regression model that predicts carbon emissions using:
- **Inputs:** `Diet`, `Transport`, `Vehicle Distance (km)`
- **Output:** `Estimated CO₂ kg/week`

## 📂 Dataset Used

- A **real dataset** with actual carbon emission values (`CarbonEmission`) based on user lifestyle.
- Columns included:
  - `Diet`: Diet type (e.g., Vegan, Vegetarian, Non-Vegetarian)
  - `Transport`: Transport mode (e.g., Car, Bike, Public)
  - `Vehicle Monthly Distance Km`: Distance traveled
  - `CarbonEmission`: Weekly CO₂ emission in kg

## Approach Summary

- **Data Preprocessing**
  - Renamed columns for clarity
  - Dropped missing entries
  - Used `OneHotEncoder` for categorical features
- **Models Trained**
  - Linear Regression 
  - Random Forest Regressor 
- **Train-Test Split:** 80/20
- **Evaluation Metric:** Mean Squared Error (MSE), Root Mean Squared Error (RMSE)

## 📈 Model Performance

| Model               | MSE          | RMSE 
 Linear Regression    652,504.19      807.78   
 Random Forest        858,456.71      926.53   

