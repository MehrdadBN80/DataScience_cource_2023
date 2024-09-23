# Recommendation System Assignment

## Overview
This project investigates two primary methods for building recommendation systems: **Content-Based Methods** and **Collaborative Filtering Methods**. The goal is to implement a model for each method to enhance personalized shopping experiences, utilizing datasets from BigBasket and Amazon.

## Datasets
1. **BigBasket Entire Product List**
   - **Source**: BigBasket Dataset
   - **Description**: Contains approximately 28,000 data points with product information, including title, category, brand, sale price, market price, rating, and description.

2. **Amazon Ratings (Beauty Products)**
   - **Source**: Amazon Ratings Dataset
   - **Description**: Contains over 2 million customer reviews and ratings for beauty products, including user ID, product ASIN, ratings, and timestamps.

## Assignment Tasks
- Implement one model for each recommendation method.
- Emphasize preprocessing steps, feature engineering, and feature selection.
- Explore advanced algorithms for potential additional scoring.
- Create a comprehensive report including findings, figures, and tables (no code in the report).

## Implementation Details

### Part 1: Content-Based Method
- **User Profile Creation**: Profiles based on historical preferences.
- **Item Profile Creation**: Profiles based on product features.
- **Similarity Score Calculation**: Using Linear Kernel to compute similarity scores.
- **Recommendation Generation**: Providing personalized suggestions based on user interests.

#### Key Findings
- Analyzed the impact of product ratings and discounts on sales.
- Explored the relationship between market prices and discounts.

### Part 2: Collaborative Filtering Method
- **Data Overview**: Analyzed user ratings to understand trends.
- **Normalization**: Addressed biases in user ratings.
- **Cosine Similarity**: Employed to find similar users and recommend products based on their preferences.

#### Key Findings
- Identified popular products and user rating patterns.
- Generated recommendations by leveraging similar users' preferences.

## Conclusion
This assignment highlights the effectiveness of recommendation systems in e-commerce by implementing both content-based and collaborative filtering methods. The results underscore the importance of data preprocessing and feature selection in enhancing recommendation accuracy.

## Future Work
- Explore additional algorithms such as Matrix Factorization or Deep Learning techniques.
- Investigate user engagement metrics to further refine recommendations.
