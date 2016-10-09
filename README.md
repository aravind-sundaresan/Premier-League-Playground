# Premier-League-Playground
## Analysis of the English Premier League using Kaggle's European Soccer Database

The sqlite database contains the following:
### Tables:

- Country: 11 European countries
- League: 11 Leagues, one per country
- Match: Home and away teams/goals, lineups with XY coordinates, betting odds. This version of the database does not include the detailed match events
- Player: ids and a few general stats.
- Player_Stats: the features from EA Sport's FIFA football video games. date_stat indicates as of when the set of features was made available
- Team: teams id and names

### Foreign Keys
Country and League are referenced in the Match table by their primary key (id). Matches and Players are linked to other tables by foreign keys *match_api_id* and *player_api_id*. These keys are different from the table's primary keys (id). I have deliberately made the joint on these *api_id* to be consistent with the original data sources
