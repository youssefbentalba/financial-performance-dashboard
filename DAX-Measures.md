# DAX Measures

This document contains the main DAX measures used in the FP&A Financial Performance Dashboard.

## 1. Total Revenue

```DAX
Total Revenue =
SUM('DATA'[Revenue])
```

---

## 2. Total Budget Revenue

```DAX
Total Budget Revenue =
SUM('DATA'[Budget Revenue])
```

---

## 3. Revenue Variance

```DAX
Revenue Variance DAX =
[Total Revenue] - [Total Budget Revenue]
```

---

## 4. Revenue Variance %

```DAX
Revenue Variance % DAX =
DIVIDE(
    [Revenue Variance DAX],
    [Total Budget Revenue],
    0
)
```

---

## 5. Total COGS

```DAX
Total COGS =
SUM('DATA'[COGS])
```

---

## 6. Total Budget COGS

```DAX
Total Budget COGS =
SUM('DATA'[Budget COGS])
```

---

## 7. COGS Variance

```DAX
COGS Variance DAX =
[Total COGS] - [Total Budget COGS]
```

---

## 8. COGS Variance %

```DAX
COGS Variance % DAX =
DIVIDE(
    [COGS Variance DAX],
    [Total Budget COGS],
    0
)
```

---

## 9. Total OPEX

```DAX
Total OPEX =
SUM('DATA'[OPEX])
```

---

## 10. Total Budget OPEX

```DAX
Total Budget OPEX =
SUM('DATA'[Budget OPEX])
```

---

## 11. OPEX Variance

```DAX
OPEX Variance DAX =
[Total OPEX] - [Total Budget OPEX]
```

---

## 12. OPEX Variance %

```DAX
OPEX Variance % DAX =
DIVIDE(
    [OPEX Variance DAX],
    [Total Budget OPEX],
    0
)
```

---

## 13. EBITDA

```DAX
EBITDA DAX =
[Total Revenue] - [Total COGS] - [Total OPEX]
```

---

## 14. EBITDA Margin %

```DAX
EBITDA Margin % DAX =
DIVIDE(
    [EBITDA DAX],
    [Total Revenue],
    0
)
```
