# understat-api
API for accessing data from understat.com

## Links
- [understat.com](https://understat.com/)
  - [(league, season) page](https://understat.com/league/EPL/2023)
    - can extract match data from page source. look for script containing `vars datesData = JSON.parse`
    - can similarly find player and team aggregate stats under `teamsData` and `playersData`
  - [(team, season) page](https://understat.com/team/Wolverhampton_Wanderers/2023)
  - [match page](https://understat.com/match/21927)
    - can extract shots data from page source. look for script containing `var shotsData = JSON.parse`
    - can similarly find some match stats (xG perteam, etc) and roster info under `match_info` and `rosterData`
  - [player page](https://understat.com/player/8260)

## Core Data Structures
- `League` - e.g. EPL
- `LeagueSeason` - e.g. EPL 2023
- `Team` - e.g. Liverpool
- `TeamSeason` - e.g. Liverpool 2023
- `Match` - e.g. Liverpool vs Manchester City, 2023-01-01
