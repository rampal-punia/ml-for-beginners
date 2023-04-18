# What is F1 score of an ML Model?

## Introduction

F1-score is an essential metric for evaluating the performance of machine learning models, particularly in binary classification problems. In this tutorial, we'll dive into F1-score, including its calculation and significance in model evaluation.

## What is F1 Score

F1-score is the harmonic mean of precision and recall, where precision is the proportion of true positives out of all positive predictions made by the model, and recall is the proportion of true positives out of all actual positive samples in the dataset. F1-score combines both precision and recall into a single metric, providing a more comprehensive evaluation of the model's performance.

## Why is F1 Score important?

F1-score is an important metric because it considers both precision and recall, providing a more balanced evaluation of the model's performance, particularly in imbalanced datasets where the number of positive and negative samples is not equal. While accuracy is a commonly used metric, it may not provide an accurate evaluation of the model's performance in such scenarios.

## How is F1 Score calculated?

F1-score is calculated as the harmonic mean of precision and recall, which gives more weight to lower values. The mathematical formula for calculating F1-score is:

F1-score = 2 *(precision* recall) / (precision + recall)

To illustrate how F1-score is calculated, consider a binary classification problem where the model predicts whether an email is spam or not. The confusion matrix for the model is as follows:

||Actual Positive|Actual Negative|
|-----|------------|--------------|
|Predicted Positive | 50 | 20|
|Predicted Negative | 10 | 70|
||||

The precision and recall values for the model can be calculated as follows:

Precision = 50 / (50 + 20) = 0.71

Recall = 50 / (50 + 10) = 0.83

Using the formula for F1-score, we can calculate the F1-score for the model as:

F1-score = 2 *(0.71* 0.83) / (0.71 + 0.83) = 0.76

## Interpreting F1 Score

F1-score values range from 0 to 1, with 1 indicating perfect precision and recall, and 0 indicating poor performance. A high F1-score indicates that the model is making accurate predictions with both high precision and recall. A low F1-score indicates that the model is not making accurate predictions, either due to low precision, low recall, or both.

When interpreting the F1-score, it's important to keep in mind the specific problem being solved and the nature of the data. For example, in a scenario where false positives are more costly than false negatives, a higher emphasis should be placed on precision than recall. On the other hand, in a scenario where false negatives are more costly than false positives, a higher emphasis should be placed on recall than precision.

It's also important to note that the F1-score should not be used in isolation to evaluate the performance of a machine learning model. It should be used in conjunction with other metrics such as accuracy, precision, and recall to get a comprehensive understanding of the model's performance.

To illustrate the use of F1-score, let's consider an example of binary classification problem where we want to predict whether a customer will buy a product based on their age and income. Let's say we have a dataset of 1000 customers, out of which 800 actually buy the product and 200 don't. We train a machine learning model on this data and obtain the following confusion matrix:

||Predicted: No| Predicted: Yes|
|-------|----------|---------|
| Actual: No | 120 | 80|
|Actual: Yes |40 |760|
||||

Using the formula for F1-score, we can calculate the F1-score of this model as follows:

Precision = 760 / (760 + 80) = 0.905

Recall = 760 / (760 + 40) = 0.950

F1-score = 2 *(Precision* Recall) / (Precision + Recall) = 0.927

This means that the model has a high F1-score, indicating that it is making accurate predictions with both high precision and recall. However, we should also look at other metrics such as accuracy and consider the specific problem being solved to get a comprehensive understanding of the model's performance.

It's important to note that while the F1-score is a useful metric for evaluating the performance of machine learning models, it does have some limitations. For example, the F1-score assumes that both precision and recall are equally important, which may not always be the case. In some scenarios, precision may be more important than recall, and vice versa. Therefore, it's important to consider the specific problem being solved and the nature of the data when evaluating the performance of a machine learning model.

In addition, the F1-score is only applicable to binary classification problems. For multi-class classification problems, alternative metrics such as the macro F1-score or micro F1-score may be used.

## Conclusion

The F1-score is a useful metric for evaluating the performance of machine learning models in binary classification problems. It provides a more comprehensive evaluation of the model's performance by considering both precision and recall. However, it should be used in conjunction with other metrics and should be interpreted in the context of the specific problem being solved and the nature of the data.
