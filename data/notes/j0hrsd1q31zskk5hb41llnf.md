
1. [[Atomare Operationen|BUS.atomOp]]

# Motivation und einfache Lösungsversuche
- Es darf auf geteilten Speicher nie gleichzeitig geschrieben und gelesen werden, um Inkonsistenzen zu vermeiden.
- 

# Semaphore
- Integer-Variable $s$ mit 3 atomaren Operationen
  - init($s$, anfangswert)
  - wait($s$)
  - signal($s$)
- Wechselseitiger Ausschluss: *Mutex* = Semaphor mit anfangswert $1$
- Mehrere Prozesse im kritischen Bereich erlaubt: *Zählsemaphor* mit Anfangswert $n$
- Zeitliche Ablaufsteuerung:
  - Initialisierung
    - init(sync, 0)
  - Prozess A
    - Operationend
  - Prozess B

# Erweiterte Konstrukte