# Premier League Playground
## Analysis of the English Premier League using Kaggle's European Soccer Database

###The ultimate Soccer database for data analysis and machine learning

What you get:

- +25,000 matches
- +10,000 players
- 11 European Countries with their lead championship
- Seasons 2008 to 2016
- Player's attributes sourced from EA Sports' FIFA video game series, including the weekly updates
- Team line up with squad formation (X, Y coordinates)
- Betting odds from up to 10 providers
- Detailed match events (goal types, possession, corner, cross, fouls, cards etc...) for +10,000 matches

### The sqlite database contains the following:
#### Tables:

- Country: 11 European countries
- League: 11 Leagues, one per country
- Match: Home and away teams/goals, lineups with XY coordinates, betting odds. This version of the database does not include the detailed match events
- Player: ids and a few general stats.
- Player_Stats: the features from EA Sport's FIFA football video games. date_stat indicates as of when the set of features was made available
- Team: teams id and names

#### Foreign Keys:
- Country and League are referenced in the Match table by their primary key (id). 
- Matches and Players are linked to other tables by foreign keys *match_api_id* and *player_api_id*. 
