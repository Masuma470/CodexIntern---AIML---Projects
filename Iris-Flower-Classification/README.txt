# Iris Flower Classification

## Project Overview
This project focuses on classifying iris flowers into three species: **Setosa, Versicolor, and Virginica**, based on sepal and petal measurements. The goal is to demonstrate basic **classification modeling** using machine learning and to gain insights from the classic Iris dataset.

## Dataset
- Source: **Iris dataset** from `scikit-learn`.
- Features: Sepal length, Sepal width, Petal length, Petal width.
- Target: Iris species (`Setosa`, `Versicolor`, `Virginica`).
- Dataset is clean and ready for analysis.

## Steps Followed
1. **Data Exploration (EDA)**  
   - Checked dataset info, statistics, and species distribution.  
   - Visualized relationships between features using pairplots and correlation heatmaps.

2. **Data Preparation**  
   - Split data into training (80%) and testing (20%) sets.  
   - Standardized features using `StandardScaler`.

3. **Model Training**  
   - Trained four classifiers:  
     - Logistic Regression  
     - K-Nearest Neighbors (KNN)  
     - Decision Tree  
     - Support Vector Machine (SVM)

4. **Model Evaluation**  
   - Evaluated models using **accuracy, classification reports, and confusion matrices**.  
   - Compared model performances with a barplot.

5. **Results**
   | Model | Accuracy |
   |-------|----------|
   | Logistic Regression | 1.00 |
   | K-Nearest Neighbors | 0.97 |
   | Decision Tree | 1.00 |
   | Support Vector Machine | 1.00 |

6. **Future Scope**
   - Perform hyperparameter tuning on other models to improve performance.  
   - Try ensemble methods like Random Forest or Gradient Boosting.  
   - Deploy the model as a web app using Flask or Streamlit.  
   - Apply workflow to other classification problems.  
   - Experiment with feature selection or dimensionality reduction for deeper insights.

## Plots
- Pairplot (`plots/pairplot.png`)  
- Correlation heatmap (`plots/heatmap.png`)  
- Species distribution (`plots/species_distribution.png`)  
- Confusion matrices (`plots/confusion_matrix_ModelName.png`)  
- Model comparison barplot (`plots/model_comparison.png`)

## Technologies & Libraries
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn

---

