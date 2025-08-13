# ❤️ Heart Disease Prediction

This project uses **Logistic Regression** to predict the likelihood of heart disease based on patient health data.

---

## 🎯 Objective
The objective of this project is to build and evaluate a **Logistic Regression** model to predict heart disease using clinical and demographic health indicators.

---

## 📂 Dataset
- **File:** `heart.csv`
- **Description:** Contains multiple patient health indicators along with a target variable (`target`) indicating the presence (1) or absence (0) of heart disease.

**Key Features:**
- `ChestPainType` (e.g., NAP, ATA, TA, ASY)  
- `ST_Slope` (e.g., Up, Flat, Down)  
- `Sex` (M/F)  
- `ExerciseAngina` (Y/N)  
- Various medical measurements (e.g., cholesterol, blood pressure)

---

## 🤖 Models Applied
- **Base Model:** Logistic Regression (`sklearn.linear_model.LogisticRegression`)
- **Enhanced Model:** Logistic Regression with **interaction terms** between the top 5 most important features.

**Top 5 Most Influential Features:**
1. `ChestPainType_NAP`  
2. `ChestPainType_ATA`  
3. `ST_Slope_Flat`  
4. `Sex_M`  
5. `ExerciseAngina_Y`

---

## 📊 Key Results & Findings

| Model | Accuracy | AUC  |
|-------|----------|------|
| Logistic Regression (Base) | 85% | 0.92 |
| Logistic Regression (Enhanced with interactions) | 86% | 0.93 |

**Insights:**
- Both models perform well in predicting **positive** and **negative** cases of heart disease.
- Adding interaction terms between the top 5 features slightly improved performance.
- Confusion matrices confirmed balanced performance across classes.

---

## 📈 Visualizations
- **Confusion Matrix:** Model performance comparison  
- **ROC Curve:** AUC measurement and classification threshold visualization  
- **Feature Importance:** Identifying the most influential predictors

---

## 🛠️ Technologies Used
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- scikit-learn  

---

## 📜 License
This project is open-source and available under the [MIT License](LICENSE).
