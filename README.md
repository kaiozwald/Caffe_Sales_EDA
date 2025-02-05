# Caffe Sales Prediction

## Overview
This project analyzes and predicts coffee shop sales based on transaction data. It includes data cleaning, exploratory data analysis (EDA), feature engineering, and a machine learning model using XGBoost for sales prediction.

## Features
- **Data Cleaning**: Handles missing values, removes errors, and preprocesses the dataset.
- **Exploratory Data Analysis (EDA)**: Visualizes sales trends, item popularity, and seasonal effects.
- **Feature Engineering**: Extracts meaningful features such as transaction date insights.
- **Modeling**: Implements an XGBoost regression model to predict total sales.
- **Evaluation**: Uses MSE and R² score to assess model performance.

## Installation
```bash
# Clone the repository
git clone https://github.com/kaiozwald/caffe-sales-prediction.git
cd caffe-sales-prediction

```

## Usage
```python
import pickle
import pandas as pd

# Load model
with open('xgboost_model.pkl', 'rb') as file:
    model = pickle.load(file)

# Prepare new data
new_data = pd.DataFrame({...})

# Predict sales
predictions = model.predict(new_data)
print(predictions)
```

## Project Structure
```
📂 caffe-sales-prediction
│-- 📄 dirty_cafe_sales.csv  # Raw dataset
│-- 📄 clean_data.csv        # Processed dataset
│-- 📄 caffe_sales.ipynb     # Jupyter Notebook for EDA & modeling
│-- 📄 xgboost_model.pkl     # Trained ML model
│-- 📄 README.md             # Project documentation
```

## Results
- Sales trends were analyzed based on time and product categories.
- XGBoost model effectively predicts sales with an optimized performance.
- Insights help in inventory management and business decision-making.

## License
This project is open-source under the MIT License.
