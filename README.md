# Recommender System Models Project

## Overview

This project focuses on configuring, evaluating, and comparing recommender system models using the MovieLens dataset. The objective is to explore the dataset, prepare it for modeling, and implement various recommender system algorithms. The models are then compared against a baseline to assess their performance.

## Dataset

The dataset used is the MovieLens dataset, containing millions of ratings from thousands of users on thousands of movies. The data includes the following fields:

- `userId`: Unique identifier for each user.
- `movieId`: Unique identifier for each movie.
- `rating`: Rating given by the user (ranging from 0.5 to 5.0 stars).
- `timestamp`: Time of rating (in seconds since January 1, 1970, UTC).

## Project Structure

### 1. Analysis of Customer Data

- **Exploratory Data Analysis (EDA)**: 
  - Compute the relative frequency of top-k movies.
  - Compute the relative frequency of top-k users.
  - Select the top-k items and update the dataframe accordingly.
  - Visualize data distributions and patterns.

### 2. Data Preparation

- Preprocess the dataset to filter and format it for model training.
- Prepare subsets of data for analysis based on the top-k movies and users.

### 3. Baseline Model

- **Normal Predictor**: Implemented as the baseline model to generate random ratings based on the distribution of the training set.

### 4. Neighborhood Method

- **KNNBasic**: A basic k-nearest neighbors algorithm for collaborative filtering.
- **KNNWithMeans**: A variant of KNN that takes into account the mean ratings of the neighbors.

### 5. Matrix Factorization Method

- **SVD (Singular Value Decomposition)**: A matrix factorization method used for collaborative filtering in recommendation systems.


## Evaluation

- Models are evaluated using **5-Fold Cross-Validation**.
- **Root Mean Square Error (RMSE)** is used as the evaluation metric to measure prediction accuracy.

## Conclusions

The notebook concludes with a discussion of the performance of different models, highlighting the strengths and weaknesses of each method compared to the baseline.



