# ML Interview Prep 🤖

A structured 14-week self-study repository for **Machine Learning Engineer** and **Prompt Engineer** roles.
Covers EDA, feature engineering, ML algorithms, SQL, LeetCode, and LLM/prompt engineering — built alongside Stanford XCS299 (April–August 2026).

---

## 📁 Repository Structure

```
ml-interview-prep/
│
├── eda/                          # Exploratory Data Analysis
│   ├── titanic/
│   │   ├── Exploratory_Data_Analysis.ipynb
│   │   └── README.md
│   ├── house-prices/
│   ├── telco-churn/
│   ├── mall-segmentation/
│   ├── instacart/
│   └── credit-card-fraud/
│
├── feature-engineering/          # Feature engineering experiments per dataset
│   ├── titanic_features.ipynb
│   └── ...
│
├── ml-algorithms/                # Algorithm implementations from scratch
│   ├── logistic_regression.ipynb
│   ├── decision_tree.ipynb
│   └── ...
│
├── sql/                          # SQL practice queries
│   └── practice_queries.sql
│
├── ml-system-design/             # System design case study notes
│   ├── recommendation_system.md
│   └── fraud_detection.md
│
├── prompt-engineering/           # LLM + PE track projects
│   ├── cli-chatbot/
│   ├── rag-chatbot/
│   └── ...
│
└── README.md                     # This file
```

---

## 📊 EDA Progress

| Dataset | Topic | Notebook | Status |
|---|---|---|---|
| Titanic | Missing data, classification baseline | [notebook](eda/titanic/Exploratory_Data_Analysis.ipynb) | ✅ Done |
| House Prices | Regression, skew, multicollinearity | coming soon | 🔜 Week 5 |
| Telco Churn | Imbalanced classes | coming soon | 🔜 Week 6 |
| Mall Segmentation | Clustering | coming soon | 🔜 Week 7 |
| Instacart Market Basket | Recommendation FE | coming soon | 🔜 Week 8 |
| Credit Card Fraud | Fraud detection FE | coming soon | 🔜 Week 9 |

---

## 🗺️ Study Roadmap

| Phase | Weeks | Focus |
|---|---|---|
| Phase 1 | 1–4 | Probability (CS109), ML Basics, Linear Algebra |
| Phase 2 | 5–9 | Stanford XCS299, Algorithms, SQL, LeetCode, EDA |
| Phase 3 | 10–14 | Deep Learning, System Design, Mock Interviews, Capstone |

---

## 🧪 Titanic — Key Findings

> Full analysis: [eda/titanic/Exploratory_Data_Analysis.ipynb](eda/titanic/Exploratory_Data_Analysis.ipynb)

- **38% survival rate** — imbalanced target; accuracy alone is a misleading metric
- **Sex is the strongest predictor** — female survival ~74% vs male ~19%
- **Pclass strongly correlated with survival** — 1st class had ~3x survival rate of 3rd class
- **Age had ~20% missing values** — imputed using class-specific medians (Class 1: 37, Class 2: 29, Class 3: 24)
- **Cabin dropped** — 77% missing, not worth imputing
- **Logistic Regression baseline accuracy: ~80%** on 30% holdout

---

## 🛠️ Tools & Stack

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Pandas](https://img.shields.io/badge/Pandas-2.0-lightblue)
![Sklearn](https://img.shields.io/badge/Scikit--Learn-1.3-orange)
![Seaborn](https://img.shields.io/badge/Seaborn-0.13-teal)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-yellow)

- **EDA & Feature Engineering:** Pandas, NumPy, Seaborn, Matplotlib
- **Modelling:** Scikit-Learn, XGBoost
- **LLM / PE Track:** OpenAI API, Anthropic API, LangChain, ChromaDB
- **SQL Practice:** StrataScratch, SQLZoo
- **LeetCode:** NeetCode 150

---

## 📈 Overall Progress

- [x] Week 1 — CS109 Probability Basics + ML Foundations
- [x] Week 2 — Expectation, MLE/MAP, Naive Bayes
- [x] Week 3 — Model Evaluation, Regularisation
- [x] Week 4 — Feature Engineering Pipelines + Titanic EDA ← *current*
- [ ] Week 5 — SVMs, Decision Trees, SQL begins
- [ ] Week 6 — Ensembles, LeetCode begins
- [ ] Week 7 — Clustering
- [ ] Week 8 — ML System Design I
- [ ] Week 9 — ML System Design II
- [ ] Week 10 — Neural Networks
- [ ] Week 11 — Practical Deep Learning
- [ ] Week 12 — Mock Interviews
- [ ] Week 13 — Capstone Project
- [ ] Week 14 — Final Review

---

## 📬 Connect

If you're on a similar prep journey, feel free to open an issue or reach out!
