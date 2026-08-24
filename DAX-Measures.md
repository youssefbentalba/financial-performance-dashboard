# DAX Measures

This document contains the main DAX measures used in the FP&A Financial Performance Dashboard.

## Revenue

### Total Revenue

```DAX
Total Revenue =
SUM('DATA V2'[Revenue])

Total Budget Revenue =
SUM('DATA V2'[Budget Revenue])

Revenue Variance DAX =
[Total Revenue] - [Total Budget Revenue]

Revenue Variance % DAX =
DIVIDE(
    [Revenue Variance DAX],
    [Total Budget Revenue],
    0
)

Total COGS =
SUM('DATA V2'[COGS])

Total Budget COGS =
SUM('DATA V2'[Budget COGS])

COGS Variance DAX =
[Total COGS] - [Total Budget COGS]

COGS Variance % DAX =
DIVIDE(
    [COGS Variance DAX],
    [Total Budget COGS],
    0
)

Total OPEX =
SUM('DATA V2'[OPEX])

Total Budget OPEX =
SUM('DATA V2'[Budget OPEX])

OPEX Variance DAX =
[Total OPEX] - [Total Budget OPEX]

OPEX Variance % DAX =
DIVIDE(
    [OPEX Variance DAX],
    [Total Budget OPEX],
    0
)

EBITDA DAX =
[Total Revenue] - [Total COGS] - [Total OPEX]

EBITDA Margin % DAX =
DIVIDE(
    [EBITDA DAX],
    [Total Revenue],
    0
)


**Important :** si tes mesures Power BI ont des noms légèrement différents, garde les noms qui existent réellement dans ton `.pbix`.

Ensuite clique sur **Commit changes...** et mets :

```text
Add DAX measures documentation
