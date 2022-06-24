
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

# Beispiele
1. Natürliche zahlen $n\in\mathbb{N}$
   - Alphabet: $\sum=\{0,\dotsc,9\}$ oder $\sum=\{\mathbb{N}\}$
   - $\{w\in\sum_a^*\vert w\text{ hat keine führende }0\}$
     - $0001\notin\mathbb{N}$
   - $v\{0\}$
2. Alle möglichen Stundenpläne
   - $\sum=\{\#,\}\cup\{'m','d','m','d','f'\}$
3. Sucher nach Abgabegruppen
   - $(\sum_{UTF_8})^*$
   - $\{w\in \sum_{UTF_8}^*\vert \text{als Infix "Grüße"}\}\cap L_{email}$

## Beweise
### Zeige oder widerlege
- $(KL)M=K(LM),$
  - $x\in(KL)M.\quad\text{Sei }x=uvw, \text{ mit }u\in K,v\in L,w\in M\\\text{Dann ist }x=(uv)w=uvw=u(vw)\in K(LM), vw\in LM,u\in K$
  - Analog, assozieativität von Kompositionen, gilt genau
- $L\{\epsilon\}=\{\epsilon\}L=L$
  - $L\{\epsilon\}\subseteq\{\epsilon\}: \text{ Sei } w \in L\{\epsilon\}. w\in L, \text{ und damit }\epsilon w\in \{\epsilon\}$
