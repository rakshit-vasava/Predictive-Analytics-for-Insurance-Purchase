# 🌐 Homesite Quote Conversion Problem

This project addresses the **Homesite Quote Conversion Problem** on Kaggle, where the objective is to predict whether a customer will buy an insurance policy based on provided data. The solution involves **SMOTE**, **stacking models**, and **hyperparameter tuning** to achieve optimal predictions.

## 🚀 Project Overview

The project focuses on using machine learning techniques to predict if a customer will purchase insurance. We employ **stacking ensemble models** to combine the strengths of various algorithms and address the class imbalance problem using **SMOTE**.

## 🔨 Key Steps

1. **Experimentation with SMOTE**:  
   Synthetic Minority Over-sampling Technique (SMOTE) was used to handle the imbalance in the dataset. In this project, the ratio was set to 0.5, ensuring that the minority class represents half of the majority class.

2. **Stacking Model Implementation**:  
   A one-layer stacking model was created using five base models:
   - **Decision Tree**
   - **Random Forest**
   - **Support Vector Machines (SVM)**
   - **Multilayer Perceptron (MLP)**
   - **K-Nearest Neighbors (KNN)**

   Stacking creates two datasets:
   - `S_Train`: Stacked predictions from base models for training data.
   - `S_Test`: Stacked predictions for test data.

   A **Random Forest classifier** was used as the final meta-model to make predictions.

3. **Hyperparameter Tuning**:  
   Tuning was performed on the stacked model, particularly the Random Forest meta-classifier, improving the model's accuracy.

4. **Kaggle Submission**:  
   Two submissions were made with the following results:
   - **Without tuning**: Private score of 0.80029, Public score of 0.80351.
   - **With tuning**: Private score of 0.8241, Public score of 0.82155.

## 🛠️ Technologies Used

- **Python**
- **Scikit-learn**
- **SMOTE (Synthetic Minority Over-sampling Technique)**
- **Random Forest**
- **K-Nearest Neighbors**
- **Support Vector Machines (SVM)**
- **Multilayer Perceptron**
- **Gradient Boosting**
- **Kaggle Submission Tools**

## 📝 To-Do

- [x] Experiment with SMOTE and tune the minority class ratio.
- [x] Implement ensemble models and perform stacking.
- [x] Hyperparameter tuning for stacked models.
- [x] Submit to Kaggle and report results.

## 📊 Kaggle Results

| Submission Type         | Private Score | Public Score |
|-------------------------|---------------|--------------|
| Stacked Model (no tuning)| 0.80029       | 0.80351      |
| Stacked Model (tuned)    | 0.8241        | 0.82155      |

