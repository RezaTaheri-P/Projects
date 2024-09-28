# **Titanic Survival Prediction Project**

## **Introduction**

This project focuses on predicting the survival of passengers aboard the Titanic using machine learning techniques. The dataset contains various demographic and socio-economic features such as age, gender, ticket class, and fare. By building predictive models, we aim to analyze the factors that most influenced passenger survival and achieve high accuracy in survival predictions.

### **Dataset Overview**:
- **Number of Training Examples**: 891
- **Number of Test Examples**: 418
- **Number of Features**: 12 (including Age, Sex, Passenger Class, Fare, etc.)
- **Objective**: To predict whether a passenger survived or not (binary classification) using machine learning algorithms.

## **Algorithms Used**

Several classification algorithms were implemented to predict whether passengers survived based on the provided features:

1. **K-Nearest Neighbors (KNN)**
2. **Logistic Regression**
3. **Support Vector Machine (SVM)**
4. **Decision Tree**

Each model was evaluated using metrics like **accuracy**, **precision**, **recall**, and **F1-score**, and the results were compared.

## **Project Workflow**

### **Step 1: Data Exploration**
- Analyzed the dataset to understand the distribution of features like age, gender, ticket class, and fare.
- Visualized relationships between passenger survival and key features, such as survival rates based on gender, age, and passenger class.

### **Step 2: Data Preprocessing**
- Handled missing values in features such as **Age**, **Embarked**, and **Fare**.
- Encoded categorical variables (e.g., **Sex**, **Embarked**) using label encoding and one-hot encoding.
- Created new features, like **Family Size** (combining siblings/spouses and parents/children).
  
### **Step 3: Model Building and Training**
- Applied multiple classification algorithms (KNN, Logistic Regression, SVM, and Decision Tree) to predict survival.
- Split the training data into training and validation sets to assess model performance.
- Tuned model hyperparameters to optimize accuracy.

### **Step 4: Evaluation and Comparison**
- Evaluated the models using metrics like accuracy, precision, recall, and F1-score.
- **Confusion Matrix**: Used to understand the performance of the models in predicting survivors and non-survivors.
  
### **Model Performance Summary**:

- **K-Nearest Neighbors (KNN)**:
  - **Accuracy**: 84%
  - Struggled with recall for survivors, with a recall of 68% for class 1.

- **Logistic Regression**:
  - **Accuracy**: 84%
  - Balanced performance with a recall of 80% for survivors, making it a strong contender for this task.

- **Support Vector Machine (SVM)**:
  - **Accuracy**: 85%
  - Best overall performance, providing a good balance between precision and recall.

- **Decision Tree**:
  - **Accuracy**: 83%
  - High precision but lower recall for survivors, indicating it may miss some positive cases.

### **Step 5: Test Set Predictions**
- Used the best-performing model (SVM) to make predictions on the test set.
- Generated a submission file with passenger IDs and predicted survival outcomes.

## **Conclusion**

After evaluating multiple models, **Support Vector Machine (SVM)** provided the highest accuracy at 85% with balanced precision and recall for both survivors and non-survivors. **Logistic Regression** also performed well, showing balanced precision and recall, making it another strong option.

This analysis highlights how demographic factors such as **Sex**, **Pclass**, and **Age** played significant roles in determining the likelihood of survival.

### **Business Application**:
The insights gained from this analysis can be used for future predictions in similar scenarios where binary outcomes are needed, such as risk assessments in insurance or predicting customer churn.

## **Future Work**

- Experiment with more advanced algorithms, such as **Random Forest** and **XGBoost**, to improve predictive performance.
- Perform hyperparameter tuning using **Grid Search** or **Random Search** to optimize models further.
- Investigate feature importance using models like **Gradient Boosting** to understand which features most significantly influence survival.

## **Acknowledgments**

- [Kaggle Titanic Dataset](https://www.kaggle.com/c/titanic)
- [Scikit-learn Documentation](https://scikit-learn.org/stable/)
- [Pandas Documentation](https://pandas.pydata.org/)
- [Matplotlib Documentation](https://matplotlib.org/)