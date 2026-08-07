# From Data to Decision: Predicting Student Academic Outcomes Using Artificial Neural Networks

## Overview

This notebook develops and evaluates Artificial Neural Network (ANN) models to predict student academic outcomes (**Dropout**, **Enrolled**, and **Graduate**). The primary objective is to compare prediction using only information available at enrollment with prediction using additional semester-performance data, and to translate the findings into practical recommendations for early student intervention.

---

## Running the Notebook

1. Upload the dataset file **`ann-datatset.csv`** when prompted in the section A.1 Load and Inspect the Dataset.

2. Run all notebook cells sequentially from top to bottom without skipping any cells.

The notebook uses a fixed random seed (`SEED = 42`) together with TensorFlow deterministic operations to improve reproducibility. Minor variations in neural network performance may still occur due to platform-specific execution differences.

---

## Dataset

**File:** `ann-datatset.csv`

- **Records:** 4,424 students
- **Input Features:** 36
- **Target Classes:** Dropout, Enrolled, Graduate

The dataset contains demographic, socioeconomic, academic background, institutional, financial, and semester-performance information.


---

## Notebook Structure

### A. Data Understanding & Preparation
- Dataset inspection and quality checks
- Prediction scenario definition
- Train/validation/test split
- Data preprocessing pipeline

### B. Exploratory Data Analysis
- Class distribution
- Financial standing and student outcomes
- Scholarship status
- Age and gender analysis

### C. Neural Network Modeling
- ANN architecture
- Model training
- Baseline model comparison

### D. Evaluation & Interpretation
- Training behaviour
- Classification performance
- Confusion matrix analysis
- Robustness evaluation
- Permutation feature importance

### E. From Insight to Decision
- Two-stage early-warning advising
- Targeted financial-standing outreach

---

## Setup and Reproducibility

### Library Versions

| Library | Version |
|---------|:-------:|
| Python | Google Colab Runtime |
| NumPy | 2.0.2 |
| Pandas | 2.2.2 |
| Scikit-learn | 1.6.1 |
| TensorFlow | 2.20.0 |
| Matplotlib | 3.10.0 |
| Seaborn | 0.13.2 |

**Standard Libraries:** `os`, `random`, and `warnings` (included with the Python standard library)

**Colab Utility:** `google.colab.files` (built-in Google Colab module)

---

## Conclusion

The study demonstrates that enrollment-time information is sufficient to build a meaningful early-warning model, while semester-performance variables substantially improve predictive performance once students begin their studies. These findings support a practical two-stage intervention framework that combines early identification with more targeted academic and financial support as additional student information becomes available.
