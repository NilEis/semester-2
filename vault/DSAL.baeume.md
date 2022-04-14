---
id: zvbaxijpphhgr878gipd8mp
title: Bäume
desc: ''
updated: 1649927947074
created: 1649925191942
---

<img src="https://c.tenor.com/W8pYfpTSrYIAAAAS/roomba-cat.gif" alt="cat" id=cat>

<script>

    const cat = document.getElementById("cat");
    const n = Math.floor(cat.parentElement.offsetWidth/cat.width)*4;
    for(let i = 0; i < 13; i++)
        cat.parentElement.append(cat);

</script>

- Hierarische Datenstrukturen
  - Zusammenfassung von Gruppen
  - Eindeutige Schachtelung

# Implementation
```py
class Node:
    def __init__(self,value):
        self.value = value
        self.right = None
        self.left = None
```
## Array
- Vollständige Bäume
- $N(k)$ = Anzahl der Knoten der Tiefe $k$
- $N(k) = 2\times N(k-1) \rightarrow N(k)=2^k$
- Speichere die Knoten der Tiefe $k$ in den Array-Einträgen $A[2^k\dotsc2^{k+1}-1]$
- Jeder Knoten `A[i]` findet seinen Nachfolger in `A[2i]` und `A[2+1]`

```py
def ReadTerm():
    L = ReadProduct()
    op = getChar()
    while op = '+' or op = '-':
        R = ReadProduct()
        L = Node(L,op,R)
        op = getChar()
    return L
```
