# What is Recall Of an ML Model

## Introduction

Recall is a performance metric used in machine learning models to measure the ability of the model to correctly identify all the positive samples out of the total positive samples present in the dataset. In this tutorial, we will explore the concept of recall, how it is calculated, and its importance in evaluating the performance of a machine learning model.

## Definition of Recall

Recall is a metric used to evaluate the performance of a machine learning model in terms of its ability to identify all relevant instances in a dataset. It measures the proportion of true positive samples that are correctly identified by the model out of all positive samples in the dataset.

## Calculations

Mathematically, recall is calculated as the number of true positives divided by the sum of true positives and false negatives:

**Recall = True Positives / (True Positives + False Negatives)**

For example, if we have 100 positive instances in our dataset, and our model correctly identifies 80 of them, then the number of true positives is 80. If the model fails to identify the remaining 20 positive instances, then the number of false negatives is 20. Using the formula for recall, we get:

**Recall = 80 / (80 + 20) = 0.8 or 80%**

This means that our model correctly identified 80% of the positive instances in the dataset, and missed 20%.

## Importance of Recall

A high recall value indicates that the model is correctly identifying a large proportion of the relevant samples in the dataset. Recall is an important metric in applications where it is important to identify as many positive samples as possible.

For example, in medical diagnosis, it is crucial to identify all cases of a disease, even if it means some false positives. Similarly, in fraud detection, it is important to identify as many fraudulent transactions as possible, even if it means generating some false alarms.

## Limitations of Recall

It is important to note that recall should not be used in isolation to evaluate the performance of a machine learning model. This is because a high recall can be achieved by classifying all instances as positive, which is not ideal in most cases. Therefore, recall should be used in conjunction with other metrics such as precision, accuracy, and F1-score to get a comprehensive understanding of the model's performance. Additionally, the choice of metrics depends on the specific problem being solved and the nature of the data.

## Conclusion

Recall is a critical metric in scenarios where it is important to identify all relevant instances in a dataset. Understanding the concept of recall, how it is calculated, and its importance in evaluating the performance of a machine learning model is essential to building effective machine learning systems.
