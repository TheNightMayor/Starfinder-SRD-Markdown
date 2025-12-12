---
cssclasses:
aliases: []
tags: []
---

# Public Items & Service

Beyond weapons, armor, and crucial technological, magical, and hybrid equipment, explorers and adventurers need food, clothing, survival supplies, and other basic gear. Characters can also spend their hard-earned credits on lodging, services, and transportation. The equipment and services in this section are not considered technological or magical unless they specify otherwise.

## Food & Drinks

``` dataview
TABLE
Category, Price
FROM "Compendium/SF1E/Items/Public Items/Food, Drinks, Lodgings"
SORT Category ASC
```

## Transportation

``` dataview
TABLE
Price, type
FROM "Compendium/SF1E/Items/Public Items/Transportation"
WHERE !contains(file.name, "Transportation")
SORT Category ASC
```

## Trade Goods

``` dataview
TABLE
Category, Price
FROM "Compendium/SF1E/Items/Public Items/Trade Goods"
SORT Category ASC
```

## Recharging Stations

``` dataview
TABLE
Category, Price
FROM "Compendium/SF1E/Items/Public Items/Recharging Stations"
```

## Personal Items

``` dataview
TABLE
Category, Price
FROM "Compendium/SF1E/Items/Public Items/Personal Items"
```

## Professional Services

``` dataview
TABLE
Category, Price
FROM "Compendium/SF1E/Items/Public Items/Professional Services"
```

## Medicinals

``` dataview
TABLE
Category, Price
FROM "Compendium/SF1E/Items/Public Items/Medicinals"
```
