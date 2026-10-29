# Findings and limitations

## Sample and scope

- Current analysis subset: 160 rows in `Sichei_Only`.
- All 160 rows are labelled `Site = Sichei`.
- The current sample has 131 fields/columns in the worksheet.
- These figures describe this prepared subset, not the full source dataset.

## Land-use distribution

| Category | n | Percentage |
|---|---:|---:|
| annual_agroforestry | 79 | 49.4% |
| annual_crop | 45 | 28.1% |
| perennial_agroforestry | 14 | 8.8% |
| perennial_crop | 10 | 6.3% |
| woodlot | 4 | 2.5% |
| pasture_rangeland | 4 | 2.5% |
| fallow | 3 | 1.9% |
| other | 1 | 0.6% |
| **Total** | **160** | **100% before rounding** |

The two largest categories total 124 records, or 77.5% of this subset. Individual percentages are rounded to one decimal place, so displayed percentages may not add exactly to 100.0%.

## Selected management fields

| Field | Yes | No | Blank | Yes among valid yes/no records |
|---|---:|---:|---:|---:|
| fym | 19 | 141 | 0 | 11.9% |
| inorg_fert | 134 | 26 | 0 | 83.8% |
| fallow | 3 | 151 | 6 | 1.9% |
| brnt | 0 | 160 | 0 | 0.0% |

Definitions are provisional until checked against the companion code descriptions. Percentages describe recorded responses in this sample, not quantities applied or effectiveness of a practice.

## Selected SWC fields

`SWCStructures` codes: 0 = 118; 1 = 29; 2 = 8; 3 = 5.

`SWCDescr` labels: none = 118; veg = 21; veg struc = 16; struc = 5.

Do not infer the meaning or order of numeric codes from their appearance alone; verify the codebook.

## Recorded erosion fields

- `visEros`: code 0 in 158 records; code 1 in 2 records.
- `Erosion3`: `none` in 158 records; `gully` in 2 records.
- `Erosion1`, `Erosion2`, and `Erosion4`: all 160 records are labelled `none` in the current subset.
- `SEVEREROS`: 0 in all 160 rows in the current copy.

These numbers describe stored codes only. Before calling them absence/presence of erosion, confirm definitions, field protocol, and valid codes in the official companion file.

## Interpretation and limitations

1. **Descriptive only:** the current analysis is frequencies, percentages, and cross-tabulations; no causal claim is supported.
2. **Low erosion variation:** only two positive `visEros` codes and two `gully` labels are present. This is too sparse to support a robust conventional comparison of erosion across land-use groups.
3. **Codebook verification is still needed:** field names and values alone do not fully establish the variable definitions, scales, units, or measurement protocol.
4. **Sampling representativeness is not established here:** the tables describe the current Sichei subset; they should not be treated as area-wide estimates without reviewing the sampling design.
5. **Missing values remain missing:** six `fallow` fields are blank; all `SoilConservation` entries are blank. They are not recoded as no.
6. **Source dataset licensing:** the source record identifies CC BY 4.0. Attribute the authors, link the source and licence, and note changes.
7. **No causal inference:** management patterns may reflect soil, slope, access, previous erosion, or other factors not controlled for in these summaries.

## Recommended next scientific action

Review the companion source file `ldsf_description of codesv5.tab` and relevant LDSF field documentation. Confirm variable definitions and units. Then decide whether a documented soil-health outcome with adequate variation can support a revised exploratory question. Do not run tests simply because they are available.
