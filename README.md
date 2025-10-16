# 🍷 Wine Quality Prediction

![Wine Pouring GIF](https://media.tenor.com/PLIr_VkF6ywAAAAM/ghostedvpn-hacker-cat.gif)

Predicting wine quality based on physicochemical properties like **acidity, sugar, sulphates, and alcohol** using Machine Learning models.  

---

## 📊 Dataset Overview

| Feature             | Type   | Description                              |
|--------------------|-------|------------------------------------------|
| Records            | 1,143 | Wine samples                              |
| Columns            | 13    | 11 float + 2 integer                      |
| Target Variable    | quality | Wine quality score (3–8)                 |
| Missing Values     | 0     | Clean dataset                             |

---

## 🧹 Data Preprocessing & EDA

- Checked data structure using `.info()` and `.describe()`.  
- Imbalanced classes (mostly 5 & 6) verified with `train['quality'].value_counts()`.  



---

## ⚙️ Feature Preparation

- **Feature-Target Split:**  
  - `X` → all chemical attributes  
  - `y` → quality labels  
- **Train-Test Split:** 80% / 20% (`random_state=42`)  
- **Scaling:** StandardScaler applied to normalize features  

---

## ⚖️ Handling Class Imbalance

- **SMOTE:** Oversampled minority classes  
- **RandomUnderSampler:** Balanced majority classes  
- Verified using `y_resampled.value_counts(normalize=True)` ✅  

---

## 🧠 Modeling Stage

| Model                 | Accuracy | Badge |
|----------------------|---------|-------|
| Logistic Regression   | 88.60%  | ![LR](https://img.shields.io/badge/Logistic%20Regression-88.6%25-brightgreen) |
| Support Vector        | 88.17%  | ![SVC](https://img.shields.io/badge/SVC-88.2%25-green) |
| GaussianNB            | 77.20%  | ![Gaussian](https://img.shields.io/badge/GaussianNB-77.2%25-yellow) |
| Decision Tree         | 57.63%  | ![DT](https://img.shields.io/badge/Decision%20Tree-57.6%25-orange) |
| Random Forest         | 88.00%  | ![RF](https://img.shields.io/badge/Random%20Forest-88%25-brightgreen) |

**💡 Top Models:** Logistic Regression, SVC, Random Forest  

---

## 🔑 Key Insights

![Wine Insight GIF](https://media.giphy.com/media/3o7abKhOpu0NwenH3O/giphy.gif)

- Higher **alcohol** → higher wine quality 🍷  
- Higher **volatile acidity** → lower quality ⚠️  

---

## 🚀 Conclusion

- Cleaned, scaled, and balanced dataset ✅  
- Visualizations revealed **key factors** affecting wine quality 📊  
- Top models achieved **~88% accuracy** 💯  
- Ready for deployment or further experimentation 💻  

---

## 🛠️ Tech Stack



- Python 3  
- Pandas, NumPy  
- Scikit-learn  
- Seaborn, Matplotlib  
- Imbalanced-learn (SMOTE & UnderSampling)  

---

> Made with ❤️ by **Humna Ghouri**

