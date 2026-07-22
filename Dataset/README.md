## Dataset Description

The dataset was constructed to analyze the relationship between player performance and market valuation within the U-23 football transfer market.

The study focuses on league performance data from the 2025/26 season across Europe's five major leagues:

- English Premier League (EPL)
- La Liga
- Bundesliga
- Serie A
- Ligue 1

Only league-level performance data was considered in this analysis. Cup competitions, international matches, and other non-league competitions were excluded.

The dataset consists of U-23 players across three positional groups:

- Defenders
- Midfielders
- Forwards

Players were evaluated using position-specific performance metrics, market value information, and player profile characteristics.

The dataset includes variables related to:

### Player Profile
- Player age
- Club
- Position
- Market value
- Club reputation indicator

### Playing Time
- League minutes
- Normalized playing time (90-minute equivalent)

### Performance Metrics

Metrics were selected based on positional responsibilities:

**Defenders**
- Defensive actions
- Tackles won
- Recoveries
- Dispossessions

**Midfielders**
- Ball recoveries
- Interceptions
- Chance creation
- Expected assists

**Forwards**
- Expected goals
- Shots on target
- Dribbling output
- Expected assists

To ensure that the analysis focused on players with meaningful league contributions, the valuation models were trained using players with at least 10 normalized league appearances (90-minute equivalent).

Players below this threshold were analyzed separately to explore the relationship between limited league playing time and market valuation.
