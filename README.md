# DataQuest '25 - Pulzion Competition 🏆

## Achievement 
**Secured 3rd Place** 🎉 in DataQuest 2025, organized by Pulzion '25!

![3rd Place Achievement](./images/scoreboard.jpeg)
*Proud to have achieved 3rd place in this competitive data science hackathon*

---

## Competition Overview

**DataQuest 2025** was an inter-college machine learning competition organized by ACM Pict as part of Pulzion '25 event.

### Challenge Details
- **Evaluation Metric**: F1 Score (Macro)
- **Submission Limit**: 5 submissions in total

---

## Problem Statement

The competition involved predicting Air Quality Index (ASI) categories based on meteorological and environmental features. The target variable `ASI_category` had three classes: **Good**, **Moderate**, and **Poor**.

---

## Notebooks Overview

### Initial Exploration & Hyperparameter Tuning

#### [main.ipynb](main.ipynb)
- Initial data exploration and preprocessing
- XGBoost baseline model implementation
- Optuna-based hyperparameter optimization
- Achieved best F1 Score: **0.9260** with optimized parameters

#### [nb1.ipynb](nb1.ipynb)
- Extended hyperparameter tuning for multiple algorithms
- Comprehensive Optuna studies for:
  - XGBoost
  - LightGBM (with L1/L2 regularization)
  - Random Forest
- Stratified train-validation splits for robust evaluation

### Feature Engineering Experiments

#### [nb2.1.ipynb](nb2.1.ipynb)
- Basic feature engineering with meteorological interactions
- Feature selection using XGBoost importance
- StandardScaler normalization
- Model evaluation with tuned hyperparameters

#### [nb2.2.ipynb](nb2.2.ipynb)
- **Advanced meteorological feature engineering**:
  - Heat index and thermal comfort calculations
  - Atmospheric stability indicators
  - Wind shear and turbulence metrics
  - Daylight and cloud interaction features
  - Cyclic wind direction encoding
  - Pressure trend analysis
- Comprehensive feature importance analysis
- Duplicate feature removal

#### [nb3.ipynb](nb3.ipynb)
- Implementation of best tuned XGBoost parameters
- Refined model training pipeline
- Label encoding and stratified splitting

### Post-Competition Ensemble Methods

#### [AfterPulzion.ipynb](AfterPulzion.ipynb)
- **Soft Voting Ensemble** combining:
  - XGBoost
  - LightGBM (with early stopping)
  - Random Forest
- Individual model performance comparison
- Ensemble prediction aggregation

#### [AfterPulzion2.ipynb](AfterPulzion2.ipynb)
- **Advanced ensemble techniques**:
  - Memory-optimized data loading
  - Calibrated classifiers using CalibratedClassifierCV
  - Meta-stacking with Logistic Regression
  - Weighted ensemble optimization via grid search
  - Pseudo-labeling for semi-supervised learning
  - Polynomial feature transformations

#### [AfterPulzion_Exploratory.ipynb](AfterPulzion_Exploratory.ipynb)
- **Comprehensive ensemble exploration**:
  - Weighted blending with optimized weights
  - Multi-level stacking architectures
  - Bayesian model averaging
  - Knowledge distillation techniques
  - Neural network meta-learners
  - Detailed F1 score tracking and comparison

### Final Submission

#### [final.ipynb](final.ipynb)
- **Production-ready pipeline**:
  - Stratified K-Fold cross-validation
  - Multi-algorithm ensemble:
    - XGBoost with calibration
    - LightGBM with early stopping
    - **CatBoost** for categorical feature handling
    - Gaussian Naive Bayes
  - Isotonic regression for probability calibration
  - Sample weighting for class balance
  - Optimized hyperparameters from all experiments
  - Final submission CSV generation

---

## Key Technologies & Libraries

- **Python 3.x**
- **Pandas & NumPy** - Data manipulation
- **Scikit-learn** - Model training, preprocessing, metrics
- **XGBoost** - Gradient boosting
- **LightGBM** - Fast gradient boosting
- **CatBoost** - Categorical features handling
- **Optuna** - Hyperparameter optimization
- **Matplotlib** - Visualization

---

## Key Techniques Applied

### Feature Engineering
- Meteorological feature interactions (temperature, humidity, wind)
- Thermal comfort indicators (heat index, wind chill)
- Atmospheric stability metrics
- Cyclic encoding for directional features
- Polynomial feature transformations

### Model Optimization
- Bayesian hyperparameter optimization (Optuna)
- Stratified K-Fold cross-validation
- Early stopping to prevent overfitting
- L1/L2 regularization

### Ensemble Methods
- Soft voting classifiers
- Weighted blending
- Multi-level stacking
- Bayesian model averaging
- Knowledge distillation
- Calibrated probability predictions

### Advanced Techniques
- Isotonic regression calibration
- Sample weighting for class imbalance
- Memory-optimized data processing

---

## Results

Successfully achieved **3rd place** in the competition with a strong macro F1 score through:
- Iterative feature engineering
- Extensive hyperparameter tuning
- Multiple ensemble strategies
- Rigorous cross-validation

---

## License

This project is licensed under the terms specified in the [LICENSE](LICENSE) file.