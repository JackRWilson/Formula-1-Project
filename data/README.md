
# Intermediate CSVs

This folder contains the various stages of CSVs used in the analysis and cleaning process.

| Folder                   | Description                                                                                                   | Columns                                      |
| --------------------------- | ------------------------------------------------------------------------------------------------------------- | ---------------------------------------------|
| raw | Driver ranks for each season, used to merge into the final analysis dataset                                   | `year`, `season_rank`, `driver`              |
| intermediate | Raw end position split into end position and position status, used to merge into raw dataset                  | `race_url`, `raw_end_position`, `end_position`, `position_status`, `driver`, `team_name`, `laps_completed`, `time_gap`, `points` |
| final | Fully merged but unclean dataframe, merging winners, results, starts, fastest laps, pit info, and driver info |
