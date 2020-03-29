# bbref_team_game_logs
This python package scrapes Basketball Reference to return a team's game log for an entire NBA season. 

## Installing this package 
1. git clone https://github.com/sherpan/bbref_team_game_logs.git
2. cd bbref_team_game_logs
3. pip install . 

## API
  ### get_team_game_logs(team,season_end_year)
   #### Parameters:
   * team: abbreviation for NBA team i.e(PHO,DAL,BOS)
   * season_end_year: end year of an NBA season (2005 for the 2004-2005 season)
   #### Returns
   A pandas data frame with the following columns
   
  ```python
import foobar

foobar.pluralize('word') # returns 'words'
foobar.pluralize('goose') # returns 'geese'
foobar.singularize('phenomena') # returns 'phenomenon'
```
