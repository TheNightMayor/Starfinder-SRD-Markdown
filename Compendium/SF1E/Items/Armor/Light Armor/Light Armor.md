---
aliases: 
tags: 
---

# Light Armor

``` dataview
TABLE
Level, KAC, EAC, Armor-Check-Penalty as Penalty, Upgrade-slots as U-Slots, Bulk, Price
FROM "Compendium/SF1E/Items/Armor/Light Armor"
SORT Level ASC
WHERE file.name != "Light Armor"
```