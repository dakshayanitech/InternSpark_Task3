# Model Fairness, Bias and Explainability using SHAP and LIME

## Project Overview

This project analyzes the fairness, bias, and explainability of a Machine Learning model using the Adult Census Income dataset.

A Random Forest Classifier is trained to predict whether a person's annual income is greater than $50K. The project uses SHAP and LIME to explain model predictions and evaluates fairness across gender groups.

---

## Objective

The objectives of this project are to:

- Train a Random Forest classification model.
- Evaluate model performance.
- Compute feature importance.
- Explain model predictions using SHAP.
- Explain individual predictions using LIME.
- Analyze bias across sensitive groups (Male and Female).
- Suggest practical mitigation strategies to reduce bias.

---

## Dataset

**Dataset Name:** Adult Census Income Dataset

The dataset contains demographic and employment-related information used to predict whether a person's income exceeds $50,000 per year.

### Target Variable

- Income
  - <=50K
  - >50K

### Sensitive Attribute

- Sex (Male / Female)

---

## Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- SHAP
- LIME

---

## Project Workflow

### Step 1
Import all required libraries.

### Step 2
Load the Adult Census Income dataset.

### Step 3
Preprocess the dataset.

- Remove missing values
- Encode categorical variables
- Split data into training and testing sets

### Step 4
Train a Random Forest Classifier.

### Step 5
Evaluate model accuracy.

### Step 6
Calculate Feature Importance.

### Step 7
Generate SHAP explanations.

- Global explanation using Beeswarm Plot
- Local explanation using Waterfall Plot

### Step 8
Generate LIME explanation for an individual prediction.

### Step 9
Evaluate fairness by comparing prediction accuracy across Male and Female groups.

### Step 10
Recommend bias mitigation techniques.

---

## Results

The model achieved good classification accuracy on the Adult Census Income dataset.

The most important features identified by SHAP include:

- Education
- Age
- Capital Gain
- Hours per Week
- Marital Status

The SHAP and LIME explanations help understand why the model makes specific predictions.

The fairness analysis compares prediction accuracy between male and female groups to identify potential bias.

---

## Bias Analysis

The model was evaluated separately for Male and Female groups.

Example:

Male Accuracy : 87%

Female Accuracy : 84%

Bias Gap : 3%

A small bias gap indicates relatively balanced model performance, although continuous monitoring is recommended.

---

## Bias Mitigation Recommendations

To reduce potential bias in future versions of the model:

- Collect more balanced training data.
- Monitor fairness metrics regularly.
- Retrain the model using updated datasets.
- Apply fairness-aware machine learning techniques.
- Perform periodic bias audits.
- Evaluate additional fairness metrics.

---

## Explainability

### SHAP

SHAP provides global and local explanations of model predictions.

The project includes:

- SHAP Beeswarm Plot
- SHAP Waterfall Plot

These visualizations show how each feature contributes to model predictions.

### LIME

LIME explains individual predictions by identifying the features that most influenced the model's decision.

This improves model transparency and interpretability.

---

## Files Included

```
Fairness_Bias_Analysis.ipynb
README.md
requirements.txt
```

---

## Requirements

Install the required libraries using:

```bash
pip install -r requirements.txt
```

---

## requirements.txt

```
pandas
numpy
matplotlib
scikit-learn
shap
lime
```

---

## How to Run

1. Open the notebook in Google Colab.

2. Upload the Adult Census Income dataset (`adult.csv`).

3. Run all cells from top to bottom.

4. Review the outputs:

- Model Accuracy
- Feature Importance
- SHAP Beeswarm Plot
- SHAP Waterfall Plot
- LIME Explanation
- Bias Analysis

---

## Conclusion

This project demonstrates how explainable AI techniques can improve transparency and trust in machine learning models.

SHAP and LIME provide meaningful explanations for both global and local predictions, while the fairness analysis helps identify potential bias across sensitive groups. The proposed mitigation strategies support the development of more fair and responsible AI systems.

---

## Author

Dakshayani

Artificial Intelligence Intern
