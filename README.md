# Auto Insurance Claim Prediction  ✨ 🚗📈  ✨

This project demonstrates my ability to work with large, messy datasets in the insurance domain, focusing on two key predictive goals:
1. **The probability of a car crash** (`TARGET_FLAG`) - Binary Logistic Regression
2. **The potential claim amount if a crash occurs** (`TARGET_AMT`) - Multiple Linear Regression

## Why This Matters
Insurance providers rely on accurate predictions for:
1. **Assessing risk effectively
2. **Setting fair premiums
3. **Streamlining claim processes


## 🛠️ Project Workflow

The project follows a systematic data preparation and modeling workflow to handle this high-dimensional dataset, clean inconsistencies, address class imbalances, and tackle multicollinearity. Below is the comprehensive flowchart of the workflow:

![Data Preparation Workflow](https://github.com/yinaS1234/Auto-Insurance-Regression/blob/main/Resources/flowchart.png)

## 🚀 Models Built and Evaluated

### 1. Multiple Linear Regression (MLR)
   - **Full Model**: Includes all predictors to assess the overall feature impact.
   - **Stepwise Model**: Refined using stepwise selection to improve simplicity and interpretability.

### 2. Binary Logistic Regression (BLR)
   - **Null Model**: Serves as a baseline.
   - **Full Model**: Includes all predictors to explore all possible risk factors.
   - **Stepwise Model**: Adds preprocessing steps (removing near-zero variance and correlated features) for a leaner, more focused model.

## 📊 Key Results and Visualizations

Each model was evaluated on a set of important metrics to identify the best-performing approach.

### Multiple Linear Regression (MLR) Metrics
MLR models were evaluated on **Mean Squared Error (MSE)**, **Root Mean Squared Error (RMSE)**, **R-squared**, **Adjusted R-squared**, and **F-statistic**:
- **MSE & RMSE**: These metrics help measure the average and root error between actual and predicted values, providing insight into prediction accuracy.
- **R-squared & Adjusted R-squared**: These scores indicate the proportion of variance in the target variable explained by the model. Adjusted R-squared adjusts for the number of predictors, giving a more accurate assessment as predictors are added.
- **F-statistic**: Assesses the overall significance of the model, with higher values indicating a better fit.

The Stepwise MLR model slightly outperformed the Full Model with a higher Adjusted R-squared and F-statistic, indicating a more parsimonious model with similar predictive power.

![MLR Model Metrics](https://github.com/yinaS1234/Auto-Insurance-Regression/blob/main/Resources/mlr%20model%20metrics.png)
![MLR Residual Plot](https://github.com/yinaS1234/Auto-Insurance-Regression/blob/main/Resources/mlr%20resi-plot.png)

### Binary Logistic Regression (BLR) Metrics
BLR models were assessed with **Accuracy**, **Error Rate**, **Kappa**, **Precision**, **Sensitivity**, **Specificity**, **F1 Score**, and **AUC** (Area Under the Curve):
- **Accuracy & Error Rate**: Measure the model's correctness and error rate, providing a straightforward performance overview.
- **Kappa**: Indicates how well the predictions match the actual values, adjusted for agreement by chance, offering a fairer metric than accuracy in imbalanced datasets.
- **Precision & Sensitivity**: Evaluate the model's ability to correctly identify positive cases (crash likelihood), essential in risk prediction.
- **Specificity**: Indicates the model’s ability to correctly classify non-crash cases.
- **F1 Score & AUC**: F1 balances precision and sensitivity, while AUC reflects the overall ability to discriminate between crash and non-crash cases.

The Stepwise BLR model achieved the best AUC, Kappa, and F1 scores, demonstrating balanced predictive power with reduced predictor redundancy.

![BLR Model Metrics](https://github.com/yinaS1234/Auto-Insurance-Regression/blob/main/Resources/blr%20model%20metrics.png)
![Confusion Matrix Grid](https://github.com/yinaS1234/Auto-Insurance-Regression/blob/main/Resources/confusion%20matrix%20grid.png)

---

By analyzing these metrics, the Stepwise models for both MLR and BLR were chosen for their ability to balance predictive power with simplicity. These models were then retrained on the full dataset to produce robust final models for prediction on unseen data.

---

## 📂 File Structure

- **Data**: Source data files.
- **Resources**: Supporting images and charts for reference.
- **Code**: R scripts for data preparation, model building, and evaluation.
- **Final Predictions**: Exported predictions on test data for easy access.


---

Happy analyzing! ✨
