---
id: l19obf46ny8oevfoomwnent
title: Lineare Datenstrukturen
desc: ''
updated: 1649324572161
created: 1649320772516
---

# Lineare Datenstrukturen
- Sequenz $\{x_1,\dotsc,x_n\}$

## Listen
- $L = \{x_1,\dotsc,x_n\}$
- Zugriff auf beliebige Elemente $x_i$
  - Per Index
    - `Get(i)`
  - Per Marker
    - `GetFirst()`
    - `GetNext()`
    - `GetPrevious()`
- Random Access
  - Implementierung durch Arrays
  - `Get(i) = L[i]`
  - Nachteile
    - Elemente Löschen erzeugt Lücken, oder alle höheren Elemnte müssen verschoben werden
    - statische Obergrenze für Listenlänge
- Sequential Access
  - Implementierung durch Pointer oder Container
  - Marker zeigt auf aktuelle Position
  - Nachteil:
    - Elementzugriff erfordert lineare Suche
  - Beliebiges Erweitern oder Löschen

