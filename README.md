# FIFA WorldCup - EDA

Liberary required to work with EDA are:

```
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
import plotly as py                
import cufflinks as cf
%matplotlib inline
from plotly.offline import iplot   
py.offline.init_notebook_mode(connected=True)
cf.go_offline()
```

## Information about the data

The FIFA World Cup is a global football competition contested by the various football-playing nations of the world. It is contested every four years and is the most prestigious and important trophy in the sport of football.

The World Cups dataset show all information about all the World Cups in the history, while the World Cup Matches dataset shows all the results from the matches contested as part of the cups.

## Data set 1: 

1. year : The year in which the match was played.
2. Datetime : The date at which match was played along with 24 hrs date format.
3. Stage : The stage at which the match was played.
4. Stadium : Satdium name where the match was held.
5. city : The city name where the match was played.
6. Home team name : Home team country name.
7. Home team gaol : Total goals scored by the home team by the end of the match.
8. Away Team Goals : Total goals scored by the away team by the end of the match.
9. Away Team Name : Away team country name.
10. Win conditions : Special win condition (if any)
11. Attendance : Total crowd present at the satdium
12. Half-time Home Goals : Goals scored by the home team until half time
13. Half-time Away Goals : Goals scored by the away team until half time
14. Referee : Name of the first refree
15. Assistant 1 : Name of the first assistant referee (linesman)
16. Assistant 2 : Name of the second assistant referee (linesman)
17. RoundID : Unique ID of the Round
18. MatchID : Unique ID of the match
19. Home Team Initials : Home team country's three letter initials
20. Away Team Initials : Away team country's three letter initials

In the data there are few names of the city which are not in order we need to find then and replace it using the command

```
df['column name'] = df['column name']. replace(['1st old value','2nd old value',...],['1st new value','2nd new value',...])
```


## Dataset 2:

1. RoundID : Unique ID of the round
2. MatchID : Unique ID of the match
3. Team Initials : Player's team initials
4. Coach Name : Name and country of the team coach
5. Line-up : S=Line-up, N=Substitute
6. Shirt Number : Shirt number if available 
7. Player Name : Name of the player
8. Position: C=Captain, GK=Goalkeeper 
9. Event : G=Goal, OG=Own Goal, Y=Yellow Card, R=Red Card, SY = Red Card by second yellow, P=Penalty, MP=Missed Penalty, I = Substitution In, O=Substitute Out 

## Dataset 3:

1. Year : Year of the worldcup
2. Country : Country of the worldcup
3. Winner : Team who won the worldcup
4. Runners-Up : Team who was the second place
5. Third : Team who was the third place
6. Fourth : Team who was the fourth place
7. GoalsScored : Total goals scored in the worldcup
8. QualifiedTeams : Total participating teams
9. MatchesPlayed : Total matches played in the cup
10. Attendance : Total attendance of the worldcup

From this data we have found the following 

```
1. Most winner in world cup
2. Number of goal per country
3. Matchs with height number of cups
```


Link : https://github.com/Diksha787/FIFA-WorldCup---EDA
