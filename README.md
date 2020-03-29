# bbref_team_game_logs
This python package scrapes Basketball Reference to return a team's game log for an entire NBA season. 

## Installing this package 
1. git clone https://github.com/sherpan/bbref_team_game_logs.git
2. cd bbref_team_game_logs
3. pip install . 

## API
  ### get_team_game_logs(team,season_end_year)
   ### Parameters:
   * team: abbreviation for NBA team i.e(PHO,DAL,BOS)
   * season_end_year: end year of an NBA season (2005 for the 2004-2005 season)
   ### Returns
   A pandas dataframe with the following columns 
   Game #           object
Date             object
H/A              object
Opponent         object
W/L              object
Team PTS        float64
Opponent PTS    float64
Team FG         float64
Team FGA        float64
Team FG%        float64
Team 3P         float64
Team 3PA        float64
Team 3P%        float64
Team FT         float64
Team FTA        float64
Team FT%        float64
Team ORB        float64
Team TRB        float64
Team AST        float64
Team STL        float64
Team BLK        float64
Team TOV        float64
Team PF         float64
Opponent FG     float64
Opponent FGA    float64
Opponent FG%    float64
Opponent 3P     float64
Opponent 3PA    float64
Opponent 3P%    float64
Opponent FT     float64
Opponent FTA    float64
Opponent FT%    float64
Opponent ORB    float64
Opponent TRB    float64
Opponent AST    float64
Opponent STL    float64
Opponent BLK    float64
Opponent TOV    float64
Opponent PF     float64
dtype: object
