# Movie-Reviews-Sentiment-Analysis-with-Logistic-Regression


This repository contains a project on sentiment analysis utilizing various machine learning algorithms to evaluate and classify text data, particularly focusing on movie reviews. The main objective is to determine the sentiment polarity (positive, negative, or neutral) of given reviews using different classification models.

## Table of Contents
- [Introduction](#introduction)
- [Data Preparation](#data-preparation)
- [Models Used](#models-used)
  - [1. Logistic Regression](#1-logistic-regression)
  - [2. Support Vector Machines](#2-support-vector-machines)
  - [3. Naïve Bayes](#3-naïve-bayes)
- [Data Leakage Prevention](#data-leakage-prevention)
- [Results and Evaluation](#results-and-evaluation)
- [Conclusion](#conclusion)
- [Proposed Improvements](#proposed-improvements)

## Introduction

Sentiment analysis has become a popular tool for determining how people feel regarding a service, product, public issue, or location. This project employs machine learning techniques to analyze and classify sentiment in textual data.

## Data Preparation

Data preparation involves preprocessing steps such as text cleaning, tokenization, and vectorization of text features using techniques like Bag of Words and TF-IDF.

## Models Used

### 1. Logistic Regression
Logistic Regression utilizes the Sigmoid function for classification. The performance is evaluated using accuracy and recall metrics, achieving an accuracy of approximately 75% before tuning.

### 2. Support Vector Machines
Support Vector Machines (SVMs) are margin-based classifiers. The model attempts to find a hyperplane that separates the classes with maximum margin. The results demonstrated a competitive performance.

### 3. Naïve Bayes
The Naïve Bayes classifier is based on Bayes' theorem. It assumes conditional independence among features, achieving comparable performance with an accuracy of around 75%.

## Data Leakage Prevention

Data leakage is a critical issue in machine learning, where external information affects model performance. To mitigate this, a pipeline was implemented to streamline data preparation and ensure that training and testing data are properly managed.

## Results and Evaluation

After implementing a pipeline and using hyperparameter tuning with Grid Search, the Logistic Regression model achieved an accuracy of 89.81%. Other classifiers such as Random Forest, Stochastic Gradient Descent, and XGBoost were also evaluated, showing promising results.

### Accuracy Comparison
- Logistic Regression: 89.81%
- Stochastic Gradient Descent: 89.34%
- Other classifiers achieved similar accuracies above 75%.

## Conclusion

The results indicate that Logistic Regression, enhanced through hyperparameter tuning, provides the best performance for this sentiment analysis task. Further improvements are proposed to enhance context understanding and classification accuracy.

## Proposed Improvements

To further enhance model performance, consider:
- Implementing n-grams (bi-grams, tri-grams) for better context capture.
- Using word vectors from CBOW or skip-gram models for improved word representation.
- Exploring deep learning techniques and other datasets for comprehensive sentiment analysis.

---

### Acknowledgements
- This project was developed with the support of various machine learning libraries including Scikit-learn.
- References for methods and algorithms can be found in relevant literature, including works by Joachims (1998) and Domingos & Pazzani (1997).

