# Breast Cancer Classification for Healthcare Diagnostics

## 📌 Project Overview
Medical professionals routinely evaluate cell nucleus measurements to determine if a tumor is malignant or benign. This project implements a machine learning solution to automate this diagnostic screening process, predicting whether a tumor sample is **Malignant (M)** or **Benign (B)** based on clinical details available from cell biopsies. Flagging high-risk tumors early helps optimize treatment timelines and can ultimately save lives.

**Developed by:** D. Jaswanth
**Dataset Source:** YBI Foundation (Cancer.csv)

---

## 📊 Dataset Specifications
The clinical dataset consists of evaluation records across 31 attributes:
* **Total Instances:** 569 tumor samples
* **Target Distribution:**
  * **Benign (B):** 357 instances
  * **Malignant (M):** 212 instances
* **Primary Key Features Evaluated:** `radius_mean`, `texture_mean`, `perimeter_mean`, `area_mean`, `smoothness_mean`, `compactness_mean`, `concavity_mean`, `concave points_mean`, `symmetry_mean`, `fractal_dimension_mean`.

---

## 🛠️ Tech Stack & Architecture
* **Environment:** Python 3 within cloud-hosted Jupyter Notebooks (Google Colab)
* **Data Pipelines & Manipulation:** Pandas, NumPy
* **Exploratory Data Graphics:** Seaborn, Matplotlib
* **Machine Learning Classifiers:** Scikit-Learn
  * Parametric Model: `LogisticRegression`
  * Ensemble Model: `RandomForestClassifier`
  * Feature Scaling: `StandardScaler`
  * Optimization Frameworks: `train_test_split`, `cross_val_score`, `GridSearchCV`

---

## 🔬 Exploratory Data Analysis (EDA) Summary
Comprehensive exploratory pipelines were constructed to visualize core data dynamics and structural qualities:
1. **Target Class Imbalance Analysis:** Combined countplots and exploded pie charts to observe the precise proportion of malignant versus benign cases.
2. **Feature Stratification Profiles:** Comparative boxplots breaking down mean cell radius and mean cell area metrics across diagnostic boundaries.
3. **Distribution Contours:** Frequency distribution histograms tracing the standard variations of critical clinical indicators.
4. **Multicollinearity Matrices:** Correlation heatmaps tracking inter-feature linear dependencies across top-level clinical measurements.
5. **High-Dimensional Pairwise Interaction:** Multivariable pairplot matrices (`sns.pairplot`) tracking feature patterns colored by target diagnosis to assess clear boundary segregations.
