# Project Title
Development of Item-based Personalized Recommendation System Using MovieLens Dataset. This project was conducted during the Big Data Processing and Application class in the second semester of 2023.

# Why I do this project?
We need efficient processing techniques for the explosive growth of data. In addition, we need to develop algorithms that can handle complex graph data. Finally, we need a personalized recommendation system for the additional value creation for each domain. So we decided on the topic of developing an Item-based personalized recommendation system using the MovieLens dataset.

# Project Process

**Preprocessing**
- Movieid deduplication
- Disconnect movies and year

**Recommendation System**
+ Create a user-item rating matrix

![image](https://github.com/user-attachments/assets/56170c00-9a93-4d75-8c37-bdca9028f988)

+ Transpositions are used to calculate the similarity between items, and missing values are used to replace missing values.

![image](https://github.com/user-attachments/assets/9e467501-bb9e-4fe2-b7d7-e44e50ea3c60)

+ The similarity between items is obtained through cosine similarity.
![image](https://github.com/user-attachments/assets/560d14af-7214-4d16-b02f-32fc21dc9596)

+ Item-Based Collaborative Filtering
+ 1. Bias from mean
Prediction by calibrating the user's bias (average rating) based on the rating of similar items.

+ 2. KNN
Based on user ratings, predictive ratings are provided without bias correction.

+ 3. Significance Weighting
User rating deviation and similarity are considered, and predictive ratings corrected for bias are provided using the sigmoid function.

# Result
+ Using deviations from the mean, the performance was good by removing individual biases of users and items, providing more accurate and fair recommendations.

![image](https://github.com/user-attachments/assets/eb309716-8b89-4fba-b1a6-317032eb0907)

# contribution
- It was developed through MoiveLens data, but it can be used in all fields in the user-product relationship.
- It improves the user experience and provides products or content that better suit the needs and tastes of the user.
- It enables more sophisticated and personalized recommendations by utilizing specific activity data of users.

# Difficult Point
- In item-based collaborative filtering, study which method should be used to increase the accuracy of the recommendation system.