---
company: 
location: 
title: 
email_work: 
email_private:
phone_work:
phone_private:
website: 
aliases:
initial_get_to_know_time: {{date}} {{time}}
date_last_spoken: {{date}}
---
tags:: [[Person MOC]]

# <% tp.file.title %>
<% await tp.file.move("/metaRef/contacts/" + tp.file.title) %>

## Notes
- 
### follow up actions
- 
## Meetings
```dataview
TABLE file.cday as Created, summary AS "Summary"
FROM "projects" OR "metaRef/meetings" where contains(file.outlinks, [[<% tp.file.title %>]])
SORT file.cday DESC
```
