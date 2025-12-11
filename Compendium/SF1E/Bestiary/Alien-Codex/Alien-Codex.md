---
cssclasses: []
aliases:
  - Alien Codex
date created: Tuesday, August 22nd 2023, 4:01:13 pm
date modified: Tuesday, July 30th 2024, 10:08:01 pm
icon: bug
tags: []
---

```dataview
TABLE WITHOUT ID
	R.cr AS "CR", R.file.link AS "Name", R.type AS "Type", embed(link(R.image, "75")) AS "Image"
FROM "Starfinder-SRD/Compendium/Bestiary/Alien-Codex" and !"Starfinder-SRD/Compendium/Bestiary/Alien-Codex/Alien-Codex.md" 
GROUP BY cr
FLATTEN rows as R
SORT R.cr ASC, R.file.link ASC
SORT choice(cr = "1/3", "1",
choice(cr = "1/2", "2", "other"))
```
