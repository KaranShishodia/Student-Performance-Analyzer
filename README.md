# Student-Performance-Analyzer
ChatGPT said: A machine learning project that analyzes student academic data and predicts pass/fail outcomes using logistic regression. Includes data visualization with Seaborn and Matplotlib, and uses Pandas, NumPy, and Scikit-learn for analysis and modeling.

#  Student Performance Analyzer & Predictor

 **Author**: Karan  
 **Goal**: Analyze student academic data and predict pass/fail outcomes using machine learning.

---

##  Project Overview

This project analyzes student academic data to understand key factors affecting performance and predicts whether a student will pass using machine learning. It combines data preprocessing, visualization, and modeling — all built with Python.

---

##  Project Structure

Student-Performance-Analyzer/
├── data/
│ └── students.csv # <- Place dataset here
├── Student_Performance_Analyzer_Karan.ipynb
├── student_performance_analyzer.py
├── requirements.txt
├── README.md
└── .gitignore


---

##  Components

### 1. **Dataset**
- Source: [UCI ML Repo](https://archive.ics.uci.edu/ml/machine-learning-databases/00320/student.zip)
- File: `student-mat.csv` (renamed to `students.csv`)
- Contains fields like study time, past grades, absences, failures, etc.

### 2. **Libraries Used**
- `pandas`: Data handling
- `numpy`: Numeric operations
- `matplotlib`, `seaborn`: Visualization
- `scikit-learn`: Machine learning and evaluation

### 3. **Data Preprocessing**
- Converts `G3` (final grade) to binary pass/fail (`1` if G3 ≥ 10, else `0`)
- Selects useful features: `studytime`, `failures`, `absences`, `G1`, `G2`
- Normalizes features using `StandardScaler`

### 4. **Exploratory Data Analysis (EDA)**
- Pass/fail distribution plot
- Correlation heatmap
- Identifies most impactful features

### 5. **Model Building**
- Algorithm: Logistic Regression
- Train/test split (80/20)
- Trains on academic features

### 6. **Evaluation**
- Accuracy score
- Classification report (precision, recall, F1-score)

### 7. **Custom Prediction**
- Tests a manual student profile:
  - Example: `[studytime=2, failures=1, absences=3, G1=11, G2=12]`
- Predicts pass/fail output

---


## OUTCOME-

You get a clean, reproducible ML pipeline that:

Visualizes student performance trends

Builds and evaluates a logistic regression classifier

Predicts student success using academic records

Can be extended with more features or models

