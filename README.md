# Titanic Predictions Project

This project focuses on predicting the survival of passengers on the Titanic using machine learning. It demonstrates the full workflow of a supervised ML classification project, from data exploration to model evaluation and prediction.

---

## 🚀 Project Overview

**Objective:**  
Predict whether a passenger survived (1) or did not survive (0) using features such as:

- Passenger class (Pclass)  
- Sex  
- Age  
- Number of siblings/spouses aboard (SibSp)  
- Number of parents/children aboard (Parch)  
- Fare paid  
- Embarked port  
- Titles extracted from names  

**Dataset:**  
Kaggle Titanic dataset (`train.csv` and `test.csv`) containing 891 training samples with 12 features and a survival label.

---

## 🛠 Tools & Libraries

- Python 3  
- Jupyter Notebook  
- pandas, numpy (data manipulation)  
- matplotlib, seaborn (visualization)  
- scikit-learn (preprocessing, classification models, evaluation metrics)  
- pickle (saving/loading trained models)

---

## 🔑 Workflow & Steps

1. **Data Exploration & Visualization**  
   - Examine distributions and missing values.  
   - Visualize survival rate by sex, passenger class, age, and family size.  
   - Example finding: ~74% of females survived, compared to only ~19% of males.  

2. **Data Cleaning & Feature Engineering**  
   - Handle missing values for `Age`, `Embarked`, and `Fare`.  
   - Encode categorical variables (e.g., Sex, Embarked, Titles) into numerical format.  
   - Create new features like `FamilySize = SibSp + Parch + 1`.  

3. **Model Building & Evaluation**  
   - Models tested: Logistic Regression, Random Forest, Support Vector Machine (SVM).  
   - Split data into training and validation sets.  
   - Metrics evaluated: Accuracy, Precision, Recall, F1-score.  

4. **Results**  
   - **Random Forest** achieved the best performance:  
     - Accuracy: ~82%  
     - Precision: ~79%  
     - Recall: ~78%  
     - F1-score: ~78%  
   - Confusion matrix showed the model correctly predicted most survivors and non-survivors, with slightly more misclassifications for passengers in 3rd class.  

5. **Prediction & Model Saving**  
   - Saved trained model and preprocessing objects using `pickle`.  
   - Example prediction function allows checking survival for new passengers.

---

## 📊 Key Insights

- Passenger **sex** and **class** were the strongest predictors of survival.  
- Children and females in 1st and 2nd class had the highest survival rates.  
- Family size influenced survival: very large or very small families had slightly lower chances.  
- Feature engineering (e.g., extracting titles) improved model performance.

---

## 🚀 How to Use

1. Clone the repository.  
2. Install required packages
3. Open the Jupyter notebook and run it step by step.  
4. Use the `predict_survival()` function to test predictions on new passengers.  

---

**This project is a practical example of applying machine learning to structured data and understanding the importance of feature engineering, model selection, and evaluation metrics.**
