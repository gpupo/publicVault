---
type: dailynote
date: "{{date}}"
day: "{{date:DD}}"
month: "{{date:MM}}"
year: "{{date:YYYY}}"
cssclasses:
  - daily
  - page-dot
  - page-sage
  - pen-black
tags:
  - bullet-journal
  - daily-notes
title: Daily note {{date:DD.MM.YYYY}}
---
# 🗓️ {{date:DD/MM/YYYY}}  {{date:dddd}}

- [o] Academia 10.00
- [ ] ≥ 15min de organização da casa
- [ ] Praticar digitação em [MonkeyType](https://monkeytype.com/)

## 🌱 Foco do dia
<><<% tp.user.bible() %>
## 󰠮 Notas

## 🧲 Links
[[i16.Notas Pessoais.Diario Intelectual]]
[[L.{{date:YYYYMM}}.monthly-log]]
< [[<% tp.date.now("YYYY-MM-DD", -1) %>]] | [[<% tp.date.now("YYYY-MM-DD", 1) %>]] >
## 🔖 Arquivos do dia
```dataview
LIST
FROM ""
WHERE dateformat(file.ctime, "yyyy-MM-dd") = "{{date:YYYY-MM-DD}}"
AND file.name != this.file.name
AND contains(file.path, "notes")
SORT file.ctime ASC
```


