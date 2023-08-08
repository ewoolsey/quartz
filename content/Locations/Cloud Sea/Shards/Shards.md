---
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

* **[Gramerai](Gramerai/Gramerai.md)**
* **[Hearthen](Hearthen/Hearthen.md)**
* [Pytax](Pytax.md)
* **[Rifton](Rifton/Rifton.md)**
* **[The Forlorn Shiver](The%20Forlorn%20Shiver/The%20Forlorn%20Shiver.md)**

%% End Waypoint %%
