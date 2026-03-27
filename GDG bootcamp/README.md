Student Performance Prediction
🔹 Project Overview

This project predicts students’ Final Scores using machine learning.
It uses features like attendance, study hours, assignments, quizzes, and midterm marks to understand what really affects student performance.

The main goal is to:

Predict student outcomes 
Understand key factors behind performance 
Help in making better academic decisions 
🔹 Dataset

The dataset includes:

Personal Info: Gender, City, Department
Academic Info: Assignments, Quizzes, Midterm
Behavioral Info: Study Hours, Attendance
Target Variable: Final_Score
🧹 Data Cleaning
Removed missing and invalid values
Standardized text (e.g., cs → CS)
Removed duplicates
Handled outliers
🔹 Feature Engineering

We created new meaningful features to improve predictions:

Total_Academic
= Midterm + (Assignments × 5) + (Quizzes × 2)
Attendance_Category
Low, Medium, High
Study_Efficiency
= Midterm / Study_Hours_Daily

These features helped the model understand student behavior better.

🔹 Machine Learning Pipeline

We used a Scikit-learn Pipeline for clean and professional workflow:

One-Hot Encoding → Gender, City, Department, Internet Access
Ordinal Encoding → Education Level, Attendance Category
Scaling → Numerical features
Model → Random Forest Regressor 
