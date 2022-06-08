---
id: yx3xmgxwr0e6wh5fimndsur
title: Basis eines Vektorraumes
desc: ''
updated: 1654701631202
created: 1654700785709
---

- $K$ Körper, $V$ Vektorraum über $K,M \subseteq V$ Teilmenge
- $M$ ist Erzeugendensystem (EZS) von $V \Leftrightarrow \left<M\right>=V$
- $M$ [[linear unabhängig|LA.lineare_unabhaengikeit]] $\Leftrightarrow$ Alle $v_1,\dotsc v_n\in M$ mit $n\in \N$ und $v_i$ paarweise verschieden sind linear unabhängig.
- Ein linear unabhängiges EZS von $V$ nennt man Basis von $V$.
  - Beispiel: $M=\{,X,X^2,\dotsc\}$ ist eine Basis des $K$-[[Vektorraums|LA.vektorraeume]] $K[X]$.
- Folgende Aussagen sind äquivalent
  1. $M$ ist Basis von $V$.
  2. $M$ ist ein minimales EZS von $V$.<br/>D.h.: $M$ ist EZS und für alle $m\in M$ ist $M\setminus \{m\}$ kein EZS.
  3. $M$ ist eine maximale linear unabhängige Teilmenge von $V$.<br/>D.h.: $M$ ist linear unabhängig und für alle $v \in V\setminus M$ ist $M\cup\{v\}$ linear abhängig.