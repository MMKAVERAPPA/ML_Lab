# K-Fold Cross-Validation with Random Forest Regressor

## Dataset
- **Wine Quality (White) dataset** from UCI repository
- Predicting wine **quality score** from chemical properties
- Dataset size: 4898 samples, 11 features

## Approach
- Use **5-Fold Cross-Validation** to evaluate model performance
- Model: **Random Forest Regressor** (100 trees)
- Pipeline steps:
  - Impute missing values with median
  - Scale features (StandardScaler)
  - Train Random Forest

## Results
| Fold | MAE (Mean Absolute Error) |
|-------|-------------------------|
| 1     | 0.419                   |
| 2     | 0.405                   |
| 3     | 0.433                   |
| 4     | 0.436                   |
| 5     | 0.456                   |

- **Mean MAE:** 0.430  
- **Standard Deviation:** 0.017

## Interpretation
- On average, predictions are off by about **0.43 quality points**.
- Low standard deviation shows consistent performance across folds.
- K-Fold CV helps estimate model generalization reliably.

---

*Note:* Lower MAE means better performance. This setup is useful for regression tasks where accuracy metrics don’t apply.

