
## Trader Behavior & Market Sentiment Analysis

### Overview

This project analyzes the relationship between market sentiment and trader behavior to understand drivers of short-term profitability. The analysis integrates behavioral metrics, sentiment classification, predictive modeling, and clustering to extract actionable insights.

---

### Methodology

**1. Data Preparation**

* Standardized and cleaned raw trading data
* Converted timestamps and aggregated at the account-date level
* Merged trading activity with sentiment classification
* Engineered behavioral features (trade size, trade frequency, loss ratio)

**2. Exploratory Analysis**

* Examined profitability distribution across sentiment regimes
* Evaluated behavioral changes under fear and greed conditions
* Identified structural differences in trading intensity

**3. Predictive Modeling**

* Built a Random Forest classifier to predict next-day profitability
* Incorporated behavioral and sentiment features
* Achieved 63% classification accuracy
* Conducted feature importance analysis

**4. Trader Segmentation**

* Applied K-Means clustering to identify behavioral archetypes
* Segmented traders based on profitability, exposure, and risk behavior

---

### Key Findings

* Trade size and trading frequency are the strongest predictors of next-day profitability.
* Market sentiment contributes incremental predictive value but is secondary to behavioral factors.
* Traders can be grouped into three primary segments:

  * Active consistent traders
  * Conservative low-exposure traders
  * High-risk, high-reward traders

---

### Business Implications

* Risk management systems should prioritize monitoring position sizing and trading intensity.
* Behavioral profiling provides stronger predictive signals than sentiment classification alone.
* Trader segmentation can support personalized risk controls and performance monitoring.

---

### How to Run

```bash
pip install pandas numpy scikit-learn matplotlib joblib
```

Run:

```
analysis.ipynb
```

Model file:

```
profitability_model.pkl
```

---
