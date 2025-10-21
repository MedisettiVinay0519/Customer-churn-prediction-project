# 📉 Telco Customer Churn Prediction: Random Forest & Hyperparameter Tuning

## Project Description

This project develops a robust **Customer Churn Prediction** model using machine learning on Telco customer data to proactively identify clients at high risk of leaving the service. The solution employs a systematic approach, ensuring model reliability and high predictive performance.

## 🛠️ Technical Implementation & Methodology

* **Goal:** Binary Classification (Predict 'Churn' or 'No Churn').
* **Data Preprocessing:** Handled missing values (e.g., in `TotalCharges`), applied **One-Hot Encoding** to numerous categorical features, and split the data into training and testing sets.
* **Model Selection:** Benchmarked multiple classification algorithms and utilized **K-Fold Cross-Validation** (`cross_val_score`) to objectively select the best-performing baseline model, which was the **Random Forest Classifier**.
* **Optimization:** Employed **Hyperparameter Tuning** (e.g., Grid Search) to fine-tune the selected Random Forest model's parameters (like `n_estimators` and `max_depth`), maximizing its predictive power.
* **Final Model:** Optimized Random Forest Classifier.

## 📈 Results

The final, optimized model provides high confidence in predicting churn risk:

* **Final Accuracy:** **92.7%** on the unseen test dataset.
* **Validation Metrics:** Performance was thoroughly validated using a **Confusion Matrix** and a detailed **Classification Report**.

---

## 📊 Visualizations

The table below displays the key visualizations from the project, including the correlation between features and the importance of each feature in the final model's predictions.


| Correlation Matrix | Feature Importance Plot |
| :---: | :---: |
| <img src="images/Screenshot%202025-10-21%20175405.png" alt="Correlation Heatmap" width="350"/> | <img src="images/Screenshot%202025-10-21%20175738.png" alt="Feature Importance" width="350"/> |

---

## 💻 Repository Structure

* `customer-churn-prediction-hp-tunning.ipynb`: The main Jupyter Notebook containing all steps: EDA, preprocessing, model benchmarking, cross-validation, hyperparameter tuning, and final evaluation.
* `images/`: Directory containing project visualizations and plots.
