# Recommendation System on MovieLens Dataset

![](https://github.com/ttam37/dsc-mod-4-project-v2-1-onl01-dtsc-ft-052620/blob/master/images/recommender-system-for-movie-recommendation.jpg)

For this project, I will be modeling a recommender system for the MovieLens Dataset, which is a classic dataset used for recommendation system models. The purpose of a recommendation system is to predict future preferences for users by recommending the top items based on the user.

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

Python 
* Pandas for Data Cleaning & Data Manipulation
* Matplotlib, Seaborn for Data Visualization
* Numpy for Data Calculations
* Surprise Scikit for Building Recommendation Systems


# Description of Dataset

The dataset is scraped by Nathan Lauga and is uploaded on Kaggle. He scraped the data from the NBA stats website using the NBA API. The datasets are from 2004 to 2019 season (first 66 games of 2019 due to date scraped). 

Kaggle website can be found here: https://www.kaggle.com/harlfoxem/housesalesprediction

Description of each dataset:
* **games.csv** : all games from 2004 season to last update with the date, teams and some details like number of points, etc.
* **games_details.csv** : details of games dataset, all statistics of players for a given game
* **players.csv** : players details (name)
* **ranking.csv** : ranking of NBA given a day (split into west and east on CONFERENCE column
* **teams.csv** : all teams of NBA


# Exploratory Data Analysis

## 2004-2018 vs 2019 (First 66 Games) FG, 3FG, FT Statistics

![](https://github.com/ttam37/dsc-mod-3-project-v2-1-onl01-dtsc-ft-052620/blob/master/images/percentage_statistics.png)

## 2004-2018 vs 2019 (First 66 Games) PTS, REB, AST Statistics

![](https://github.com/ttam37/dsc-mod-3-project-v2-1-onl01-dtsc-ft-052620/blob/master/images/general_statistics.png)

## 2004 - 2019 (FIrst 66 Games) Statistics over the Seasons

![](https://github.com/ttam37/dsc-mod-3-project-v2-1-onl01-dtsc-ft-052620/blob/master/images/statistics_2004_2019_lineplot.png)

# Modeling

The algorithms that were used:
* Logistic Regression
* Decision Trees
* Random Forest
* K-Nearest Neighbors
* XGBoost
* Gradient Boosting
* LinearSVC

![](https://github.com/ttam37/dsc-mod-3-project-v2-1-onl01-dtsc-ft-052620/blob/master/images/ROC_curve.png)


# Final Model Results

**Best Model**: Linear SVC
**Final Accuracy Score**: 89.74%

![](https://github.com/ttam37/dsc-mod-3-project-v2-1-onl01-dtsc-ft-052620/blob/master/images/LinearSVC_metrics.png)
![](https://github.com/ttam37/dsc-mod-3-project-v2-1-onl01-dtsc-ft-052620/blob/master/images/LinearSVC_confusion_matrix_result.png)
![](https://github.com/ttam37/dsc-mod-3-project-v2-1-onl01-dtsc-ft-052620/blob/master/images/LinearSVC_confusion_matrix_result1.png)




