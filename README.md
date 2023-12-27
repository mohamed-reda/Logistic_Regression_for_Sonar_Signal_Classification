# Logistic Regression for Sonar Signal Classification

## Overview

This project focuses on utilizing logistic regression for the classification of sonar signals into two categories:
Rock (R) and Mine (M). The primary objective is to build a predictive model capable of distinguishing between underwater
objects based on the features extracted from sonar data.

## Project Structure

The project is organized into the following sections:

### 1. Importing the Dependencies

In this section, essential libraries such as NumPy, Pandas, and scikit-learn are imported to facilitate data
manipulation, processing, and model training.

### 2. Data Collection and Data Processing

This section involves loading the sonar dataset into a Pandas DataFrame and performing initial exploratory data
analysis. Descriptive statistics and data visualization are employed to understand the characteristics of the dataset.

### 3. Training and Test Data Split

The dataset is divided into training and test sets using the `train_test_split` function from scikit-learn. This ensures
the model's ability to generalize to unseen data.

### 4. Model Training - Logistic Regression

The logistic regression model is instantiated and trained on the training data using the `fit` method.

### 5. Model Evaluation

The accuracy of the trained model is assessed on both the training and test datasets. The `accuracy_score` metric is
used to quantify the model's performance.

### 6. Making a Predictive System

A sample input data point is provided to the trained model to demonstrate its ability to classify the object as either a
Rock or a Mine. The result is then displayed with a corresponding interpretation.

## How to Run the Code

To run the code, follow these steps:

1. Ensure you have the necessary dependencies installed (NumPy, Pandas, scikit-learn).
2. Download the sonar dataset (`sonar data.csv`) and update the file path in the code accordingly.
3. Execute the code in a Python environment.

## Conclusion

This project showcases the application of logistic regression in sonar signal classification. The trained model can be
used to predict the nature of underwater objects based on input features derived from sonar data.

Feel free to explore and modify the code to enhance the model or apply it to other datasets with similar classification
tasks.

---


to run jupyter:

jupyter notebook

(Use Control-C to stop this server)

----
pip install -r requirements.txt

python -m pip install jupyter

---
memory profile:

@memory_profiler.profile

python -m memory_profiler main.py

---

from line_profiler_pycharm import profile

@profile

python -m line_profiler main.py.lprof > results.txt
