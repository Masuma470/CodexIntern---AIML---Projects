# California House Price Prediction

## Project Overview
This project predicts median house values in California districts using machine learning.  
The main goal is to demonstrate a full ML workflow including data loading, exploration, preprocessing, modeling, evaluation, and interpretation.

---
## Summary at a Glance

**Project:** California House Price Prediction  
**Goal:** Predict median house values in California districts using machine learning  
**Dataset:** California Housing dataset (`sklearn.datasets`) – 20,640 samples, 8 numeric features  

**Best Model:** Random Forest Regressor  
- R² = 0.798 ✅  
- RMSE ≈ 0.515  
- MAE ≈ 0.333  

**Other Models:** Linear Regression, Ridge, Lasso  
- R² range: 0.577 – 0.582  

**Key Features:** MedInc, AveRooms, Latitude, Longitude, RoomsPerHousehold, PopulationPerHousehold  
**Total Visualizations:** 24 plots saved in `plots/` folder


## Dataset
- **Source:** California Housing dataset from `scikit-learn`  
- **Number of samples:** 20,640  
- **Number of features:** 8 numeric predictors + target  
- **Target variable:** `MedHouseVal` (median house value in $100,000s)  

---

## Folder Structure
HousePricePrediction/
│── artifacts/ # Dataset summaries, metrics
│── plots/ # All visualizations (histograms, heatmaps, residuals, parity plots, feature importance, R² comparison)
│── models/ # Trained ML models + best model
│── house_price_prediction.ipynb


---

## Steps Completed

### 1. Data Loading & Exploration
- Loaded the California Housing dataset.  
- Explored feature distributions using histograms and scatter plots.  
- Generated a correlation heatmap to understand relationships between features.  

### 2. Preprocessing & Feature Engineering
- Checked for missing values (none found).  
- Created derived features:
  - `RoomsPerHousehold`
  - `PopulationPerHousehold`  
- Scaled numeric features using `StandardScaler`.

### 3. Train/Test Split
- Split the dataset into **train (80%)** and **test (20%)** sets.

### 4. Model Training
- Trained multiple regression models:
  - Linear Regression  
  - Ridge Regression  
  - Lasso Regression  
  - Random Forest Regressor  

### 5. Model Evaluation
- Calculated **MAE, MSE, RMSE, and R²** for all models.  
- Created residual plots and parity plots to assess model performance.  
- Plotted feature importance (Random Forest) and coefficients (Ridge/Lasso).  
- Compared R² scores for all models visually.

---

## Model Performance Summary

| Model              | MAE     | MSE     | RMSE    | R²       |
|------------------ |--------|--------|--------|----------|
| Random Forest      | 0.333  | 0.265  | 0.515  | 0.798 ✅ |
| Lasso              | 0.535  | 0.548  | 0.740  | 0.582    |
| Ridge              | 0.533  | 0.555  | 0.745  | 0.577    |
| Linear Regression  | 0.533  | 0.555  | 0.745  | 0.577    |

**Best Model:** Random Forest  
- Highest R² = 0.798  
- Lowest RMSE ≈ 0.515  
- Lowest MAE ≈ 0.333

---

## Visual Summary
- All plots are saved in the `plots/` folder.  
- Key visualizations include:
  - Feature distributions and correlation heatmap  
  - Residual and parity plots for all models  
  - Feature importance and coefficient plots  
  - R² comparison bar chart showing the best model

---

## Insights
- Random Forest outperforms linear models on this dataset.  
- Median income (`MedInc`) is the strongest predictor of house prices.  
- Derived features (`RoomsPerHousehold`, `PopulationPerHousehold`) improve understanding of housing patterns.  
- Ensemble methods capture non-linear relationships better than linear regression models.

---

## How to Run
1. Clone the repository.  
2. Open `house_price_prediction.ipynb` in Jupyter Notebook.  
3. Run all cells sequentially.  
4. All plots, models, and evaluation metrics are saved in their respective folders automatically.

---

## Skills Demonstrated
- Data exploration and visualization  
- Regression modeling (Linear, Ridge, Lasso, Random Forest)  
- Model evaluation using MAE, MSE, RMSE, R²  
- Feature importance analysis and interpretation  
- Reproducible project structure

---

## Future Scope
- Hyperparameter tuning (GridSearchCV) for Random Forest  
- Deploy the best model using Flask or Dash  
- Apply the workflow to larger datasets like Ames Housing for more complex predictions.

## Notes
⚠️ Trained models and artifacts are not included in this repository due to GitHub size restrictions.  
To reproduce them, please run the provided Jupyter notebooks or training scripts.  
