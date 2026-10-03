# Practical-Statistics-for-Data-Scientist-Books

> **Tugas 1: Enrichment for Machine Learning and Deep Learning Classes**  
> **Code Reproduction + Theoretical Deep-Dive from Practical Statistics for Data Scientists (O'Reilly)**  
> 
> **Informasi Mahasiswa:**  
> - **Nama:** SatrioArjuna Putra  
> - **NIM:** 101032330178  
> - **Kelas:** TK-47-05  
> - **Repository:** [SatrioArjunaPutra/Practical-Statistics-for-Data-Scientist-Books](https://github.com/SatrioArjunaPutra/Practical-Statistics-for-Data-Scientist-Books)  

<p align="center">
  <a href="https://www.amazon.com/Practical-Statistics-Data-Scientists-Essential/dp/149207294X">
    <img alt="Practical Statistics for Data Scientists Cover" src="./cover.jpeg" width="220" style="border-radius: 8px; box-shadow: 0 4px 12px rgba(0,0,0,0.15);">
  </a>
</p>

---

## 📖 Executive Summary & Overview

This repository contains an end-to-end, rigorous Python code reproduction and structured theoretical deep-dive based on the book:
**"Practical Statistics for Data Scientists: 50+ Essential Concepts Using R and Python"** (Peter Bruce, Andrew Bruce, and Peter Gedeck — O'Reilly).

Each notebook is designed with a high-standard pedagogical framework:
1. **Interactive Cloud Execution:** Every notebook features an **Open in Colab** badge for zero-friction 1-click execution.
2. **Robust Multi-Environment Data Loading:** Data loaders automatically check local directories first and fallback dynamically to the official raw repository URLs.
3. **Structured Theoretical Foundations:** Comprehensive mathematical definitions, formulas, statistical intuitions, and practical implications for Machine Learning / Deep Learning.
4. **Complete Code Reproduction:** Exact reproduction of the book's experiments, tables, figures, algorithms, and diagnostic visualizations.
5. **Output Interpretation:** Deep analytical explanations of numeric coefficients, statistical tests, model metrics, and plots.
6. **Cross-Chapter Synthesis:** Direct connections linking classical statistics to modern AI algorithms (e.g., OLS to Neural Network loss surfaces, Logistic Regression to Cross-Entropy, PCA to Latent Representations).

---

## 🚀 Interactive Notebooks & Table of Contents

| Chapter | Title | Primary Focus & Statistical Algorithms | Interactive Colab Badge |
| :---: | :--- | :--- | :---: |
| **01** | **Exploratory Data Analysis** | Location (Mean, Median, MAD), Variability, Boxplots, Hexbin, Correlation Matrix | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/SatrioArjunaPutra/Practical-Statistics-for-Data-Scientist-Books/blob/main/PracticalStatisticsChapter1.ipynb) |
| **02** | **Data and Sampling Distributions** | Central Limit Theorem (CLT), Bootstrap Confidence Intervals, Normal, QQ-Plot, Poisson, Weibull | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/SatrioArjunaPutra/Practical-Statistics-for-Data-Scientist-Books/blob/main/PracticalStatisticsChapter2.ipynb) |
| **03** | **Statistical Experiments & Testing** | A/B Testing, Resampling & Permutation Tests, p-Values, ANOVA (F-statistic), Chi-Square | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/SatrioArjunaPutra/Practical-Statistics-for-Data-Scientist-Books/blob/main/PracticalStatisticsChapter3.ipynb) |
| **04** | **Regression and Prediction** | OLS Simple/Multiple Regression, Residual Diagnostics, Stepwise AIC/BIC, Factor Dummies, Splines & GAM | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/SatrioArjunaPutra/Practical-Statistics-for-Data-Scientist-Books/blob/main/PracticalStatisticsChapter4.ipynb) |
| **05** | **Classification** | Naive Bayes, Linear Discriminant Analysis (LDA), Logistic Regression (Logit/Odds), Confusion Matrix, ROC-AUC, SMOTE | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/SatrioArjunaPutra/Practical-Statistics-for-Data-Scientist-Books/blob/main/PracticalStatisticsChapter5.ipynb) |
| **06** | **Statistical Machine Learning** | K-Nearest Neighbors (KNN), Decision Trees & Impurity (Gini/Entropy), Random Forests (OOB), XGBoost Regularization | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/SatrioArjunaPutra/Practical-Statistics-for-Data-Scientist-Books/blob/main/PracticalStatisticsChapter6.ipynb) |
| **07** | **Unsupervised Learning** | Principal Component Analysis (PCA & Scree plot), Correspondence Analysis, K-Means, Hierarchical Clustering (Dendrograms), GMM | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/SatrioArjunaPutra/Practical-Statistics-for-Data-Scientist-Books/blob/main/PracticalStatisticsChapter7.ipynb) |

---

## 📂 Repository File Structure

```
Practical-Statistics-for-Data-Scientist-Books/
│
├── PracticalStatisticsChapter1.ipynb    # Chapter 1: Exploratory Data Analysis
├── PracticalStatisticsChapter2.ipynb    # Chapter 2: Data and Sampling Distributions
├── PracticalStatisticsChapter3.ipynb    # Chapter 3: Statistical Experiments & Significance Testing
├── PracticalStatisticsChapter4.ipynb    # Chapter 4: Regression and Prediction
├── PracticalStatisticsChapter5.ipynb    # Chapter 5: Classification
├── PracticalStatisticsChapter6.ipynb    # Chapter 6: Statistical Machine Learning
├── PracticalStatisticsChapter7.ipynb    # Chapter 7: Unsupervised Learning
│
├── cover.jpeg                           # Official book cover image
├── _config.yml                          # GitHub Pages Jekyll theme configuration
├── requirements.txt                     # Complete project dependencies
└── README.md                            # Comprehensive project documentation
```

---

## 📘 Comprehensive Chapter-by-Chapter Summaries

### Chapter 1: Exploratory Data Analysis (EDA)
Exploratory Data Analysis, pioneered by John Tukey, forms the empirical foundation of data science. EDA emphasizes looking beyond summary numbers to uncover underlying distributions, anomalies, and multivariate structures.
* **Estimates of Location:** Comparison of arithmetic mean, trimmed mean (which dampens extreme outliers), weighted mean (adjusting for sample sizes), and median (the 50th percentile robust metric).
* **Estimates of Variability:** Quantifying dispersion via variance, standard deviation, interquartile range ($IQR = Q_3 - Q_1$), and median absolute deviation from the median ($MAD$).
* **Distribution Exploration:** Visualizing single features using percentiles, Tukey boxplots (highlighting outliers $> 1.5 \times IQR$), histograms, and kernel density estimation (KDE).
* **Binary & Categorical Data:** Frequency analysis, mode, bar plots, and proportions.
* **Multivariate Relationships:** Quantifying linear association using Pearson's correlation coefficient, and addressing overplotting through hexagonal binning (hexbin), contour density plots, violin plots, and correlation heatmaps.

### Chapter 2: Data and Sampling Distributions
In data science, we rarely possess the entire census population; instead, we infer population traits from finite samples.
* **Sampling Bias & Random Sampling:** Distinguishing between data quality and data quantity. Big data is not immune to selection bias if the sampling mechanism is systematic.
* **Sampling Distribution of a Statistic:** The critical distinction between the distribution of individual data points and the distribution of a sample statistic (e.g., the distribution of sample means).
* **Central Limit Theorem (CLT):** Demonstrates that the sampling distribution of the mean approaches normality as sample size $n$ increases, even when the underlying population distribution is heavily skewed.
* **The Bootstrap:** A non-parametric resampling technique that samples with replacement from the observed dataset to generate empirical confidence intervals without assuming a theoretical distribution.
* **Standard Probability Distributions:** Normal (Gaussian), Student's $t$ (for heavier tails and small sample sizes), Binomial (Bernoulli trials), Poisson (event rates in fixed intervals), and Weibull (reliability/survival modeling).

### Chapter 3: Statistical Experiments and Significance Testing
This chapter establishes the scientific framework for decision-making and hypothesis testing.
* **A/B Testing:** Controlled experimental design with randomized assignment into control and treatment variants to establish causal inference.
* **Hypothesis Testing & Permutation Tests:** Formulation of the Null Hypothesis ($H_0$) and Alternative Hypothesis ($H_a$). Permutation/randomization tests reshuffle observed data to calculate exact empirical p-values without normality assumptions.
* **p-Values & Significance:** The true meaning of a p-value: the probability of observing an effect at least as extreme as the sample data, assuming $H_0$ is true. Reporting effect sizes alongside significance to distinguish practical significance from statistical significance.
* **Type I & Type II Errors:** Alpha ($\alpha$, false positive) vs. Beta ($\beta$, false negative), and experimental statistical power ($1 - \beta$).
* **Multi-Arm Experiments & ANOVA:** Analysis of Variance using the $F$-statistic to compare variances across three or more treatment groups while controlling the family-wise error rate.
* **Chi-Square Test:** Testing independence between categorical variables and goodness-of-fit against expected counts.

### Chapter 4: Regression and Prediction
Linear regression is the cornerstone of statistical modeling and supervised learning.
* **Simple & Multiple Linear Regression:** Ordinary Least Squares (OLS) optimization minimizing the Sum of Squared Residuals ($SSE = \sum (y_i - \hat{y}_i)^2$). Interpreting coefficients as partial effects holding all other predictors constant.
* **Model Assessment & Diagnostics:** Root Mean Squared Error ($RMSE$), Coefficient of Determination ($R^2$), and residual analysis for homoscedasticity, normality, and absence of autocorrelation.
* **Factor Variables & Encoding:** Dummy encoding (one-hot encoding) and the necessity of dropping the reference category (`drop_first=True`) to avoid the dummy variable trap (perfect multicollinearity).
* **Model Selection Criteria:** Stepwise selection penalizing model complexity using Akaike Information Criterion ($AIC = 2k - 2\ln(L)$) and Bayesian Information Criterion ($BIC = k\ln(n) - 2\ln(L)$).
* **Non-Linear Relationships:** Polynomial regression, basis splines (B-splines), and Generalized Additive Models (GAM) modeling flexible non-linear curves without overfitting.

### Chapter 5: Classification
Supervised classification focuses on assigning records into discrete categories.
* **Naive Bayes:** Probabilistic classification based on Bayes' Theorem ($P(Y|X) \propto P(Y) \prod P(X_i|Y)$) under the strong (naive) assumption of feature conditional independence.
* **Linear Discriminant Analysis (LDA):** Modeling class-conditional feature distributions as multivariate normals with equal covariance matrices to maximize between-class variance relative to within-class variance.
* **Logistic Regression & Generalized Linear Models (GLM):** Modeling the log-odds (logit transformation $\ln(p / (1-p)) = X\beta$) through the sigmoid function, allowing direct probabilistic interpretation.
* **Model Evaluation:** Moving beyond raw accuracy on imbalanced datasets by analyzing the Confusion Matrix, Precision, Recall/Sensitivity, Specificity, and the Area Under the ROC Curve ($AUC$).
* **Strategies for Imbalanced Data:** Cost-sensitive learning, class weighting, undersampling majority classes, and synthetic data generation via SMOTE (Synthetic Minority Over-sampling Technique).

### Chapter 6: Statistical Machine Learning
Bridging statistical models with modern non-parametric algorithms and regularization.
* **K-Nearest Neighbors (KNN):** Distance-based non-parametric classifier. Highlights the critical requirement of feature standardization (Z-scores) and demonstrates using KNN as a feature engineering score (`borrower_score`).
* **Decision Trees (CART):** Recursive binary partitioning optimizing node purity using Gini Impurity ($1 - \sum p_i^2$) and Information Entropy ($-\sum p_i \log_2 p_i$).
* **Ensemble Learning — Bagging & Random Forests:** Bootstrap aggregation across randomized subsets of features, evaluating generalization error using Out-of-Bag (OOB) accuracy, and calculating Gini and Permutation feature importances.
* **Boosting & Regularization (XGBoost):** Sequential residual learning with shrinkage (learning rate), tree depth constraints, and early stopping to prevent severe overfitting.
* **Hyperparameter Tuning & Cross-Validation:** Systematic $K$-fold cross-validation exploring hyperparameters to ensure true out-of-sample generalization.

### Chapter 7: Unsupervised Learning
Extracting latent structure, clusters, and dimensionality reductions without ground truth labels.
* **Principal Component Analysis (PCA):** Orthogonal linear transformation mapping high-dimensional correlated features to uncorrelated principal components maximizing variance. Scree plots and cumulative variance curves guide component selection.
* **Correspondence Analysis (CA):** Biplot visualization of associations between categorical variables in contingency tables.
* **K-Means Clustering:** Partitioning data into $K$ spherical clusters minimizing within-cluster sum of squares (inertia), with $K$ determined via the Elbow Method.
* **Hierarchical Clustering:** Bottom-up agglomerative clustering visualized via Dendrograms, comparing Complete, Average, Single, and Ward linkage methods.
* **Model-Based Clustering (Gaussian Mixture Models - GMM):** Soft probabilistic cluster assignments fitting mixtures of multivariate Gaussians, selecting optimal component counts via BIC.
* **Data Scale Sensitivity:** Demonstrating how unscaled variables and binary dummy encoding can distort distance calculations and cluster assignments.

---

## 🛠️ Prerequisites & Installation

To run these notebooks locally, set up a Python 3.9+ environment and install the required dependencies:

```bash
# Clone this repository
git clone https://github.com/SatrioArjunaPutra/Practical-Statistics-for-Data-Scientist-Books.git
cd Practical-Statistics-for-Data-Scientist-Books

# Create and activate virtual environment (optional but recommended)
python -m venv venv
# On Windows:
venv\Scripts\activate
# On Linux/macOS:
source venv/bin/activate

# Install required packages
pip install -r requirements.txt
```

To launch the Jupyter Notebook interface locally:
```bash
jupyter notebook
```

---

## 📦 Key Dependencies

All required libraries are detailed in [`requirements.txt`](./requirements.txt):
* **Core & Numerical:** `numpy`, `pandas`, `scipy`
* **Machine Learning & Modeling:** `scikit-learn`, `statsmodels`, `xgboost`, `pygam`, `dmba`, `prince`, `imblearn`
* **Data Visualization:** `matplotlib`, `seaborn`, `adjustText`
* **Statistics Extensions:** `wquantiles`, `pydotplus`

---

## 📑 References

* **Primary Reference Book:**  
  Bruce, P., Bruce, A., & Gedeck, P. (2020). *Practical Statistics for Data Scientists: 50+ Essential Concepts Using R and Python* (2nd ed.). O'Reilly Media. ISBN: 978-1492072942.

---

## 👤 Informasi Mahasiswa / Author Information

* **Nama:** SatrioArjuna Putra
* **NIM:** 101032330178
* **Kelas:** TK-47-05
* **Mata Kuliah:** Tugas 1: Enrichment for Machine Learning and Deep Learning Classes
* **GitHub:** [@SatrioArjunaPutra](https://github.com/SatrioArjunaPutra)
