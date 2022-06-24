# Prozessverwaltung

# Threads
- user-threads
  - thread-management im programm, nicht im Betriebssystem
  - Kernel sieht nur den Prozess
  - Wenn ein Thread hängen bleibt, bleiben alle hängen
- Kernel-Thread
  - Management durch Kernel
  - Blockiert ein Thread, weist der Kernel die Cpu weiter zu
  - Multicore-CPUs können genutzt werden
  - Wechsel zwischen Threads so aufwendig wie von Prozessen

Bluetoos -> Bluetoof -> bluetooth
# Scheduling

- Mehrere Prozesse müssen gleichzeitig ausgeführt werden
  - Prozess muss geladen werden
  - CPU-Zeit muss zugeteilt werden

## Strategien
- Long-Term_scheduler
  - Entscheidet welche Prozesse zur ready-queue hinzugefügt werden
- Welche Prozesse sollen bedient werden?
  - Fairness: Kein Prozess soll zu lange warten
  - Wichtigkeit: Prozesse mit hoher Priorität sollen bevorzugt werden.
- Round Robin
- 