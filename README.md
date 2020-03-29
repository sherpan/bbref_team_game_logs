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
   ['Game #', 'Date', 'H/A', 'Opponent', 'W/L', 'Team PTS', 'Opponent PTS',
       'Team FG', 'Team FGA', 'Team FG%', 'Team 3P', 'Team 3PA', 'Team 3P%',
       'Team FT', 'Team FTA', 'Team FT%', 'Team ORB', 'Team TRB', 'Team AST',
       'Team STL', 'Team BLK', 'Team TOV', 'Team PF', 'Opponent FG',
       'Opponent FGA', 'Opponent FG%', 'Opponent 3P', 'Opponent 3PA',
       'Opponent 3P%', 'Opponent FT', 'Opponent FTA', 'Opponent FT%',
       'Opponent ORB', 'Opponent TRB', 'Opponent AST', 'Opponent STL',
       'Opponent BLK', 'Opponent TOV', 'Opponent PF']
