# Titanic Survival Prediction using Decision Tree 🌳

## 📌 Project Overview
This project implements a **Decision Tree Classifier** on the Kaggle Titanic dataset to predict passenger survival. The focus is on building an interpretable model, controlling overfitting through hyperparameter tuning, and evaluating performance using cross-validation.

## 📊 Dataset
* **Source:** Kaggle Titanic Dataset
* **Total Records:** 891
* **Target Variable:** `Survived` (0 = Did not survive, 1 = Survived)


## 🔧 Data Preprocessing
* Handled missing values (Age, Embarked)
* Encoded categorical variables (Sex, Embarked)
* Selected relevant numerical and categorical features
* Performed train–test split with cross-validation

📌 *Feature scaling was not applied, as Decision Trees are not sensitive to feature magnitude.*

## 🤖 Model: Decision Tree Classifier
Decision Trees create rule-based splits on features, making them easy to interpret but prone to overfitting if not tuned properly.

### 🔍 Hyperparameter Tuning
Optimized the model using **GridSearchCV** with the following key parameters:

* `max_depth`
* `min_samples_split`
* `min_samples_leaf`

## 📈 Model Performance

* **Training Accuracy:** ~84.7%
* **Cross-Validation Accuracy:** ~79.8%
* **Test Accuracy:** ~85.5%

The close alignment between training and test accuracy indicates good generalization after tuning.

## ⭐ Feature Importance
* Extracted feature importance using:

  ```python
  best_estimator_.feature_importances_
  ```
* Helped identify the most influential factors affecting survival predictions

## 🛠️ Tech Stack
* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn

## 🧠 Key Learnings
* Decision Trees are highly interpretable but require tuning to prevent overfitting
* Cross-validation is essential for reliable model evaluation
* Tree-based models do not require feature scaling
* Hyperparameter constraints significantly improve generalization

## 🚀 Future Improvements
* Visualize the decision tree structure
* Compare with ensemble models like Random Forest and Gradient Boosting
* Optimize evaluation using recall or F1-score

## 📬 Contact

Feel free to connect with me on **LinkedIn** to discuss data analytics, machine learning, and project learnings.
