# Health-Insurance-Premium-Prediction# 🏥 Health Insurance Cost Prediction using Random Forest

> A machine learning project to predict health insurance charges based on demographic and lifestyle factors.

## 📌 Overview

This project builds a regression model to estimate medical insurance costs (charges) for individuals. Using features like age, sex, BMI, and smoking status, a **Random Forest Regressor** is trained on historical data to predict the premium amount. The project also includes exploratory data analysis (EDA) to understand the distribution of smokers, regional population, and feature correlations.

## ✨ Key Features

- **Data Preprocessing**: Mapped categorical variables (`sex` and `smoker`) to numerical values.
- **Exploratory Data Analysis**:
  - Histogram of smoker distribution by sex.
  - Pie chart of regional population.
  - Correlation matrix heatmap (numeric features only).
- **Model Training**: Used a **Random Forest Regressor** from scikit-learn to predict charges.
- **Evaluation**: Predicts premium amounts on a test set (20% hold-out).
- **Prediction Output**: Displays predicted charges for sample data points.

## 🛠️ Technologies & Libraries Used

- **Python 3.x**
- **pandas** – Data loading and manipulation
- **numpy** – Numerical operations
- **scikit-learn** – For `train_test_split` and `RandomForestRegressor`
- **plotly.express** – Interactive visualizations (histogram, pie chart)
- **Jupyter Notebook** – Development environment

## 📦 Installation & Setup

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Aymanel7r/health-insurance-cost-prediction.git
   cd health-insurance-cost-prediction
   ```

2. **Install required libraries**:
   ```bash
   pip install pandas numpy scikit-learn plotly
   ```

3. **Ensure the dataset** (`Health_insurance.csv`) is in the same directory as the notebook.

## 🚀 How to Use

1. Open the Jupyter Notebook:
   ```bash
   jupyter notebook "your_notebook_name.ipynb"
   ```
2. Run all cells sequentially to:
   - Load the dataset and check for missing values.
   - Visualize smoker distribution by sex.
   - Display regional population with a pie chart.
   - Compute and display correlation matrix.
   - Preprocess data (encode categorical features).
   - Split data into training and test sets (80% train, 20% test).
   - Train a Random Forest Regressor.
   - Generate predictions on the test set.
   - View predicted premium amounts.

## 📊 Results

The Random Forest Regressor was trained on features: `['age', 'sex', 'bmi', 'smoker']` to predict `charges`.

- **Test set size**: 20% of the data
- **Sample predictions** (first 5 test instances):

| Predicted Premium Amount |
|--------------------------|
| 9760.54                  |
| 5429.21                  |
| 28209.08                 |
| 9509.24                  |
| 34561.47                 |

## 📁 Project Structure

```
├── your_notebook.ipynb          # Main Jupyter notebook with all code
├── Health_insurance.csv         # Dataset file
└── README.md                    # This file
```

## 📄 CSV Data Format

The dataset should contain the following columns:
- `age` – Age of the individual
- `sex` – Gender (female/male)
- `bmi` – Body Mass Index
- `children` – Number of children covered
- `smoker` – Smoking status (yes/no)
- `region` – Geographic region (southwest, southeast, northwest, etc.)
- `charges` – Individual medical insurance cost (target variable)

## 🙏 Acknowledgements

- Data source (Kaggle's Medical Cost Personal Dataset)
- The scikit-learn team for providing robust machine learning tools
- Plotly for interactive visualizations
