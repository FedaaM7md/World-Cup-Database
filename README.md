# World Cup Database

A freeCodeCamp Relational Database project: Bash scripts that load World Cup results into PostgreSQL and answer questions about them with SQL.

## Files

- `worldcup.sql` - database dump with the `teams` and `games` tables
- `insert_data.sh` - reads `games.csv` and inserts every team and game, avoiding duplicate teams
- `queries.sh` - runs the analysis queries (goal totals and averages, champions by year, teams per round and more)

## Tech

Bash, PostgreSQL, SQL (joins, aggregates, `UNION`, `ON CONFLICT`)

## Run

```bash
psql -U postgres < worldcup.sql
./insert_data.sh
./queries.sh
```
