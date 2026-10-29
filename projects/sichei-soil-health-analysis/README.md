# Sichei Soil Health: Exploratory Land-Use and Erosion Analysis

**Status:** Exploratory descriptive analysis; variable-code verification and final interpretation remain in progress.

## Project overview

This project uses a Sichei-only subset of a public ICRAF soil and land-health dataset to describe recorded land-use categories, selected management-practice fields, and recorded erosion indicators. It is designed as a transparent agricultural-research workflow: audit the data, document variables, summarize patterns, and avoid conclusions that the available data cannot support.

### Research question

> How are land-use categories and selected land-management practices associated with recorded erosion indicators among the Sichei plot records represented in the working dataset?

This is an exploratory association question, not a causal-impact question.

## Dataset and attribution

The source is:

Winowiecki, L. A., Thiongo Maina, J., Bargués-Tobella, A., Otieno Onyango, J., Dennis, N., Kersting, D., & Vågen, T.-G. (2022). *Spatial Assessments of Changes in Soil Health Indicators in Kenya* (Version 2.1). World Agroforestry (ICRAF). https://doi.org/10.34725/DVN/MR2COM

The source record lists the file `table_plotproperties_Kenya_cleaned_dataversecsv.tab` as containing 131 variables and 316 observations in the full dataset. The analysis documented here uses **160 records labelled Sichei** in the current working subset. These are different dimensions: 131 fields/columns in the source file versus 160 Sichei records in this working extract.

The source dataset is made available under **CC BY 4.0**. Please cite the authors and dataset, link to the licence, and identify modifications when reusing data. The raw data are not copied into this repository; obtain them from the official DOI above.

## Preliminary descriptive results

The current 160-record working subset contains:

| Land-use category | Records | Share of sample |
|---|---:|---:|
| Annual agroforestry | 79 | 49.4% |
| Annual crop | 45 | 28.1% |
| Perennial agroforestry | 14 | 8.8% |
| Perennial crop | 10 | 6.3% |
| Woodlot | 4 | 2.5% |
| Pasture/rangeland | 4 | 2.5% |
| Fallow | 3 | 1.9% |
| Other | 1 | 0.6% |

The two largest categories—annual agroforestry and annual crop—account for 124/160 records (77.5%).

Selected management fields as recorded:

- `fym`: 19 yes, 141 no, 0 blank (11.9% yes).
- `inorg_fert`: 134 yes, 26 no, 0 blank (83.8% yes).
- `fallow`: 3 yes, 151 no, 6 blank. Among 154 valid yes/no responses, 1.9% are yes.
- `brnt`: all 160 rows are coded no; the field has no observed variation in this subset.
- `SWCStructures`: recorded codes are 0 (118), 1 (29), 2 (8), and 3 (5).

Recorded erosion-field values are sparse: `visEros` is coded 1 in 2 records and 0 in 158; `Erosion3` is `gully` in 2 records and `none` in 158. Other selected erosion fields show little or no variation in this working subset.

**These are preliminary descriptions of recorded codes, not verified statements about true erosion prevalence or causes.** Code meanings, measurement definitions, units, and the companion LDSF code descriptions must be confirmed before final interpretation.

## Methods and reproducibility

1. Preserve the source and working data; do not overwrite raw observations.
2. Filter a separate analysis subset to records whose `Site` value is exactly `Sichei`.
3. Audit IDs, site labels, missing values, duplicate keys, and data types.
4. Create a first-pass data dictionary and flag provisional definitions.
5. Calculate category counts and percentages using Excel formulas or PivotTables.
6. Treat blanks as unknown, not as a recorded “no.”
7. Summarize erosion fields before deciding whether statistical comparisons are appropriate.
8. Record every cleaning decision and report data limitations.

See the project documentation:
- [Step-by-step Excel procedure and formulas](docs/analysis-procedure.md)
- [Findings and limitations](docs/findings-and-limitations.md)
- [Selected variable dictionary](docs/selected-data-dictionary.md)
- [Citation and licence notes](CITATION.md)

## Key limitation

Only two records in the working subset are coded as positive in `visEros`, and only two are recorded as `gully` in `Erosion3`. This offers too little outcome variation for a robust comparison of erosion across land-use groups using conventional inferential models. The project therefore reports descriptive patterns and does not claim causal effects.

Before publication, verify the source code-description file and measurement definitions. If an appropriate soil-health outcome with adequate variation is available, revise the analysis question and method to fit that outcome.

## Tools

Excel formulas, frequency tables, cross-tabulations, data-quality checks, descriptive statistics, and documented research interpretation.

## Research integrity

This repository does not reproduce the raw source dataset. All numbers above describe the current Sichei working subset and should be rechecked against the validated analysis workbook before external publication. The analysis is independent and does not imply endorsement by ICRAF or the dataset authors.
