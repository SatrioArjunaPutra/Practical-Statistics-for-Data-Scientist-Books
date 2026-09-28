# Practical-Statistics-for-Data-Scientist-Books

> **Code Reproduction + Theoretical Deep-Dive** from *Practical Statistics for Data Scientists* (O'Reilly)  
> **Author:** Satrio Arjuna Putra  
> **Course:** Enrichment for Machine Learning and Deep Learning Classes — Individual Task

---

## 📖 About This Repository

This repository contains Python notebook reproductions of the code from each chapter of the book:

> **Practical Statistics for Data Scientists** — Peter Bruce, Andrew Bruce & Peter Gedeck (O'Reilly, 2nd Edition)

Each notebook includes:
- ✅ **Reproduced code** from the chapter
- 📚 **Theoretical explanations** of every concept
- 📊 **Visualisations** to aid understanding
- 🔑 **Key takeaways** summarising the chapter

Data is loaded **directly from the official book GitHub repository** — no local files needed.

---

## 📂 Repository Structure

```
Practical-Statistics-for-Data-Scientist-Books/
│
├── Chapter1_Exploratory_Data_Analysis.ipynb
├── Chapter2_Data_and_Sampling_Distributions.ipynb
├── Chapter3_Statistical_Experiments_Significance_Testing.ipynb
├── Chapter4_Regression_and_Prediction.ipynb
├── Chapter5_Classification.ipynb
├── Chapter6_Statistical_Machine_Learning.ipynb
├── Chapter7_Unsupervised_Learning.ipynb
│
├── requirements.txt
└── README.md
```

---

## 📋 Chapter Summaries

### Chapter 1 — Exploratory Data Analysis

**Exploratory Data Analysis (EDA)** is the process of summarising, visualising, and understanding a dataset before formal modelling.

| Topic | Key Concepts |
|-------|-------------|
| **Estimates of Location** | Mean, trimmed mean, weighted mean, median |
| **Estimates of Variability** | Standard deviation, variance, IQR, MAD |
| **Exploring the Distribution** | Percentiles, boxplots, histograms, density plots |
| **Categorical Data** | Mode, bar charts |
| **Exploring Relationships** | Correlation, scatter plots, heat maps, hexbin plots |

**Key Insights:**
- Use the **median** or **trimmed mean** when data has outliers
- **IQR and MAD** are robust measures of spread
- Visualisations reveal patterns that summary statistics hide
- **Correlation ≠ Causation**

---

### Chapter 2 — Data and Sampling Distributions

This chapter covers **sampling** and **probability distributions** — fundamental to statistical inference.

| Topic | Key Concepts |
|-------|-------------|
| **Random Sampling** | Population vs sample, sampling bias |
| **Central Limit Theorem** | Sample means → Normal as n → ∞ |
| **Bootstrap** | Resampling with replacement to estimate uncertainty |
| **Confidence Intervals** | Range of plausible values for a parameter |
| **Normal Distribution** | Bell curve, z-scores, 68-95-99.7 rule |
| **Long-Tailed Distributions** | Heavy tails, power laws |
| **t / Binomial / Poisson** | Small samples, count distributions |

**Key Insights:**
- **CLT:** Sample means are approximately normal for large n — regardless of population shape
- **Bootstrap** works for *any* statistic without distributional assumptions
- Real-world data often follows **heavy-tailed distributions**

---

### Chapter 3 — Statistical Experiments and Significance Testing

This chapter covers the formal statistical framework for drawing conclusions from data.

| Topic | Key Concepts |
|-------|-------------|
| **A/B Testing** | Randomised experiment; gold standard for causal inference |
| **Hypothesis Tests** | Null/alternative hypothesis, Type I/II errors |
| **Permutation Tests** | Resampling-based; no distributional assumptions |
| **p-values** | Evidence against H0 — NOT probability H0 is true |
| **t-tests** | Comparing means between groups |
| **Multiple Testing** | Bonferroni correction, False Discovery Rate |
| **ANOVA** | Comparing means across 3+ groups (F-statistic) |
| **Chi-Square Test** | Independence of categorical variables |

**Key Insights:**
- **p < 0.05 is not practically important** — always report effect sizes
- **Multiple testing** inflates false positives — always correct (Bonferroni or FDR)
- **ANOVA** tells you *if* any group differs; use post-hoc tests to find *which* ones

---

### Chapter 4 — Regression and Prediction

This chapter covers **regression modelling** — the workhorse of predictive analytics.

| Topic | Key Concepts |
|-------|-------------|
| **Simple Linear Regression** | OLS; slope; minimise SSE |
| **Multiple Linear Regression** | Multiple predictors; partial effects |
| **Model Assessment** | R², Adjusted R², RMSE, residual analysis |
| **Factor Variables** | One-hot encoding; dummy variable trap |
| **Multicollinearity** | VIF; unstable coefficients |
| **Polynomial / Interaction** | Non-linear relationships and interaction effects |
| **Model Selection** | AIC/BIC; stepwise selection |

**Key Insights:**
- In multiple regression, each coefficient = **partial effect** (controlling for all other variables)
- **R² alone is insufficient** — always inspect residual plots
- **Multicollinearity** (high VIF) makes coefficients unstable

---

### Chapter 5 — Classification

This chapter introduces supervised learning for **categorical targets**.

| Topic | Key Concepts |
|-------|-------------|
| **Naive Bayes** | Probabilistic; assumes feature independence |
| **Discriminant Analysis (LDA)** | Linear decision boundary; multivariate normal assumption |
| **Logistic Regression** | Models log-odds; sigmoid function |
| **Evaluating Classifiers** | Confusion matrix, Precision, Recall, F1, AUC-ROC |
| **Decision Trees** | Recursive binary partitioning; Gini/Entropy impurity |
| **Random Forests** | Ensemble of trees; OOB score; feature importance |
| **XGBoost (Boosting)** | Sequential ensemble; regularisation; state-of-the-art |

**Key Insights:**
- **Accuracy is misleading** with imbalanced classes — use F1 or AUC
- **Random Forests** are a reliable baseline for tabular classification
- **XGBoost** consistently wins ML competitions — tune `n_estimators` + `learning_rate`

---

### Chapter 6 — Statistical Machine Learning

This chapter bridges classical statistics and modern ML with key cross-cutting methods.

| Topic | Key Concepts |
|-------|-------------|
| **K-Nearest Neighbors (KNN)** | Non-parametric; lazy learning; scale features |
| **Cross-Validation** | Honest model evaluation; k-fold, LOOCV |
| **Bias-Variance Trade-off** | Complexity vs generalisation |
| **Ridge Regression (L2)** | Shrinks all coefficients; no feature selection |
| **Lasso Regression (L1)** | Zero-out irrelevant features; automatic selection |
| **Elastic Net** | Combines Ridge + Lasso; robust to correlated features |
| **Model Interpretability** | Partial Dependence Plots; SHAP values |

**Key Insights:**
- **Never tune hyperparameters on the test set** — use cross-validation
- **Lasso** performs automatic feature selection by zeroing coefficients
- **SHAP values** are the gold standard for model explanation

---

### Chapter 7 — Unsupervised Learning

This chapter covers finding structure in data *without* labeled responses.

| Topic | Key Concepts |
|-------|-------------|
| **PCA** | Dimensionality reduction; explained variance; loadings |
| **K-Means Clustering** | Partition into K clusters; elbow method |
| **Hierarchical Clustering** | Dendrogram; no need to specify K; Ward's linkage |
| **Gaussian Mixture Models** | Soft assignments; flexible shapes; BIC for model selection |
| **Scaling** | Critical for distance-based methods |
| **Categorical Data** | One-hot encoding; Gower's distance |

**Key Insights:**
- **PCA:** Use scree plot to choose number of components (>=80% cumulative variance)
- **K-Means:** Use elbow method; sensitive to scale — always standardise
- **GMM:** Probabilistic soft assignments; use BIC to select K
- **Always scale** numeric features before distance-based clustering

---

## 🔧 Requirements

```bash
pip install numpy pandas scipy scikit-learn statsmodels matplotlib seaborn wquantiles xgboost
```

Or install all at once:
```bash
pip install -r requirements.txt
```

---

## 🚀 How to Run

1. **Clone this repository:**
   ```bash
   git clone https://github.com/SatrioArjunaPutra/Practical-Statistics-for-Data-Scientist-Books.git
   cd Practical-Statistics-for-Data-Scientist-Books
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Open any notebook in Jupyter:**
   ```bash
   jupyter notebook Chapter1_Exploratory_Data_Analysis.ipynb
   ```

> Note: All datasets are loaded automatically from the official book repository. An internet connection is required.

---

## 📚 Reference

- **Book:** Practical Statistics for Data Scientists, 2nd Edition — Peter Bruce, Andrew Bruce & Peter Gedeck (O'Reilly)
- **Official Code Repository:** https://github.com/gedeck/practical-statistics-for-data-scientists
- **Example Submission:** https://github.com/farrelrassya/Practical-Statistics-for-Data-Scientist-Books

---

## Academic Integrity

All code in this repository is original work based on the referenced book. Theoretical explanations are written by the author and may use LLM assistance as permitted by the assignment guidelines. All work adheres to academic integrity standards.
