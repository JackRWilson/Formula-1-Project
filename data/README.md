
# Folder Overview

This folder contains the various stages of CSVs used in the analysis and cleaning process.

| Folder       | Description                                                                  |
| ------------ | ---------------------------------------------------------------------------- |
| raw          | Raw files from scraping                                                      |
| intermediate | Files that have been altered or enriched, used later in the analysis process |
| final        | Clean and analysis ready files                                               |

# Data Overview

- All data was scraped from the [Official F1 Results Website](https://www.formula1.com/en/results/2025/races)

- Data was scraped from all races years 1950 - 2024

### Final Analysis Data

- The final analysis data contains 3510 rows and 50 features. Each row represents a driver's aggregated performance across all races in a given season. Many of the features are engineered based on existing columns to improve machine learning and other analysis. 

### Data Dictionary

| Column                    | Description                                                              |
| ------------------------- | ------------------------------------------------------------------------ |
| `year`                    | The season year                                                          |
| `driver`                  | Driver name                                                              |
| `team_name`               | Name of the constructor/team                                             |
| `continent`               | Continent of the driver                                                  |
| `season_rank`             | Driver’s final rank in the season                                        |
| `avg_start_pos`           | Average start position across the season                                 |
| `std_start_pos`           | Standard deviation of starting positions                                 |
| `best_start_pos`          | Best start position                                                      |
| `worst_start_pos`         | Worst start position                                                     |
| `races_participated`      | Number of races competed in                                              |
| `avg_finish_pos`          | Average finishing position                                               |
| `std_finish_pos`          | Standard deviation of finishing positions                                |
| `best_finish_pos`         | Best race finish                                                         |
| `worst_finish_pos`        | Worst race finish                                                        |
| `total_pos_gain`          | Total positions gained from start to finish across all races             |
| `avg_pos_gain`            | Average position gain per race                                           |
| `total_points`            | Total points scored                                                      |
| `avg_points_per_race`     | Average points scored per race                                           |
| `total_pct_season_points` | Percentage of total available season points earned                       |
| `avg_pct_season_points`   | Average percentage of available season points per race                   |
| `worst_pct_season_points` | Lowest points percentage in a race                                       |
| `best_pct_season_points`  | Highest points percentage in a race                                      |
| `total_laps_completed`    | Number of laps completed                                                 |
| `total_laps`              | Total laps possible                                                      |
| `total_fastest_laps`      | Number of fastest laps earned                                            |
| `CLAS_total`              | Number of classified finishes                                            |
| `DNF_total`               | Number of Did Not Finish results                                         |
| `DNS_total`               | Number of Did Not Start results                                          |
| `DQ_total`                | Number of Disqualified results                                           |
| `NC_total`                | Number of Not Classified results                                         |
| `backmarker`              | Backmarker indication                                                    |
| `midfield`                | Midfielder indication                                                    |
| `podium_regular`          | Podium regular indication                                                |
| `points_regular`          | Points regular indication                                                |
| `years_experience`        | Number of years the driver has competed in                               |
| `total_podium_finishes`   | Total podium finishes in the season                                      |
| `total_points_finishes`   | Total points finishes in the season                                      |
| `dnf_rate`                | Percentage of DNFs over races entered                                    |
| `finish_rate`             | Percentage of races finished                                             |
| `lap_completion_rate`     | Percentage of laps completed                                             |
| `fastest_lap_rate`        | Fastest laps as a percentage of races entered                            |
| `podium_rate`             | Podium finishes as a percentage of races entered                         |
| `points_rate`             | Points finishes as a percentage of races entered                         |
| `consistency_score`       | Consistency in finish positions                                          |
| `qualifying_consistency`  | Consistency in start positions                                           |
| `reliability_score`       | Measures a drivers finish rate with lap completion rate                  |
| `qualifying_vs_race`      | Comparison of qualifying vs finishing positions                          |
| `championship_impact`     | How strongly the driver contributed to the championship outcome          |
| `race_improvement`        | Average improvement from start to finish positions                       |
| `driver_retained`         | Whether the driver was retained by the team for the next season          |
