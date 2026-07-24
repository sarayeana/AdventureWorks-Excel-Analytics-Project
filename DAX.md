# DAX KPI Measures

## Sales KPIs

### Total Sales

```DAX
Total Sales :=
SUM(Sales[Sales])
```

### Total Cost

```DAX
Total Cost :=
SUM(Sales[Cost])
```

### Total Profit

```DAX
Total Profit :=
[Total Sales] - [Total Cost]
```

### Profit Margin

```DAX
Profit Margin :=
DIVIDE(
    [Total Profit],
    [Total Sales],
    0
)
```

### Total Orders

```DAX
Total Orders :=
DISTINCTCOUNT(Sales[SalesOrderNumber])
```

### Total Quantity Sold

```DAX
Total Quantity Sold :=
SUM(Sales[Quantity])
```

### Average Order Value

```DAX
Average Order Value :=
DIVIDE(
    [Total Sales],
    [Total Orders],
    0
)
```

---

## Product KPIs

### Top Product by Sales

```DAX
Top Product by Sales :=
MAXX(
    TOPN(
        1,
        ALL(Product[Product]),
        [Total Sales],
        DESC
    ),
    Product[Product]
)
```

### Top Product by Profit

```DAX
Top Product by Profit :=
MAXX(
    TOPN(
        1,
        ALL(Product[Product]),
        [Total Profit],
        DESC
    ),
    Product[Product]
)
```

### Top Category

```DAX
Top Category :=
MAXX(
    TOPN(
        1,
        ALL(Product[Category]),
        [Total Sales],
        DESC
    ),
    Product[Category]
)
```

### Top Subcategory

```DAX
Top Subcategory :=
MAXX(
    TOPN(
        1,
        ALL(Product[Subcategory]),
        [Total Sales],
        DESC
    ),
    Product[Subcategory]
)
```

---

## Reseller KPIs

### Top Reseller

```DAX
Top Reseller :=
MAXX(
    TOPN(
        1,
        ALL(Reseller[Reseller]),
        [Total Sales],
        DESC
    ),
    Reseller[Reseller]
)
```

### Top Business Type

```DAX
Top Business Type :=
MAXX(
    TOPN(
        1,
        ALL(Reseller[Business Type]),
        [Total Sales],
        DESC
    ),
    Reseller[Business Type]
)
```

### Average Sales per Reseller

```DAX
Average Sales per Reseller :=
DIVIDE(
    [Total Sales],
    DISTINCTCOUNT(Reseller[ResellerKey]),
    0
)
```

---

## Regional KPIs

### Top Region

```DAX
Top Region :=
MAXX(
    TOPN(
        1,
        ALL(Region[Region]),
        [Total Sales],
        DESC
    ),
    Region[Region]
)
```

### Top Country

```DAX
Top Country :=
MAXX(
    TOPN(
        1,
        ALL(Region[Country]),
        [Total Sales],
        DESC
    ),
    Region[Country]
)
```

### Top Territory

```DAX
Top Territory :=
MAXX(
    TOPN(
        1,
        ALL(Region[SalesTerritoryKey]),
        [Total Sales],
        DESC
    ),
    Region[SalesTerritoryKey]
)
```

---

## Employee KPIs

### Top Salesperson

```DAX
Top Salesperson :=
MAXX(
    TOPN(
        1,
        ALL(Salesperson[Salesperson]),
        [Total Sales],
        DESC
    ),
    Salesperson[Salesperson]
)
```

### Salesperson Target

```DAX
Salesperson Target :=
SUM(Targets[Target])
```

### Actual Sales

```DAX
Actual Sales :=
[Total Sales]
```

### Target Achievement %

```DAX
Target Achievement % :=
DIVIDE(
    [Actual Sales],
    [Salesperson Target],
    0
)
```
