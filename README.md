# Soccer xG Prediction Model

## Project Summary
In this project, we aim to build a model that predicts the **xG (expected goals)** of any given shot taken in a soccer match. xG is a statistic that quantifies how many goals a team could have reasonably expected to score based on the chances it created. This metric is essential for analyzing match performance, as it gives a more accurate picture of a team’s effectiveness than just looking at the final scoreline.

For example, if a team wins 3-0 but trails in xG (e.g., 0.5 to 2.5), we can attribute the result to either luck or exceptional finishing, rather than dominance in play. By predicting xG, we can better understand how likely a shot is to result in a goal and use this to analyze team or player performance.

## Data
The dataset used in this project is obtained from [StatsBomb](https://statsbomb.com/), a provider of detailed soccer data. The dataset contains thousands of match events, including detailed information on roughly **20,000 shots** across various seasons. From this data, we extracted relevant features related to each shot, such as:

- **Distance to goal**
- **Angle to goal**
- **Number of defenders and attackers near the ball**
- **Body part used for the shot**
- **Type of assist leading to the shot**
- And many more engineered features that we hypothesized would affect xG.

## Modeling Approach
To estimate xG, we modeled each shot as a binary classification problem (goal vs. no goal) and used machine learning models that provide probability estimates. The models explored in this project include:

- **Logistic Regression**
- **Random Forest**
- **XGBoost**

Each model was trained and evaluated to predict the likelihood of a goal based on the shot features, allowing us to calculate xG for each shot.

### Evaluation
Our models were evaluated on their ability to provide accurate xG estimates, which were compared to the official xG values provided by StatsBomb. We found that our models could closely replicate these values, providing useful insights into shot quality.

## Practical Applications

### Shot Selection Analysis
We used our xG model to generate visualizations that highlight which types of shots are more likely to result in goals. These insights can help teams focus on creating opportunities that maximize xG and avoid taking low-probability shots.

### Player Performance Analysis
We applied the xG model to individual player shot data to assess shot quality, providing insights similar to those used by professional clubs in scouting and player evaluation.



