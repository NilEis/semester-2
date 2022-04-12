---
id: y0iae8lac01iyy5t3bq0myg
title: Linearkombination
desc: ''
updated: 1649761557141
created: 1649759267615
---

# Definition
$n \in \mathbb{N},(v_1,\dotsc,v_n) n\text{-Tupel in }V\\$
Eine Linearkombination von $(v_1,\dotsc,v_n)$ ist ein $v\in V$ der Form
$$
v = \sum_{i=1}^na_iv_i
$$
mit $a_1,\dotsc,a_n \in K$ (Koeffizienten der Linearkombination)
## Mit Körpern
$K$ Körper, $V$ ein $K$-Vektorraum, $M \subseteq V$
- Linearkombination aus $M$:
- Linearkombinationen von $(v_1, \dotsc, v_n)$ mit $v_1,\dotsc, v_n \in M$

# Beispiele
- in $\mathbb{Q}^{1\times3}: \quad(-1,-4,-1)\in((1,2,1),(1,3,1))$

# Bemerkung 1
- $n \in \mathbb{N}, \tau = (v_1,\dotsc,v_n)$ Tupel in $V$
- $\lambda\tau: K^n \rightarrow V,\begin{pmatrix}a_1\\\vdots\\a_n\end{pmatrix}\mapsto \sum^n_{i=1}a_iv_i$
$$
    \left<v_1,\dotsc, v_2\right> = \lambda\tau(K^n) = \text{Bild von }\lambda\tau
$$

# Bemerkung 2
- $n \in \mathbb{N}, (v_1,\dotsc,v_n)$ Tupel in $V$

$$
    \left<v_1,\dotsc, v_2\right>\leq V
$$
# Proposition
$$
    n \in \mathbb{N}\text{Tupel in } V, v \in V\\
    \text{Dann sind äquivalent:}\\
    \begin{aligned}
        &\triangleright&&v \in \left<v_1,\dotsc, v_2\right>&\\
        &\triangleright&&\left<v_1,\dotsc, v_2,v\right> \subseteq \left<v_1,\dotsc, v_2\right>&\\
        &\triangleright&&\left<v_1,\dotsc, v_2,v\right> = \left<v_1,\dotsc, v_2\right>&\\
    \end{aligned}
$$
# Korollar
- $n \in \mathbb{N}, (v_1,\dotsc,v_n)$ Tupel in $V$
  - Für $\pi \in S_n:$
    - $\left<v_1,\dotsc, v_2\right> = \left<v_{\pi(1)},\dotsc, v_{\pi(n)}\right>$
  - Für $1\neq k\in\underline{n}$ und $a \in K$
    - $\left<v_1,\dotsc, v_2\right>=\left<v_1+av_k,\dotsc, v_2\right>$
  - Für $a \in K^\times:$
    - $\left<v_1,\dotsc, v_2\right>=\left<av_1,\dotsc, v_2\right>$

# Erzeugendensystem:
- Eine Menge heißt so, wenn sie den ganzen Vektorraum erzeugt

TIME: -17:27