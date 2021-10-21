# Project Proposal

For Riot Games I intend examine data pulled from League of Legends to help them determine the odds of winning a game so they may better plan their tournament rewards around teams of Diamond league players. To this end I plan to build a classification model designed to predict the winning team of each game based on a number of factors within the first 15 minutes of several games as these are critical stages for the remainder of the match. 
Riot can then use the model in tandem with their player database to balance the teams around players who have high performance in the factors that have the strongest predictive factor.

## MVP and Data Used

To answer this question I plan on using this data set of 50,000 games played in the 2020 season of League of Legends available on [Kaggle](https://www.kaggle.com/benfattori/league-of-legends-diamond-games-first-15-minutes) that includes data such as the total gold per team, the average experience per team, how many of which objective they captured, as well as other features that will be important for determining the target of which team won. This data covers the first 15 minutes of a game which is the duration before which a team can surrender.

The **MVP** for this project would look like a bar chart examining the highest average stats for winning teams in order of importance, with the eventual final goal being to build a logistic regression module to predict said winners. 
I plan on using pandas to clean and explore the data, scikit-learn for building the model and scoring it, and matplotlib, seaborn, and potentially tableau for visualization and plotting the data.
