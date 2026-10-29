# Selected variable dictionary (first-pass)

This is a project-oriented short list, not the full 131-field dictionary. Definitions below are working descriptions; confirm against the source code-description file before using them substantively.

| Variable | Current worksheet column | Working role | Recorded values / issue | Verification required |
|---|---|---|---|---|
| `Site` | E | Site filter | All 160 selected rows labelled Sichei | Confirm source field and sample design |
| `KEY` | DN | Record identifier | Nonblank and unique in current subset | Confirm intended unit and uniqueness rule |
| `Cluster` | verify in workbook | Sampling structure | Cluster grouping used in audit | Confirm sampling design and how plots cluster |
| `Plot` | verify in workbook | Plot identifier | Used with cluster / key as context | Confirm uniqueness logic |
| `landuse` | DR | Explanatory category | 8 recorded categories | Confirm official category definitions |
| `fym` | DI | Management field | 19 yes, 141 no | Confirm meaning of FYM and coding |
| `inorg_fert` | DK | Management field | 134 yes, 26 no | Confirm exact question and coding |
| `fallow` | DL | Management field | 3 yes, 151 no, 6 blank | Confirm reference period and codes |
| `brnt` | DM | Management field | All 160 coded no | Confirm definition and coding |
| `SWCStructures` | BN | Conservation-related field | 0:118, 1:29, 2:8, 3:5 | Verify every numeric code |
| `SWCDescr` | verify in workbook | Text description | none:118, veg:21, veg struc:16, struc:5 | Verify categories/meaning |
| `visEros` | BK | Candidate erosion outcome | 0:158, 1:2 | Verify coding, observation protocol, missing codes |
| `Erosion1` | BC | Erosion field | `none` in all 160 rows | Verify what feature this field describes |
| `Erosion2` | BD | Erosion field | `none` in all 160 rows | Verify what feature this field describes |
| `Erosion3` | BE | Erosion field | `none`:158, `gully`:2 | Verify meaning and categories |
| `Erosion4` | BF | Erosion field | `none` in all 160 rows | Verify what feature this field describes |
| `SEVEREROS` | BL | Candidate severity field | 0 in all 160 rows | Verify scale, thresholds, and coding |
| `SoilConservation` | BM | Candidate management field | All 160 values blank | Check whether unavailable or intentionally unrecorded |
| `Altitude` | verify in workbook | Context / numerical field | Available in worksheet | Confirm units |
| `AvSlope` | verify in workbook | Context / numerical field | Numeric-looking entries cleaned in helper sheet | Confirm units and method |
| `SlopeDn` / `SlopeUp` | verify in workbook | Context / numerical field | Numeric-looking entries cleaned in helper sheet | Confirm definitions and units |

The source dataset provides a companion code-description file, `ldsf_description of codesv5.tab`, that should be used to verify codes. The source listing itself includes 131 variables and 316 observations in the full table; this project describes 160 Sichei-labelled records from the current working subset.
