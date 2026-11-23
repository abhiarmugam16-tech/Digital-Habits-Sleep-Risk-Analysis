# Dashboard Chart Guide

Professional chart titles and field mappings based on the supplied dashboard and analysis plan.

| # | Professional chart title | Suggested X-axis / category | Suggested Y-axis / value |
|---:|---|---|---|
| 1 | Sleep Risk Category Distribution | Sleep Risk Category | Record Count / % of Records |
| 2 | Average Stress Score by Occupation | Occupation | Average Stress Score |
| 3 | Sleep Quality by Stress Level and Night Awakening Category | Stress Score / Stress Band | Average Sleep Quality; use night-awakening category as legend |
| 4 | Average Cognitive Performance by Sleep Risk Category | Sleep Risk Category | Average Cognitive Performance Score |
| 5 | Lifestyle Risk Factor Count by Age | Age / Age Group | Lifestyle Risk Factor Count |
| 6 | Average Sleep Duration and Quality by Screen-Time Category | Screen-Time Category | Average Sleep Duration (hours) and Average Sleep Quality (score) |

## Chart Selection Notes

- For chart 6, use a combo chart with a secondary axis or separate charts because hours and quality scores have different units.
- For chart 3, use Average Sleep Quality rather than Sum when comparing groups with different record counts. A heatmap can work well with stress bands and night-awakening categories.
- For chart 2, sort occupations by average stress score descending and consider displaying Top 5 or Top 10. Show record counts in tooltips to add context.
- For chart 5, document the exact definition and thresholds used to count lifestyle risk factors.
- For chart 1, show both count and percentage in labels or tooltips where useful.

## Dashboard Design

Suggested slicers:
1. Gender
2. Occupation
3. Sleep Disorder Risk
4. Age Group (additional)
5. Season (additional)

Ensure all visuals respond to filters as intended and provide clear units, legends, and tooltip definitions.
