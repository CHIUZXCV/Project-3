# Project-3
# Project-3
Our motivation in this project is to predict the results of the English premier league (EPL) fixtures with machine learning to guide a potential betting model. Once the model is up and running we will use it to predict the fixtures of any other league by changing league and team ids. A machine learning model is used in an attempt to accurately predict the outcome of a match. The core idea is to create a model that would predict the winner of any given match at a higher success rate than betting odds-makers were currently achieving.

### Features
We will use an API, utilize season, year, and league id to request data from v3.football.api-sports.io. We got such features as 

shots_on_goal

shots_off_goal 

total_shots

blocked_shots

shots_insidebox 

shots_outsidebox

fouls

cornerkicks

offsides

possession 

yellowcards

redcards 

gk_saves 

pass_percentage 

We will use these features for home team and away team.

### Logistic Regression Model
We selected a Logistic Regression model due to the clarity of the results. We will build, train and evaluate the model to predict team performance using historical data from the league itself. We were able to source comprehensive league data for all previous seasons in csv format. We used data from 2015 to 2018 as training data and data from 2019 season as testing data. Our model was designed to find the outcome of any given match. Results were assigned a "-1", "0" and "1" which represent loss, draw or win. Betting in English premier league matches is generally split in to “Win” or “Did not win” for the favored team, negating draws as an important factor. We tested the model using the 2019 data.

### Data discrepencies
We have noticed some discrepancies in the datasets due to the fact that every season 3 teams are relegated and 3 other teams are promoted. Also, some teams stay long time out of the premier league making it difficult to get enough data for such teams. So we filled in NaNs where data didn't exists and dropped the NaNs later.

### Notebooks
We run one master notebook, and started with the data cleaning process to get clean dataframes. We created training and testing dataframes, using data from 2015 to 2018 for training and data from 2019 for testing. 


