---
aliases: []
cssclasses: hcl,
date created: Friday, January 12th 2024, 10:01:56 pm
date modified: Wednesday, August 21st 2024, 7:56:12 pm
tags: []
type: 
---

## Core

```dataviewjs
const data = dv.pages('"Compendium/SF1E/Character/Species"')
  .where(p => p.section && p.section == "core");
  
dv.table(
  ["Species", "HP", "Mods", "Size", "Type"],
  data.map((page, index) => [
    dv.span(page.blurb.complete ? ('<a aria-label="'+page.file.path+'" data-href="'+page.file.path+'" href="'+page.file.path+'" class="internal-link" target="_blank" ref="noopener"><img src="'+app.vault.getResourcePath(dv.fileLink(page.blurb.path))+'" referrerpolicy="no-referrer" height="100px" width="auto"></a>') : page.file.link),
 page.hitpoints, page.abilitymodifiers, page.size, page.type]), 
);
```

## Legacy

```dataviewjs
const data = dv.pages('"Compendium/SF1E/Character/Species"')
  .where(p => p.section && p.section == "legacy");
  
dv.table(
  ["Species", "HP", "Mods", "Size", "Type"],
  data.map((page, index) => [
    dv.span(page.blurb.complete ? ('<a aria-label="'+page.file.path+'" data-href="'+page.file.path+'" href="'+page.file.path+'" class="internal-link" target="_blank" ref="noopener"><img src="'+app.vault.getResourcePath(dv.fileLink(page.blurb.path))+'" referrerpolicy="no-referrer" height="100px" width="auto"></a>') : page.file.link),
 page.hitpoints, page.abilitymodifiers, page.size, page.type]), 
);
```

## Alien Species
```dataviewjs
const data = dv.pages('"Compendium/SF1E/Character/Species"')
  .where(p => p.blurb).where(p => p.section != "legacy").where(p => p.section != "core");
  
dv.table(
  ["Species", "HP", "Mods", "Size", "Type"],
  data
  .sort(page => page.file.name)
  .map((page, index) => [
    dv.span(page.blurb.complete ? ('<a aria-label="'+page.file.path+'" data-href="'+page.file.path+'" href="'+page.file.path+'" class="internal-link" target="_blank" ref="noopener"><img src="'+app.vault.getResourcePath(dv.fileLink(page.blurb.path))+'" referrerpolicy="no-referrer" height="100px" width="auto"></a>') : page.file.link),
 page.hitpoints, page.abilitymodifiers, page.size, page.type]) 
);
```

```dataviewjs
const data = dv.pages('"Compendium/SF1E/Character/Species"')
  .where(p => !p.blurb);
  
dv.table(
  ["Species", "HP", "Mods", "Size", "Type"],
  data.sort(page => page.file.name)
  .map((page, index) => [page.file.link, page.hitpoints, page.abilitymodifiers, page.size, page.type]), 
);
```

