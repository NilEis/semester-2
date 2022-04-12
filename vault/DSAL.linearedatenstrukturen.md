---
id: l19obf46ny8oevfoomwnent
title: Lineare Datenstrukturen
desc: ''
updated: 1649766822542
created: 1649320772516
---

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

### Stack
- Nur einfügen am Anfang
- Auslesen auch nur am Anfang
- Last in, First out

# Suche im Labyrinth
- Annahme: Array hat keine Zykel
- Pfad = Liste

# Baum
- Jeder Knoten ist Wurzelknoten eines Teilbaumes
- Tiefe: Anzahl der Kanten von Wurzel bis Knoten
- Grad: Anzahl der Nachfolger
- Blätter: Knoten ohne Nachfolger