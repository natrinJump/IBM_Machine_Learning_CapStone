# IBM-Machine-Learning-Capstone-Recommender-System

# Introduction
![image](https://github.com/natrinJump/IBM_Machine_Learning_Recommender_System/assets/143831822/bbd5f878-d9ef-49f1-ac32-42ac4a4e5305)

## Background
Machine Learning has emerged as a transformative force in the realm of data-driven technologies, empowering systems to learn patterns and insights from data without explicit programming. At its core, ML allows computers to make data-driven decisions, improving performance over time based on the information it processes. One captivating application of machine learning is the development of Recommender Systems. These systems utilize algorithms to analyze user behavior, preferences, and historical interactions to predict and recommend items or content tailored to individual tastes. Consider popular platforms like Netflix, where ML-driven Recommender Systems suggest movies or series based on viewing history, or e-commerce giants like Amazon, which leverage similar systems to propose products suited to a user's preferences. The versatility and impact of Recommender Systems showcase the potential of machine learning to enhance user experiences across diverse domains.

## Dataset
* Dataset contains 307 datapoints.
* Dataset contains the features: 'COURSE_ID', 'TITLE', 'Database', 'Python', 'CloudComputing','DataAnalysis', 'Containers', 'MachineLearning', 'ComputerVision','DataScience', 'BigData', 'Chatbot', 'R', 'BackendDev', 'FrontendDev','Blockchain'.
* Each with the following datatypes:
  
![image](https://github.com/natrinJump/IBM_Machine_Learning_Recommender_System/assets/143831822/38175328-2c04-4f7c-82b8-eac2e2ec24cd)


# Content

## 01-Exploratory Data Analysis on Online Course Enrollment Data
* Identify keywords in course titles using a WordCloud
* Calculate the summary statistics and visualizations of the online course content dataset
* Determine popular course genre
* Calculate the summary statistics and create visualizations of the online course enrollment dataset

We use seaborn library to plot the most popular genre and use rating to determine the most popular courses. 'Python for Data Science' was the most popular courses.

## 02-Extract Bag of Words Features from Course Textual Content
* Extract Bag of Words (BoW) features from course titles and descriptions
* Build a course BoW dataset to be used for building a content-based recommender system later

Once the Bag of Words feature extraction process is complete, we can then apply machine learning algorithms such as similarity measurements, clustering, or classification on the courses

## 03-Calculate Course Similarity using BoW Features
* Calculate the similarity between any two courses using BoW feature vectors

Similarity measurement between items is the foundation of many recommendation algorithms, especially for content-based recommendation algorithms. For example, if a new course is similar to user's enrolled courses, we could recommend that new similar course to the user. Or If user A is similar to user B, then we can recommend some of user B's courses to user A (the unseen courses) because user A and user B may have similar interests. 

## 04-Content-based Course Recommender System Using User Profile and Course Genres
* Generate a user profile based on course genres and rating
* Generate course recommendations based on a user's profile and course genres

The most common type of content-based recommendation system is to recommend items to users based on their profiles. The user's profile revolves around that user's preferences and tastes. It is shaped based on user ratings, including the number of times a user has clicked on different items or liked those items.

## 05-Content-based Course Recommender System using Course Similarities
* Obtain the similarity between courses from a course similarity matrix
* Use the course similarity matrix to find and recommend new courses which are similar to enrolled courses

Applying the course similarities metric to recommend new courses which are similar to a user's presently enrolled course.

## 06-Clustering based Course Recommender System
* Perform k-means clustering on the original user profile feature vectors
* Apply PCA (Principle Component Analysis ) on user profile feature vectors to reduce dimensions
* Perform k-means clustering on the PCA transformed main components
* Generate course recommendations based on other group members' enrollment history

Perform clustering algorithms such as K-means or DBSCAN to group users with similar learning interests. For example, in the below user clusters, we have user clusters whom have learned courses related to machine learning, cloud computing, databases, and web development

## 07-Collaborative Filtering based Recommender System using K Nearest Neighbor
* Perform KNN-based collaborative filtering on the user-item interaction matrix

Now to determine if two users are similar, we can simply calculate the similarities between their row vectors in the interaction matrix. Then based on the similarity measurements, we can find the k nearest neighbor as the similar users.

## 08-Collaborative Filtering based Recommender System using Non-negative Matrix Factorization
* Perform NMF-based collaborative filtering on the user-item matrix

In the previous lab, we have performed KNN on user-item interaction matrix to estimate the rating of unknown items based on the aggregation of the user's K nearest neighbor's ratings. Finding nearest neighbors are based on similarity measurements among users or items with big similarity matrices.

The KNN algorithm is memory-based which means we need to keep all instances for prediction and maintain a big similarity matrix. These can be infeasible if our user/item scale is large, for example, 1 million users will require a 1 million by 1 million similarity matrix, which is very hard to load into RAM for most computation environments.

Non-negative matrix factorization can be one solution to big matrix issues. The main idea is to decompose the big and sparse user-interaction into two smaller dense matrices, one represents the transformed user features and another represents the transformed item features.

## 09-Course Rating Prediction using Neural Network
* Use tensorflow to train neural networks to extract the user and item latent features from the hidden's layers
* Predict course ratings with trained neural networks

In addition to NMF, neural networks can also be used to extract the latent user and item features? In fact, neural networks are very good at learning patterns from data and are widely used to extract latent features. When training neural networks, it gradually captures and stores the features within its hidden layers as weight matrices and can be extracted to represent the original data.

## 10-Regression-based Rating Score Prediction using Embedding Features
* Build regression models to predict ratings using the combined embedding vectors

  
## 11-Classification-based Rating Mode Prediction using Embedding Features
* Build classification models to predict rating modes using the combined embedding vectors


# Conclusion
In conclusion, this project demonstrates a comprehensive approach to course recommendation by leveraging various techniques in exploratory data analysis, bag-of-words modeling, K-nearest neighbors, and K-means clustering. The integration of neural networks further enhances the recommendation engine by extracting latent features from user-item interactions. The incorporation of regression and classification models contributes to a robust understanding of user preferences and aids in tailoring recommendations. The seamless presentation of these insights through a Streamlit app ensures a user-friendly interface, making the course recommender system accessible and effective. This amalgamation of diverse methodologies underscores the versatility of machine learning in optimizing personalized experiences and showcases the potential for innovative solutions in the field of educational recommendation systems.




