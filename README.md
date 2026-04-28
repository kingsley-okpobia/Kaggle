# House Prices: Advanced Regression Techniques

![Python](https://img.shields.io/badge/python-3.12-blue.svg)
![Kaggle](https://img.shields.io/badge/Kaggle-Notebook-blue.svg)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Latest-orange.svg)

Predicting house prices using advanced regression techniques, including gradient boosting, ensemble learning, and specialized data preprocessing. This project was developed as part of the Kaggle House Prices Competition.

## Project Overview
The goal of this project is to predict the sales price of residential homes in Ames, Iowa, given 79 explanatory variables. The challenge involves extensive data cleaning, handling missing values, feature engineering, and implementing a robust blending model to achieve a low Root-Mean-Squared-Error (RMSE).

## Tech Stack
- Language: Python 3.12
- Libraries:
    - Preprocessing: Pandas, NumPy, Scipy (Box-Cox transformations)
    - Modeling: Scikit-Learn, XGBoost, LightGBM
    - Visualization: Matplotlib, Seaborn

## Key Features
- Data Engineering: Applied log-transformations to skewed target variables and Box-Cox transformations to independent features.
- Missing Data Imputation: Strategic filling of null values based on feature relationships (e.g., LotFrontage based on Neighborhood).
- Categorical Encoding: Leveraged One-Hot Encoding and manual mapping for ordinal variables.
- Ensemble Modeling: Implemented a weighted blend of multiple high-performing regressors to ensure stability and accuracy.

## Models Implemented
- Ridge & Lasso: Linear models with RobustScaler to handle outliers.
- ElasticNet: Balancing L1 and L2 penalties for feature selection.
- SVR: Support Vector Regression with an RBF kernel.
- Gradient Boosting: High-performance ensemble using Huber loss.
- XGBoost & LightGBM: Optimized gradient boosting frameworks for speed and accuracy.
- Model Blending: A custom weighted ensemble approach to minimize variance.

## Performance
The final model utilizes a manual blend of predictions, prioritizing XGBoost and Ridge Regression, achieving a significantly reduced RMSE on the leaderboard.

## Project Structure
- data/
    - train.csv         # Training data
    - test.csv          # Test data
- notebooks/
    - house_prices.ipynb # Main analysis and modeling notebook
- README.md             # Project documentation

## Installation & Usage
1. Clone the repository:
   git clone https://github.com/yourusername/house-prices-regression.git

2. Install dependencies:
   pip install pandas numpy scikit-learn xgboost lightgbm seaborn

3. Run the notebook:
   Open house_prices.ipynb in Jupyter or Kaggle and execute the cells.

## License
This project is licensed under the MIT License.

---
### Author
Kingsley Okpobia
[Kaggle Profile](https://www.kaggle.com/kingsleyokpobia) | [GitHub](https://github.com/kingsley-okpobia)
