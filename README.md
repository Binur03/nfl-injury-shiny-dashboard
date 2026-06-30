# NFL Injury Shiny Dashboard (Team 6)

An R Shiny dashboard exploring NFL injury data (2010–2024) with predictive models
(XGBoost, random forest, and LASSO).

## Features explored
- Turf vs. grass
- Play type
- Regular season vs. playoff
- Type of injury
- Yards
- Positions
- Defense vs. offense vs. special teams
- Seconds remaining
- Stadium
- Down

## Repository contents
- `Updated Shiny Shell 2010-2024.Rmd` — main Shiny app (2010–2024 data).
- `Updated Shiny Shell.Rmd`, `Shiny Shell Original.Rmd`, `CopyOfUpdatedShinyShell.Rmd` — earlier/variant versions of the app.
- `Creating Models RDS.Rmd` — trains the models and saves them as `.rds` files.
- `2010-2024csvmaker.Rmd` — builds `master_data.csv` from the source data.
- `rds files 2/`, `rds files original/`, `updated rds files/` — saved trained models.
- `2024-2010_Data.csv` — supporting data.

## Note on `master_data.csv`
The full `master_data.csv` (~91 MB) is **not** included in this repository because it
exceeds GitHub's file-size limits for standard uploads. To recreate it, run
`2010-2024csvmaker.Rmd`, which writes `master_data.csv` to the project root. The Shiny
apps and `Creating Models RDS.Rmd` expect this file to be present locally.
