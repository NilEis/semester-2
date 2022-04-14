---
id: zvbaxijpphhgr878gipd8mp
title: Bäume
desc: ''
updated: 1649927245246
created: 1649925191942
---

<img src="https://c.tenor.com/W8pYfpTSrYIAAAAS/roomba-cat.gif" alt="cat" id=cat>

<script>

    for(let i = 0; i < 10; i++)
    document.getElementById("cat").parentElement.append(document.getElementById("cat").cloneNode())

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
- 