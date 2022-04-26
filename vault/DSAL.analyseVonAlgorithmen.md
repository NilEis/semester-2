---
id: 86qyjdsuf73nhr1v9lk61uv
title: Analyse von Algorithmen
desc: ''
updated: 1650966488637
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

--------------------------------------------------------------------------
## Fibonacci
$$
\begin{aligned}
  F(n)&=F(n-1)+F(n-2)\\
  &>2\times F(n-2)\\
  &>4\times F(n-2)\\
  &>\dotsc\\
  &>2^{n}\times F(n-2)
\end{aligned}
$$
--------------------------------------------------------------------------
$$
\begin{aligned}
  &O(1) &-&\text{Elementaroperation}\\
  &O(\log n) &-&\text{Binäre Suche}\\
  &O(n) &-&\text{Lineare Suche}\\
  &O(n\times \log n) &-&\text{Sortieren (später)}\\
  &O(n^2) &-&\text{Sortieren (neulich)}\\
  &O(n^3) &-&\text{Invertieren von Matrizen}\\
  &O(2^n) &-&\text{Labyrinth-Suche (Vollständig)}\\
  &O(n!) &-&\text{Permutationen}\\
\end{aligned}
$$
--------------------------------------------------------------------------
- Beweis durch vollständige Induktion

## Rekursionsgleichung
- Elimination
  - Einsetzen
  - Summenformel
- Master-Theorem
  - ![](/assets/images/2022-04-26-11-48-06.png)
- Direkter Ansatz
  - 