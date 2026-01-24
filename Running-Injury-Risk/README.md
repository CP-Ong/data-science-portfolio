# 🏃 Early Warning Modelling for Running Injury Risk Using Wearable Data

## 📌 Business Problem
Running-related injuries are common and often preventable, but most interventions happen **after** an injury occurs. With the widespread adoption of wearable devices, runners generate daily training data that can potentially be used to detect **early warning signs of injury risk**.

The challenge is to identify periods of elevated injury risk **before injuries happen**, while minimizing false alerts that could negatively impact user experience and training adherence.

---

## 🎯 Project Objective
The objective of this project is to develop an **early-warning injury risk model** using wearable training data that:
- Identifies high-risk periods ahead of injury events
- Produces interpretable risk scores rather than black-box predictions
- Balances the trade-off between false positives and false negatives
- Could realistically be integrated into a consumer fitness or sports analytics product

---

## 📊 Dataset
**Injury Prediction for Competitive Runners**  
Source: Kaggle  
https://www.kaggle.com/datasets/shashwatwork/injury-prediction-for-competitive-runners

The dataset contains time-ordered training records for competitive runners, including daily training metrics and injury labels.

---

## 🧠 Approach Overview
This project is structured to mirror a real-world data science workflow, from problem framing to model interpretation.

---

## 1️⃣ Exploratory Data Analysis (EDA)
**Goal:** Understand injury patterns, training behavior, and data quality.

Planned analyses:
- Injury frequency and class imbalance assessment
- Distribution and trends of key training metrics
- Comparison of training patterns before injury vs non-injury periods
- Missing data and outlier analysis

---

## 2️⃣ Feature Engineering
**Goal:** Transform raw daily metrics into meaningful signals that capture training load and fatigue.

Planned features:
- Rolling averages and cumulative training load metrics
- Acute vs chronic workload ratios
- Recovery-related indicators (rest days, sudden load spikes)
- Lagged features to preserve temporal causality

These features are designed to reflect **sports science principles**, not just model convenience.

---

## 3️⃣ Modeling Strategy
**Goal:** Predict elevated injury risk while respecting time dependencies.

Planned models:
- Logistic Regression as an interpretable baseline
- Tree-based models (Random Forest, Gradient Boosting) for nonlinear relationships
- Time-aware train/validation splits to prevent data leakage

Class imbalance will be explicitly addressed during model training and evaluation.

---

## 4️⃣ Model Evaluation
**Goal:** Evaluate models using metrics aligned with real-world impact.

Planned evaluation:
- Precision, recall, and F1-score
- Recall-focused analysis to minimize missed injury risks
- Threshold analysis to explore false-positive vs false-negative tradeoffs
- Comparison of model performance across runners

---

## 5️⃣ Explainability & Risk Scoring
**Goal:** Translate model outputs into actionable insights.

Planned outputs:
- Injury risk scores over time per runner
- Feature importance and explainability analysis (e.g. SHAP)
- Identification of key drivers contributing to elevated injury risk

This step ensures the model is **interpretable and product-ready**.

---

## 6️⃣ Visualization & Product Perspective
**Goal:** Demonstrate how insights could be consumed by end users.

Planned deliverables:
- Time-series plots of injury risk trends
- Examples of early-warning alerts before injury events
- Conceptual dashboards for runners or coaches

---

## 🚀 Future Enhancements
- Survival analysis / time-to-injury modeling
- Personalized risk models per runner
- Integration of additional wearable signals (e.g. HRV)
- Real-time risk scoring simulation

---

## ⭐ Why This Project Matters
This project goes beyond injury prediction to demonstrate:
- Time-series feature engineering
- Imbalanced classification handling
- Explainable machine learning
- Product-aware decision-making

It is intentionally designed to reflect how data science is applied in **consumer tech, health, and fitness products**.

---

