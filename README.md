# bbref_team_game_logs
This python package scrapes Basketball Reference to return a team's regular season game log for an entire NBA season.

## Installing this package
pip install bbref-team-game-logs

## API
  ### get_team_game_logs(team,season_end_year)
   #### Parameters:
   * team : abbreviation for NBA team i.e ('PHO','DAL','BOS')
   * season_end_year: end year of an NBA season ('2005' for the 2004-2005 season)
   #### Returns:
   A pandas data frame with the following columns

  ```python
['Game #' 'Date' 'H/A' 'Opponent' 'W/L' 'Team PTS' 'Opponent PTS'
 'Team FG' 'Team FGA' 'Team FG%' 'Team 3P' 'Team 3PA' 'Team 3P%' 'Team FT'
 'Team FTA' 'Team FT%' 'Team ORB' 'Team TRB' 'Team AST' 'Team STL'
 'Team BLK' 'Team TOV' 'Team PF' 'Opponent FG' 'Opponent FGA'
 'Opponent FG%' 'Opponent 3P' 'Opponent 3PA' 'Opponent 3P%' 'Opponent FT'
 'Opponent FTA' 'Opponent FT%' 'Opponent ORB' 'Opponent TRB'
 'Opponent AST' 'Opponent STL' 'Opponent BLK' 'Opponent TOV' 'Opponent PF']
```
  ### get_team_game_logs_adv(team,season_end_year)
   #### Parameters:
   * team : abbreviation for NBA team i.e ('PHO','DAL','BOS')
   * season_end_year: end year of an NBA season ('2005' for the 2004-2005 season)
   #### Returns:
   A pandas data frame with the following columns

  ```python
['Game #' 'Date' 'H/A' 'Opponent' 'W/L' 'Team PTS' 'Opponent PTS' 'ORtg'
 'DRtg' 'Pace' 'FTr' '3PAr' 'TS%' 'TRB%' 'AST%' 'STL%' 'BLK%'
 'Offensive eFG%' 'Offensive TOV%' 'Offensive ORB%' 'Offensive FT/FGA'
 'Defensive eFG%' 'Defensive TOV%' 'Defensive DRB%' 'Defensive FT/FGA']
```
## Example
 ```python
from bbref_team_game_logs import get_team_game_logs, get_team_game_logs_adv
team = 'PHO'
year = '2005'
df = get_team_game_logs(team,year)
df_adv = get_team_game_logs_adv(team,year)
```
The code above should retreive the data from the following pages [here](https://www.basketball-reference.com/teams/PHO/2005/gamelog/) and [here](https://www.basketball-reference.com/teams/PHO/2005/gamelog-advanced/)

## Basketball Reference Team Abbreviations
These are BBREF's abbreviation for NBA teams. Use this link [here](https://www.basketball-reference.com/teams/) to figure out what years they have been active
 ```python
ATLANTA HAWKS : ATL
ST. LOUIS HAWKS : SLH
MILWAUKEE HAWKS : MIL
TRI-CITIES BLACKHAWKS : TCB
BOSTON CELTICS : BOS
BROOKLYN NETS : BRK
NEW JERSEY NETS : NJN
CHICAGO BULLS : CHI
CHARLOTTE HORNETS : CHO
CHARLOTTE BOBCATS : CHA
CLEVELAND CAVALIERS : CLE
DALLAS MAVERICKS : DAL
DENVER NUGGETS : DEN
DETROIT PISTONS : DET
FORT WAYNE PISTONS : FWP
GOLDEN STATE WARRIORS : GSW
SAN FRANCISCO WARRIORS : SFW
PHILADELPHIA WARRIORS : PHI
HOUSTON ROCKETS : HOU
INDIANA PACERS : IND
LOS ANGELES CLIPPERS : LAC
SAN DIEGO CLIPPERS : SDC
BUFFALO BRAVES : BUF
LOS ANGELES LAKERS : LAL
MINNEAPOLIS LAKERS : MIN
MEMPHIS GRIZZLIES : MEM
VANCOUVER GRIZZLIES : VAN
MIAMI HEAT : MIA
MILWAUKEE BUCKS : MIL
MINNESOTA TIMBERWOLVES : MIN
NEW ORLEANS PELICANS : NOP
NEW ORLEANS/OKLAHOMA CITY HORNETS : NOK
NEW ORLEANS HORNETS : NOH
NEW YORK KNICKS : NYK
OKLAHOMA CITY THUNDER : OKC
SEATTLE SUPERSONICS : SEA
ORLANDO MAGIC : ORL
PHILADELPHIA 76ERS : PHI
SYRACUSE NATIONALS : SYR
PHOENIX SUNS : PHO
PORTLAND TRAIL BLAZERS : POR
SACRAMENTO KINGS : SAC
KANSAS CITY KINGS : KCK
KANSAS CITY-OMAHA KINGS : KCK
CINCINNATI ROYALS : CIN
ROCHESTER ROYALS : ROR
SAN ANTONIO SPURS : SAS
TORONTO RAPTORS : TOR
UTAH JAZZ : UTA
NEW ORLEANS JAZZ : NOJ
WASHINGTON WIZARDS : WAS
WASHINGTON BULLETS : WAS
CAPITAL BULLETS : CAP
BALTIMORE BULLETS : BAL
CHICAGO ZEPHYRS : CHI
CHICAGO PACKERS : CHI
ANDERSON PACKERS : AND
CHICAGO STAGS : CHI
INDIANAPOLIS OLYMPIANS : IND
SHEBOYGAN RED SKINS : SRS
ST. LOUIS BOMBERS : SLB
WASHINGTON CAPITOLS : WAS
WATERLOO HAWKS : WAT
```
