The purpose of this project is to build a tool that can predict the standings and win totals within the NBA regular season

# Data Collection
Data was collected from balldontlie.io between seasons 1998-2020

# Data Exploration
Using the season of 1998-2002, data was filtered to only include regular season games. After further filtering, I was able to show a scatter plot of each team by each season by score and differentials.
![image](https://user-images.githubusercontent.com/98375141/175560600-4cad925f-a3cd-4b5c-8327-f285c37bd2f7.png)
![image](https://user-images.githubusercontent.com/98375141/175560652-186862d2-260e-4c33-b9ab-4fefee2c8a4f.png)

# Feature Engineering
Created features to get the total average of stats (i.e. points, rebounds, assists, turnovers) including the team and their opponents. I also created features that describes the trend of the teams (i.e. score average of the last 10 games vs opponents score average of last 10 games)

# Model
Both random forest classificaiton and support vector classification was used to train the model. Saw a precision score of 0.685 for random forest classification and 0.672 for SVM. I decided to use random forest classification to train my model.

# Model results
Model did a decent job in predicting the standing order withing an NBA regular season, but had too big of variance in win totals. It predicted the lowest win total to be 5 games which is really hard to do.
