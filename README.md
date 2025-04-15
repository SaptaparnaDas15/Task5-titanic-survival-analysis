# 🧠 Titanic Survival Analysis - Kaggle Dataset

This project performs a complete **Exploratory Data Analysis (EDA)** and builds a **Logistic Regression model** to predict passenger survival from the Titanic dataset.

## 📂 Dataset
- Source: [Kaggle Titanic Competition](https://www.kaggle.com/competitions/titanic/data)
- Files used: `train.csv`, `test.csv`

---

## 🔧 Tools & Libraries
- Python
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn (for model building)

---

## 📊 Project Workflow

### 1. **Data Exploration**
- Viewing dataset structure using `.info()`, `.describe()`
- Identifying null values
- Analyzing features like `Sex`, `Pclass`, `Age`, and `Fare`

### 2. **Data Cleaning**
- Filled missing `Age` with median
- Filled missing `Embarked` with mode
- Dropped the `Cabin` column due to excessive missing values

### 3. **Feature Engineering**
- Converted `Sex` into numeric (0 = male, 1 = female)
- One-hot encoded `Embarked` column

### 4. **Visualizations**
- Count plots for survival by sex and class
- Age distribution histograms
- Correlation heatmap to identify key relationships

### 5. **Model Building**
- Used `LogisticRegression` from scikit-learn
- Features used: `Pclass`, `Sex`, `Age`, `SibSp`, `Parch`, `Fare`, `Embarked_Q`, `Embarked_S`
- Evaluated using:
  - Accuracy score
  - Confusion matrix
  - Classification report

---

## ✅ Results
- Achieved predictive performance with a basic model
- Key findings:
  - Women had higher survival rates
  - Passengers in higher classes had better chances
  - Age and fare influenced survival probability

---

## 📁 Files Included
- `titanic_analysis.ipynb`: Complete analysis notebook
- `titanic_analysis.pdf`: Exported version of notebook
- `train.csv`: Training dataset (from Kaggle)

---

## 💬 How to Run
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
jupyter notebook titanic_analysis.ipynb
