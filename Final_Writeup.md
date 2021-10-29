# Predicting Winning Teams in League of Legends

Alex Stake

## Abstract



## Design

For Riot Games I examined data pulled from League of Legends to help them determine the odds of winning a game so they may better plan their tournament rewards around teams of Diamond league players. To this end I built a logistic regression model designed to predict whether or not a team would win a game based on a number of factors within the first 15 minutes of several games as these are critical stages for the remainder of the match. Riot can then use the model in tandem with their player database to balance the teams around players who have high performance in the factors that have the strongest predictive power.

## Data

The data comes from Kaggle covering the first 15 minutes of 50,000 games from the Diamond Ranked League. This data comes from the 2020 season of League of Legends, and includes data such as the total gold per team, the average experience per team, how many of which objective they captured, as well as other features that will be important for determining the target of which team won.

## Algorithms



## Tools

- Numpy and Pandas for data manipulation and exploration
- Scikit-Learn for modeling
- Matplotlib and Seaborn for plotting

## Communication

The data is presented through the [slides]() and [figures]() provided.
