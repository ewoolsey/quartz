---
title: |
  Shards
---

# Hooks

### In Progress

````dataview
LIST
FROM #hooks/in-progress
WHERE any(map(file.outlinks, (x) => contains(x.file.path, this.file.folder)))
SORT file.mtime DESCENDING
````

### To Do

````dataview
LIST
FROM #hooks/todo
WHERE any(map(file.outlinks, (x) => contains(x.file.path, this.file.folder)))
SORT file.mtime DESCENDING
````

### Complete

````dataview
LIST
FROM #hooks/complete
WHERE any(map(file.outlinks, (x) => contains(x.file.path, this.file.folder)))
SORT file.mtime DESCENDING
````

%% Begin Waypoint %%

* **[Gramerai](Locations/Cloud%20Sea/Shards/Gramerai/Gramerai.md)**
* **[Hearthen](Locations/Cloud%20Sea/Shards/Hearthen/Hearthen.md)**
* [Pytax](Locations/Cloud%20Sea/Shards/Pytax.md)
* **[Rifton](Locations/Cloud%20Sea/Shards/Rifton/Rifton.md)**
* **[The Forlorn Shiver](Locations/Cloud%20Sea/Shards/The%20Forlorn%20Shiver/The%20Forlorn%20Shiver.md)**

%% End Waypoint %%
