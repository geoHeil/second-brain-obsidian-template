```dataview
TABLE summary AS "Summary", company AS "Company", project AS "Project"
FROM "metaRef/meetings" or "projects" WHERE type = "meeting"
SORT file.cday DESC
```

