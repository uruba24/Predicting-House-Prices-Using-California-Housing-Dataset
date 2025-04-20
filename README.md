
# 🏠 House Price Prediction Using California Housing Dataset

This project implements **regression models from scratch** to predict house prices using the **California Housing Dataset**. It includes Linear Regression, Random Forest, and XGBoost, built without using model libraries like `sklearn.linear_model` or `xgboost`.

---

## 📂 Project Structure

```
.
├── main.py               # Main script to run models and compare performance
├── README.md             # Project description and instructions
├── models/
│   ├── linear_regression.py
│   ├── random_forest.py
│   └── xgboost.py
├── utils/
│   ├── metrics.py        # RMSE and R² implementations
│   └── visualizations.py # Feature importance plots
```

---

## 🚀 How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/your-username/house-price-prediction-scratch.git
cd house-price-prediction-scratch
```

### 2. Install dependencies

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

### 3. Run the main script

```bash
python main.py
```

---

## 🔄 Steps Followed

### 1. **Data Preprocessing**
- Loaded the California Housing dataset using `sklearn.datasets`.
- Normalized all numerical features.
- Converted data to NumPy arrays for model compatibility.

### 2. **Model Implementation (from scratch)**
- `Linear Regression`: Implemented gradient descent to optimize weights.
- `Random Forest`: Built multiple decision trees using bootstrap samples.
- `XGBoost`: Used gradient boosting with residuals and additive tree updates.

### 3. **Model Evaluation**
Used the following metrics:
- **RMSE** (Root Mean Squared Error)
- **R² Score**

### 4. **Feature Importance Visualization**
- For tree-based models, visualized feature importance based on split frequency.

---

## 📊 Observations

| Model             | RMSE     | R² Score |
|------------------|----------|----------|
| Linear Regression| ~0.75    | ~0.58    |
| Random Forest     | ~0.49    | ~0.82    |
| XGBoost           | ~0.46    | ~0.85    |

> 🚨 *Note: Values may vary slightly due to random sampling.*

- Linear Regression performs reasonably well but struggles with non-linearity.
- Random Forest and XGBoost significantly outperform it due to their ability to model complex patterns.
- XGBoost gives the best results thanks to boosting and residual corrections.

---

## 📈 Visualizations

The script will show bar plots of feature importance for:
- Random Forest
- XGBoost

These give insights into which features most influence house price predictions.

---

## 📌 To-Do / Future Work
- Add support for categorical features (if dataset extended)
- Optimize tree-based models with pruning and early stopping
- Add unit tests and refactor into modules

---

## 📧 Contact

Feel free to reach out if you have questions or suggestions!

📮 **Your Name**  
🔗 [GitHub](https://github.com/your-username) | 📬 your.email@example.com

---
