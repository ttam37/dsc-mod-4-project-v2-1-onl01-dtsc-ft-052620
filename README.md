# Recommendation System on MovieLens Dataset

![](https://github.com/ttam37/dsc-mod-4-project-v2-1-onl01-dtsc-ft-052620/blob/master/images/recommender-system-for-movie-recommendation.jpg)

For this project, I will be modeling a recommender system for the MovieLens Dataset, which is a classic dataset used for recommendation system models. The purpose of a recommendation system is to predict future preferences for users by recommending the top items based on the user. I did a simple content-based filtering method and used the surprise library for collaborative filtering.

Why is recommender system important? Recommender system is a decision making strategy which helps relieve users from the amount of overloaded information provided today. E-commerce websites such as Amazon and Ebay have an endless selection of goods and services ranging from high demand to low demand goods. This can be overwhelming to the customer in which they need to browse through possibly millions of items to find what they need. Recommendation systems help alleviate this problem of information overload by providing them with personalized recommendations.

**There are two types of recommender systems, Content-Based Filtering and Collaborative Filtering.**

![](https://github.com/ttam37/dsc-mod-4-project-v2-1-onl01-dtsc-ft-052620/blob/master/images/Content-based-filtering-vs-Collaborative-filtering-Source.png)

### Content Filtering

"Show me more of the same of what I've liked before"

Content-based filtering is based on a profile of the user's characteristics and description of the items. The user's characteristics is used to indicate the type of items an user likes. A content filtering algorithm will recommend items that are similar to what an user likes. The idea behind the algorithm is to tag products using certain features, understand what the user likes, look up those features in the item database, and recommend different items with the same features to the user.

### Collaborative Filtering

"Show me what is popular among similar users like me"

Collaborative filtering is that similar users share similar interests and that users tend to like items that are to similar one another. It is based on collecting a large amount of data on users' behavior and preferences, and predict what users will like based on their similarities to other users. Many recommender systems use collaborative filtering to find user and item relationships to give an accurate prediction of what an user might like.


# Technologies Used

**Python**
* Pandas for Data Cleaning & Data Manipulation
* Matplotlib, Seaborn for Data Visualization
* Numpy for Data Calculations
* Surprise Scikit for Building Recommendation Systems


# Description of Dataset

GroupLens is a research lab that has provided a public dataset for movie ratings for education purposes. We will be using a subset of the larger dataset for movies that is used to build a movie recommendation system. Subset dataset includes 100,000 ratings and 3,600 tag applications applied to 9,000 movies by 600 users. Last updated 9/2018.

Dataset can be found on the GroupLens website: https://grouplens.org/datasets/movielens/latest/

**Dataset is split into 4 individual files:**
* **movies.csv** : movieId, Title, Genres 
* **ratings.csv** : userId, MovieId, Rating, Timestamp
* **tags.csv** : UserId, MovieId, Tag, Timestamp
* **links.csv** : MovieId, imdbId, tmdbId


# Exploratory Data Analysis

![](https://github.com/ttam37/dsc-mod-4-project-v2-1-onl01-dtsc-ft-052620/blob/master/images/frequency_number_ratings_per_user.png)

![](https://github.com/ttam37/dsc-mod-4-project-v2-1-onl01-dtsc-ft-052620/blob/master/images/movie_count_per_genre.png)

![](https://github.com/ttam37/dsc-mod-4-project-v2-1-onl01-dtsc-ft-052620/blob/master/images/total_count_movies_per_rating.png)

![](https://github.com/ttam37/dsc-mod-4-project-v2-1-onl01-dtsc-ft-052620/blob/master/images/average_rating_x_number_ratings.png)


# Algorithms

The algorithms that were used (pred

#### Basic Algorithms
* **NormalPredictor**: algorithm predicts a random rating based on the distribution of the training set, which is assumed to be normal. This is one of the most basic algorithms that do not do much work.
* **BaselineOnly**: algorithm predicts the baseline estimate for given user and item.

#### K-NN Algorithms
* **KNNBasic**: KNNBasic is a basic collaborative filtering algorithm.
* **KNNWithMeans**: basic collaborative filtering algorithm, taking into account the mean ratings of each user.
* **KNNWithZScore**: basic collaborative filtering algorithm, taking into account the z-score normalization of each user.
* **KNNBaseline**: basic collaborative filtering algorithm taking into account a baseline rating.

#### Matrix Factorization-Based Algorithms
* **SVD**: algorithm is equivalent to Probabilistic Matrix Factorization
* **SVDpp**: algorithm is an extension of SVD that takes into account implicit ratings.
* **NMF**: collaborative filtering algorithm based on Non-negative Matrix Factorization. It is very similar with SVD.
* **Slope One**: straightforward implementation of the SlopeOne algorithm.
* **Co-clustering**: collaborative filtering algorithm based on co-clustering.


# Final Model Results

![](https://github.com/ttam37/dsc-mod-3-project-v2-1-onl01-dtsc-ft-052620/blob/master/images/algorithm_best_rmse.png)




