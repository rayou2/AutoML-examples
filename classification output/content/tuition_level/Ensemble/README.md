# Summary of Ensemble

[<< Go back](../README.md)


## Ensemble structure
| Model             |   Weight |
|:------------------|---------:|
| 4_Default_Xgboost |        1 |

### Metric details
|           |   2 yr Undergrad |   4 yr Undergrad |   5 yr Undergrad |       Grad |     STAP |   Unknown |   accuracy |   macro avg |   weighted avg |   logloss |
|:----------|-----------------:|-----------------:|-----------------:|-----------:|---------:|----------:|-----------:|------------:|---------------:|----------:|
| precision |         0.946429 |         0.959722 |         0.880342 |   0.996429 | 1        |  0.833333 |   0.942611 |    0.936042 |       0.943681 |  0.175651 |
| recall    |         0.946429 |         0.933784 |         0.927928 |   1        | 0.142857 |  1        |   0.942611 |    0.825166 |       0.942611 |  0.175651 |
| f1-score  |         0.946429 |         0.946575 |         0.903509 |   0.998211 | 0.25     |  0.909091 |   0.942611 |    0.825636 |       0.941856 |  0.175651 |
| support   |       616        |       740        |       444        | 279        | 7        |  5        |   0.942611 | 2091        |    2091        |  0.175651 |


## Confusion matrix
|                           |   Predicted as 2 yr Undergrad |   Predicted as 4 yr Undergrad |   Predicted as 5 yr Undergrad |   Predicted as Grad |   Predicted as STAP |   Predicted as Unknown |
|:--------------------------|------------------------------:|------------------------------:|------------------------------:|--------------------:|--------------------:|-----------------------:|
| Labeled as 2 yr Undergrad |                           583 |                             8 |                            25 |                   0 |                   0 |                      0 |
| Labeled as 4 yr Undergrad |                            16 |                           691 |                            31 |                   1 |                   0 |                      1 |
| Labeled as 5 yr Undergrad |                            15 |                            17 |                           412 |                   0 |                   0 |                      0 |
| Labeled as Grad           |                             0 |                             0 |                             0 |                 279 |                   0 |                      0 |
| Labeled as STAP           |                             2 |                             4 |                             0 |                   0 |                   1 |                      0 |
| Labeled as Unknown        |                             0 |                             0 |                             0 |                   0 |                   0 |                      5 |

## Learning curves
![Learning curves](learning_curves.png)
## Confusion Matrix

![Confusion Matrix](confusion_matrix.png)


## Normalized Confusion Matrix

![Normalized Confusion Matrix](confusion_matrix_normalized.png)


## ROC Curve

![ROC Curve](roc_curve.png)


## Precision Recall Curve

![Precision Recall Curve](precision_recall_curve.png)



[<< Go back](../README.md)
