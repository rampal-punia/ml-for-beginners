# What is Recall Of an ML Model

Recall is a metric used to evaluate the performance of a machine learning model in terms of its ability to identify all relevant instances in a dataset.

It measures the proportion of true positive samples that are correctly identified by the model out of all positive samples in the dataset.

In simpler terms, recall or true positive rate (TPR) measures the ability of a machine learning model to correctly identify all the positive samples out of the total positive samples present in the dataset. It gives the percentage of positive samples that the model correctly identifies as positive.

Mathematically, recall is calculated as the number of true positives divided by the sum of true positives and false negatives:

Recall = True Positives / (True Positives + False Negatives)

If we have 100 positive instances in our dataset, and our model correctly identifies 80 of them, then the number of true positives is 80. If the model fails to identify the remaining 20 positive instances, then the number of false negatives is 20.

Using the formula for recall, we get:

Recall = 80 / (80 + 20) = 0.8 or 80%

This means that our model correctly identified 80% of the positive instances in the dataset, and missed 20%.

So we can say for 100 positive instances in our dataset, if our model correctly identifies 80 of them, then our recall is 80%.

A high recall value indicates that the model is correctly identifying a large proportion of the relevant samples in the dataset. Conversely, a low recall value indicates that the model is missing a significant number of relevant samples.

Recall is an important metric in applications where it is important to identify as many positive samples as possible.

For example, in medical diagnosis, it is important to identify as many cases of a disease as possible, even if it means sacrificing some precision (i.e., identifying some false positives). Similarly, in fraud detection, it is important to identify as many fraudulent transactions as possible, even if it means generating some false alarms.

However, it is important to note that recall should not be used in isolation to evaluate the performance of a machine learning model. It should be used in conjunction with other metrics such as precision, accuracy, and F1-score to get a comprehensive understanding of the model's performance. Additionally, the choice of metrics depends on the specific problem being solved and the nature of the data.
