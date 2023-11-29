# NFL Big Data Bowl: Tackling Big Data 

## Introduction
In collaboration with the NFL, we will be using Next Gen Stats player tracking data to generate an analysis of player statistics for fans, players, teams, and coaches to understand their performance. We will focusing on examining tackling performance across the NFL using data from weeks 1-9 of the 2022 NFL season analyzing the location, speed and acceleration of all 22 players on the field, along with the location of the football during a given play.

### Objective of Football Game
+ There are 4 fifteen minute quarters where one team will receive and the other team will defend
+ The objective is to score more points than the other team by getting a touchdown (6 points) Field Goal (3 Points) Safety (2 Points) Extra Point (1 Point)
+ Once an offensive player receives a handoff or catches a pass, all 11 defenders focus on one task - tackle the ball carrier as soon as possible
+ The ball carrier’s role is to advance the ball down the field to gain as many yards as possible until he is tacked, scores, or runs out of bounds

## Data
The data was provided by NFL NextGen Stats and collected through AWS and compiled into seperate CSV files from [Kaggle](https://www.kaggle.com/competitions/nfl-big-data-bowl-2024/data). 

Next Gen Stats Data includes Weeks 1-9 of 2022 NFL season with player and games demographics and information:
+ Location, Speed, and Acceleration of players on field
+ Football location
+ PFF Scouting Data

### File descriptions
+ Game data: The games.csv contains the teams playing in each game.
+ Play data: The plays.csv file contains play-level information from each game. 
+ Player data: The players.csv file contains player-level information from players that participated in any of the tracking data files. 
+ Tackles data: The tackles.csv file contains player-level tackle information for each game and play. 
+ Tracking data: Files tracking_week_[week].csv contain player tracking data from week number [week]. 
  
## Data Analysis & Visualizations
1. Data Clean Up using Excel and Python Pandas
Since the data has 12 weeks worth of data, we dropped columns to clean and merge data to decrease the size of the file and focus on ball snaps, touchdowns, and tackles. 

2. Play Analysis with Python from Ball Snap to Touchdown
Ball Snap:
+ Frequency and timing of plays
+ Player positioning and movement at the start of a play
+ Compare pre-snap player arrangements against outcomes

Touchdown:
+ Analyzing the plays leading to touchdowns
+ Player speed and trajectories on scoring plays
+ Efficiency of offensive plays or breakdowns in defense

3. Data Visualizations through Tableau
+ [2022 NFL Season Playor Information & Tackles Tableau Dashboard](https://public.tableau.com/app/profile/hannahvarghese/viz/2022NFLSeasonPlayerInformationTackles/2022NFLSeasonPlayerInformationTackles?publish=yes)
In this dashboard, we are able to see the information regarding the player and their position based on birth year, university attended, and tackles. By clicking on the dropdown, we are able to select positions to see which age demographics of players, universities that bring in the most talent, and the overarching question of which players help defend the ball. 
 
We can see here that our oldest player here is Tom Brady who is a 46 years old QB (now retired) or the fact that you see that latest players that joined the NFL were majority wide receivers. Looking at age can show a pattern of the talent hired or the need of talent, coaches can see at what ages certain positions have their best performance and this could be seen over years worth of data. 

Looking at the position by university, this information is great for future professional athletes who are considering where they should go to school based on the position they want to play and which schools have great football programs. 

Lastly, we can see the Inside Linebackers (ILB) main goal is to tackle the ball carriers and see which players do well so that coaches can create their plays based on what is and isn’t successful with other players. 

<img width="563" alt="Screenshot 2023-11-29 at 10 28 24 AM" src="https://github.com/aclima88/NFL_BigDataBowl/assets/132293452/be58e344-afe4-43cc-863a-d1bf4f46a6b1">
<img width="926" alt="Screenshot 2023-11-29 at 10 28 51 AM" src="https://github.com/aclima88/NFL_BigDataBowl/assets/132293452/be2576eb-9bef-4cd4-b3ca-2f5597d01aa0">

4. Predicting if Play will end in a Tackle through Machine Learning using Scikit-learn

[Presentation](https://docs.google.com/presentation/d/15WZJKeTo2RUz-7cuYlhPmSaFu1G3BG81mtE-iGe00EE/edit?usp=sharing)

### Factors that Impact Player Performance
+ Impact of Environmental Factors: Analyze how external factors such as weather conditions, stadium types, or crowd noise affect player movements and performance.
+ Play Calling Analysis: Predict or analyze the effectiveness of different play-calling strategies based on past data, player positioning, and movement patterns.

## Opportunities for Future Analysis
+ Game Outcome Prediction: Import historical data and player performance metrics to predict the outcome of games or the performance of teams during the remainder of the season
+ Tackle range: angle of pursuit, speed and acceleration, closing speed
+ Player evaluation (e.g, yards saved, tackle value, missed tackles)
+ Credit assignment (e.g, one player makes a tackle because of another player, blocks shed, area of influence)
+ Tackle type (solo vs gang, open field vs in the trenches, etc)
+ Team and player roles and responsibilities (setting the edge, filling gaps, etc)

## Built With
* Python - Programming Language
* Pandas - Data manipulation library
* Tableau - Data Visualization software
* Scikit-learn - Machine Learning
  
### Index
* [Data Terminology/Dataset Description](https://www.kaggle.com/competitions/nfl-big-data-bowl-2024/data) 
* Installing git LFS:
* https://stackoverflow.com/questions/65820300/pushing-files-over-100mb-to-github 
If git lfs install does not work right away, you will need to run ‘brew install git-lfs’ before running git lfs install in the terminal.
* [NFL Next Gen Stats](https://operations.nfl.com/gameday/technology/nfl-next-gen-stats/)

## Contact
If you have any questions or concerns regarding the data handling in this project, please do not hesitate to reach out to us: 
+ Aaron Summers [LinkedIn](https://www.linkedin.com/in/aaron-summers-643725216/) | [Github](https://github.com/summers-lee)
+ Angelo Lima [LinkedIn](https://www.linkedin.com/in/angelo-lima-23780467/) | [GitHub](https://github.com/aclima88)
+ Hannah Varghese [LinkedIn](https://www.linkedin.com/in/hannahvarghese/) | [GitHub](https://github.com/hannahvarghese) 
+ Latrice Moore [LinkedIn](https://www.linkedin.com/in/latrice-moore-4a3241248/) | [GitHub](https://github.com/lmoore5460)
+ Marshal Rockafellow [LinkedIn](https://www.linkedin.com/in/marshal-rockafellow-628293140/) | [GitHub](https://github.com/mrockafe) 
