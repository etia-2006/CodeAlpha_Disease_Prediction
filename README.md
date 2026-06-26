# Disease Prediction from Medical Data (CodeAlpha Task 4)

This repository contains the solution for Task 4 of the CodeAlpha Data Science Internship. The project focuses on predicting whether a patient has diabetes based on diagnostic measurements from the Pima Indians Diabetes Database.

## 📊 Approach & Workflow
1. **Data Preprocessing:** Loaded the `diabetes.csv` dataset and stripped any whitespace from column names.
2. **Feature & Target Split:** Separated the dataset into features (X) and the target variable (Outcome - y).
3. **Train-Test Split:** Divided the data into training (80%) and testing (20%) sets using `train_test_split` with a fixed `random_state=42` for reproducibility.
4. **Feature Scaling:** Applied `StandardScaler` to normalize the numeric features, ensuring all inputs are on the same scale for distance-based and linear models.
5. **Model Comparison:** Trained and evaluated three classification models specified in the internship guidelines.

## 📈 Evaluation Results
* **Logistic Regression:** 75.32% 🏆 *(Best Performance)*
* **Support Vector Machine (SVM):** 73.37%
* **Random Forest:** 72.07%

## 💡 Conclusion
In this specific task, **Logistic Regression** outperformed the other models. This is a common occurrence with smaller datasets (768 records), where simpler linear boundaries generalize better on unseen test data and help prevent overfitting compared to more complex architectures like Random Forest.

## 🛠️ Tech Stack & Libraries
* **Environment:** Google Colab / Python
* **Data Manipulation:** Pandas, NumPy
* **Machine Learning:** Scikit-Learn (`LogisticRegression`, `SVC`, `RandomForestClassifier`, `StandardScaler`)
* **Visualization:** Matplotlib
