# xG-Model-for-Soccer

Project Summary:
In this project, we attempt to build a model that predicts the xG, or expected goals, of any given shot taken
within a soccer match. Because relatively few goals are scored in a given match, the randomness of whether
good chances are converted can sometimes influence a match’s outcome more than the game’s dominance or
the quality of chances created. To fill the gap, xG is a statistic that is able to explain how many goals a
team could have expected to score given the chances it created, thus being more descriptive of how a team
performed in a match. If a team won 3 to 0 against an opponent but trailed in xG 0.5 to 2.5, we can attribute
their win to either luck or world-class shooting.
We obtain data from StatsBomb, a commercial soccer data provider, serving as a launchpad for our
investigation. From a dataset containing information regarding each recordable action in soccer matches over
a given season, we prepare a dataset of roughly twenty-thousand shots to train and test our models. We
model xG by using a variety of given and engineered features: distance to goal, angle to goal, the number of
defenders and attackers on the ball, and many more. To provide xG estimates, we select machine learning
models that are able to provide binary class probability predictions. We evaluate the efficacy of various
logistic regression, random forest, and XGBoost models in calculating xG, and are able to attain xG estimates
that are comparable overall to xG metrics calculated and provided by StatsBomb.
After building and evaluating our xG models, we produced a few examples of how xG can be used in practice.
We produce visualizations regarding which types of shots are worthwhile and have a high probability of
resulting in a goal, as well as which types of shots may not be worthwhile and have low probability of resulting
in a goal. This can lead to teams focusing their attention on creating opportunities that lead to a higher
xG, thus boosting their chances of winning. We also produce analyses of players using xG, similar to how
professional clubs might in their scouting and player-evaluation efforts.
