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
### Objectives
* Identify keywords in course titles using a WordCloud
* Calculate the summary statistics and visualizations of the online course content dataset
* Determine popular course genre
* Calculate the summary statistics and create visualizations of the online course enrollment dataset

We use seaborn library to plot the most popular genre and use rating to determine the most popular courses. 'Python for Data Science' was the most popular courses.

## 02-Extract Bag of Words Features from Course Textual Content
### Objective
* Extract Bag of Words (BoW) features from course titles and descriptions
* Build a course BoW dataset to be used for building a content-based recommender system later

Once the Bag of Words feature extraction process is complete, we can then apply machine learning algorithms such as similarity measurements, clustering, or classification on the courses

## 03-Calculate Course Similarity using BoW Features
### Objective
* Calculate the similarity between any two courses using BoW feature vectors

## 04-Content-based Course Recommender System Using User Profile and Course Genres
### Objective
* Generate a user profile based on course genres and rating
* Generate course recommendations based on a user's profile and course genres

## 05-Content-based Course Recommender System using Course Similarities
### Objective
* Obtain the similarity between courses from a course similarity matrix
* Use the course similarity matrix to find and recommend new courses which are similar to enrolled courses


## 06-Clustering based Course Recommender System
### Objective
* Perform k-means clustering on the original user profile feature vectors
* Apply PCA (Principle Component Analysis ) on user profile feature vectors to reduce dimensions
* Perform k-means clustering on the PCA transformed main components
* Generate course recommendations based on other group members' enrollment history


## 07-Collaborative Filtering based Recommender System using K Nearest Neighbor
### Objective
* Perform KNN-based collaborative filtering on the user-item interaction matrix

## 08-Collaborative Filtering based Recommender System using Non-negative Matrix Factorization
### Objective
* Perform NMF-based collaborative filtering on the user-item matrix

## 09-Course Rating Prediction using Neural Network
### Objective
* Use tensorflow to train neural networks to extract the user and item latent features from the hidden's layers
* Predict course ratings with trained neural networks

## 10-Regression-based Rating Score Prediction using Embedding Features
### Objective
* Build regression models to predict ratings using the combined embedding vectors


## 11-Classification-based Rating Mode Prediction using Embedding Features
### Objective
* Build classification models to predict rating modes using the combined embedding vectors



