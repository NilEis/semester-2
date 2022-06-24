

# Setup
- $K$ Körper: Z.B. $K = \mathbb{R},\mathbb{Q},\mathbb{C},\mathbb{F}_p,p \in \mathbb{R}, Z.B. \mathbb{F}_2=\{0,1\}$
- nach Definition: $V$ Vektorraum über $K$

# Definition
## $K$-Vektorraum:
Besteht aus
- $V$ Menge
- $V \times V \rightarrow V, (v,w) \mapsto v+w$ Abbildung
- $K \times V \rightarrow V, (a,w) \mapsto av$ Abbildung
so, dass die Vektorraumaxiome gelten.

## Terminologien und Notationen:
$$
\begin{aligned}
    &a,b,c...&&\qquad\text{Skalare}&&\qquad\text{Element von $K$}\\
    &u,v,w...&&\qquad\text{Vektoren}&&\qquad\text{Element von $V$}\\
    &\text{Nullvektor}&&\qquad&&\qquad\text{$0$}\\
    &\text{für $v \in V$:}&&\qquad\text{negativer Vektor zu $v$}&&\qquad-v\\
\end{aligned}
$$
# VektorraumaxiomeAxiome
$$
\begin{aligned}
    &\text{für $v,w,x \in V$:}&&v+(w+x)=(v+w)+x&\\
    &\text{Es existiert $0 \in V$ so, dass für $v \in V$:}&&0+v=v+0=v&\\
    &\text{für $v \in V$ existiert $w \in V$:}&&w+v=v+w=0&\\
    &\text{für $v,w \in V$:}&&v+w=w+v&\\
    &\text{für $a,b \in K, v \in V$:}&&a(bv)=(ab)v&\\
    &\text{für $v \in V$:}&&1v=v&\\
    &\text{für $a,b \in K, v \in V$:}&&(a+b)v=(av)+(bv)&\\
    &\text{für $a \in K, v,w \in V$:}&&a(v+w)=(av)+(aw)&\\
\end{aligned}
$$
# Beispiel
- $K$ wird $K$-Vektorraum mit
  - Addition - Körperaddition
  - Skalarmultiplikation - Körpermultiplikation
- $m,n \in \mathbb{N};\quad K^{m \times n}$ wird $K$-Vektorraum mit
  - Addition - Matrixaddition
  - Skalarmultiplikation - Multiplikation einer Matrix mit einem Skalar
- Spezialfälle
  - $K^m \coloneqq K^{m \times 1}$ - Spaltenvektorraum: $\small{\{\begin{pmatrix}a_1\\\vdots\\a_m\end{pmatrix}}\vert a_i \in K, 1 \leq i \leq m\}$
  - $K^{1 \times n}$ - Zeilenvektorraum: $\{(a_1,\dots,a_n)\vert a_i \in K, 1 \leq i \leq n\}$
- $M$ Menge: $\overbrace{\text{Abb}(M,K)}^{K^M}$ wird $K$ Vektorraum mit:
  - Addition - $f+g: M \rightarrow K, (f+g)(m)\coloneqq f(m)+g(m)$
  - Skalarmultiplikation: $af: M \rightarrow K, (af)(m) \coloneqq af(m)$
- $K[X]$ wird $K$-Vektorraum mit:
  - Addition:$\sum_{i=0}^na_i\cdot X^i + \sum_{i=0}^nb_i\cdot X^i = \sum_{i=0}^n(a_i+b_i)\cdot X^i$
  - Skalarmultiplikation: $a\cdot(\sum_{i=0}^na_i\cdot X^i)=\sum_{i=0}^n(a\cdot a_i)\cdot X^i$
  - $K[X] = \{\sum_{i=0}^na_i\cdot X^i\vert a_i\in K, 0\leq i \leq n, n\in \mathbb{N}_0\}$: Polynomring

# Lemma
$$
a\in K,v\in V\\
av=0\Rightarrow a=0 \vee v=0\\
\text{Beweis:}\\
\text{Sei }av=0,a\neq 0, \text{d.h. }a\in K^x\\
\Rightarrow v = a^{-1}0=0
$$
# Korollar
$a,b\in K,v\in V\setminus\{0\}$
$$
av=bv\Rightarrow a=b\\
av=bv\Rightarrow av-bv=0\\
\Rightarrow (a-b)v=0\\
\Rightarrow a-b=0\\
\Rightarrow a=b\\
$$

# Untervektorraum
$U\subseteq V$ heißt $K$-Untervektorraum von $V$, falls $U$ mit der Addition und der skalaren Multiplikation auf $V$ ein Vektorraum ist.
