# Data Cleaning & Preparation

## Objective

Prepare the CSV for reliable Power BI analysis while preserving valid observations and documenting transformations.

## Initial Checks

The initial inspection of the uploaded project CSV reported 100,000 rows, 32 columns, no missing values, and no exact duplicate rows. Repeat these checks after importing the file into Power BI.

## Recommended Power Query Workflow

1. **Import:** Home → Get Data → Text/CSV.
2. **Inspect:** Open Transform Data and review column names, profiling, and sample values.
3. **Set types:** Assign whole-number, decimal, date, text, and binary/category types based on actual values.
4. **Null checks:** Use Column Quality and filter for null/blank values.
5. **Duplicate checks:** Check exact duplicates and separately test whether `person_id` is unique. Do not remove records solely because a person appears more than once unless the dataset grain requires one row per person.
6. **Category standardization:** Trim whitespace and standardize spelling/capitalization where inconsistent.
7. **Range validation:** Check age, sleep hours, percentages, scores, steps, duration fields, and binary indicators against documented valid ranges.
8. **Outlier review:** Investigate unusual values; do not automatically delete legitimate extremes.
9. **Derived groups:** Create age bands, screen-time bands, stress bands, and night-awakening groups with documented thresholds.
10. **Apply:** Close & Apply and verify row counts after transformations.

## Useful Power Query Operations

- Change Type
- Column Quality / Column Distribution
- Trim and Clean
- Replace Values
- Remove Duplicates (only when justified)
- Conditional Column
- Filter Rows
- Keep/Remove Columns

## Tableau Alternative

Use the Data Source page to review fields and data types, aliases to standardize category labels, filters to inspect invalid values, and calculated fields for derived groups.

## Data Preparation Log Template

| Step | Issue / check | Action | Reason |
|---|---|---|---|
| 1 | Field data types | Verify and correct types | Ensure calculations behave correctly |
| 2 | Missing values | Check each relevant field | Avoid silent omissions |
| 3 | Duplicate rows | Verify exact duplicates | Prevent double counting |
| 4 | Identifier uniqueness | Test `person_id` | Confirm record grain |
| 5 | Categories | Standardize labels if needed | Consistent grouping |
| 6 | Range validation | Investigate invalid values | Improve reliability |
| 7 | Derived groups | Create documented bands | Enable comparisons |

Record the actual action taken and before/after row counts in the final report. Do not claim a transformation was performed unless completed.
