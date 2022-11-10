# Summary of 6_Default_RandomForest

[<< Go back](../README.md)


## Random Forest
- **n_jobs**: -1
- **criterion**: gini
- **max_features**: 0.9
- **min_samples_split**: 30
- **max_depth**: 4
- **eval_metric_name**: logloss
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

17.5 seconds

### Metric details
|           |   2 yr Undergrad |   4 yr Undergrad |   5 yr Undergrad |       Grad |   STAP |   Unknown |   accuracy |   macro avg |   weighted avg |   logloss |
|:----------|-----------------:|-----------------:|-----------------:|-----------:|-------:|----------:|-----------:|------------:|---------------:|----------:|
| precision |         0.754829 |         0.870036 |         0.652397 |   0.996429 |      0 |         0 |   0.789096 |    0.545615 |       0.801755 |  0.527478 |
| recall    |         0.824675 |         0.651351 |         0.858108 |   1        |      0 |         0 |   0.789096 |    0.555689 |       0.789096 |  0.527478 |
| f1-score  |         0.788208 |         0.744977 |         0.741245 |   0.998211 |      0 |         0 |   0.789096 |    0.54544  |       0.786434 |  0.527478 |
| support   |       616        |       740        |       444        | 279        |      7 |         5 |   0.789096 | 2091        |    2091        |  0.527478 |


## Confusion matrix
|                           |   Predicted as 2 yr Undergrad |   Predicted as 4 yr Undergrad |   Predicted as 5 yr Undergrad |   Predicted as Grad |   Predicted as STAP |   Predicted as Unknown |
|:--------------------------|------------------------------:|------------------------------:|------------------------------:|--------------------:|--------------------:|-----------------------:|
| Labeled as 2 yr Undergrad |                           508 |                            19 |                            89 |                   0 |                   0 |                      0 |
| Labeled as 4 yr Undergrad |                           150 |                           482 |                           107 |                   1 |                   0 |                      0 |
| Labeled as 5 yr Undergrad |                            15 |                            48 |                           381 |                   0 |                   0 |                      0 |
| Labeled as Grad           |                             0 |                             0 |                             0 |                 279 |                   0 |                      0 |
| Labeled as STAP           |                             0 |                             0 |                             7 |                   0 |                   0 |                      0 |
| Labeled as Unknown        |                             0 |                             5 |                             0 |                   0 |                   0 |                      0 |

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
