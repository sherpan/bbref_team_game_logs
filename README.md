# bbref_team_game_logs
This python package scrapes Basketball Reference to return a team's game log for an entire NBA season. 

# Installing this package 
1. git clone https://github.com/sherpan/bbref_team_game_logs.git
2. cd bbref_team_game_logs
3. pip install . 

# API
  ## get_team_game_logs(team,season_end_year)
    Parameters:
    team: NBA team abbreiviation (PHO,DAL)
    season_end_year: The year an NBA season ends (2005 for the 04-05 season)
    Returns:
    A panda data fram with the following columns 
