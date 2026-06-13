# Instamart Next Product Prediction

This repository contains an end-to-end notebook workflow for analyzing Instacart order history data and building models to predict a user's next purchased products.

## Project workflow

The project is organized as sequential Jupyter notebooks:

1. **`1. Data_Analysis.ipynb`** - Dataset overview and initial data understanding.
2. **`2. Exploratory_Data_Analysis.ipynb`** - Visual EDA and behavioral insights.
3. **`3. Customer_Segementation.ipynb`** - Customer segmentation using PCA and K-Means.
4. **`4. Market_Basket_Analysis.ipynb`** - Association-rule mining and basket analysis.
5. **`5. Feature Extraction.ipynb`** - Product, aisle, department, and user-level feature engineering.
6. **`6. ANN Model.ipynb`** - Neural-network based prediction model.
7. **`7. XGBoost Model.ipynb`** - Gradient-boosted tree model for final prediction.

## Dataset

These notebooks expect Instacart CSV files such as:

- `aisles.csv`
- `departments.csv`
- `orders.csv`
- `products.csv`
- `order_products__prior.csv`
- `order_products__train.csv`
- `sample_submission.csv`

Some notebooks reference a local folder like `instacart-market_basket_analysis/`. Update paths to match your local dataset location before execution.

## Environment setup

Use Python 3.9+ and install the common dependencies used across notebooks:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost tensorflow imbalanced-learn mlxtend category-encoders
```

## How to run

1. Place the dataset CSV files in a local directory.
2. Open notebooks in the listed order.
3. Update dataset paths in notebook cells if needed.
4. Run all cells for each notebook to reproduce analysis and models.

## Notes

- This repository is notebook-first and currently does not include a packaged training pipeline or automated tests.
- Feature extraction and model notebooks are intended to be run after completing the earlier analysis notebooks.
