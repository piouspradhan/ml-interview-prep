# Titanic EDA 🚢

**Dataset:** [Kaggle Titanic](https://www.kaggle.com/c/titanic)
**Notebook:** [eda.ipynb](eda.ipynb)
**Study Week:** Week 4 — Feature Engineering & Pipelines

---

## What I Did

- Explored survival rates by Sex, Pclass, Age, Fare, and SibSp
- Visualised missing data using a Seaborn heatmap
- Imputed missing Age values using class-specific medians
- Dropped Cabin (77% missing)
- Encoded categorical features (Sex, Embarked) using `pd.get_dummies`
- Trained a Logistic Regression baseline model

## Key Findings

| Finding | Detail |
|---|---|
| Survival rate | ~38% — imbalanced dataset |
| Strongest predictor | Sex — female survival 74% vs male 19% |
| Class effect | 1st class survival ~3x higher than 3rd class |
| Missing Age | ~20% missing — imputed by Pclass median |
| Missing Cabin | ~77% missing — dropped |
| Baseline accuracy | ~80% with Logistic Regression |

## Baseline Model

```python
from sklearn.linear_model import LogisticRegression
from sklearn.metrics import accuracy_score

logModel = LogisticRegression()
logModel.fit(X_train, y_train)
predictions = logModel.predict(X_test)
accuracy_score(y_test, predictions)  # ~0.80
```

## Next Steps

- [ ] Extract `Title` from Name before dropping it (Mr, Mrs, Miss, Master)
- [ ] Engineer `FamilySize = SibSp + Parch + 1`
- [ ] Add `classification_report` — precision/recall breakdown per class
- [ ] Try Random Forest and compare accuracy
- [ ] Log-transform `Fare` to handle right skew
