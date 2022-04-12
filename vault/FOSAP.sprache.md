---
id: oe241jb9h8q8qqkm146bcuo
title: Sprachen
desc: ''
updated: 1649770290602
created: 1649769189570
---

# Verkettung
- $vw$ bezeichnet die Verkettung der Wörter $u,v,w\in \sum^*$

## Definition 1.23
Sei $L\subseteq \sum^*$. Die Potenzen $L^n$, für $n\in\mathbb{N}$, sind induktiv wie folgt definiert.
$$
    L^0\coloneqq \{\epsilon\},\\
    L^{n+1} \coloneqq L^nL
$$
für alle $n\in\mathbb{N}$.
## Definition 1.26
Die Iteration (auch Kleene-Stern) einer Sprache $L$ ist die Sprache
$$
    L^* \coloneqq \bigcup_{n\in\mathbb{N}}L^n
$$
### Beobachtung
1. $\epsilon \in L^0 \subseteq L^*$
2. Ein Wort $u \neq \epsilon$ liegt genau dann in $L^*$, wenn es ein $n\geq1$ und Wörter $v_1,\dotsc,v_n \in L$ gibt.
