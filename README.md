# Restaurant Price Prediction Project

## Introduction

This project aims to predict restaurant prices in Bengaluru using machine learning techniques. By analyzing various factors, including restaurant features, customer reviews, and location details, the goal is to provide accurate price predictions that can aid both customers and investors in understanding pricing trends and making informed decisions.

For a detailed report of the analysis, including non-technical insights, please visit: [Comprehensive Data Analysis and Insights](https://ahmedayoupds.blogspot.com/2024/08/comprehensive-data-analysis-and.html).

To view the interactive Google Colab notebook used for this project, visit: [Google Colab Project](https://colab.research.google.com/drive/17hybci2ENtSJ4DEXN6jkFJkVQXJQeyES?usp=drive_link).

## Objectives

- **Predict Restaurant Prices:** Develop a model to accurately predict the cost for two people at restaurants.
- **Evaluate Pricing Strategies:** Assess how different factors influence pricing.
- **Enhance Customer Experience:** Provide insights that help customers choose restaurants based on their budget.
- **Identify High-Performing Establishments:** Highlight top-performing restaurants in terms of pricing and popularity.
- **Develop Predictive Models:** Build machine learning models to forecast restaurant prices and recommend pricing strategies.
- **Explore Market Trends:** Analyze the restaurant market in Bengaluru, including cuisine preferences and pricing trends.
- **Provide Investment Recommendations:** Offer insights and recommendations for investors based on pricing trends and market analysis.

## Data Cleaning and Preparation

1. **Data Cleaning:**
   - Removed irrelevant columns: `url`, `address`, `name`, `rest_type`, `dish_liked`, `cuisines`, `reviews_list`, `review_sentiment_list`, `menu_item`.
   - Applied binary encoding to columns: `online_order`, `book_table`, `is_new`, `is_road`.
   - Applied ordinal encoding for classes.
   - Removed outlier with the highest restaurant cost.
   - Split data into training and test sets to prevent target encoding leakage.

2. **Target Encoding:**
   - Applied target encoding to categorical features: `rest_type_0`, `rest_type_1`, `cuisines_0` to `cuisines_7`, `dish_liked_0` to `dish_liked_6`, `listed_in(type)`, `listed_in(city)`, `location`.
   - Created feature maps to replace values in the test set.

3. **Correlation Analysis:**
   - Reviewed heatmap to assess correlation between features.
   - Addressed multicollinearity using Variance Inflation Factor (VIF) analysis.

4. **Selected Features:**
   - Based on VIF and heatmap analysis, selected features include: `rest_type`, `cuisines`, `approx_cost(for two people)`, `classes`, `num_spec`, `num_cuisines`, `num_dish_liked`, `listed_in(type)`, `listed_in(city)`, `num_reviews`, `book_table`, `online_order`, `votes`, `is_rate_valid`.

5. **Standardization:**
   - Applied `StandardScaler` to normalize feature values.

## Machine Learning Models

1. **Random Forest:**
   - **Configuration:** 600 estimators.
   - **Results:**
     - Training Score: 0.9685
     - R² Score: 0.7961
     - MAE: 111.75
     - MSE: 26100.80
     - RMSE: 161.56

   ![Random Forest Results](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhQNVrUKo_fyM9yWtTY5RMumso9xHzTstR6eC1lIipaOeq8DbRaN4ROoodKZgJhyphenhyphenvhOBkDBCgeZdfe_-BKOOyufDdQi6def6afV1gFPO7-nz0uGlby8C7GsEtSPaguhV2j5WsMmIM3-9wV3kULgPamM6hVt6nexG35Nwd9OGTyiEnW29Xt7_RcU9suY2f4/s1600/download.png)

2. **XGBoost:**
   - **Configuration:**
     - Objective: 'reg:squarederror'
     - Learning Rate: 0.1
     - Max Depth: 6
     - Alpha: 10
     - Number of Estimators: 1000
   - **Results:**
     - Training Score: 0.9418
     - R² Score: 0.7918
     - MAE: 113.57
     - MSE: 28603.34
     - RMSE: 168.74

   ![XGBoost Results](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgn7O5g0G_Uh15g3MGAeSnEKot75Cyb9QEGvMj0CEpLEp47-8J9fP9F8EFiOdm2QOlaCnK8d1n9ZlN5HGe_1jEnqxUoG3kQQGkzTZzO9K9b2CL7dz8Gb8CkSx6fivCnBwp6g5hCMED5_FANsQkS-5wIs7c8YN4Ra0GJdInF8eZXIVLOdpO79NiXwMLI5DUnVVDDrFgFsgp3Yf2M2Q/s1600/download.png)

3. **LightGBM:**
   - **Configuration:**
     - Objective: 'regression'
     - Boosting Type: 'gbdt'
     - Learning Rate: 0.1
     - Number of Leaves: 31
     - Number of Estimators: 500
   - **Results:**
     - Training Score: 0.9675
     - R² Score: 0.7915
     - MAE: 113.21
     - MSE: 28726.52
     - RMSE: 169.48

   ![LightGBM Results](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhhKY5GldvANvyd-k7-Gk8R46eC1aAnKRXamLaWzeWeSsz8Vs-SU2CTZms6TmCBdHs-_H2sb1rRQUu2HqXcOtO_wv5C4m9PTvOB2RBXxk0RC8mRi3zJvOp9NwqSImyoXJcn84XMXCUM7kW5t9sMaXz82mgWfE4A7OXQzUSiNq4BwvRJNaLsZJ1kpM/s1600/download.png)

## Conclusion

The Random Forest model demonstrated the best performance in terms of training score and R² score, making it a strong candidate for predicting restaurant prices. However, XGBoost and LightGBM also provided competitive results, offering alternative approaches depending on specific project needs.

## Future Work

- **Enhance Model Accuracy:** Explore additional features and advanced hyperparameter tuning to improve model accuracy.
- **Expand Data Sources:** Integrate more diverse datasets to capture a wider range of restaurant types and pricing trends.
- **Real-Time Predictions:** Implement real-time prediction capabilities to provide up-to-date pricing information.
- **User Interface:** Develop a user-friendly interface for easier access and interaction with the price prediction model.

## Contact

For any inquiries or additional information, please contact me at: [ahmedatia456123@gmail.com](mailto:ahmedatia456123@gmail.com)
