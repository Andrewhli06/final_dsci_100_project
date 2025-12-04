# final_dsci_100_project
PlaiCraft Project




High-level question: (Probably) Q2 (predicting high playtime)
    -> Current Interest: Predicting playtime from age and player experience
        -> Probably a linear regression(?)



Notes:
  Expecting age to be highly influential (lower age = more time available to play)

  Andrew: Available for anything, volunteers for programming in particular
  
  Emma: Available for anything, volunteers for writing final report/prose specifically

  Areas of improvement from initial template:
  - Data description: Misidentified subscribe and gender as 'irrelevant variables' without justification.
  - Questions: No wrangling needed is incorrect i.e. Age has NAs, Experience is categorical and must be transformed for KNN
  - EDA: Interpretations are slightly surface level - describe what the plot looks like but not what it implies for the predictive question. Looking at distribution of predictors independently is also very insightful (eg.      histogram of Age).
  - Methods: Using ordinal encoding for experience in KNN does not reflect real distances. Does not mention metrics of evaluation for your model.
