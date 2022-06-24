
- Für leeres Wort: $A\rightarrow\epsilon$
- Für jede Grammatik $G$ gibt es eine Grammatik $G'$ für die gilt: $L(G')=L(G)\setminus L(\epsilon)$
- Erweiterungsschritt:
  - Sind $A\rightarrow \epsilon$ und $B\rightarrow \alpha A\beta$, so füge die Regel $B\rightarrow \alpha\beta$ hinzu

# Chomsky-Normalform
Gilt wenn:
- $A\rightarrow BC$
- $A\rightarrow a$

Jede Kontextfreie Grammatik ist äquivalent zu einer Kontextfreien Grammatik in Chomsky-Normalform
## Umwandlung
1. Elimination der $\epsilon$-Regeln
2. Terminalsymbole nur in Regeln der Form $A\rightarrow A_1\dotsc A_m$ mit $m>2$
3. Elimination der Regeln $A\rightarrow B$
4. Elimination der Regeln $A\rightarrow A_1 \dotsc A_m$
