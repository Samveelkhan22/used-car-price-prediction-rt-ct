# Used Car Price Prediction: Regression Tree vs Classification Tree

This project explores two different machine learning methods to predict the price of a used Toyota Corolla car using:
- **Regression Tree (RT)** for continuous price prediction
- **Classification Tree (CT)** for binned price prediction

## Project Overview

In this project, we compare the performance of a **Regression Tree (RT)** and a **Classification Tree (CT)** to predict used car prices. We use specifications of Toyota Corolla cars as input features and evaluate the performance of both methods.

### Key Tasks:
1. **Data Preprocessing**:
   - Categorical variables (e.g., fuel type) are converted to dummy variables for model compatibility.
   - The price variable is binned into 20 categories for classification purposes.
   
2. **Model Training**:
   - A **Regression Tree (RT)** is trained to predict the car price directly.
   - A **Classification Tree (CT)** is trained to predict binned price categories.
   - **GridSearchCV** is used to fine-tune both models and find the best hyperparameters.
   
3. **Prediction**:
   - Predict the price of a Toyota Corolla based on specific features.
   - Compare predictions from both models.

### Features:
- **Age_08_04**: Age of the car in months.
- **KM**: Kilometers driven.
- **Fuel_Type**: Type of fuel (Petrol/Diesel).
- **HP**: Horsepower.
- **Automatic**: Whether the car is automatic or not.
- **Doors**: Number of doors.
- **Quarterly_Tax**: Quarterly road tax.
- **Mfg_Guarantee**: Manufacturer guarantee.
- **Guarantee_Period**: Remaining guarantee period.
- **Airco**: Whether the car has air conditioning.
- **Automatic_Airco**: Whether the car has automatic air conditioning.
- **CD_Player**: Whether the car has a CD player.
- **Powered_Windows**: Whether the car has powered windows.
- **Sport_Model**: Whether the car is a sport model.
- **Tow_Bar**: Whether the car has a tow bar.

## Results
- **Predicted Price (RT)**: 10,000.0
- **Predicted Binned Price (CT)**: 0 (Bin category)
- **Estimated Price from CT**: 10,123.75

### Model Comparison
- **Regression Tree (RT)**:
  - Predicts continuous values.
  - More precise, but sensitive to overfitting and outliers.
  
- **Classification Tree (CT)**:
  - Predicts in discrete bins.
  - Easier to interpret in terms of categories, but less accurate for specific price estimation.

## Future Improvements
- Experiment with additional models (e.g., Random Forest, XGBoost).
- Add more input features to improve prediction accuracy.
- Implement more detailed hyperparameter tuning.
