# RLCS-Player-Shot-vs.-Win-Percentage

This project analyzes the correlation between professional Rocket League players' quantities of shots vs. their teams win percentage. The goal was to identify who should be taking the shots. 

This was done using 3 primary csv files. First, the "main" csv file (dfMain) was cleaned to only include games played at events listed as major tournaments. This was done because the file containing player data (dfPlayers) did not include what type of event each game was played at. After dfMain contained only relevant games, the game IDs could be cross referenced between dfPlayers and dfMain to create a new dataframe containing player data only for relevant games. Additionally, the team data file (dfTeams) was used to replace each team ID with the more recognizable team name.

A linear regression was then performed for each player using their shot quantities throughout the season and their teams win percentage. Finally, a new dataframe was created with each player's name and the slope of their regression lines with higher slopes indicating a greater positive correlation between shots and win percentage.
