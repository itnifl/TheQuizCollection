# TDT4259 Applied Data Science

[← All courses](../readme.md)

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://en.wikipedia.org/wiki/Python_(programming_language))
[![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)](https://en.wikipedia.org/wiki/Scikit-learn)
[![CRISP-DM](https://img.shields.io/badge/CRISP--DM-2E7D32?style=for-the-badge&logoColor=white)](https://en.wikipedia.org/wiki/Cross-industry_standard_process_for_data_mining)
[![PCA](https://img.shields.io/badge/PCA-EF6C00?style=for-the-badge&logoColor=white)](https://en.wikipedia.org/wiki/Principal_component_analysis)

**Content:**
- The lifecycle of a data science project (CRISP-DM phases: business understanding, data understanding, preparation, modelling, evaluation, deployment, monitoring)
- Types of data analytics: descriptive, diagnostic, predictive, prescriptive
- Data sources, quality issues, preparation and feature engineering
- Business problem framing, value creation and data-driven decision-making
- Documentation practices: one-pagers and design documents (why–what–how)
- Tools and techniques for data collection, exploration, modelling and visualisation
- Group projects: solving real-world problems with open or provided datasets
- Individual assignments: design documents for proposed data-driven solutions
- Ethics and responsible data science (privacy, bias, fairness, societal impact)

**Learning outcomes:**
- **Knowledge:** the phases of CRISP-DM; the main types of data analytics and when to apply them; principles of data preparation, quality assessment and monitoring; ethical issues in applied data science
- **Skills:** frame business problems as data science tasks; collect, prepare and analyse data; evaluate models against business objectives; document and communicate solutions through one-pagers, design documents and visualisations
- **General competence:** apply data science methods to create value for organisations; work effectively in teams on real-world projects; reflect critically on the ethical and societal impact of data-driven decisions

## Quizzes

### Part 3 – Lifecycle of a data science project

*Based on Lecture 3: the CRISP-DM methodology, types of data analytics, one-pagers and design documents, business understanding, data understanding, data preparation, the Aneo grid-loss case study, and monitoring and maintenance.*

**Quiz:** [Applied Data Science – Part 3](https://dev-quizmachine.itautomasjon.no/Quiz/Take/applieddatascience3)

| Topic | Details |
|---|---|
| **CRISP-DM framework**                           | Business understanding → Data understanding → Data preparation → Modeling → Evaluation → Deployment → Monitoring |
| **Business understanding**                       | Clarify goals, scope, value, problem definition; often refine or reduce scope                |
| **Data understanding**                           | Collect, describe, explore, verify data quality; domain insights; detect anomalies/outliers  |
| **Data preparation**                             | Select, clean, construct, integrate, and format data for modeling                            |
| **Modeling**                                     | Apply statistical/ML methods; compare baselines; validate with metrics                      |
| **Evaluation**                                   | Check model results against business objectives; visualize insights                         |
| **Deployment**                                   | Translate results into actionable recommendations; plan implementation                      |
| **Monitoring & maintenance**                     | Track KPIs, retrain models, set alarms, dashboards, ensure business + technical health       |
| **Types of analytics**                           | Descriptive (what happened), Diagnostic (why), Predictive (what might happen), Prescriptive (what should we do) |
| **One-pagers**                                   | Summarize intent, desired outcome, deliverable, constraints                                 |
| **Design documents**                             | Capture Why, What, How (+ risks, infra, monitoring, cost); expensive but cheap → avoid waste |
| **Case study: Aneo grid loss**                   | Grid loss = produced – consumed electricity; data issues: missing/delayed values, small sets |
| **Assignment (Group)**                           | Solve a business problem with data; report + 5-min presentation                             |
| **Assignment (Individual)**                      | One-pager + ~10 page design doc; different dataset/company than group project               |

[↑ Back to top](#tdt4259-applied-data-science)

### Part 4 – Data, features and algorithms

*Based on Lecture 4: variables vs features, feature engineering, missing-value and low-variance filters, scaling and normalisation, PCA, supervised vs unsupervised learning, core algorithms (k-NN, SVM, trees, Naïve Bayes, neural nets), evaluation metrics and a leakage-free pipeline.*

**Quiz:** [Applied Data Science – Part 4](https://dev-quizmachine.itautomasjon.no/Quiz/Take/applieddatascience4)

| Topic | Details |
|---|---|
| **Variables → Features**                         | Variables = raw columns; **features = model-ready signals** (transformed/engineered variables). |
| **Feature engineering examples**                  | `age` → buckets, z-score; `price` → `log1p(price)`; `signup_datetime` → hour/day/recency; text → TF-IDF / embeddings; image → CNN embedding |
| **Missing Values Ratio**                         | Fraction of nulls in a column. Use it to decide drop vs impute; common thresholds: <10% simple impute, 10–30% smarter impute or flag, >30–50% drop or require justification |
| **Low-variance filter**                          | Remove near-constant features (e.g., same value >95–99% rows). Scale-sensitive — check predictive power before dropping. |
| **Scaling / Normalization**                      | Required for distance/dot-product/variance methods (kNN, SVM, PCA, many NN optimizers). Use StandardScaler by default; MinMax/Robust/MaxAbs depending on context. Always fit scalers inside CV pipeline. |
| **PCA (Principal Component Analysis)**           | Linear dimensionality reduction: center (and usually scale) → compute covariance or SVD → keep top components by explained variance (e.g., 80–95%). Good for correlated numeric features; linear and less interpretable. |
| **Supervised vs Unsupervised**                   | Supervised = X + y (classification/regression). Unsupervised = X only (clustering, PCA). |
| **Core algorithms — short**                      | **Nearest Centroid**: mean of each class; simple baseline. **k-NN**: local, distance-based; scale required. **Decision Trees**: greedy splits by impurity (Gini/entropy); no scaling required. **Random Forests / Ensembles**: robust, strong baselines. **Naïve Bayes**: generative, assumes conditional independence (great for text). **SVM**: max-margin; kernel trick for nonlinear boundaries; scale mandatory. **Neural Nets**: neurons = weighted sum + activation; deep nets learn hierarchical features; need data + tuning. |
| **Evaluation (regression)**                      | **MAE** (mean absolute error) — robust; **RMSE** — penalizes large errors more. |
| **Evaluation (classification)**                  | **Confusion matrix** (TP/FP/FN/TN). **Precision** = TP/(TP+FP). **Recall** = TP/(TP+FN). **Accuracy** = (TP+TN)/total (can mislead on imbalance). Use ROC/PR curves and choose thresholds per business needs. |
| **Likelihood vs Probability**                    | Probability: parameters fixed → probability of data (e.g., P(x \| θ)). Likelihood: data fixed → how plausible parameters are given data (used for fitting models). |
| **Practical pipeline (safe defaults)**           | 1) Train/val/test split or K-fold CV. 2) Build pipeline: impute → encode → scale → (optional PCA/feature selection) → model. 3) Tune hyperparameters inside CV. 4) Final evaluation on untouched test set. |
| **Feature/leakage warning**                       | Never compute scalers/encoders/statistics on full dataset before CV—this leaks info. Create "missing" indicator flags when missingness may be informative. |
| **When to prefer which method**                   | Text/sparse: Naïve Bayes, Linear models. Mixed types/interpretability: Trees/RandomForest. Smooth numeric boundaries: SVM. Complex high-D patterns (images/audio): Deep nets. k-NN for quick, small datasets / nonparametric baseline. |

[↑ Back to top](#tdt4259-applied-data-science)
