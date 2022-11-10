# Summary of 4_Default_Xgboost

[<< Go back](../README.md)


## Extreme Gradient Boosting (Xgboost)
- **n_jobs**: -1
- **objective**: multi:softprob
- **eta**: 0.075
- **max_depth**: 6
- **min_child_weight**: 1
- **subsample**: 1.0
- **colsample_bytree**: 1.0
- **eval_metric**: mlogloss
- **num_class**: 6
- **explain_level**: 2

## Validation
 - **validation_type**: split
 - **train_ratio**: 0.75
 - **shuffle**: True
 - **stratify**: True

## Optimized metric
logloss

## Training time

39.6 seconds

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

## Permutation-based Importance
![Permutation-based Importance](permutation_importance.png)
## Confusion Matrix

![Confusion Matrix](confusion_matrix.png)


## Normalized Confusion Matrix

![Normalized Confusion Matrix](confusion_matrix_normalized.png)


## ROC Curve

![ROC Curve](roc_curve.png)


## Precision Recall Curve

![Precision Recall Curve](precision_recall_curve.png)



## SHAP Importance
![SHAP Importance](shap_importance.png)

## SHAP Dependence plots

### Dependence 2 yr Undergrad (Fold 1)
![SHAP Dependence from fold 1](learner_fold_0_shap_dependence_class_2 yr Undergrad.png)
### Dependence 4 yr Undergrad (Fold 1)
![SHAP Dependence from fold 1](learner_fold_0_shap_dependence_class_4 yr Undergrad.png)
### Dependence 5 yr Undergrad (Fold 1)
![SHAP Dependence from fold 1](learner_fold_0_shap_dependence_class_5 yr Undergrad.png)
### Dependence Grad (Fold 1)
![SHAP Dependence from fold 1](learner_fold_0_shap_dependence_class_Grad.png)
### Dependence STAP (Fold 1)
![SHAP Dependence from fold 1](learner_fold_0_shap_dependence_class_STAP.png)
### Dependence Unknown (Fold 1)
![SHAP Dependence from fold 1](learner_fold_0_shap_dependence_class_Unknown.png)

## SHAP Decision plots

### Worst decisions for selected sample 1 (Fold 1)
![SHAP worst decisions from Fold 1](learner_fold_0_sample_0_worst_decisions.png)
### Worst decisions for selected sample 2 (Fold 1)
![SHAP worst decisions from Fold 1](learner_fold_0_sample_1_worst_decisions.png)
### Worst decisions for selected sample 3 (Fold 1)
![SHAP worst decisions from Fold 1](learner_fold_0_sample_2_worst_decisions.png)
### Worst decisions for selected sample 4 (Fold 1)
![SHAP worst decisions from Fold 1](learner_fold_0_sample_3_worst_decisions.png)
### Best decisions for selected sample 1 (Fold 1)
![SHAP best decisions from Fold 1](learner_fold_0_sample_0_best_decisions.png)
### Best decisions for selected sample 2 (Fold 1)
![SHAP best decisions from Fold 1](learner_fold_0_sample_1_best_decisions.png)
### Best decisions for selected sample 3 (Fold 1)
![SHAP best decisions from Fold 1](learner_fold_0_sample_2_best_decisions.png)
### Best decisions for selected sample 4 (Fold 1)
![SHAP best decisions from Fold 1](learner_fold_0_sample_3_best_decisions.png)

[<< Go back](../README.md)
