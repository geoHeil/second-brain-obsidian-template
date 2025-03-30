---
date: <% tp.file.creation_date() %>
type: link
summary: " "
category:
URI: 
---
tags: [[🗣 LINKS MOC]]
Date: [[<% tp.date.now("YYYY-MM-DD-dddd") %>]]
<% await tp.file.move("/metaRef/linklist/" +tp.date.now("YYYY")+"/"+tp.date.now("MM-MMMM") +"/"+ tp.date.now("YYYY-MM-DD") + " " + tp.file.title) %>
# [[<% tp.date.now("YYYY-MM-DD") + " " + tp.file.title %>]]

## Notes
- 
