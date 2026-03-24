# House Prices EDA 🏠

**Dataset:** [Kaggle House Prices](https://www.kaggle.com/c/house-prices-advanced-regression-techniques)
**Notebook:** [house_prices_eda.ipynb](house_prices_eda.ipynb)
**Study Week:** Week 5 — SVMs, Trees & Regression

## What I Did
- Identified 19 features with missing values; analysed missingness vs SalePrice
- Separated numerical features into temporal, discrete, and continuous
- Applied log transformation to linearise continuous feature relationships
- Detected outliers via boxplots post log-transform
- Analysed 43 categorical features and their cardinality

## Key Findings
- `OverallQual` is the strongest predictor — nearly linear with SalePrice
- Missing values are informative (MNAR) — missingness flag is a useful feature
- Most continuous features are right-skewed — log transform required
- Temporal features should be converted to elapsed time, not used raw
- Many categoricals are ordinal — label encode, don't one-hot encode

## Next Steps
- [ ] Feature Engineering notebook
- [ ] Ordinal encoding for quality/condition features
- [ ] Remove GrLivArea outliers
