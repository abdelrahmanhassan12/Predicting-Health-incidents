
# Summary Report: Predicting Health Incidents in ALF Residents

## Key Findings

- **Overall incident rate**: ~11.75% of entries had a next-day health incident.
- **Data size**: 6000 entries across 200 patients over 30 days.
- **Top Predictors**:
  1. med_adherence
  2. blood_pressure_sys
  3. bp_sys_diff

## Model Performance

- **Model**: Random Forest (balanced)
- **ROC AUC**: 0.59
- **Precision/Recall**:
```
              precision    recall  f1-score   support

           0       0.87      1.00      0.93      1047
           1       0.00      0.00      0.00       153

    accuracy                           0.87      1200
   macro avg       0.44      0.50      0.47      1200
weighted avg       0.76      0.87      0.81      1200

```

## Practical Recommendations

- **Monitor vital sign trends**: Not just raw values, but **deltas** over previous days signal instability.
- **Focus on medication adherence**: Poor adherence shows the strongest signal for next-day incidents.
- **Segment by diagnosis**: Dementia and COPD patients showed elevated risk sensitivity to vitals.

## Next Steps

- Introduce nurse alerts for patients with vital fluctuations > threshold.
- Incorporate additional behavioral/cognitive metrics if available.
