# Early Findings

After some EDA I identified 5 features from the data that are associated with a victory from the first 15 minutes with those being the team's minions killed, their overall gold, the team's collective champion (player) kills, the number of enemy towers destroyed, and the difference of the team's gold against the enemy team's.
Using these features, I focused on the metric of F1 score as to get as precise a model as possible while also attempting to account for factors that are not in the model, such as the enemy team's gold, towers, and kills. This also should account for factors outside of the data such as the team composition, what lanes have more kills, and what items each player has purchased with their gold.
I then built a Logistic Regression model that had an F1 score of 0.78575, which is a good score but could be missing the previous factors as the confusion matrix shown below shows a large amount of false positives.

![](https://raw.githubusercontent.com/ajstake/League_Classification/main/figures/Blue_team_confusion_matrix.svg)

The next step would be to add more features to the model to improve the fit and create a more accurate representation of the data. I may also use a decision tree model to see if that would be a better fit for the data.
