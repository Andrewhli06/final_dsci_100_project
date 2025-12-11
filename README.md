# PlaiCraft Server Usage Prediction Project

### Relevant Background Information:
This project aims to answer a predictive question about a dataset using concepts such as data description, exploration, visualisation, and analysis. The dataset to be used, ‘players.csv’, is collected from a Minecraft Server set up to record player statistics. The dataset contains data of each individual players’ actions and information. In order to recruit more players to the game, it is important to know what characteristics of players are most likely to contribute to a large amount of data, or more hours played. Specifically, the project aims to examine to what extent does player experience level predict number of hours played, and does that vary with age?   
### Investigative Questions: Will be using players.csv exclusively
- Broad: We would like to know which "kinds" of players are most likely to contribute a large amount of data so that we can target those players in our recruiting efforts.
- Specific: To what extent does player experience predict played_hours, and does that vary with age?
- How the data will help address this question:
    - We can look at the effects of using only age or experience as a predictor for played_hours, then look at how that differs from using both as predictors simultaneously. Intuitively speaking, the more experience you have, the less you need to play (until you reach a competitive threshold). The less experience you have, the more you need to play. And vice versa. Finally, age determines how much time you can dedicate to Minecraft.
- Data wrangling plans:
    - In terms of wrangling, players.csv looks generally. All the players' information is contained within a row, each cell measures one thing, and each column represents one distinct variable. That being said, the age variable contains 2 NAs, so imputation will be required, and for our regression model, encoding of the categorical variables will be needed.
- Evaluation plans:
    - Seeing as the data does not exhibit a linear relationship, and has some extreme outliers, we will be using knn regression to predict played_hours. In terms of our evaluation metric of choice, we will be using RMSE. The reason for RMSE is due to the fact that there a lots of small values, and quite a few extreme outliers. So, using the square root, we should be able to tighten up the values, so that magnitude does not play much of a role in error.
