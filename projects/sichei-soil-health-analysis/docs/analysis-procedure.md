# Step-by-step Excel procedure

This procedure reproduces the first-pass descriptive analysis from the 160-row Sichei subset. If your Excel uses commas instead of semicolons as argument separators, replace each semicolon with a comma. Check the actual column headings before running formulas.

## 1. Preserve the source

Keep an untouched copy of the original workbook. Perform filtering and analysis in a separate sheet or file. The current working sheet is named `Sichei_Only`; the ranges below cover rows 2–161 (160 data rows).

## 2. Initial quality checks

**Count rows in the selected range**

```excel
=ROWS('Sichei_Only'!$DN$2:$DN$161)
```

**Count nonblank record IDs in KEY (column DN)**

```excel
=COUNTA('Sichei_Only'!$DN$2:$DN$161)
```

**Count rows labelled Sichei (Site in column E)**

```excel
=COUNTIF('Sichei_Only'!$E$2:$E$161;"Sichei")
```

**Count blank fallow values (column DL)**

```excel
=COUNTBLANK('Sichei_Only'!$DL$2:$DL$161)
```

**Count rows with repeated KEY identifiers**

First put this in `Analysis_Data` (or another helper sheet) in the first data row, adjusting the referenced KEY cell if necessary:

```excel
=COUNTIF($DN$2:$DN$161;DN2)
```

Fill down. A result greater than 1 flags an identifier that appears more than once; investigate rather than automatically deleting records.

## 3. Land-use frequencies

The `landuse` field is in column DR in the current workbook. List the exact category labels in a summary sheet.

**Count records matching the category in A5**

```excel
=COUNTIF('Sichei_Only'!$DR$2:$DR$161;A5)
```

**Calculate the share of nonblank land-use records**

```excel
=IFERROR(B5/COUNTA('Sichei_Only'!$DR$2:$DR$161);0)
```

Format the percentage cell as Percentage. Repeat for each category. To make a chart, select the category and count columns and choose Insert → Bar Chart.

## 4. Management-practice frequencies

The current columns are: `fym` = DI, `inorg_fert` = DK, `fallow` = DL, and `brnt` = DM. Verify these locations in the workbook before use.

**Count yes responses in fym**

```excel
=COUNTIF('Sichei_Only'!$DI$2:$DI$161;"yes")
```

**Count no responses in fym**

```excel
=COUNTIF('Sichei_Only'!$DI$2:$DI$161;"no")
```

**Count missing fym values**

```excel
=COUNTBLANK('Sichei_Only'!$DI$2:$DI$161)
```

**Percent yes among valid yes/no responses**

If the yes count is in F5 and no count in G5:

```excel
=IFERROR(F5/(F5+G5);0)
```

For `inorg_fert`, replace column DI with DK. For `fallow`, replace DI with DL and report missing records separately; blanks are not “no.”

## 5. Compare management practices across land-use categories

List the exact land-use categories in H2:H9.

**Count records per category**

```excel
=COUNTIF('Sichei_Only'!$DR$2:$DR$161;H2)
```

**Count category records with fym=yes**

```excel
=COUNTIFS('Sichei_Only'!$DR$2:$DR$161;H2;'Sichei_Only'!$DI$2:$DI$161;"yes")
```

**Calculate the percentage of valid records in that category with fym=yes**

If I2 is the count of valid responses, J2 the yes count:

```excel
=IFERROR(J2/I2;0)
```

Repeat for inorganic fertilizer by changing the practice column from DI to DK. Use valid responses as the denominator; do not treat blanks as no.

## 6. Erosion-field checks

In this workbook, `visEros` is column BK, `Erosion3` is column BE, and `SEVEREROS` is column BL. Confirm the locations and code definitions in the official code-description file.

**Count visEros code 0**

```excel
=COUNTIF('Sichei_Only'!$BK$2:$BK$161;0)
```

**Count visEros code 1**

```excel
=COUNTIF('Sichei_Only'!$BK$2:$BK$161;1)
```

**Count Erosion3=gully**

```excel
=COUNTIF('Sichei_Only'!$BE$2:$BE$161;"gully")
```

**Count Erosion3=none**

```excel
=COUNTIF('Sichei_Only'!$BE$2:$BE$161;"none")
```

Describe these as recorded values until code definitions are confirmed. With only two positive records in the current subset, do not force standard inferential tests on this outcome.

## 7. PivotTable alternative

1. Select the data table.
2. Choose Insert → PivotTable → New Worksheet.
3. Drag `landuse` to Rows and `KEY` to Values.
4. Set the value calculation to Count, not Sum.
5. To compare practices, add `fym` to Columns.
6. For percentages, right-click a count → Show Values As → % of Row Total.

## 8. Quality and interpretation rules

- Keep raw records unchanged; document cleaning in a log.
- Do not convert blank cells to zero or no unless the codebook explicitly defines that convention.
- Confirm exact definitions of abbreviations, code values, and units before substantive interpretation.
- Describe counts and percentages as properties of this working sample; do not generalize beyond its sampling design.
- Do not infer causation from descriptive cross-tabs.
- Recheck every summary against the workbook before publishing.
