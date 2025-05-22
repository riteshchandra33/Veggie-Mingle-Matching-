# Veggie-Mingle-Matching
This project aims to build a machine learning model that predicts customer churn in the credit card industry. Using historical customer data, it identifies key features contributing to account cancellations, helping businesses improve customer retention strategies.

## 📘 Overview

**Veggie Mingle** is a health-focused dating platform designed for users with dietary preferences like vegetarian, vegan, and pescatarian. This analysis aims to understand the factors that contribute to successful matches and build predictive models using demographic, behavioral, and lifestyle attributes of users.

This final case assignment explores:
- Exploratory Data Analysis (EDA)
- Correlation mapping
- Principal Component Analysis (PCA)
- Model building using Logistic Regression, KNN, and Decision Trees
- Strategic recommendations based on insights

---

## 📦 Dataset Summary

- Total Records: 5,000 users
- Columns: 33 variables
- Types: Demographics, dietary habits, lifestyle, behavioral interaction, system usage, and match status

Key Features:
- `diet_type`, `cooking_skill`, `online_activity`, `profile_completeness`, `matched`, `response_rate`, `music_taste`, etc.

---

## 🧪 Techniques & Tools

- **Language**: R
- **Libraries**: `tidyverse`, `ggplot2`, `caret`, `rpart`, `factoextra`, `corrplot`, `GGally`
- **Models**: PCA, Logistic Regression, KNN, Decision Tree
- **EDA**: Correlation heatmaps, boxplots, bar plots

---

## 📊 Key Insights from EDA

- **Activity & Engagement**: Features like `online_activity` and `response_rate` have stronger relationships with the match outcome.
- **Profile Completeness**: Marginal effect; incentivizing full profiles can help improve matching algorithms.
- **Diet & Cooking**: `diet_type` and `cooking_skill` are moderately influential and useful for niche segmentation.
- **Visualization**: 
  - Match Distribution by demographic & lifestyle factors
  - Correlation heatmaps of numeric variables
  - Boxplots comparing match outcomes for key variables

---

## 🔍 PCA & Modeling Summary

### PCA
- Retained top 2 components (PC1 & PC2) explaining 80%+ variance
- Key influencers: Cooking Skill, Age, Online Activity

### Models Evaluated

| Model              | Accuracy | Sensitivity | Specificity | Notes |
|-------------------|----------|-------------|-------------|-------|
| Logistic Regression | 65%     | 100%        | 0%          | Predicts “No” matches well |
| KNN (k=5)           | 60%     | 85.6%       | 12.8%       | Slightly better at capturing variability |
| Decision Tree       | 65%     | 100%        | 0%          | Overfits to majority class |

---

## ✅ Strategic Recommendations

- **Enhance Matching Algorithm**: Prioritize features like `cooking_skill`, `age`, and `online_activity`.
- **Interaction Effects**: Model pairings that consider interaction between variables (e.g., `age × cooking skill`).
- **Behavioral Nudges**: Notifications for low-engagement users to increase visibility.
- **Community Features**: Introduce recipe or interest groups around shared food preferences.
- **Model Selection**: Adopt ensemble learning methods (e.g., Random Forest) in future versions for better generalization.

---

## 🗂 Folder Structure

```
project-root/
│
├── Veggiemingle.csv                   # Raw data
├── Veggie_mingle_matching.docx        # Final report
├── Veggie_mindgle_matching.docx       # Code/analysis walkthrough
├── README.md                          # Project summary & documentation
```

---

## 🙋‍♂️ Author

**Ritesh Somashekar**  

## 🔗 References

- R packages: `caret`, `rpart`, `factoextra`, `GGally`
- Data simulated for academic purposes

