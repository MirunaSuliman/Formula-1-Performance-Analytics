# Formula 1 Performance Analytics Through Predictive Modeling and Data Mining

A machine learning project developed in **Python** that analyzes Formula 1 telemetry data to identify driving styles through unsupervised learning and predict race performance using behavior-aware predictive models.

This project was developed as my **Master's Dissertation** for the Master's Degree in **Software Development and Business Information Systems** at **Alexandru Ioan Cuza University of Iași**.

---

## Project Overview

Modern Formula 1 cars generate millions of telemetry data points during every race weekend, providing detailed information about driver behavior and vehicle performance.

This project investigates whether drivers exhibit distinct driving styles based on qualifying telemetry and whether these behavioral patterns improve the prediction of race performance.

The complete analytical workflow includes:

- Telemetry data extraction
- Data cleaning and preprocessing
- Missing value reconstruction
- Feature engineering
- Dimensionality reduction
- Behavioral clustering
- Predictive modeling
- Model evaluation and interpretation

---

## Research Methodology

### Hypothesis H₁ – Behavioral Clustering

**H₁:** *Formula 1 drivers exhibit distinct driving styles that can be identified from qualifying telemetry.*

Telemetry variables—including average throttle, brake usage, and speed—were standardized and reduced using **Principal Component Analysis (PCA)** before applying **K-Means clustering**.

The resulting clusters were validated through **Hierarchical Clustering**, revealing three consistent driving styles:

- Aggressive
- Balanced
- Cautious

These behavioral groups demonstrate that meaningful driving styles can be extracted directly from telemetry data.

---

### Hypothesis H₂ – Predictive Modeling

**H₂:** *Driving style influences the relationship between telemetry-derived performance characteristics and race outcomes.*

Each behavioral cluster was modeled independently using **Random Forest classifiers** to predict whether a driver would finish in a points-scoring position.

Race-level features include:

- Average Pace
- Pace Consistency
- Peak Pace
- Sector Balance

The resulting models demonstrate that different driving styles rely on different predictive features, supporting a behavior-aware framework for Formula 1 performance analytics.

---

## Machine Learning Pipeline

The analytical workflow follows these stages:

```
Telemetry Extraction
        ↓
Data Cleaning & Validation
        ↓
Missing Value Reconstruction
        ↓
Feature Engineering
        ↓
Principal Component Analysis (PCA)
        ↓
Behavioral Clustering (K-Means)
        ↓
Hierarchical Validation
        ↓
Race-Level Dataset Construction
        ↓
Random Forest Classification
        ↓
Model Evaluation
```

Additional comparative experiments using **Support Vector Machines (SVM)** and **XGBoost** were also performed to evaluate the robustness of the predictive framework.

---

## Technologies

### Languages

- Python

### Libraries

- Pandas
- NumPy
- Scikit-learn
- FastF1
- Matplotlib
- Seaborn

### Machine Learning

- Principal Component Analysis (PCA)
- K-Means Clustering
- Hierarchical Clustering
- Random Forest
- Support Vector Machines (SVM)
- XGBoost

### Concepts

- Machine Learning
- Predictive Analytics
- Data Mining
- Feature Engineering
- Data Cleaning
- Data Visualization
- Model Evaluation

---

## Repository Structure

```
data/
    Raw telemetry dataset

scripts/
    01_data_extraction.py
    02_data_cleaning.py
    03_exclude_anomalies.py
    04_driver_clustering.py
    05_prepare_race_data.py
    06_random_forest_by_style.py

output/
    Clustering results
    Model outputs
    Figures
    Evaluation metrics

docs/
    Master's Dissertation.pdf
```

---

## Key Contributions

- Developed an end-to-end telemetry analytics pipeline using Formula 1 telemetry.
- Identified distinct driver behavioral profiles through unsupervised learning.
- Built behavior-aware predictive models using Random Forest classifiers.
- Compared multiple machine learning algorithms across behavioral groups.
- Demonstrated that driving style influences the predictive importance of race performance features.

---

## Documentation

The complete Master's Dissertation is available in:

`docs/Dissertation Paper.docx`

---

## Learning Outcomes

This project provided practical experience in:

- Machine Learning
- Predictive Analytics
- Data Mining
- Feature Engineering
- Data Cleaning
- Unsupervised Learning
- Supervised Learning
- Model Evaluation
- Data Visualization
- Research Methodology

---

## Future Improvements

Potential future enhancements include:

- Deep Learning approaches
- Explainable AI techniques (SHAP)
- Real-time telemetry analysis
- Race strategy prediction
- Interactive performance dashboards
- Additional telemetry features
- Time-series forecasting models

---

## Author

**Miruna Suliman**

Master's Degree in Software Development and Business Information Systems

Alexandru Ioan Cuza University of Iași

- GitHub: https://github.com/MirunaSuliman
- LinkedIn: https://www.linkedin.com/in/miruna-suliman/
