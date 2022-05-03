---
id: gaoww6pfwoli8l6kw7sxkpx
title: Reguläre Sprachen
desc: ''
updated: 1651583162937
created: 1650976425062
---

Der reguläre Ausdruck $a(a+b)^*bb$ beschreibt die Sprache über das Alphabet $\sum=\{a,b\}$, in der alle Wörter mit a beginnen und auf 2 b enden.

## Basisregeln
- $\emptyset\in RA_{\sum}$
- $\epsilon \in RA_{\sum}$
- $a \in RA_{\sum}$ für alle $a\in \sum$

## Rekursive Regeln
- Wenn $r,s\in RA_{\sum}$, dann $(r+s)\in RA_{\sum}$
- Wenn $r,s\in RA_{\sum}$, dann $(r\cdot s)\in RA_{\sum}$
- Wenn $r\in RA_{\sum}$, dann $r^*\in RA_{\sum}$

![](/assets/images/2022-04-26-14-46-10.png)

- Semantik
  - ![](/assets/images/2022-04-26-14-52-39.png)

## Pumping-Lemma
- L ist regulär. Dann ist $n\geq 1$, so dass für alle $w \in L$ eine Zerlegung $w=xyz$ existiert, für die gilt.
  1. $y\neq \epsilon$
  2. $|xy|\neq w$
  3. $xy^kz\in L$ für alle $k\geq 0$

## Myhill-Nerode-Äuivalenz
- Sei $L\subseteq\sum^*$ eine Sprache. Wir definieren
- Eine Sprache $L$ ist genau dann regulär, wenn index($L$)$<\infty$
