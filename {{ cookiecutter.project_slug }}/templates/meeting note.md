---
date: <% tp.file.creation_date() %>
type: meeting
company: 
location: 
project: 
summary: " "
---
tags: [[🗣 Meetings MOC]]
Date: [[<% tp.date.now("YYYY-MM-DD-dddd") %>]]
<% await tp.file.move("/metaRef/meetings/" +tp.date.now("YYYY")+"/"+tp.date.now("MM-MMMM") +"/"+ tp.date.now("YYYY-MM-DD") + " " + tp.file.title) %>
# [[<% tp.date.now("YYYY-MM-DD") + " " + tp.file.title %>]]

**Attendees**: 
- 

## Agenda/Questions
- 

## Notes
- 

## Tasks
- [ ] 