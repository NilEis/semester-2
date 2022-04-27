---
id: gaoww6pfwoli8l6kw7sxkpx
title: Reguläre Sprachen
desc: ''
updated: 1650980188720
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
