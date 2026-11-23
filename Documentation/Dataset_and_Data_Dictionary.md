# Dataset & Data Dictionary

## Dataset Summary

- **Dataset:** Sleep Health and Daily Performance Dataset
- **Source:** [Kaggle dataset page](https://www.kaggle.com/datasets/mohankrishnathalla/sleep-health-and-daily-performance-dataset)
- **Analyzed file:** `sleep_health_dataset(2).csv`
- **Reported shape:** 100,000 rows × 32 columns
- **Domain:** Sleep health, lifestyle, and daily performance
- **Format:** CSV

Use the Kaggle page as the canonical source and verify its data dictionary, license, and dataset description before redistribution. The raw CSV is not committed in this repository update.

## Fields Referenced in the Analysis

| Field | Expected role / type | Analysis purpose |
|---|---|---|
| `person_id` | Identifier / integer | Record count and detail |
| `age` | Numeric | Age-group segmentation |
| `gender` | Categorical | Demographic filtering |
| `occupation` | Categorical | Occupational comparisons |
| `country` | Categorical | Geographic segmentation |
| `sleep_duration_hrs` | Numeric / decimal | Average sleep duration |
| `sleep_quality_score` | Numeric / decimal | Sleep quality analysis |
| `stress_score` | Numeric / decimal | Stress analysis |
| `sleep_latency_mins` | Numeric | Time taken to fall asleep |
| `screen_time_before_bed_mins` | Numeric | Digital-habit analysis |
| `caffeine_mg_before_bed` | Numeric | Bedtime caffeine analysis |
| `alcohol_units_before_bed` | Numeric | Bedtime alcohol analysis |
| `steps_that_day` | Numeric | Activity indicator |
| `sleep_disorder_risk` | Categorical | Risk-category comparison |
| `cognitive_performance_score` | Numeric / decimal | Cognitive performance comparison |
| `felt_rested` | Binary / categorical | Perceived-rest analysis |
| `wake_episodes_per_night` | Numeric | Night-awakening analysis |
| `shift_work` | Categorical / binary | Work-pattern segmentation |
| `chronotype` | Categorical | Sleep-preference segmentation |
| `season` | Categorical | Seasonal segmentation |

Additional fields include BMI, REM and deep-sleep percentages, exercise, naps, work hours, mental-health indicators, resting heart rate, sleep-aid use, room temperature, weekend sleep difference, and day type. Confirm exact names and types against the CSV.

## Data Quality Notes

The initial inspection of the uploaded CSV reported:
- 100,000 rows and 32 columns.
- No missing values.
- No exact duplicate rows.

Recheck these properties in Power Query. Also inspect identifier uniqueness, allowed category values, invalid measurements, and outliers.

## Dataset Use and Licensing

The repository links to Kaggle rather than redistributing the raw dataset. Check the dataset's license and terms before uploading a copy. Public availability does not automatically mean unrestricted redistribution.
