# Data Analytics Assignments

This repository contains projects and assignments completed for a graduate-level Data Analytics Seminar. It serves as a portfolio and archive of coursework exploring how data can be prepared, analyzed, visualized, and communicated to support informed decision-making.

## Projects

### Telecom Customer Churn Decision Tree

[`Garza_Oscar_DecisionTree.ipynb`](Garza_Oscar_DecisionTree.ipynb) develops an interpretable classification model for identifying telecom customers at risk of churn.

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/oegarza1/6308-data-analytics-assignments/blob/main/Garza_Oscar_DecisionTree.ipynb)

#### Analysis Overview

- Explores a public telecom dataset containing 3,333 customer records and 20 columns
- Reviews data types, missing values, class balance, and correlations with churn
- Uses a stratified 80/20 training and test split to preserve the 14.49% churn rate
- Preprocesses categorical features with one-hot encoding in a scikit-learn pipeline
- Trains a class-balanced `DecisionTreeClassifier` with a maximum depth of 5
- Visualizes the tree, extracts readable decision rules, and evaluates feature importance

#### Key Findings

The model identified customer service calls, international plan status, and total daytime minutes as the strongest churn indicators. Frequent service contacts may signal unresolved customer issues, while international plans and high usage or charge patterns also appear in higher-risk decision paths. These findings suggest that retention efforts could focus on customers with repeated support interactions and potentially costly usage patterns.

#### Model Performance

| Metric | Test Result |
| --- | ---: |
| Accuracy | 90.56% |
| Precision | 66.04% |
| Recall | 72.16% |
| F1 score | 68.97% |

On the 667-customer test set, the model correctly identified 70 of 97 customers who churned. It produced 36 false positives and missed 27 actual churners.

#### Tools and Libraries

- Python
- pandas and NumPy
- scikit-learn
- Matplotlib and seaborn
- Graphviz
- Google Colab / Jupyter Notebook

## Running the Notebook

Open the notebook using the Colab badge above and run the cells in order. The telecom dataset is loaded directly from its public GitHub source, so no local data download is required. A local Jupyter environment will need the libraries listed in the notebook imports.

Additional seminar projects may be added as the coursework collection grows.

## Purpose

The work collected here demonstrates the practical application of data preparation, exploratory analysis, predictive modeling, visualization, and business-focused interpretation developed during graduate study.

## Author

Oscar Garza  
Graduate Student

## Academic Use

These materials are shared for educational and portfolio purposes. Course requirements, datasets, and third-party resources remain subject to their respective terms of use.
