---
id: 86qyjdsuf73nhr1v9lk61uv
title: Analyse von Algorithmen
desc: ''
updated: 1650535221924
created: 1650531964149
---

- Effizienz
  - Gute Nutzung von Ressourcen
  - Komplexität von Algorithmen
- Ressourcen
  - Rechenzeit
  - Speicherplatz
  - Energie
- Aufwand / Komplexität
  - Tatsächlicher Verbrauch von Ressourcen
- Performance Charts
  - X: Größe der Eingabedaten
  - Y: Benötigte Rechenzeit

```
Y
^
|   //  
|  //  /
| /|  /
|/|  /
| | /                      
|| /          _____________---------------
||/-----------
+----------------------------------------->X
```
- Abstrakte Analyse
  - Anzahl der wesentlichen Operationen auf einem idelaisierten Computer
  - Unabhängig von der Programmiersprache

## Stripped Python
- Teilmenge von Python
  - Prozedur Aufrufe
  - Integer-Arithmetik
  - Zuweisungen (Lesen / Schreiben)
  - if-then-else
  - while
- Vollständig, aber einfacher zu analysieren als Python
- Berechnungsaufwand
  - Prozedur-Aufruf
    - Speichere Kontext
    - Speichere Rücksprungadresse
    - Kopiere Parameter
    - Generiere neuen Kontext
    - $\dotsc$
    - Kopiere Rückgabewert
    - Stelle alten Kontext wieder her
  - Kosten $C_{PC}$
  - if-then-else
    - `if X then Y else Z`
      - worst case:
        - OP = OP(X) + max{OP(Y),OP(Z)}
      - Average
        - P = Prob(X=True)
        - OP = OP(X) + p * OP(Y) + (1-P) OP(Z)
  - Kombinatorik
    - Permutationen: $n!$
    - Kombinationen: $\binom{n}{k}=\frac{n!}{k!(n-k)!}$
    - Summe der Kombinationen:$\sum_{k=0}^n\binom{n}{k}=2^n$

--------------------------------------------------------------------------

- Definitionen von Schranken für Funktionen

![](/assets/images/2022-04-21-12-00-18.png)