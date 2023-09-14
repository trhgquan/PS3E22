# PS3E22 - Predict Health Outcomes of Horses
[PS3E22 - Predict Health Outcomes of Horses](https://www.kaggle.com/competitions/playground-series-s3e22)

**Your Goal:** Given various medical indicators, predict the health outcomes of horses.

**Evaluation:** Submissions are evaluated on micro-averaged F1-Score between predicted and actual values.


This project is licensed under [The GNU GPL v3.0](LICENSE)

## Important features

```python
[
    "surgery",
    "age",
    "respiratory_rate",
    "peripheral_pulse",
    "peristalsis",
    "abdominal_distention",
    "rectal_exam_feces",
    "abdomen",
    "rectal_temp", 
    "mucous_membrane", 
    "pain", 
    "nasogastric_tube", 
    "nasogastric_reflux", 
    "nasogastric_reflux_ph", 
    "abdomo_protein", 
    "total_protein",
    "lesion_1",	
    "lesion_2",	
    "lesion_3",	
    "cp_data"
]
```

## Baselines
| Rank/Overall | Model                                     | Features                                                            | Public Score | Private Score |
| ------------ | ----------------------------------------- | ------------------------------------------------------------------- | ------------ | ------------- |
| 126/221      | `sklearn.ensemble.RandomForestClassifier` | All except `id` and `hospital_number`                               | 0.77439      | TBD           |
| 120/226      | `xgboost.XGBClassifier`                   | 20 features mentioned in [#important-features](#important-features) | **0.78048**  | TBD           |