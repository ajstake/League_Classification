# Predicting Winning Teams in League of Legends

Alex Stake

## Abstract

The goal of this project was to predict whether a team would win a game of League of Legends based on data from the first 15 minutes of the game. The data was retrieved from Kaggle and covered 50,000 games from the Diamond ranked league, having features such as each team's gold total, total kills, number of enemy towers destroyed, and average player level.
I explored multiple classification models including logistic regression, decision trees, and random forest models. This goal was achieved through logistic regression, having built a model with an F1 score of 0.80068 and an accuracy of 0.79560.

## Design

For Riot Games I examined data pulled from League of Legends to help them determine the odds of winning a game so they may better plan their tournament rewards around teams of Diamond league players. To this end I built a logistic regression model designed to predict whether or not a team would win a game based on a number of factors within the first 15 minutes of several games as these are critical stages for the remainder of the match. Riot can then use the model in tandem with their player database to balance the teams around players who have high performance in the factors that have the strongest predictive power.
The model was examined with the F1 score as the primary evaluation metric with accuracy as a secondary metric as I sought to balance a precise model while also capturing as many victories as possible.

## Data

The data comes from Kaggle covering the first 15 minutes of 50,000 games from the Diamond Ranked League. This data comes from the 2020 season of League of Legends, and includes data such as the total gold per team, the average experience per team, how many of which objective they captured, as well as other features that will be important for determining the target of which team won.

## Algorithms

*Feature Engineering*
1. Dropped columns with no values when there should be (Dragon Kills) and unique indicators (Match ID)
2. Subtracted the Red team gold from the Blue team gold to create Gold Difference
3. Subtracted the Red team champion kills from Blue team kills to create Kill Difference

*Models*

Logistic regression, decision trees, and random forest models were examined before settling on logistic regression as it had similar F1 score performance to the decision tree model, but had higher accuracy after a 5 K-fold cross validation.

*Model Evaluation*

After splitting the data 80/20 I ran a 5 fold cross validation grid to determine the best parameters to run the model. I then scaled the data for logistic regression to properly train the data as some features had much higher continuous values than others. With this, I got an F1 score of 0.78740 on the training data, with the model having an F1 score of 0.80068 on the holdout data and an accuracy of 0.79560.

## Tools

- Numpy and Pandas for data manipulation and exploration
- Scikit-Learn for modeling
- Matplotlib and Seaborn for plotting

## Communication

The data is presented through the [slides](https://github.com/ajstake/League_Classification/blob/main/League_Classification.pdf) and [figures](https://github.com/ajstake/League_Classification/tree/main/figures) provided.
