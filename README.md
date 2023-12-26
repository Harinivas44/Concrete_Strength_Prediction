# Concrete Strength Prediction 🏗️

#### Overview:
Predicting the compressive strength of concrete is crucial for ensuring the durability and stability of structures. In this project, I use various machine learning algorithms to predict concrete compressive strength based on different input features.

#### Dataset:
The dataset consists of 1030 samples with 9 features:

- **Inputs:**
  - Cement
  - Blast Furnace Slag
  - Fly Ash
  - Water
  - Superplasticizer
  - Coarse Aggregate
  - Fine Aggregate
  - Age

- **Output:**
  - Concrete Compressive Strength

#### Data Exploration:
- Checked for missing values and data types.
- Explored descriptive statistics to understand the data distribution.
- Visualized feature correlations using a heatmap.

#### Data Preprocessing:
- Handled outliers using the IQR method to improve model performance.
- Scaled input features to ensure uniformity across different scales.

#### Model Building:
1. **Random Forest Regressor:**
   - Achieved a training score of 98.20% and testing score of 88.20%.
   - Utilized cross-validation with k-fold (k=20) and obtained an accuracy of 76.19%.

2. **Gradient Boosting Regressor:**
   - Achieved a training score of 97.44% and testing score of 91.21%.
   - Cross-validated with k-fold (k=25) resulted in an accuracy of 79.24%.

3. **AdaBoost Regressor:**
   - Achieved a training score of 82.63% and testing score of 77.26%.
   - Cross-validation with k-fold (k=20) resulted in an accuracy of 59.27%.

4. **K-Nearest Neighbors (KNN) Regressor:**
   - Optimal k=3, achieved a training score of 99.34% and testing score of 77.02%.
   - Cross-validated with k-fold (k=20) resulted in an accuracy of 72.23%.

5. **Bagging Regressor:**
   - Achieved a training score of 98.24% and testing score of 88.21%.
   - Cross-validated with k-fold (k=20) resulted in an accuracy of 76.16%.

6. **Support Vector Regressor (SVR):**
   - Achieved a training score of 71.99% and testing score of 69.14%.
   - Cross-validated with k-fold (k=20) resulted in an accuracy of 61.55%.

7. **XGBoost Regressor:**
   - Achieved a training score of 98.64% and testing score of 90.18%.
   - Utilized cross-validation with k-fold (k=20) and obtained an accuracy of 76.16%.

8. **Decision Tree Regressor:**
   - Achieved a training score of 99.27% and testing score of 79.86%.
   - Cross-validated with k-fold (k=120) resulted in an accuracy of 87.04%.

#### Model Comparison:
| Algorithm                  | Accuracy |
|----------------------------|----------|
| Random Forest              | 88.20%   |
| Gradient Boosting           | 91.21%   |
| AdaBoost                   | 77.26%   |
| KNN                        | 77.02%   |
| Bagging                    | 88.21%   |
| SVR                        | 69.14%   |
| XGBoost                    | 90.18%   |
| Decision Tree              | 79.86%   |

#### Conclusion:
- Gradient Boosting and XGBoost performed exceptionally well in predicting concrete compressive strength.
- Adequate preprocessing, handling outliers, and model tuning significantly improved performance.
- Further optimization and feature engineering could enhance model accuracy.

