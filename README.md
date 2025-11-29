# 🚢 Titanic Survival Prediction using KNN

A complete beginner-friendly machine learning project to predict whether a passenger survived the Titanic disaster using the **K-Nearest Neighbors (KNN)** algorithm.

This project is part of my data science learning journey.

---

# 📘 Project Overview

This project uses the Kaggle Titanic dataset to:

* Clean and preprocess data
* Create new features
* Encode categorical variables
* Scale numerical values
* Tune KNN (k = 1 to 20)
* Train the final model
* Generate a prediction file for Kaggle

The complete implementation is inside the Jupyter Notebook: **titanic.ipynb**.

---

# 📂 Project Files

```
├── titanic.ipynb          # Notebook with all code
├── submission.csv         # Final predictions for Kaggle
└── README.md              # Project documentation
```

---

# 🎯 Objective

To build a machine learning model that predicts the survival of Titanic passengers using simple, clean preprocessing steps and the KNN algorithm.

Dataset: **Kaggle Titanic Competition**.

---

# 🧹 Data Preprocessing

### ✔ Handle Missing Values

* `Age`: filled using median
* `Fare`: filled using median
* `Embarked`: filled using mode

### ✔ New Feature

* `HasCabin` → 1 if cabin present, 0 if missing

### ✔ Encoding

Applied **One-Hot Encoding** to:

* `Sex`
* `Embarked`

### ✔ Scaling

Used **StandardScaler** to normalize numerical features.

---

# 🧾 Features Used in the Model

* `Pclass`
* `Age`
* `SibSp`
* `Parch`
* `Fare`
* `HasCabin`
* `Sex_male`
* `Embarked_Q`
* `Embarked_S`

---

# 🤖 Machine Learning Model – KNN

KNN works by comparing the distance between passengers in the dataset.

### 🔧 Model Tuning

Tried **k from 1 to 20** and selected the value with the best validation accuracy.

### 📌 Final Model Parameter

```
n_neighbors = 15
```

*(Your value may differ based on tuning)*

---

# 📄 Kaggle Submission

The notebook generates a file:

```
submission.csv
```

Upload this to Kaggle → Submit Predictions.

---

# 🛠 How to Run This Project

### **1️⃣ Download the dataset from Kaggle**

Get `train.csv` and `test.csv`.

### **2️⃣ Open the notebook**

Use Jupyter Notebook or VS Code.

```
jupyter notebook titanic_knn.ipynb
```

### **3️⃣ Install required libraries**

```
pip install pandas numpy scikit-learn
```

### **4️⃣ Run all cells**

Click **Run All**.

### **5️⃣ Get submission file**

After running, the notebook creates **submission.csv**.

---

# 📈 Results

* Completed full preprocessing pipeline
* Built and tuned a KNN model
* Generated valid Kaggle predictions
* Typical leaderboard score: **0.64 – 0.70**

---

# 🚀 Future Improvements

* Try Logistic Regression / Random Forest / XGBoost
* Add cross-validation
* Perform GridSearchCV tuning
* Add data visualization

---

# 📬 Contact

Feel free to connect with me on LinkedIn!

If you found this project useful, ⭐ star the repo!
