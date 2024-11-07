# Auto-Insurance-Regression


# Auto Insurance Claim Prediction 🚗📈

This project focuses on predicting two essential outcomes for auto insurance claims:
1. **The probability of a car crash** (`TARGET_FLAG`) - Binary Logistic Regression
2. **The potential claim amount if a crash occurs** (`TARGET_AMT`) - Multiple Linear Regression

### Why This Matters
Accurate predictions of accident probability and claim amounts allow insurance providers to assess risks better, set fair premiums, and handle claims efficiently. This project uses advanced data preparation and modeling techniques to maximize prediction accuracy, ensuring models are ready to tackle real-world scenarios with high variability.

---

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
For model selection and evaluation, critical performance metrics like AUC and residuals were used to determine the best models, then validated on a held-out test set to simulate real-world predictions.

---

## 📂 File Structure

- **Data**: Source data files.
- **Resources**: Supporting images and charts for reference.
- **Code**: R scripts for data preparation, model building, and evaluation.
- **Final Predictions**: Exported predictions on test data for easy access.


---

Happy analyzing! ✨
