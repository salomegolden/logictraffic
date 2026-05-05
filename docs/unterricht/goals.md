
# Lernziele für den Einsatz von *Logic Traffic* im Informatikunterricht

Dieses Dokument fasst die Lernziele zusammen, die auf Basis der Funktionen von **Logic Traffic** (Wahrheitstabelle, Formeleditor, Simulation) formuliert wurden. Diese wurden sowohl mit dem Lehrplan21[^1] als auch mit dem Rahmenlehrplan Gymnasium[^2] verknüpft um für alle Schularten Anknüpfungspunkte zu bieten.  
Die Einordnung erfolgt entlang der Wissensdimensionen nach **Anderson [^3] (2009)**:  

Die Lernziele sind so formuliert, dass sie die spezifischen Funktionen von Logic Traffic (Wahrheitstabelle, Formeleditor, Simulation) abdecken.  
Sie sind bezogen auf die aufgeführten Inhalte aus den Lehrplänen und formuliert nach Anderson[^3]. Somit sollen unterschiedliche Wissens- und Lern

| Wissensart               | Erinnern | Verstehen | Anwenden | Analysieren | Bewerten | Erzeugen |
|--------------------------|----------|-----------|----------|-------------|----------|----------|
| **Faktenwissen**         | [LZ1](#lernziel-1-logische-operatoren-wahrheitstabellen)     |           |          |             |          |          |
| **Konzeptuelles Wissen** |          | [LZ1](#lernziel-1-logische-operatoren-wahrheitstabellen)       |          | [LZ3](#lernziel-3-debugging-einer-fehlerhaften-ampelsteuerung)         |          |          |
| **Prozedurales Wissen**  |          |           | [LZ2](#lernziel-2-boolesche-formeln-aus-textbeschreibungen-ableiten)      | [LZ3](#lernziel-3-debugging-einer-fehlerhaften-ampelsteuerung)         | [LZ4](#lernziel-4-normalformen-minimierung-boolescher-ausdrücke)     | [LZ4](#lernziel-4-normalformen-minimierung-boolescher-ausdrücke)      |
| **Metakognitives Wissen**|          |           |          |             | [LZ4](#lernziel-4-normalformen-minimierung-boolescher-ausdrücke)      | [LZ4](#lernziel-4-normalformen-minimierung-boolescher-ausdrücke)      |

---

## Lernziel 1  - Logische Operatoren & Wahrheitstabellen

**Die Schülerinnen und Schüler können** die logischen Operatoren **AND**, **OR**, **NOT** benennen, ihre Formelzeichen kennen und die Zustände einer Kreuzung (z. B. *Ampel A Grün = 1*) in einer Wahrheitstabelle korrekt zuordnen.

### Bezüge zu Lehrplänen

**Rahmenlehrplan Gymnasium** Die Maturandinnen und Maturanden können grundlegende arithmetische und logische Operationen und Funktionen in Programmiersprachen umsetzen ([^2] S. 69).

**Lehrplan 21** MI.2.1.g: Daten mit verschiedenen Symbolsystemen darstellen und interpretieren  
  (z. B. logische Verknüpfungen, Symbole für Verkehrszeichen) ([^1] S. 484).

---

## Lernziel 2 - Boolesche Formeln aus Textbeschreibungen ableiten

**Die Schülerinnen und Schüler können** eine sprachliche Beschreibung sicherer Zustände einer Kreuzung in eine **boolesche Formel** übersetzen und diese im **Formeleditor von Logic Traffic** implementieren.
### Bezüge zu Lehrplänen
**Rahmenlehrplan Gymnasium**  

- Informationen strukturieren und modellieren (analytisches und vernetztes Denken) ([^2], S. 68).
- Verschiedene Darstellungen von Informationen erläutern und deren Besonderheiten analysieren ([^2], S. 68).

**Lehrplan 21** MI.2.2.a: Abläufe mit Entscheidungen und Schleifen lesen, verstehen und in formaler Sprache ausführen ([^1], S. 485).

---

## Lernziel 3 - Debugging einer fehlerhaften Ampelsteuerung

**Die Schülerinnen und Schüler können** eine fehlerhafte Ampelsteuerung systematisch untersuchen, mithilfe der Simulation logische Konflikte identifizieren (z. B. *gleichzeitiges Grün für kreuzende Ströme*) und die entsprechende Zeile in der Wahrheitstabelle lokalisieren.

### Bezüge zu Lehrplänen
**Rahmenlehrplan Gymnasium**  

- Fehler in einem Programm durch systematisches Testen identifizieren und korrigieren ([^2], S. 69).
- Struktur von Programmcode und technischen Texten analysieren ([^2], S. 68).

**Lehrplan 21** MI.2.2.c: Fehler in Abläufen finden und beheben (Debugging) ([^1], S. 485).


## Lernziel 4  - Normalformen & Minimierung boolescher Ausdrücke

**Die Schülerinnen und Schüler können** für eine komplexe Kreuzung (z. B. mit Bus‑Priorisierung) eine **lückenlose Wahrheitstabelle** erstellen, daraus die **Disjunktive Normalform (DNF)** und **Konjunktive Normalform (KNF)** ableiten und diese mithilfe der **booleschen Gesetze** (z. B. De Morgan, Distributivgesetz) minimieren, um eine logisch elegante und redundanzfreie Steuerung zu erzeugen.

### Bezüge zu Lehrplänen

**Rahmenlehrplan Gymnasium**  

- Entwicklung einer formalen und systematischen Vorgehensweise zur Problemlösung ([^2], S. 67).
- Präzise mathematische Beschreibung mit Symbolen und Nutzen von Abstraktion ([^2], S. 63–64).

**Lehrplan 21** MI.2.2.b: Einfache Algorithmen zur Lösung von Problemen entwerfen ([^1], S. 485).

---
[^1]: D-EDK, D. E. (2016). Lehrplan 21. Gesamtausgabe. Luzern: D-EDK Geschäftsstelle. https://v-fe.lehrplan.ch/container/V_FE_DE_Gesamtausgabe.pdf
[^2]: Rahmenlehrplan gymnasiale Maturitätsschulen. (2024, Juni 20). EDK. https://edudoc.ch/record/232281
[^3]: Anderson, L. W. (Hrsg.). (2009). A taxonomy for learning, teaching, and assessing: A revision of Bloom’s taxonomy of educational objectives (Complete ed., [Nachdr.]). Longman.




