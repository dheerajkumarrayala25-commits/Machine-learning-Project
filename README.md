# Course Completion Time Prediction for SkillBridge

## 📌 Project Overview
The objective of this machine learning project is to build a predictive model that estimates the number of days required for a learner to complete a SkillBridge course. By analyzing learner characteristics, study habits, previous performance indicators, and engagement metrics, the model helps educational platforms optimize course pacing and provide personalized support systems for student success.

* **Developed by:** Rayala Dheeraj kumar
* **Organization:** YBI Foundation Project Platform
* **Core Task:** Regression (Predicting a continuous numerical value representing days)

---

## 📊 Model Evaluation & Performance Metrics
The project successfully implemented a **Linear Regression** model to predict completion timelines. The model achieved the following performance evaluation metrics on the test dataset:

* **Mean Absolute Error (MAE):** 4.41 days (On average, predictions deviate by about 4.4 days from the actual completion time)
* **Mean Squared Error (MSE):** 29.49
* **Root Mean Squared Error (RMSE):** 5.43 days
* **R² Score (Coefficient of Determination):** 0.712 (~71.2% of the variance in course completion times is successfully explained by the model's features)

---

## 🛠️ Tech Stack & Libraries Used
* **Language Environment:** Python 3 (Google Colab Notebook)
* **Data Ingestion & Engineering:** Pandas, NumPy
* **Data Visualization & EDA:** Matplotlib, Seaborn
* **Machine Learning Framework:** Scikit-Learn
  * **Model:** `LinearRegression`
  * **Validation Splitting:** `train_test_split`
  * **Evaluation Suite:** `mean_absolute_error`, `mean_squared_error`, `r2_score`

---

## 🚀 Project Workflow Breakdown

### 1. Data Source & Library Initialization
Imported essential python packages for tabular analysis, predictive metrics calculation, and graphical subplots. The SkillBridge training dataset was pulled into the environment using structured Pandas DataFrames.

### 2. Exploratory Data Analysis (EDA)
Performed standard data validation checks to review data structure shapes, investigate feature parameters, verify columns, clean up data duplicates, and check for missing null variables. Visual distributions and correlation heatmaps were utilized to map how behavioral habits directly impact completion times.

### 3. Data Preprocessing & Target Splitting
Isolated the continuous target metric from independent learner features. The dataset was split systematically into training and testing components using `train_test_split` to prevent overfitting.

### 4. Model Training & Evaluation
Initialized and fitted the `LinearRegression` algorithm on the behavioral training data subset. Evaluated the final predictions against actual test labels using standard error metrics (MAE, RMSE,and $R^2$) to verify performance reliability.
