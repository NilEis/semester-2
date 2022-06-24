---
id: xypymb99679v9l00rou9pze
title: Speicherverwaltung
desc: ''
updated: 1655462720650
created: 1654255972582
---

# Swapping
- Swap-files

# Probleme
- Arbeitsspeicher kleiner als benötigter Adressraum
- Benötigter Arbeitsspeicher aller Prozesse

## Frühe Lösung: Overlays
- Es gibt Teile eines Programmes, die nie gleichzeitig im Hauptspeicher benötigt werden

## virtueller Speicher
- Virtuell mehr Speicher bereit als vorhanden

# Segmentierung
- Prozess hat logischen Adressraum: Sammlung von Segmenten
  - Unterprogramm
  - Programmdaten
  - Variablen
  - Stack
- Besitzt einen Namen und eine Länge
- Logische Adresse: $\text{Segmentnummer}+\text{offset}$

# Adressierung
- Logische (Virtuelle Adressen)
  - `0x00000000 - 0xC0000000`
  - 