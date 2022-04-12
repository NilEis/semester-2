---
id: usuwijfnfz44i3bvexmb3vr
title: Abstrakte Datenstrukturen
desc: ''
updated: 1649766815147
created: 1649320831716
---

- Keine Festlegung der Implementierung
- Axiome beschreiben statische Beziehungen
- Beispiele
  - Aufzählungstypen (`bool`, `enum`)
  - Skalare Typen (`char`, `int`, `float`, ...)
    - Eindimensionaler Wertebereich
    - In Praxis meist endlich 
  - Zusammengesetzte Typen (`struct`, `class`)
  - Lineare Strukturen (`list`, `queue`, `stack`)
  - Bäume
  - Graphen
- endlicher Wertebereich
  - vollständig durch Tabellen spezifizierbar
- Verallgemeinerung
  - Aufzählungstypen: `enum`
  - z.B. Wochentage, chemische Elemente
  - Kodierung (oft) als ganze Zahl Modulo n (implizite Ordnungsrelation)

## Natürliche Zahlen

```py
def ZERO():
    return []

def SUCC(x):
    return x + [1]

def PRED(x):
    return x[1:]

def VALUE(x):
    return len(x)

def ADD(x, y):
    if x == ZERO():
        return y
    return SUCC(ADD(PRED(X),y))

def MUL(x, y):
    if x == ZERO():
        return ZERO()
    return ADD(MUL(PRED(x), y), y)
```
