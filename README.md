# DECISION-TREE-IMPLEMENTATION

COMPANY: CodTech IT Solutions

NAME: Yash Kumar

INTERN ID: CT06DG602

DOMAIN: Machine Learning

DURATION: 6 Weeks

MENTOR: Neela Santosh

Diabetes Prediction Using Decision Tree Classifier

📌 Overview

This project presents a machine learning approach to predicting the presence of diabetes using patient medical data. Utilizing the PIMA Indians Diabetes dataset, the model is trained with a Decision Tree Classifier, a simple yet powerful supervised learning algorithm for classification tasks.

The goal is to identify whether a patient is diabetic (1) or not (0) based on features like glucose level, blood pressure, insulin levels, age, BMI, and more. The project emphasizes interpretability, visualization, and model evaluation, making it ideal for both beginners and professionals looking to understand medical classification problems.

📂 Dataset

Name: PIMA Indians Diabetes Dataset

Source: Kaggle - PIMA Diabetes Dataset

File Used: diabetes1.csv

Shape: 768 rows × 9 columns

📊 Features:

Column	          Description

Pregnancies      	Number of times pregnant
Glucose	          Plasma glucose concentration
BloodPressure	    Diastolic blood pressure
SkinThickness	    Triceps skinfold thickness
Insulin	          2-Hour serum insulin
BMI	              Body mass index
Age	              Age in years
Outcome	          Class variable (0: No Diabetes, 1: Diabetes)

🔍 Exploratory Data Analysis

All values were numeric and had no missing entries.

Class distribution: Reasonably balanced

Data types: int64 and float64

⚙️ ML Pipeline
1. Data Preparation
   
Split the dataset into features (X) and target (y).

Performed an 80-20 train-test split using train_test_split.

2. Model Training
   
Algorithm used: DecisionTreeClassifier

Parameters: max_depth=3 to prevent overfitting and improve generalization.

3. Predictions
   
Model predicted class labels on the test set using clf.predict(X_test)

Confusion Matrix

Provides insight into true/false positives and negatives

 Classification Report
 
 Precision: How many predicted positive cases were actually positive.

Recall: How many actual positive cases were correctly identified.

F1-score: Harmonic mean of precision and recall.

While precision for both classes is decent, recall for diabetic patients is relatively low due to the decision tree's depth limitation.

🌲 Decision Tree Visualization
Using plot_tree() from sklearn.tree, a full decision tree was visualized with:

Node information

Splitting conditions

Class probabilities

Color-coded nodes (confidence)

This makes it interpretable, ideal for medical professionals who prefer explainable models

📊 Feature Importance
The relative importance of features in making split decisions was visualized using a bar chart.

Top Features:
Glucose

BMI

Age

Diabetes Pedigree Function

These features heavily influenced the model's decision-making, aligning well with known medical risk factors

🛠️ Technologies Used
Python

Pandas / NumPy

Matplotlib / Seaborn

Scikit-learn

Decision Tree Classifier

Train-Test Split

Accuracy / Confusion Matrix / Classification Report
