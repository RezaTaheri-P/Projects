# **Tehran House Price Prediction Project**

## **Introduction**

This project aims to predict house prices in Tehran based on various property features such as area, number of rooms, parking availability, and more. Using a dataset of residential properties, we applied machine learning techniques to build a predictive model that helps estimate property prices. This project can be useful for real estate agents, buyers, and sellers in assessing property values more accurately.

### **Dataset Overview**:
- **Number of Examples**: 3480
- **Number of Features**: 7 (including Area, Room, Parking, Warehouse, Elevator, Address, Price)
- **Target Variable**: Property price in Iranian Rials (IRR)

## **Algorithms Used**

For this project, we used **Linear Regression** to predict house prices. Additionally, data preprocessing steps were applied to handle missing values, categorical encoding, and feature scaling.

## **Project Workflow**

### **Step 1: Data Exploration**
- Loaded and previewed the dataset to inspect key features.
- Conducted an exploratory data analysis (EDA) using visualizations such as histograms and boxplots to understand the distribution of house prices and how they relate to other features like area and number of rooms.

### **Step 2: Data Preprocessing**
- Converted features such as area to a numeric format and handled missing values in the dataset.
- Encoded categorical variables such as Parking, Warehouse, Elevator, and Address using OneHotEncoding to make them usable for the machine learning model.
- Split the data into training and test sets (80% training, 20% testing) to evaluate model performance.

### **Step 3: Building the Prediction Model**
- Applied **Linear Regression** using a Scikit-learn pipeline that handled both preprocessing and model fitting.
- Trained the model on the training data and used the test data to evaluate its performance.
- Used metrics like **Mean Absolute Error (MAE)**, **Mean Squared Error (MSE)**, and **R² score** to assess model accuracy.
- **R² Score**: The model achieved an **R² score of 0.78**, indicating that 78% of the variance in house prices can be explained by the features used.

### **Step 4: Custom Price Prediction**
- Implemented a custom function that allows users to input specific property features and predict the house price. This function takes into account area, number of rooms, parking availability, and other factors to provide an estimate.

### **Model Performance Summary**:

- **Linear Regression Model**:
  - **Mean Absolute Error (MAE)**: Measures the average absolute difference between predicted and actual prices.
  - **Mean Squared Error (MSE)**: Measures the average squared difference between predicted and actual prices.
  - **R² Score**: The model achieved a **score of 0.78**, demonstrating strong predictive performance.

### **Conclusion**

- The **Linear Regression** model performed reasonably well, providing useful estimates for house prices in Tehran based on the selected features.
- The custom prediction function allows for flexible price estimates based on user-provided inputs, making it a valuable tool for real estate evaluations.

## **Business Application**:

This predictive model can be used by:
- **Real Estate Agents**: To provide price estimates for clients based on specific property features.
- **Home Buyers/Sellers**: To get an idea of property value before listing or buying.
- **Market Analysts**: To analyze trends in the housing market and understand how different features affect property prices.

## **Future Work**

- Experiment with more advanced regression models, such as **Random Forest** or **Gradient Boosting**, to improve prediction accuracy.
- Explore external data sources (e.g., economic factors, neighborhood crime rates) to enhance the predictive power of the model.
- Implement cross-validation techniques to further refine model performance.

## **Acknowledgments**

- [Scikit-learn Documentation](https://scikit-learn.org/stable/)
- [Matplotlib Documentation](https://matplotlib.org/)
- [Pandas Documentation](https://pandas.pydata.org/)