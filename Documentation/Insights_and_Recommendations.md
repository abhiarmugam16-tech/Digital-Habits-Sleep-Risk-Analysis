# Insights & Recommendations

## Descriptive Findings from the Uploaded CSV

The following values were produced during the earlier analysis of the uploaded dataset. Recalculate and validate them in the final Power BI model before formal reporting.

| Sleep risk category | Records | Share of total | Avg. sleep duration (hrs) | Avg. sleep quality | Avg. stress |
|---|---:|---:|---:|---:|---:|
| Healthy | 54,156 | 54.16% | 6.93 | 5.77 | 5.04 |
| Mild | 33,479 | 33.48% | 6.05 | 4.17 | 6.32 |
| Moderate | 8,299 | 8.30% | 5.41 | 3.12 | 7.05 |
| Severe | 4,066 | 4.07% | 4.84 | 2.29 | 7.48 |

### Key Observations

1. **Healthy category is the largest group:** 54,156 records (approximately 54.16%) are classified as Healthy.
2. **Moderate and Severe categories:** Together they represent 12,365 records (approximately 12.37%).
3. **Sleep duration differs by category:** The average is 6.93 hours in Healthy records and 4.84 hours in Severe records.
4. **Stress differs by category:** Average stress ranges from 5.04 in Healthy to 7.48 in Severe.
5. **Sleep quality differs by category:** Average quality ranges from 5.77 in Healthy to 2.29 in Severe.

These observations are descriptive associations within this dataset. They do not show that stress or sleep duration causes a particular risk classification.

## Recommendations

| # | Recommendation | Proposed action | Intended value |
|---:|---|---|---|
| 1 | Review higher-risk groups | Segment Moderate and Severe records by occupation, age, shift work, and lifestyle | Identify where additional investigation may be useful |
| 2 | Explore stress patterns | Compare stress by occupation and sleep outcomes | Inform workplace wellness discussions |
| 3 | Promote bedtime-habit awareness | Explore screen time, caffeine, and alcohol patterns and provide general sleep-hygiene education | Support informed lifestyle choices |
| 4 | Review work-pattern differences | Compare sleep duration and quality across occupations and shift-work status | Identify potential work-schedule concerns |
| 5 | Monitor indicators over time | Track average duration, quality, stress, rested share, and risk distribution in future data | Evaluate changes consistently |

## Evaluation Approach

Where real-world follow-up data exists, define a baseline, document the wellness initiative, and monitor the same KPIs at regular intervals. Consider other factors that may affect changes. Before-and-after differences alone do not prove an intervention caused an outcome.

## Limitations

- Dataset category definitions and scoring methodology should be checked against the source.
- Confirm whether the dataset is synthetic before describing results as representative of a real population.
- Results are descriptive and should not be used as medical diagnoses.
- The analysis does not establish causal relationships.
- Occupational averages should be interpreted alongside record counts.
