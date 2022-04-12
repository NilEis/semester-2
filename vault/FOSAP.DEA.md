---
id: wo161knnxca4andavb1d2g3
title: Deterministische Endliche Automaten
desc: ''
updated: 1649766848698
created: 1649315714532
---

## Endliche Automaten
- Berechnungsmodell zur Beschreibung sequentiller Prozesse
- endliche Menge an Zuständen
- Hat einen Startzustand und 1 oder mehr Endzustände

### Mustererkennung
```mermaid
graph LR
n((nichts)) -->|0|n((nichts))
n((nichts)) -->|1|1((1))
1((1))-->|0|n((nichts))
1((1))-->|1|11((11))-->|1|11((11))
11((11))-->|0|110((110))
110((110))-->|0|n((nichts))
110((110))-->|1|1101((1101))-->|0,1|1101((1101))
```
### Teilbarkeit durch 3
```mermaid
graph LR
0((0))
1((1))
2((2))
0-->|1,4,7|1
1-->|2,5,8|0
1-->|1,4,7|2
2-->|2,5,8|1
2-->|1,4,7|0
0-->|2,5,8|2
0-->|0,3,6,9|0
1-->|0,3,6,9|1
2-->|0,3,6,9|2
```
## Alphabet
- Nicht leere Menge
  - behinhaltet Symbole,Buchstaben oder Zeichen
- Ein Wort ist eine endliche Folge von Zeichen aus dem Alphabet

### Notation
- $\sum$,$\Gamma$ und Varianten wie $\sum_1$, $\Gamma'$
- $a,b,c,\dotsc$ und Varianten stehen für Zeichen

### Beispiele
1. Boolsche Alphabet $\{0,1\}$
2. Morsealphabet $\{.,-,\quad\}$

## Wörter
### Notation
- Ohne Klammern und Kommata
- $u,v,w,\dotsc$ und Varianten stehen für Wörter

## Sprache
- Menge von Wörtern

# DEA
- 5-Tupel $(Q,\sum,\delta,q_0,F)$
  - $Q$: Menge der Zustände
  - $\sum$: Eingabealphabet
  - $\delta: Q \times \sum \rightarrow Q$: Abbildung: die Transitionsfunktionen
  - $q_0 \in Q$: Der Anfangszustand
  - $F \subseteq Q$: Die Menge der Endzustände

