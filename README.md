# 🚢 Titanic - Machine Learning from Disaster

This repository contains a full data science pipeline to predict passenger survival on the Titanic using machine learning. The project was developed as part of a personal learning journey and follows the standard approach used in Kaggle competitions.

---

## 📌 Problem Statement

The sinking of the Titanic is one of the most infamous shipwrecks in history. The goal of this project is to build a predictive model that answers the question:  
> **“What sorts of people were more likely to survive?”**

Using passenger data (name, age, gender, class, etc.), we predict whether a passenger survived.

---

## 🧰 Tools & Libraries

- Python
- Pandas
- NumPy
- Matplotlib & Seaborn
- Scikit-learn

---

## 📊 Project Workflow

### 1. Data Exploration
- Checked data types and null values using `.info()` and `.isnull().sum()`.
- Visualized distributions and relationships with `pairplot`, `boxplot`, etc.

### 2. Data Cleaning & Preprocessing
- Handled missing values in:
  - `Age` (filled with median)
  - `Embarked` (filled with mode or unknown)
  - `Cabin` (filled and encoded)
  - `Fare` (filled with median in test set)
- Removed or capped outliers using IQR method.

### 3. Feature Engineering
- Created missing value indicators (e.g., `Cabin_missing`, `Age_missing`).
- Encoded categorical features like `Sex`, `Embarked`, and `Cabin` using:
  - `LabelEncoder`
  - `OrdinalEncoder`

### 4. Model Building
- Split data into `train` and `test` using `train_test_split`.
- Trained a classifier model (e.g., XGBClassifier / Random Forest).
- Evaluated using:
  - Accuracy
  - Classification Report

### 5. Final Prediction
- Applied the same preprocessing on the test set.
- Predicted survival status.
- Generated a `submission.csv` ready for Kaggle upload.

---

## ✅ Results

- Full pipeline completed: preprocessing, training, evaluation, and Kaggle-ready submission.
- Achieved accurate and reproducible results.
- Notebook designed for modular updates and improvements (e.g., feature engineering, model tuning).

---

## 📂 Files Included

- `Titanic.ipynb` — Main Jupyter Notebook with code and results.
- `submission.csv` — Final prediction file for Kaggle submission.
- `README.md` — Project overview and documentation.

---

## 🏁 Future Work

- Improve model with feature engineering (e.g., extract titles from names, family size).
- Try ensemble models like XGBoost or LightGBM.
- Perform hyperparameter tuning using `GridSearchCV`.
- Add cross-validation for better generalization.

---

## 💡 Inspiration

Based on the classic Kaggle Titanic dataset challenge. A great beginner-friendly project to practice:
- EDA
- Feature engineering
- Model building
- Data storytelling

---

## 🤝 Contributions

This project was completed as a solo learning initiative by **[Your Name]**. Suggestions and pull requests are welcome!

---

## 📎 License

This project is open-source and available under the MIT License.
