---
date: <% tp.file.creation_date() %>
type: idea
summary: " "
category:
reference_uri:
URI: 
---
tags: [[Idea MOC]]
Date: [[<% tp.date.now("YYYY-MM-DD-dddd") %>]]
<% await tp.file.move("/metaRef/ideas/" +tp.date.now("YYYY")+"/"+tp.date.now("MM-MMMM") +"/"+ tp.date.now("YYYY-MM-DD") + " " + tp.file.title) %>
# [[<% tp.date.now("YYYY-MM-DD") + " " + tp.file.title %>]]

## Notes
- 