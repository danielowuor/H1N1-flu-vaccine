# H1N1 Vaccine Prediction Project

## Project Overview

This project uses machine learning to predict whether individuals received the **H1N1 vaccine** using data from the **National 2009 H1N1 Flu Survey**.

The goal is to better understand factors associated with vaccination behavior and support public health decision-making during disease outbreaks such as H1N1 influenza.

This is a **binary classification problem**, where the model predicts:

* **1** → Individual received the vaccine
* **0** → Individual did not receive the vaccine

---

## Objective

To build and compare multiple classification models in order to:
* Identify the best-performing predictive model
* Evaluate model performance using appropriate metrics
* Apply ensemble modeling techniques
* Interpret results in a public health context

---

## Dataset

The dataset contains demographic, behavioral, and attitudinal variables such as:
* Age group
* Education level
* Health status
* Risk perception
* Doctor recommendations
* Household information
* Behavioral indicators

Target variable:

* `h1n1_vaccine`

---

## Methodology

The project follows a structured machine learning workflow:

### 1 Data Preprocessing

* Train_test split
* Encoding categorical variables
* Handling missing values
* Feature preparation

### 2 Model Development

The following models were implemented:

* Logistic Regression (Baseline Model)
* Tuned Logistic Regression
* Decision Tree
* Random Forest (Ensemble Model)
* Voting Classifier (Ensemble Combination Model)

---

## Evaluation Metrics

Models were evaluated using:

* **Accuracy**
* **ROC-AUC Score**
* **Precision**
* **Recall**
* **F1-Score**
* **ROC Curves**

ROC-AUC was particularly important because the dataset is slightly imbalanced.

---

## Final Model

The **Random Forest ensemble model** achieved the best overall performance, with the highest accuracy and strong ROC-AUC score.

This model was selected as the final model because it:
* Captured complex patterns in the data
* Provided strong predictive performance
* Performed better than simpler models

---

## Key Insights

* Doctor recommendations and personal risk perception strongly influence vaccination behavior.
* Ensemble methods improved predictive performance compared to a single decision tree.
* Handling class imbalance improved recall for vaccinated individuals.
* Machine learning models can support public health planning and targeted vaccination strategies.

---

##  Project Structure

```
├── data/
├── notebooks/
├── models/
├── README.md
└── requirements.txt

---

## Reference
DrivenData. (2020). Flu Shot Learning: Predict H1N1 and Seasonal Flu Vaccines. Retrieved [Month Day Year] from https://www.drivendata.org/competitions/66/flu-shot-learning.

