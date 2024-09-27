# **Phone Recommendation System**

## **Introduction**

This project focuses on recommending mobile phones to users based on collaborative filtering techniques. Collaborative filtering leverages past user behavior, such as reviews and ratings, to predict which products a user may like. By identifying users with similar preferences, this recommendation system suggests phones that align with individual tastes.

### **Dataset Overview**:
Two datasets were used in this project:

1. **items.csv**: Contains information about the phones.
   - **Number of Examples**: 148 (phones)
   - **Number of Features**: 5 (including `asin`, `brand`, `title`, `price`, and `rating`)
   
2. **reviews.csv**: Contains user reviews for the phones.
   - **Number of Examples**: 679 (user reviews)
   - **Number of Features**: 4 (including `asin`, `name`, `rating`, and `date`)

**Objective**:  
The objective of this project is to develop a recommendation system that suggests mobile phones to users based on their previous reviews and ratings, utilizing collaborative filtering techniques.

## **Algorithms Used**

The collaborative filtering algorithm implemented in this project includes:

1. **Collaborative Filtering**: This method identifies similarities between users based on their past ratings and reviews to generate personalized phone recommendations.

## **Project Workflow**

### **Step 1: Data Exploration**
- Analyzed both datasets to understand the distribution of phones and user ratings.
- Explored features such as phone brands, prices, and ratings to identify useful patterns.

### **Step 2: Data Preprocessing**
- Cleaned the data by handling missing values and ensuring that all phones in the `reviews.csv` file matched with the phones in the `items.csv` file.
- Created a user-item matrix where each row represents a user, and each column represents a phone. The entries of the matrix contain user ratings for the phones.

### **Step 3: Model Implementation**
- Implemented collaborative filtering techniques to compute similarities between users and to generate recommendations based on the preferences of similar users.

### **Step 4: Recommendations**
- Generated phone recommendations for specific users based on the trained model, suggesting phones they may like based on the ratings of similar users.

### **Model Performance Summary**:

The collaborative filtering model showed good potential in recommending relevant phones to users based on their past preferences and reviews from similar users. The model effectively provided personalized recommendations, making it a suitable approach for recommendation systems in e-commerce.

## **Conclusion**

The collaborative filtering approach was successfully implemented to develop a phone recommendation system. The system provides personalized suggestions by identifying similarities between users' preferences and behavior. The model performs well by recommending phones that users with similar tastes have rated highly.

Despite its effectiveness, the model may face challenges with new or inactive users (cold start problem), as it relies on existing user data for recommendations.

## **Future Work**

- Incorporate more advanced recommendation algorithms to further improve recommendation quality.
- Explore content-based filtering by utilizing phone attributes such as brand, price, and features to enhance recommendation accuracy.
- Perform hyperparameter tuning to optimize the performance of the collaborative filtering model.

## **Acknowledgments**

- [Surprise Library Documentation](https://surprise.readthedocs.io/en/stable/)
- [Pandas Documentation](https://pandas.pydata.org/)
- [Matplotlib Documentation](https://matplotlib.org/)