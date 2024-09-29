# Hybrid-Recommender-Model
# Hybrid Fashion Product Recommendation System

## Introduction

In the world of online fashion retail, providing personalized recommendations is key to enhancing user experience and increasing sales. This project develops a hybrid recommendation system that combines content-based filtering and collaborative filtering to suggest fashion products to users based on their past interactions and product attributes.

## Recommendation System Analysis

The system integrates two different recommendation approaches:

1. **Content-Based Filtering**: Recommends products similar to those a user has liked based on attributes like brand, category, color, and size.
2. **Collaborative Filtering**: Suggests products based on the preferences of similar users, using a matrix factorization technique.

By combining these methods, the hybrid recommendation system offers more accurate and diverse recommendations.

## Features

- **Data Preprocessing**:
  - Extract and preprocess product information including brand, category, color, and size.
  - Merge user ratings with product attributes to create a comprehensive dataset for modeling.

- **Content-Based Filtering Setup**:
  - Utilize product attributes to calculate similarity between products.
  - Generate recommendations based on product content features.

- **Collaborative Filtering Setup**:
  - Use the Surprise library to implement collaborative filtering with SVD (Singular Value Decomposition).
  - Split the dataset into training and testing sets to evaluate model performance.

- **Hybrid Recommendation Function**:
  - Combine content-based and collaborative filtering recommendations to provide a balanced set of product suggestions.
  - Implement a custom function to fetch hybrid recommendations for specific users and products.

- **Performance Evaluation**:
  - Calculate performance metrics like RMSE (Root Mean Square Error) and MAE (Mean Absolute Error) to evaluate the accuracy of the collaborative filtering model.

## Dataset

The dataset used in this analysis includes the following columns:

- **Product ID**: Unique identifier for each product.
- **Product Name**: Name of the product.
- **Brand**: Brand of the product.
- **Category**: Product category (e.g., shirt, pants, shoes).
- **Color**: Color of the product.
- **Size**: Size of the product.
- **User ID**: Unique identifier for each user.
- **Rating**: User rating for the product.

## Visualizations

- **Ratings Distribution**:
  - A histogram showing the distribution of product ratings, which helps to understand the overall user rating behavior.

- **Content-Based Similarity Visualization**:
  - Visualize the similarity between products based on content attributes to understand the clustering of similar products.

- **Collaborative Filtering Predictions**:
  - Scatter plots and line graphs showing the prediction accuracy of the collaborative filtering model.

- **Hybrid Recommendation Example**:
  - Display hybrid recommendations for a specific user, combining content-based and collaborative suggestions.

