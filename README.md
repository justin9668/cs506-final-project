# NBA Player Prop Prediction Project

## Project Description
We will use the [nba_api](https://github.com/swar/nba_api) and historical betting datasets to collect NBA player game logs and team statistics in order to **predict whether a player will go over or under a given prop line** (e.g., points, rebounds, assists). We will also extend this idea to **team-based predictions**, such as forecasting the final team scores or game winners.

Our goal is to build reproducible models that forecast prop outcomes better than simple baselines, while also producing clear visualizations of player performance trends.

---

## Project Goals
- Predict the probability of players going over/under on common props (points, rebounds, assists, 3-pointers).
- Predict team-level outcomes such as final scores or game winners.
- Benchmark against naive methods (e.g., season averages) to show improvement.  
- Visualize how player performance interacts with matchup and game context.  
- Ensure the workflow is fully reproducible from our GitHub repo.

---

## Data Collection
We will use:
- **nba_api**:  
  - **Box score data**: points, rebounds, assists, 3PT attempts/makes, minutes played.  
  - **Game logs**: per-player, per-game history.  
  - **Team stats**: opponent defensive rankings, pace, home/away context.  
  - **Schedule data**: rest days, back-to-back games.
- **Kaggle Datasets**: [NBA Betting Lines](https://www.kaggle.com/datasets/thedevastator/uncovering-hidden-trends-in-nba-betting-lines-20), [NBA Odds Data](https://www.kaggle.com/datasets/christophertreasure/nba-odds-data)  
  - Historical betting lines and prop odds.  
  - Provides ground truth "line" data to compare against actual outcomes.  
  - Allows evaluation of how predictive our models are compared to betting markets.  

---

## Modeling Plan
- **Logistic Regression** to predict whether a player will go over or under their prop line.
- **Linear Regression** for predicting raw stats like points or rebounds.
- **K-Nearest Neighbors (KNN)** to compare similar players or matchups using distance-based similarity.
- **Clustering (K-Means)** to explore player or team groupings based on stat patterns.
We'll decide what works best once we explore the data more.

---

## Visualization
We'll make basic visualizations to help us understand trends and model performance, like:
- Line plots of player stats over time.
- Scatter plots showing relationships between features.
- Heatmaps comparing teams or matchups.

---

## Test Plan
We'll train on 80% of the games and test on the final 20% to see how well our models generalize. We'll also:
- Compare our predictions to simple baselines (like season averages).
- Use metrics like accuracy or MAE depending on the task.
- Try cross-validation if needed for more reliable results.

## Group Members
- Alim (ackura@bu.edu)
- Ash (payaalayushman@gmail.com)
- Jonah (jonahr@bu.edu)
- Justin (justin1@bu.edu)
- Shawn (xianghu0605@gmail.com)
