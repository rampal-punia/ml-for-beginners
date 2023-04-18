# What is Accuracy of an ML Model

## Introduction

Accuracy is one of the most common metrics used to evaluate the performance of a machine learning model. It measures the proportion of correct predictions made by the model out of all the predictions made. In other words, it is the ratio of the number of correct predictions to the total number of predictions made.

## What is accuracy in machine learning?

Accuracy is a statistical measure of how well a binary classification model can correctly identify the class labels of a given dataset. Binary classification is a type of classification problem where the goal is to predict one of two possible outcomes (e.g., spam vs. not spam, fraud vs. not fraud). The accuracy score is calculated as the ratio of the total number of correct predictions to the total number of predictions made. A perfect classifier would have an accuracy of 1, while an untrained model would have an accuracy close to 0.5 (50% chance of guessing correctly).

## Mathematically, accuracy can be expressed as

Accuracy = (Number of Correct Predictions) / (Total Number of Samples)

Accuracy = (TP + TN) / (TP + TN + FP + FN)

Where:

TP (True Positive) is the number of correctly predicted positive samples

TN (True Negative) is the number of correctly predicted negative samples

FP (False Positive) is the number of wrongly predicted positive samples, and

FN (False Negative) is the number of wrongly predicted negative samples

## Why is accuracy important?

Accuracy is a very important metric for machine learning models, especially in binary classification problems. It helps to measure the model's ability to make correct predictions, and hence, it provides insights into the overall performance of the model. However, accuracy should not be used in isolation to evaluate the performance of a model, as it has several limitations.

## Examples of accuracy in machine learning

To better understand accuracy, let's consider a few examples:

### Example 1: Email Spam Classifier

Suppose you have built an email spam classifier that predicts whether an email is spam or not. You have tested the model on 100 emails, and it has correctly classified 80 emails as not spam and 10 emails as spam. However, it has also misclassified 5 non-spam emails as spam and 5 spam emails as non-spam. In this case, the accuracy of the model can be calculated as follows:

Accuracy = (80 + 10) / (80 + 10 + 5 + 5) = 0.9

Thus, the accuracy of the email spam classifier is 90%.

### Example 2: Credit Card Fraud Detection

Suppose you have built a machine learning model that predicts whether a credit card transaction is fraudulent or not. You have tested the model on a dataset of 1000 transactions, out of which 950 are genuine and 50 are fraudulent. The model correctly predicts 900 genuine transactions and 45 fraudulent transactions. However, it also wrongly predicts 25 genuine transactions as fraudulent and 30 fraudulent transactions as genuine. In this case, the accuracy of the model can be calculated as follows:

Accuracy = (900 + 45) / (900 + 45 + 25 + 30) = 0.945

Thus, the accuracy of the credit card fraud detection model is 94.5%.

## Limitations of accuracy

Accuracy can be misleading in certain cases, making it a less than perfect metric for evaluating model performance. Here are some of the limitations of accuracy:

### Imbalanced datasets

When one class is much more frequent than the other, the dataset is said to be imbalanced. In such cases, a model can achieve high accuracy by simply predicting the majority class for all samples. For example, in a dataset with 95% of samples belonging to the negative class and only 5% belonging to the positive class, a model that predicts all samples as negative would achieve an accuracy of 95%. In such cases, other metrics such as precision, recall, and F1-score may provide a better indication of the model's performance.

### Cost-sensitive classification

In some cases, the cost of a false positive (a prediction that a sample belongs to a particular class when it does not) is different from the cost of a false negative (a prediction that a sample does not belong to a particular class when it does). For example, in medical diagnosis, the cost of a false negative (a missed diagnosis) may be much higher than the cost of a false positive (an incorrect diagnosis). In such cases, the model should be optimized for other metrics, such as sensitivity and specificity, that take into account the relative costs of false positives and false negatives.

### Label errors

The accuracy of a model can be impacted if there are errors in the labels of the training data. If the training data contains mislabeled samples, the model may learn incorrect patterns, leading to poor performance on unseen data. To mitigate this, it's important to carefully clean and validate the training data.

### Limited scope of evaluation

Accuracy measures how well a model performs on the samples it was trained on and evaluated on. It doesn't necessarily reflect how well the model will perform on new, unseen data. Therefore, it's important to use techniques such as cross-validation to get a more accurate estimate of the model's performance.

## Conclusion

Accuracy is a widely used metric for evaluating the performance of machine learning models, but it has its limitations. It is important to be aware of these limitations when using accuracy to evaluate a model's performance. In addition to accuracy, it is recommended to use other evaluation metrics to gain a more comprehensive understanding of the model's performance.
