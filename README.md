# Student-Exam-Score-Prediction
Predicting student exam scores using machine learning

# 🎓 Student Exam Score Prediction using Machine Learning

## 📌 Project Overview
This project focuses on predicting students’ **exam scores** using academic, behavioral, and socio-economic factors.  
Machine learning regression models are applied to understand key performance drivers and build an accurate predictive system.

---

## 📂 Dataset Description
- **Total records:** 6,607 students  
- **Total features:** 19 input features + 1 target variable  
- **Target variable:** `Exam_Score`

### Feature Types
**Numerical Features**
- Hours_Studied  
- Attendance  
- Sleep_Hours  
- Previous_Scores  
- Tutoring_Sessions  
- Physical_Activity  

**Categorical Features**
- Parental_Involvement  
- Access_to_Resources  
- Extracurricular_Activities  
- Motivation_Level  
- Internet_Access  
- Family_Income  
- Teacher_Quality  
- School_Type  
- Peer_Influence  
- Learning_Disabilities  
- Parental_Education_Level  
- Distance_from_Home  
- Gender  

---

## 🧹 Data Preprocessing
- Handled missing values in categorical columns using **mode imputation**
- Converted categorical variables using **One-Hot Encoding**
- Applied **feature scaling** using StandardScaler for Linear Regression and SVR
- Split the dataset into **80% training** and **20% testing** sets

---

## 🔍 Exploratory Data Analysis (EDA)
- Studied the distribution of exam scores
- Analyzed relationships between academic habits and performance
- Identified important influencing features such as:
  - Previous_Scores
  - Attendance
  - Hours_Studied

---

## 🤖 Machine Learning Models Used

### 1️⃣ Linear Regression
- Used as a **baseline model**
- Helps understand linear relationships between features and exam scores

### 2️⃣ Random Forest Regressor (Final Model)
- Captures complex non-linear patterns
- Robust to noise and feature interactions
- Delivered the **best overall performance**

### 3️⃣ Support Vector Regression (SVR)
- Uses kernel-based learning to model non-linear relationships
- Added for advanced model comparison

---

## 📊 Model Evaluation Metrics

To evaluate regression performance, the following metrics were used:

### 🔹 Mean Absolute Error (MAE)
MAE measures the **average absolute difference** between predicted and actual exam scores.

\[
MAE = \frac{1}{n} \sum |y_{actual} - y_{predicted}|
\]

- Lower MAE indicates better prediction accuracy
- Easy to interpret since it is measured in **exam score units**
- Shows how many marks the model is wrong by on average

**Example:**  
An MAE of 2 means the prediction is off by about **2 marks on average**.

---

### 🔹 R² Score (Coefficient of Determination)
R² score represents how well the model explains the **variation in exam scores**.

\[
R^2 = 1 - \frac{SS_{residual}}{SS_{total}}
\]

- Ranges from **0 to 1**
- Higher values indicate a better fit
- Shows the proportion of variance explained by the model

**Example:**  
An R² score of 0.85 means the model explains **85% of the variability** in exam scores.

---

### 🔹 Why These Metrics Were Chosen
- **MAE** provides a clear measure of prediction error
- **R² Score** helps compare how well different models explain the data
- Together, they give a balanced evaluation of model performance

---

## 🏆 Model Comparison Summary
- Linear Regression served as a baseline
- SVR captured non-linear trends
- **Random Forest achieved the lowest MAE and highest R² score**

✅ **Random Forest Regressor was selected as the final model**

---

## ⭐ Key Insights
- Previous academic performance is the strongest predictor of exam scores
- Attendance and hours studied significantly impact outcomes
- Sleep hours and physical activity have moderate influence
- Socio-economic and parental factors also contribute to student performance

---

## 🛠️ Technologies Used
- Python  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib, Seaborn  

---

## 📁 Project Structure

- Student_Performance_Prediction.ipynb
- dataset.csv
- README.md



---

## 👤 Author
**Hirannya Mhaisbadwe**  
B.Tech Student, IIT Bhilai  
