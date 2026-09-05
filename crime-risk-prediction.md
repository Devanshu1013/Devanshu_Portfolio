# Modeling Urban Crime Risk and Arrest Probability Using Spatio-Temporal Machine Learning Techniques

🔗 **Original Repository:** [github.com/Devanshu1013/MODELING-URBAN-CRIME-RISK-AND-ARREST-PROBABILITY-USING-SPATIO-TEMPORAL-MACHINE-LEARNING-TECHNIQUES](https://github.com/Devanshu1013/MODELING-URBAN-CRIME-RISK-AND-ARREST-PROBABILITY-USING-SPATIO-TEMPORAL-MACHINE-LEARNING-TECHNIQUES)

[← Back to portfolio](../README.md)

---

A full-scale research study (my Major Research Project, supervised by **Dr. Xingwei (Nancy) Yang**) that builds a spatio-temporal machine learning framework to predict the probability of arrest for a reported crime, using over two decades of real-world Chicago crime records enriched with socio-economic, weather, and public-transit mobility data — aimed at supporting data-driven public safety decisions.

**Problem & Motivation**
Not every reported crime results in an arrest, and arrest likelihood varies systematically by location, time, crime type, and the surrounding socio-economic context. This project models that variation directly, treating arrest prediction as a spatio-temporal classification problem rather than a simple crime-count forecast.

**Data**
- **Chicago crime data, 2001–2023** — the core dataset of reported incidents, crime types, locations, and arrest outcomes
- **Socio-economic indicators** by community area — income, unemployment, and related quintile-level features
- **Weather data** — temperature, rain/snow, and other daily conditions
- **Mobility / transit data** — public transit ridership trends, joined at the daily and community-area level

**Pipeline**
1. **Literature review** — grounding the approach in prior crime-prediction research
2. **Data preprocessing & integration** — merging crime, socio-economic, weather, and mobility sources into a single spatio-temporal dataset
3. **Exploratory Data Analysis (EDA)** — crime trends by year, month, day of week, and hour; domestic vs. non-domestic breakdowns; top community areas and crime types; correlation analysis between crime, socio-economic, weather, and mobility factors
4. **Feature engineering** — spatio-temporal features capturing location- and time-based patterns
5. **Experiments** — training and tuning 15 models across three sampling strategies (original, oversampled, undersampled) to handle class imbalance
6. **Results & evaluation** — comparing models on accuracy, precision, recall, F1, ROC-AUC, and PR-AUC

**Models benchmarked:** Random Forest, Extra Trees, LightGBM, XGBoost, CatBoost, Gradient Boosting, AdaBoost, Decision Tree, Logistic Regression, Linear SVM, SGD Linear SVM, MLP, LSTM, GRU, and TCN

**Key Result**
Across all sampling strategies, **Random Forest with oversampling** delivered the best overall performance, consistently topping the accuracy and F1-score rankings — ahead of boosting methods (LightGBM, XGBoost, CatBoost) and deep sequence models (LSTM, GRU, TCN).

**Status:** Written up as a formal academic research paper; currently being finalized for publication.

**Tech stack:** `Python` `Scikit-learn` `XGBoost` `LightGBM` `CatBoost` `PyTorch` `Pandas` `Spatio-Temporal Feature Engineering`

![Top 10 Performing Models — Crime Risk Project](../assets/crime-risk-preview.png)

---

[← Back to portfolio](../README.md) &nbsp;|&nbsp; [🔗 View on GitHub](https://github.com/Devanshu1013/MODELING-URBAN-CRIME-RISK-AND-ARREST-PROBABILITY-USING-SPATIO-TEMPORAL-MACHINE-LEARNING-TECHNIQUES)
