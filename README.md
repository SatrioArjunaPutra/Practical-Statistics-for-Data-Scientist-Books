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
│
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
- **IQR and MAD** are robust measures of spread (less sensitive to outliers than std dev)
- Visualisations reveal patterns (skewness, outliers, modes) that summary statistics hide
- **Correlation ≠ Causation** — always visualise before interpreting relationships

---

### Chapter 2 — Data and Sampling Distributions

This chapter covers the **theory of sampling** and **probability distributions** — fundamental to understanding statistical inference.

| Topic | Key Concepts |
|-------|-------------|
| **Random Sampling** | Population vs sample, sampling bias |
| **Sampling Distribution** | Distribution of a statistic across many samples |
| **Central Limit Theorem** | Sample means → Normal as n → ∞ |
| **Bootstrap** | Resampling with replacement to estimate uncertainty |
| **Confidence Intervals** | Range of plausible values for a parameter |
| **Normal Distribution** | Bell curve, z-scores, 68-95-99.7 rule |
| **Long-Tailed Distributions** | Heavy tails, power laws |
| **t-Distribution** | For small samples or unknown σ |
| **Binomial/Poisson** | Count distributions |

**Key Insights:**
- **CLT:** Sample means are approximately normal for large n — regardless of population shape
- **Bootstrap** works for *any* statistic without distributional assumptions
- **Confidence Intervals** quantify uncertainty — wider CI = more uncertainty
- Real-world data (income, web traffic) often follows **heavy-tailed distributions**

---

### Chapter 3 — Statistical Experiments and Significance Testing

This chapter covers **hypothesis testing** — the formal statistical framework for drawing conclusions from data.

| Topic | Key Concepts |
|-------|-------------|
| **A/B Testing** | Comparing two treatments; the gold standard for causal inference |
| **Hypothesis Tests** | Null/alternative hypothesis, Type I/II errors |
| **Permutation Tests** | Resampling-based; no distributional assumptions |
| **p-values** | Evidence against H₀ — NOT probability H₀ is true |
| **t-tests** | Comparing means between groups |
| **Multiple Testing** | Bonferroni correction, False Discovery Rate |
| **ANOVA** | Comparing means across 3+ groups (F-statistic) |
| **Chi-Square Test** | Independence of categorical variables |

**Key Insights:**
- **Randomisation** in A/B tests ensures groups are comparable (causal inference)
- **p < 0.05 ≠ practically important** — always report effect sizes
- **Multiple testing** inflates false positives — always correct (Bonferroni or FDR)
- **ANOVA** tells you *if* any group differs; use post-hoc tests to find *which* ones

---

### Chapter 4 — Regression and Prediction

This chapter covers **regression modelling** — the workhorse of predictive analytics.

| Topic | Key Concepts |
|-------|-------------|
| **Simple Linear Regression** | OLS; β₁ = slope; minimise SSE |
| **Multiple Linear Regression** | Multiple predictors; partial effects |
| **Model Assessment** | R², Adjusted R², RMSE, residual analysis |
| **Factor Variables** | One-hot encoding; dummy variable trap |
| **Multicollinearity** | VIF; unstable coefficients |
| **Polynomial Regression** | Non-linear relationships with polynomial features |
| **Interaction Terms** | When effect of X₁ depends on X₂ |
| **Model Selection** | AIC/BIC; stepwise selection |

**Key Insights:**
- In multiple regression, each β = **partial effect** (controlling for all other variables)
- **R² alone is insufficient** — always inspect residual plots to validate assumptions
- **Multicollinearity** (high VIF) makes coefficients unstable — check with VIF
- Use **AIC/BIC** to balance model fit and complexity (prevent overfitting)

---

## 🔧 Requirements

```bash
pip install numpy pandas scipy scikit-learn statsmodels matplotlib seaborn wquantiles
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
   pip install numpy pandas scipy scikit-learn statsmodels matplotlib seaborn wquantiles
   ```

3. **Open any notebook in Jupyter:**
   ```bash
   jupyter notebook Chapter1_Exploratory_Data_Analysis.ipynb
   ```

> ⚠️ **Note:** All datasets are loaded automatically from the official book repository. An internet connection is required.

---

## 📚 Reference

- **Book:** [Practical Statistics for Data Scientists, 2nd Edition](https://www.oreilly.com/library/view/practical-statistics-for/9781492072935/) — Peter Bruce, Andrew Bruce & Peter Gedeck
- **Official Code Repository:** [github.com/gedeck/practical-statistics-for-data-scientists](https://github.com/gedeck/practical-statistics-for-data-scientists)
- **Example Submission:** [github.com/farrelrassya/Practical-Statistics-for-Data-Scientist-Books](https://github.com/farrelrassya/Practical-Statistics-for-Data-Scientist-Books)

---

## ⚖️ Academic Integrity

All code in this repository is original work based on the referenced book. Theoretical explanations are written by the author and may use LLM assistance as permitted by the assignment guidelines. All work adheres to academic integrity standards.
