---
layout: post
title: SSG-plugin
date: 2023-09-18T10:02:35.571Z
last_modified_at: 2023-09-18T12:20:07.900Z
tags: 
- blog
- teblog
- Blog
---
Es gibt mehrere plugins für Static site generation.

1. ... erstellt direkt html und lädt es hoch zu github
2. ... exportiert ausgewählte markdown files
3. ... for von 2. 

ssg hatte einen wichtigen fehler: hat nur in den ersten 100 notes nach den richtigen notes gesucht.

mein fork tssg benutzt die API um nach allen notes mit dem tag "blog" zu suchen und benutzt diese...

### Development

code is in D:\joplin\joplin-exports-to-ssg\src 
index.ts

build:npm run dist
baut eine jpl datei, diese muss man einmal in den Plugin einstellungen bei development eintragen:
![66eca4fb8f5dce2224b2b55946c4af5e.png](D:\dev\web\teblog.github.io\66eca4fb8f5dce2224b2b55946c4af5e.png)

beim neustart wird die neue Erweiterung geladen.

#### data api
https://joplinapp.org/api/references/plugin_api/classes/joplindata.html

## todo
publish the plugin on github
find write into the issues other had

features:
connect directly to github (look at code from github pages plugin)
move button from context-menu to other menu


