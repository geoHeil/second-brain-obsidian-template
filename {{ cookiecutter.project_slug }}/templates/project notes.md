<% "---" %>
project-tag: <%* const projectTag = await tp.system.prompt("What is the project tag?", "", false, false) %> <% projectTag %>
tags:
  - <% projectTag %>
project: <%* const project = await tp.system.prompt("What is the project name?", "", false, false) %> <% project %>
project: <% project %>
<% "---" %>

<% await tp.file.move("/metaRef/projects/" + tp.file.title) %>

tags:: [[🗣 Projects MOC]] #project/active
## Open Tasks

### high priority
```tasks
tags includes <% projectTag %>
priority is high
not done 
```
### normal
```tasks
tags includes <% projectTag %>
priority is not high
not done 
```
## Documentation

## Meeting History
```dataview
LIST
FROM "metaRef/meetings" or "projects"
WHERE type = "meeting" 
AND project = this.project OR contains(file.tags, this.project-tag)
SORT file.day desc
```

## Status Notes
```dataview
TABLE <% projectTag %>
WHERE <% projectTag %>
SORT file.day DESC
```

## Completed Tasks
```tasks
done
tags include #<% projectTag %>
```