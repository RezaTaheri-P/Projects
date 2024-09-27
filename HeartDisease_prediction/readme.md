# **Heart Disease Prediction Project**

## **Introduction**

This project focuses on predicting the presence of heart disease in patients using various machine learning algorithms. The dataset used in this project comes from a medical study and contains demographic and clinical information about patients, including age, cholesterol levels, and exercise-induced angina, among others.

### **Dataset Overview**:
- **Number of Examples**: 303
- **Number of Features**: 13 (including age, sex, chest pain type, cholesterol levels, and more)
- **Target**: Presence of heart disease (binary classification: `1` = heart disease, `0` = no heart disease)

**Objective**:  
The main objective of this project is to accurately predict whether a patient has heart disease based on their medical attributes, using a variety of machine learning algorithms.

## **Algorithms Used**

Several machine learning algorithms were implemented to classify patients as either having heart disease or not:

1. **Support Vector Machine (SVM)**
2. **Logistic Regression**
3. **K-Nearest Neighbors (KNN)**
4. **Decision Tree Classifier**
5. **Random Forest Classifier**

Each model was evaluated and compared based on various performance metrics like precision, recall, F1-score, and accuracy.

## **Project Workflow**

### **Step 1: Data Exploration**
- Analyzed the dataset to understand the distribution of variables and their relationships with the target (presence of heart disease).
- Visualized key features such as age, cholesterol, and chest pain type to gain insights into patterns associated with heart disease.

### **Step 2: Data Preprocessing**
- Handled missing data (if applicable) by filling or removing missing values.
- Standardized the numeric features to ensure that they are on the same scale, which is particularly important for models like SVM.
- Converted categorical features into numeric format using one-hot encoding.

### **Step 3: Model Training and Evaluation**
- **Training**: Applied various classification models (SVM, Logistic Regression, KNN) to the training data.
- **Evaluation**: Each model was evaluated using accuracy, precision, recall, and F1-score to assess its performance on the test data.

### **Step 4: Model Comparison**
- Compared the performance of all models:
    - **SVM**: Achieved an accuracy of 90%, with balanced precision and recall for both heart disease and non-heart disease predictions.
    - **Logistic Regression**: Also achieved 90% accuracy, with slightly better recall for predicting heart disease.
    - **KNN**: Had a lower accuracy (84%) compared to SVM and Logistic Regression, but still performed reasonably well.


### **Model Performance Summary**:

- **Support Vector Machine (SVM)**:
  - Accuracy: 90%
  - F1-Score: 0.88 (class 0), 0.91 (class 1)

- **Logistic Regression**:
  - Accuracy: 90%
  - F1-Score: 0.87 (class 0), 0.92 (class 1)

- **K-Nearest Neighbors (KNN)**:
  - Accuracy: 84%
  - F1-Score: 0.81 (class 0), 0.86 (class 1)

### **Conclusion**

Both **SVM** and **Logistic Regression** achieved a high accuracy of 90%, performing better than **KNN**. Logistic Regression was particularly effective at identifying patients with heart disease (class 1) due to its high recall score, while SVM provided more balanced performance across both classes.

The choice of model can depend on the application: Logistic Regression may be preferred in scenarios where detecting heart disease is critical, while SVM offers a more balanced approach.

## **Future Work**

- Experiment with more advanced machine learning models, such as **XGBoost** or **Neural Networks**, to improve the prediction accuracy.
- Perform hyperparameter tuning using GridSearchCV or RandomSearch to further optimize model performance.
- Explore the use of additional feature engineering techniques or other datasets to enhance prediction accuracy.

## **Acknowledgments**

- [Scikit-learn Documentation](https://scikit-learn.org/stable/)
- [Pandas Documentation](https://pandas.pydata.org/)
- [Matplotlib Documentation](https://matplotlib.org/)
