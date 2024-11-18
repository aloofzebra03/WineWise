# WineWise

Analyze the chemical properties of red wines to identify key factors influencing quality and help winemakers optimize production and improve product appeal.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Project Workflow](#project-workflow)
- [Visualizations](#visualizations)
- [Models Used](#models-used)
- [Results](#results)
- [Future Scope](#future-scope)
- [How to Use](#how-to-use)
- [Acknowledgments](#acknowledgments)

---

## Introduction
**WineWise** focuses on predicting the quality of red wine samples based on their physicochemical properties. The dataset includes features such as acidity, sugar content, and alcohol levels, and labels wines with a quality score ranging from 0 to 10.

---

## Dataset
The dataset contains physicochemical properties and sensory quality ratings of red wine. The key features include:

- **Fixed Acidity**: Non-volatile acids (g/L)
- **Volatile Acidity**: Evaporating acids (g/L)
- **Citric Acid**: Adds freshness (g/L)
- **Residual Sugar**: Remaining sugar after fermentation (g/L)
- **Chlorides**: Salt content (g/L)
- **Free Sulfur Dioxide**: Unbound SO2 (mg/L)
- **Total Sulfur Dioxide**: Total SO2 (mg/L)
- **Density**: Mass per unit volume (g/cm³)
- **pH**: Acidity level
- **Sulphates**: Prevents spoilage (g/L)
- **Alcohol**: Percentage by volume (% vol)
- **Quality**: Quality score (0 to 10)

---

## Project Workflow
1. **Data Cleaning**: Handling duplicates and ensuring consistent data.
2. **Feature Analysis**: Visualizing correlations between chemical properties and wine quality.
3. **Model Training**:
   - Decision Tree
   - Random Forest
4. **Evaluation**: Comparing accuracy scores for both models.

---

## Visualizations
- **Wine Quality Scores**: Most wines have a score of 5, with a slight left skew.
- **Correlation Metrics**:
  - **Alcohol**: Moderately positive correlation with quality (0.48).
  - **Volatile Acidity**: Negative correlation (-0.39).
  - **Fixed Acidity**: Weak positive correlation (0.12).
  - **Free Sulfur Dioxide**: Negligible effect (-0.05).
- **Residual Sugar vs Quality**: Minimal difference between low and high-quality wines.

---

## Models Used
1. **Decision Tree**:
   - Accuracy: 50.7%
   - Pros: Simple and interpretable.
   - Cons: Overfits with complex data.
2. **Random Forest**:
   - Accuracy: 66.9%
   - Pros: Handles overfitting better and provides robust predictions.
   - Cons: Computationally intensive.

---

## Results
The Random Forest model outperformed the Decision Tree model in predicting wine quality, achieving an accuracy of **66.9%**, compared to **50.7%** for the Decision Tree. 

Key insights include:
- **Alcohol Content**: Strongly correlated with higher wine quality.
- **Volatile Acidity**: Negatively affects wine quality.
- **Residual Sugar**: Has minimal impact on wine quality.

---

## Future Scope
**WineWise** has potential for further development in the following areas:
1. **Feature Engineering**:
   - Investigate non-linear relationships between features and wine quality.
   - Include sensory data like aroma or visual appeal for a holistic prediction.
2. **Model Optimization**:
   - Fine-tune hyperparameters for Random Forest.
   - Experiment with advanced models like Gradient Boosting or Neural Networks.
3. **Data Expansion**:
   - Incorporate data from white wines or other wine varieties.
   - Use larger datasets to improve model generalization.
4. **Deployment**:
   - Create an API or web application to allow winemakers to input wine properties and predict quality in real-time.
5. **Explainability**:
   - Use techniques like SHAP values to better interpret model predictions for end users.

---
