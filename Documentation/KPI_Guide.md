# KPI Definitions & Dashboard Guide

## KPIs Displayed in the Supplied Dashboard

| KPI | Displayed value | Suggested definition |
|---|---:|---|
| Total Count | 100K | Count of records / person IDs |
| Average Sleep Quality | 4.87 | Average of `sleep_quality_score` |
| Average Stress Score | 5.73 | Average of `stress_score` |
| Average Cognitive Performance | 59.23 | Average of `cognitive_performance_score` |
| Average Sleep Hours | 6.42 | Average of `sleep_duration_hrs` |

Confirm aggregation, filter context, and whether person_id is unique in the final Power BI model.

## Additional Recommended KPIs

- High-Risk Records: records classified as Moderate or Severe.
- High-Risk Percentage: High-Risk Records divided by Total Records.
- Rested Percentage: records with `felt_rested = 1` divided by Total Records.
- Average Cognitive Performance by Risk Category.
- Average Sleep Duration by Occupation or Age Group.

## Power BI DAX Measures

Assumes the model table is named `sleep_health_dataset` and risk labels match exactly.

```dax
Total Records =
COUNT(sleep_health_dataset[person_id])

Average Sleep Duration =
AVERAGE(sleep_health_dataset[sleep_duration_hrs])

Average Sleep Quality =
AVERAGE(sleep_health_dataset[sleep_quality_score])

Average Stress Score =
AVERAGE(sleep_health_dataset[stress_score])

Average Cognitive Performance =
AVERAGE(sleep_health_dataset[cognitive_performance_score])

High Risk Records =
CALCULATE(
    [Total Records],
    sleep_health_dataset[sleep_disorder_risk]
        IN {"Moderate", "Severe"}
)

High Risk Percentage =
DIVIDE([High Risk Records], [Total Records], 0)

Rested Records =
CALCULATE(
    [Total Records],
    sleep_health_dataset[felt_rested] = 1
)

Rested Percentage =
DIVIDE([Rested Records], [Total Records], 0)
```

Format the percentage measures as Percentage in Power BI; do not multiply by 100 when percentage formatting is applied.

## Dashboard Filters

The supplied dashboard screenshot shows filters for Gender, Occupation, and Sleep Disorder Risk. Additional recommended filters include age group, season, and country.
