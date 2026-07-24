# Einführung in das Online-Tool LogicTraffic

LogicTraffic ist eine Lernumgebung, in der Verkehrssituationen, Wahrheitstabellen und boolesche Formeln miteinander verbunden werden. Ziel ist, eine logische Regel zu finden, die eine Kreuzung sicher macht.

- [KA1 - Einführung](#ka1-einfuehrung)
- [KA2 - Schaltzentrale](#ka2-schaltzentrale)
- [EA1 - Oberfläche verstehen](#ea1-oberflaeche-verstehen)
- [ÜA1 - Kreuzung und Tabelle](#ua1-kreuzung-und-tabelle)
- [ÜA2 - Tool-Führerschein](#ua2-tool-fuehrerschein)
- [SA1 - Gesamtaufgabe](#sa1-gesamtaufgabe)

## Programmaufbau

Abbildung: LogicTraffic-Oberfläche.

| Bereich | Bedeutung |
| --- | --- |
| Kreuzung | zeigt die Verkehrssituation und die Ampeln |
| Variablen | jede Spur wird mit `A`, `B`, `C` usw. bezeichnet |
| Wahrheitstabelle | listet alle Ampelkombinationen |
| Spalte "sicher" | legt fest, welche Kombinationen erlaubt sind |
| Statusanzeige | meldet, ob die aktuelle Lösung sicher und optimal ist |
| Formelbereich | zeigt passende boolesche Formeln in verschiedenen Formen |

## Aufgaben

<a id="ka1-einfuehrung"></a>
<details markdown>
<summary>KA1 - Einführung</summary>

### Ziel

Die Lernenden beschreiben eine reale oder bildlich gezeigte Kreuzung und formulieren erste Wenn-dann-Sätze.

### Ablauf

| Phase | Auftrag |
| --- | --- |
| Ausgangspunkt | Bild oder Video einer stark befahrenen Kreuzung zeigen. |
| Beobachtung | Lernende beschreiben, was gleichzeitig passieren muss, damit niemand verunfallt. |
| Sprachlicher Auftrag | Mindestens drei Wenn-dann-Sätze formulieren. |
| Übergang | Frage: Wer oder was entscheidet, wann welche Ampel leuchtet? |

Material: Bilder für KA1, Arbeitsblatt KA1

</details>

<a id="ka2-schaltzentrale"></a>
<details markdown>
<summary>KA2 - Die Schaltzentrale</summary>

### Ziel

Die Lernenden formulieren erste Steuerungsregeln und erkennen, dass sichere Ampelsteuerung klare Bedingungen braucht.

### Ablauf

| Phase | Auftrag |
| --- | --- |
| Leitfrage | "Stell dir vor, du bist die Schaltzentrale dieser Kreuzung." |
| Einzel- oder Gruppenarbeit | Kreuzung skizzieren und Ampelregeln notieren. |
| Austausch | Widersprüche oder ungeregelte Situationen suchen. |
| Plenum | Übergang zur Frage, wie ein Computer solche Regeln verarbeiten könnte. |

</details>

<a id="ea1-oberflaeche-verstehen"></a>
<details markdown>
<summary>EA1 - Oberfläche und Grundkonzept verstehen</summary>

### Ziel

Die Lernenden lernen die Oberfläche kennen und verbinden Ampelsituation, Wahrheitstabelle und Formel.

### Ablauf

| Schritt | Auftrag |
| --- | --- |
| 1. Tool öffnen | LogicTraffic öffnen und eine einfache Situation wählen. |
| 2. Oberfläche beschriften | Kreuzung, Wahrheitstabelle, Statusanzeige, Simulation und Formelbereich markieren. |
| 3. Ampelwerte zuordnen | Eine Ampel anklicken und prüfen, welcher Tabellenwert zu grün bzw. rot gehört. |
| 4. Tabelle verändern | Werte in der Spalte "sicher" ändern und die Statusanzeige beobachten. |
| 5. Formel beobachten | Zwischen DNF, KNF und einfachster Formel wechseln. |

Material: Arbeitsblatt EA1

Abbildung: Lösung zur Oberflächenbeschriftung.

</details>

<a id="ua1-kreuzung-und-tabelle"></a>
<details markdown>
<summary>ÜA1 - Von der Kreuzung zur Tabelle und zurück</summary>

### Ziel

Die Lernenden erkennen, dass die Wahrheitstabelle festlegt, welche Ampelkombinationen sicher sind, und dass die Formel genau diese Zeilen beschreibt.

### Ablauf

| Schritt | Auftrag |
| --- | --- |
| 1. Situation wählen | Wähle eine Situation mit zwei Fahrspuren. |
| 2. Ampeln ausprobieren | Teste `A` grün/rot und `B` grün/rot in allen Kombinationen. |
| 3. Tabellenzeilen prüfen | Markiere zu jeder Ampelsituation die passende Tabellenzeile. |
| 4. Regel formulieren | Schreibe eine Sicherheitsregel in Alltagssprache. |
| 5. Formel vergleichen | Vergleiche die Regel mit der Formel im Tool. |

Material: Arbeitsblatt ÜA1

</details>

<a id="ua2-tool-fuehrerschein"></a>
<details markdown>
<summary>ÜA2 - Tool-Führerschein</summary>

### Ziel

Die Lernenden festigen grundlegende Bedienhandlungen und können die Statusanzeige fachlich deuten.

### Checkliste

| Kompetenz | Ich kann ... |
| --- | --- |
| Situation wählen | eine vorgegebene Verkehrssituation auswählen. |
| Ampeln verändern | Ampeln anklicken und die passende Tabellenzeile finden. |
| Sicherheit ändern | Werte in der Spalte "sicher" ändern. |
| Status deuten | "nicht sicher", "sicher, nicht optimal" und "optimal" erklären. |
| Formelansicht wechseln | DNF, KNF und einfachste Formel vergleichen. |

Diese Aufgabe eignet sich auch als kurze formative Beurteilung.

</details>

<a id="sa1-gesamtaufgabe"></a>
<details markdown>
<summary>SA1 - LogicTraffic in einer Gesamtaufgabe anwenden</summary>

### Ziel

Die Lernenden verbinden mehrere Teilkompetenzen in einer komplexeren Aufgabe.

### Auftrag

| Schritt | Auftrag |
| --- | --- |
| 1. Situation auswählen | Wähle eine Situation mit drei Autos und beschreibe die Spuren. |
| 2. Tabelle ausfüllen | Bearbeite die Wahrheitstabelle so, dass die Lösung sicher ist. |
| 3. Status prüfen | Am Schluss soll die Statusanzeige "optimal" anzeigen. |
| 4. Formel erklären | Schreibe die einfachste Formel ab und erkläre sie in 2 bis 3 Sätzen. |

Voraussetzung: Grundlagen zu Wahrheitstabellen und Formeln sollten bereits eingeführt sein.

</details>
