# Ecoli DNA sequence classification

# To do:
1. Train 2 Machine Learning and 2 Deep Learning models on the UCI data for Promoter Gene Sequences.
2. Report the performances.

# Result insights:
1. The models, as of now, has regularization issues where training data accuracies are ~90+%, whereas the test data accuracies are significantly less than that (~10% differences).
    - Additional model regularization tasks have not been taken care of yet.
    - Grid Search or other techniques for hyperparameter optimisation has not yet been implemented due to time and resource constraints
2. As for the performance comparison:
    - In terms of absolute accuracies, Linear SVM has the best performance on the TEST dataset, followed by CNN, RNN and Random Forest.
    - The Linear SVM and Random Forest have 100% TRAIN performance, and the two NNs have ~98%.

## Accuracy Details:
| Model | Data | Accuracy |
| ------ | ------ | ------ |
| Linear Support Vector Machine | Train | 1.000000 |
| Linear Support Vector Machine | Test | 0.952381 |
| Random Forest | Train | 1.000000 |
| Random Forest | Test | 0.857143 |
| Convolutional Neural Network | Train | 0.988095 |
| Convolutional Neural Network | Test | 0.904762 |
| Recurrent Neural Network | Train | 0.988095 |
| Recurrent Neural Network | Test | 0.904762 |


## Other class-wise metrics:
| Model | Data | Class | Precision | Recall | F1-score |
| ------ | ------ | ------ | ------ | ------ | ------ |
| Linear Support Vector Machine | Train | 0 | 1.000000 | 1.000000 | 1.000000 |
| Linear Support Vector Machine | Train | 1 | 1.000000 | 1.000000 | 1.000000 |
| Linear Support Vector Machine | Test | 0 | 0.923077 | 1.000000 | 0.960000 |
| Linear Support Vector Machine | Test | 1 | 1.000000 | 0.888889 | 0.941176 |
| Random Forest | Train | 0 | 1.000000 | 1.000000 | 1.000000 |
| Random Forest | Train | 1 | 1.000000 | 1.000000 | 1.000000 |
| Random Forest | Test | 0 | 0.909091 | 0.833333 | 0.869565 |
| Random Forest | Test | 1 | 0.800000 | 0.888889 | 0.842105 |
| Convolutional Neural Network | Train | 0 | 0.976190 | 1.000000 | 0.987952 |
| Convolutional Neural Network | Train | 1 | 1.000000 | 0.976744 | 0.988235 |
| Convolutional Neural Network | Test | 0 | 0.857143 | 1.000000 | 0.923077 |
| Convolutional Neural Network | Test | 1 | 1.000000 | 0.777778 | 0.875000 |
| Recurrent Neural Network | Train | 0 | 1.000000 | 0.975610 | 0.987654 |
| Recurrent Neural Network | Train | 1 | 0.977273 | 1.000000 | 0.988506 |
| Recurrent Neural Network | Test | 0 | 0.916667 | 0.916667 | 0.916667 |
| Recurrent Neural Network | Test | 1 | 0.888889 | 0.888889 | 0.888889 |

In this table, class 1 means "+", and class 0 means "-"
