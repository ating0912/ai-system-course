Dataset README --- Week 01 Customer Churn Sample

1. Dataset Name

Week 01 Customer Churn Sample Dataset

File: week01_customer_churn_sample.csv

2. Purpose

This dataset is a small synthetic teaching dataset for Week 1 of the
course AI Systems and Industrial Applications.

It is designed to help students complete the minimum reproducible
experiment workflow:

Dataset → Train/Test Split → Baseline Model → Metric → MLflow Run →
Git Commit/Push

The goal is to practice the experimental workflow rather than achieve a
high model score.

3. Dataset Version

Version: v1.0
Type: Synthetic teaching dataset
Number of records: 40
Task: Binary classification
Target: churn

4. Feature Definitions

Field             Description       Type              Role

age             Customer age      Integer           Input feature

income          Synthetic annual  Integer           Input feature
income

usage_time      Synthetic service Integer           Input feature
usage time

complaints      Number of         Integer           Input feature
synthetic
customer
complaints

5. Classification Task

Given the following input features:

age

income

usage_time

complaints

predict:

churn = 0: customer does not churn

churn = 1: customer churns

A simple Logistic Regression model can be used as the Week 1
baseline.

6. Recommended Week 1 Experiment

Suggested workflow:

Load the CSV file with pandas.

Separate input features (X) and target (y).

Create a train/test split.

Train a Logistic Regression baseline.

Generate predictions on the test set.

Calculate at least one classification metric, such as Accuracy.

Record the model parameters and metric in MLflow.

Commit and push the experiment changes to Gitea.

Suggested initial configuration:

test_size = 0.2

random_state = 42

Baseline model = LogisticRegression

Primary teaching metric = Accuracy

These settings are for the Week 1 teaching exercise, not a claim that
they are optimal.

7. Important Limitations

This dataset is synthetic and created only for teaching purposes.

It does not represent real customer behavior.

The feature values and labels should not be interpreted as real
business relationships.

Model performance on this dataset does not demonstrate real-world
generalization.

A high Accuracy score should not be interpreted as evidence that an
AI system is ready for deployment.

The dataset is intentionally small so students can focus on the
reproducible experiment workflow.

8. Expected Evidence

Students should be able to identify:

Dataset: data/week01_customer_churn_sample.csv

Dataset version: v1.0

Dataset documentation: data/README.md

Baseline: Logistic Regression

Metric: recorded in the Week 1 Notebook and MLflow

Experiment version: Git/Gitea commit history

9. Data Source

The dataset was synthetically generated for course instruction. No real
customer records or personal information are included.
