# NBA Player Prop Prediction Project

## Project Description
We will use the [nba_api](https://github.com/swar/nba_api) to collect NBA player game logs and team statistics in order to **predict whether a player will go over or under a given prop line** (e.g., points, rebounds, assists).  

Our goal is to build reproducible models that forecast prop outcomes better than simple baselines, while also producing clear visualizations of player performance trends.

---

## Project Goals
- Predict the probability of players going over/under on common props (points, rebounds, assists, 3-pointers).  
- Benchmark against naive methods (e.g., season averages) to show improvement.  
- Visualize how player performance interacts with matchup and game context.  
- Ensure the workflow is fully reproducible from our GitHub repo.

---

## Data Collection
We will use `nba_api` to pull:  
- **Box score data**: points, rebounds, assists, 3PT attempts/makes, minutes played.  
- **Game logs**: per-player, per-game history.  
- **Team stats**: opponent defensive rankings, pace, home/away context.  
- **Schedule data**: rest days, back-to-back games.  

---
