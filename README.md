# Titanic

Titanic Survival Prediction using Supervised Classification

This repository contains a comprehensive data science project focused on predicting survival outcomes from the Titanic disaster using supervised machine learning techniques. The project explores and compares the performance of three classification algorithms — **Logistic Regression**, **k-Nearest Neighbors (k-NN)**, and **Decision Tree Classifier** — on the well-known Titanic dataset.

Project Objective

The goal of this study is to build predictive models that can determine whether a passenger survived the Titanic shipwreck based on socio-demographic and travel-related features such as age, sex, passenger class, and fare.

Dataset

The Titanic dataset was obtained from [Kaggle](https://www.kaggle.com/competitions/titanic) and includes 418 passenger records. Features used include:

* **Pclass**: Ticket class (1st, 2nd, 3rd)
* **Sex**: Gender of the passenger
* **Age**: Age in years
* **SibSp**: Number of siblings/spouses aboard
* **Parch**: Number of parents/children aboard
* **Fare**: Fare paid for the ticket
* **Embarked**: Port of embarkation (C, Q, S)
* **Survived**: Target variable (0 = No, 1 = Yes)

Methodology

1. Preprocessing

   * Handled missing values and dropped irrelevant columns
   * Applied label encoding for categorical variables
   * Standardized numerical features for use in k-NN
   * Split dataset into 80% training and 20% testing sets

2. Models Implemented

   * Logistic Regression
   * k-Nearest Neighbors (k = 5)
   * Decision Tree (Gini criterion)

3. Evaluation Metrics

   * Accuracy
   * Precision
   * Recall
   * F1-Score
   * Confusion Matrix
   * Classification Report

Results Summary

| Model               | Accuracy | Precision | Recall | F1-Score |
| ------------------- | -------- | --------- | ------ | -------- |
| Logistic Regression | 1.00     | 1.000     | 1.00   | 1.000    |
| k-NN                | 0.97     | 0.917     | 1.00   | 0.957    |
| Decision Tree       | 1.00     | 1.000     | 1.00   | 1.000    |


Visualizations

* Distribution plots for **Age**, **Fare**
* Survival count by **gender**
* Feature correlation **heatmap**
* **Confusion matrices** for each model
* **Bar chart** comparing performance metrics

Insights

* **Gender and class** significantly influenced survival.
* Logistic Regression and Decision Tree performed identically, possibly due to separability in data.
* k-NN, though slightly less accurate, provided strong performance and resilience.
* Interpretability and model behavior were key to selecting optimal classifiers.

Conclusion

This project demonstrates the effectiveness of basic classification models on a classic dataset. While high scores are promising, cross-validation and testing on additional data are recommended to validate generalizability.

References

* Cover, T., & Hart, P. (1967). *Nearest neighbour pattern classification*. IEEE Transactions on Information Theory.
* Hosmer, D. W., et al. (2013). *Applied Logistic Regression* (3rd ed.). Wiley.
* Quinlan, J. R. (1986). *Induction of decision trees*. Machine Learning.
* Zheng, Y., & Casari, A. (2018). *Feature Engineering for Machine Learning*. O’Reilly Media.
* [Kaggle Titanic Competition](https://www.kaggle.com/competitions/titanic)

