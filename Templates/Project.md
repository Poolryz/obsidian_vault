```dataview 
TABLE without id
dateformat(this.file.ctime, "dd.MM.yyyy HH:mm") as created,  dateformat(this.file.mtime, "dd.MM.yyyy HH:mm") as "last modified"
WHERE file.name = this.file.name
```
```dataview 
TABLE without id
file.outlinks AS "OUTGOING",
file.inlinks AS "BACKLINKS"	WHERE file.name = this.file.name 
```
#project
- [ ] {{title}}
# Todo List
> [!todo] Active
```dataview
TASK
FROM [[]]
WHERE !completed
SORT file.ctime desc
```
>[!todo] Completed
```dataview
TASK
FROM [[]]
WHERE completed
SORT file.ctime desc
LIMIT 30
```

# Links



# Description
