# Auto Insurance Claim Prediction  ✨ 🚗📈  ✨

This project demonstrates my ability to work with large, messy datasets in the insurance domain, focusing on two key predictive goals:
1. **The probability of a car crash** (`TARGET_FLAG`) - Binary Logistic Regression
2. **The potential claim amount if a crash occurs** (`TARGET_AMT`) - Multiple Linear Regression

## Why This Matters
Insurance providers rely on accurate predictions for:
1. Assessing risk effectively
2. Setting fair premiums
3. Streamlining claim processes


## 🛠️ Project Workflow

The project workflow is a robust, step-by-step process designed to manage high-dimensional, messy data:Below is the comprehensive flowchart of the workflow:

![Data Preparation Workflow](https://github.com/yinaS1234/Auto-Insurance-Regression/blob/main/Resources/flowchart.png)



## 🚀 Models Built and Evaluated

### 1. Multiple Linear Regression (MLR)
   - **Full Model**: Includes all predictors to assess the overall feature impact.
   - **Stepwise Model**: Refined using stepwise selection to improve simplicity and interpretability.

### 2. Binary Logistic Regression (BLR)
   - **Null Model**: Serves as a baseline.
   - **Full Model**: Includes all predictors to explore all possible risk factors.
   - **Stepwise Model**: Adds preprocessing steps (removing near-zero variance and correlated features) for a leaner, more focused model.

## 🔍 Key Contributions
### Domain Expertise:
Applied domain knowledge to select relevant predictors and interpret results for insurance-specific use cases.

### Dirty Dataset Handling:
Dealt with messy, inconsistent datasets by creating a systematic data preparation workflow.



## 📊 Key Results and Visualizations

### Stepwise Multiple Linear Regression (MLR):

The Stepwise MLR model slightly outperformed the Full Model with a higher Adjusted R-squared and F-statistic, balanced predictive power with model simplicity.

![MLR Model Metrics](https://github.com/yinaS1234/Auto-Insurance-Regression/blob/main/Resources/mlr%20model%20metrics.png)
![MLR Residual Plot](https://github.com/yinaS1234/Auto-Insurance-Regression/blob/main/Resources/mlr%20resi-plot.png)

### Binary Logistic Regression (BLR) Metrics

The Stepwise BLR model achieved the best AUC, Kappa, and F1 scores, demonstrating balanced predictive power with reduced predictor redundancy.

![BLR Model Metrics](https://github.com/yinaS1234/Auto-Insurance-Regression/blob/main/Resources/blr%20model%20metrics.png)
![Confusion Matrix Grid](https://github.com/yinaS1234/Auto-Insurance-Regression/blob/main/Resources/confusion%20matrix%20grid.png)

---





## 📂 File Structure

- **Data**: Source data files.
- **Resources**: Supporting images and charts for reference.
- **Code**: R scripts for data preparation, model building, and evaluation.
- **Final Predictions**: Exported predictions on test data for easy access.


---

Happy analyzing! ✨
