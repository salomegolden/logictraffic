# Lehrplan und Lernziele

Die Unterrichtseinheit richtet sich an **gymnasiale Klassen der 8.–9. Schulstufe ohne Vorkenntnisse in Aussagenlogik**. Am Ende des Basisteils können die Lernenden eine einfache Verkehrskreuzung untersuchen, ihre möglichen Ampelzustände vollständig erfassen und eine passende Sicherheitsformel entwickeln und überprüfen.

Die vier übergeordneten Lernziele werden in den Bausteinen schrittweise aufgebaut. Die Kennzeichnungen **LZ1–LZ4** und ihre Teilziele verbinden diese Übersicht mit den konkreten Unterrichtszielen. Den zeitlichen und didaktischen Verlauf erläutert der [Aufbau der Unterrichtseinheit](aufbau.md).

## Anspruch für die 8.–9. Klasse

**LZ1–LZ3 bilden den gemeinsamen Kern.** Selbstständige Tabellen und Formeln werden zunächst an zwei bis drei Variablen erarbeitet. Grössere Kreuzungen veranschaulichen den wachsenden Aufwand; ihre vollständige Bearbeitung ist kein allgemeines Abschlussziel des Basisteils. Das Verdoppeln der Anzahl möglicher Zustände führt anschaulich zu $2^n$; ein formaler kombinatorischer Beweis wird nicht vorausgesetzt.

**LZ4 ist eine optionale Vertiefung.** Normalformen werden an kleinen Beispielen untersucht. Das systematische Erzeugen kanonischer Formen dient als Hilfe; ein allgemeines Minimierungsverfahren oder der Nachweis einer absolut kürzesten Formel wird nicht verlangt. Auch der Transfer auf fünf Variablen ist optional.

Die fachlichen Erwartungen gelten für beide Varianten von Baustein 1. Beim [enaktiven Einstieg](../unterricht/baustein1-enaktiv.md#lernziele) werden sie handelnd, beim [lehrpersonenzentrierten Einstieg](../unterricht/baustein1-lehrpersonenzentriert.md#lernziele) anhand statischer Bilder und angeleiteter Aufgaben erarbeitet. Formale Operatoren und die Codierung mit `0` und `1` werden in diesem ersten Baustein noch nicht vorausgesetzt.

Der ergänzende [Logikblock zu Aussagen und historischen Bezugspunkten](../unterricht/baustein1-lehrpersonenzentriert.md#phase-1-logik-einordnen-und-aussagen-verstehen) bereitet das Verständnis wahrer und falscher Aussagen vor. Die geschichtliche Einordnung dient der Orientierung und ist kein gemeinsames fachliches Prüfziel. Werden beide Einstiege in einer Untersuchung verglichen, wird dieser Hintergrundteil in beiden Gruppen mit demselben Inhalt und Zeitbudget berücksichtigt.

## Lernziele und Bausteine im Überblick

| Lernziel | Erwartete Kompetenz | Wo wird sie aufgebaut? | Umfang |
| --- | --- | --- | --- |
| [LZ1](#lernziel-1-logische-operatoren-und-wahrheitstabellen) | Zustände erklären, Darstellungen verbinden, vollständige Tabellen erstellen und Operatoren deuten | Bausteine 1–3; Operatoren in Baustein 4 | Basis |
| [LZ2](#lernziel-2-boolesche-formeln-aus-textbeschreibungen-ableiten) | Sicherheitsregeln formulieren, in Formeln übersetzen und erklären | Sprachliche Vorbereitung in Baustein 1; Formeln in Baustein 4 | Basis |
| [LZ3](#lernziel-3-fehlerhafte-ampelsteuerungen-untersuchen) | Tabellen und Formeln systematisch prüfen, Fehler finden und korrigieren | Bausteine 3–4; Sicherheitsbeurteilung ab Baustein 1 | Basis |
| [LZ4](#lernziel-4-normalformen-und-minimierung-boolescher-ausdruecke) | Gleichwertige Formeln, Normalformen und einfache Vereinfachungen begründet vergleichen | Baustein 4, Phasen 4–6 | Optional |

## LZ1: Zustände, Wahrheitstabellen und Operatoren verstehen {#lernziel-1-logische-operatoren-und-wahrheitstabellen}

Die Lernenden können eine konkrete Ampelstellung sprachlich und tabellarisch beschreiben, alle Belegungen einer einfachen Kreuzung systematisch erfassen und logische Operatoren im Verkehrskontext erklären.

### LZ1a · Verkehrssituationen und Darstellungen deuten {#lz1a}

Die Lernenden können Fahrwege und Konfliktpaare erkennen und sichere von unsicheren Ampelkombinationen begründet unterscheiden. Ab Baustein 2 ordnen sie Fahrspuren den Variablen und eine Ampelstellung einer Tabellenzeile zu – auch in umgekehrter Richtung. Dabei unterscheiden sie `0`/`1` als Ampelzustand von `0`/`1` als Sicherheitsbewertung.

**Beobachtbarer Nachweis:** Eine vorgegebene Kombination wird dargestellt und begründet bewertet; die Lernenden erklären, weshalb auch „alle Rot“ kollisionsfrei ist. Sie unterscheiden eine einzelne Belegung von der gesamten Tabelle und von einer Regel für alle Belegungen.

**Erarbeitung:** [Baustein 1 enaktiv – Lernziele](../unterricht/baustein1-enaktiv.md#lernziele) oder [Baustein 1 lehrpersonenzentriert – Lernziele](../unterricht/baustein1-lehrpersonenzentriert.md#lernziele), anschliessend [Baustein 2 – Lernziele](../unterricht/baustein2-logictraffic.md#lernziele), Sicherung mit 2c.

### LZ1b · Alle möglichen Zustände systematisch erfassen {#lz1b}

Die Lernenden können für zwei und drei Variablen alle Belegungen vollständig und ohne Wiederholungen aufschreiben, nach den Fahrwegen bewerten und ihr Ordnungsmuster erläutern. Sie erklären, dass jede zusätzliche Variable die Zeilenzahl verdoppelt, und wenden $2^n$ auf kleine Beispiele an. Am Beispiel von fünf Variablen begründen sie, weshalb eine kompaktere Darstellung nützlich wird.

**Beobachtbarer Nachweis:** Eine selbst erstellte Tabelle enthält bei drei Variablen genau acht unterschiedliche Belegungen und eine begründete Sicherheitsbewertung für jede Zeile.

**Erarbeitung:** erste Rot-Grün-Sammlungen in beiden Varianten von Baustein 1; selbstständiger Aufbau in [Baustein 3 – Lernziele](../unterricht/baustein3-wahrheitstabellen.md#lernziele) mit 3a und 3b. [Fachlicher Hintergrund: Wahrheitstabellen](../fachlicher-hintergrund/wahrheitstabellen.md).

### LZ1c · Logische Operatoren im Kontext erklären {#lz1c}

Die Lernenden können NICHT (`¬`), UND (`∧`) und das einschliessende ODER (`∨`) lesen und auf konkrete Belegungen anwenden. Die Implikation (`→`) deuten sie an einfachen Konfliktregeln wie $A \rightarrow \neg B$: Die Regel ist genau dann verletzt, wenn beide kreuzenden Spuren Grün haben. Klammern machen den Aufbau der Formel eindeutig.

**Beobachtbarer Nachweis:** Die Lernenden lesen eine kurze Formel in Worten und bestimmen ihren Wahrheitswert bei vorgegebenen Belegungen. Sie können erklären, weshalb $A \rightarrow \neg B$ bei roter Ampel A keine Einschränkung für B verlangt.

**Erarbeitung:** [Baustein 4 – Basisteil](../unterricht/baustein4-boolesche-algebra.md#basisteil), insbesondere 4b und Merkblatt 4d. [Fachlicher Hintergrund: Operatoren](../fachlicher-hintergrund/boolesche-algebra.md).

## LZ2: Sicherheitsregeln entwickeln und in Formeln übersetzen {#lernziel-2-boolesche-formeln-aus-textbeschreibungen-ableiten}

Die Lernenden können die Konflikte einer einfachen Kreuzung mit zwei bis drei Variablen in eigenen Worten beschreiben und daraus eine Formel entwickeln, die genau die sicheren Belegungen zulässt. Sie übersetzen auch zurück von der Formel zur Verkehrsbedeutung.

| Teilkompetenz | Beobachtbarer Nachweis |
| --- | --- |
| Konfliktpaare bestimmen und Regeln formulieren | Die Lernenden begründen anhand der Fahrwege, welche Spuren nicht gleichzeitig Grün haben dürfen. |
| Sprache in eine Formel übersetzen | Für zwei kreuzende Spuren entsteht etwa $\neg(A \land B)$; mehrere notwendige Konfliktbedingungen werden mit UND verbunden. |
| Formel erklären und eingeben | Die Lernenden erklären die Teilbedingungen und geben die Formel mit passenden Klammern in LogicTraffic ein. |

**Erarbeitung:** sprachliche Vorbereitung in [Baustein 1 enaktiv](../unterricht/baustein1-enaktiv.md#lernziele) oder [Baustein 1 lehrpersonenzentriert](../unterricht/baustein1-lehrpersonenzentriert.md#lernziele); formale Umsetzung in [Baustein 4 – Basisteil](../unterricht/baustein4-boolesche-algebra.md#basisteil) mit 4a–4c. Die Überprüfung der Lösung gehört zu LZ3.

## LZ3: Tabellen und Sicherheitsformeln überprüfen {#lernziel-3-fehlerhafte-ampelsteuerungen-untersuchen}

Die Lernenden können Fehler in Tabellen und Formeln anhand der modellierten Kreuzung lokalisieren, erklären und korrigieren. Sie unterscheiden eine unvollständige Auflistung der Zustände von einer falschen Sicherheitsbewertung.

### LZ3a · Fehler in Wahrheitstabellen finden {#lz3a}

Die Lernenden erkennen fehlende, doppelte und falsch bewertete Belegungen. Sie begründen ihre Korrektur mit dem Ordnungsmuster oder den Fahrwegen.

**Beobachtbarer Nachweis:** Zu einer fehlerhaften Tabelle nennen sie die betroffene Zeile, die Fehlerart und eine begründete Korrektur.

**Erarbeitung:** [Baustein 3 – Lernziele](../unterricht/baustein3-wahrheitstabellen.md#lernziele), besonders die Fehleranalyse mit 3c.

### LZ3b · Formeln an allen Belegungen prüfen {#lz3b}

Die Lernenden vergleichen die Ausgabewerte einer Formel mit der unabhängig begründeten Sicherheitsbewertung aller Tabellenzeilen. Sie finden sowohl gefährliche Belegungen, die fälschlich zugelassen werden, als auch sichere Belegungen, die die Formel unnötig ausschliesst. Ein Gegenbeispiel widerlegt eine Formel; einzelne erfolgreiche Tests allein bestätigen noch nicht ihre vollständige Korrektheit.

**Beobachtbarer Nachweis:** Die Lernenden zeigen eine abweichende Belegung an der Kreuzung, berichtigen die betreffende Teilregel und kontrollieren die geänderte Formel erneut vollständig.

**Erarbeitung:** [Baustein 4 – Basisteil](../unterricht/baustein4-boolesche-algebra.md#basisteil), insbesondere 4c. Unterstützung bieten die [typischen Lernschwierigkeiten](lernschwierigkeiten.md).

## LZ4: Gleichwertige Formeln und Normalformen vergleichen {#lernziel-4-normalformen-und-minimierung-boolescher-ausdruecke}

**Optionales Vertiefungsziel:** Die Lernenden können an kleinen Beispielen erklären, weshalb verschieden aufgebaute Formeln dieselbe Sicherheitsfunktion beschreiben. Sie unterscheiden DNF und KNF, verfolgen den Weg von Tabellenzeilen zu kanonischen Formen und beurteilen einfache Vereinfachungen.

| Teilkompetenz | Beobachtbarer Nachweis | Material |
| --- | --- | --- |
| Äquivalenz überprüfen | Zwei Formeln ergeben bei jeder Belegung denselben Wahrheitswert; eine einfache De-Morgan-Umformung wird erklärt. | 4e |
| DNF und KNF unterscheiden | Die Lernenden erkennen eine ODER-Verknüpfung von UND-Termen bzw. eine UND-Verknüpfung von ODER-Klauseln. | 4e |
| Kanonische Formen nachvollziehen | Eine sichere Zeile wird einem vollständigen UND-Term der KDNF zugeordnet; eine unsichere Zeile einer ODER-Klausel der KKNF, die genau diese Belegung ausschliesst. | 4f |
| Darstellungen begründet vergleichen | Die Lernenden vergleichen gleichwertige Formeln nach Lesbarkeit, Länge und Bezug zur Kreuzung; einfache Vereinfachungen werden auf Äquivalenz geprüft. | 4g |

**Erarbeitung:** [Baustein 4 – optionale Vertiefung](../unterricht/baustein4-boolesche-algebra.md#optionale-vertiefung). [Fachlicher Hintergrund: Normalformen](../fachlicher-hintergrund/normalformen.md).

Für Lernende mit Unterstützungsbedarf genügt zunächst die KDNF als systematischer Weg. Das selbstständige Erzeugen beider kanonischer Formen und weitere algebraische Umformungen sind Erweiterungen, keine Voraussetzung zum Erreichen der Basisziele.

## Optionaler Transfer: Bekanntes auf eine grössere Kreuzung anwenden

Der [Transfer in Baustein 4](../unterricht/baustein4-boolesche-algebra.md#optionaler-transfer) mit 4h erweitert **LZ2 und LZ3b** auf fünf Variablen. Die Lernenden identifizieren Konfliktpaare, verbinden Teilregeln und prüfen die Gesamtformel anhand aller 32 Belegungen mit LogicTraffic. Sie erläutern, wie das Zerlegen in Teilprobleme ihre Lösung unterstützt.

Normalformen sind für diesen direkten Weg über die Konflikte keine Voraussetzung. Bei Bedarf kann die Wahrheitstabelle mit einer kanonischen Form als Hilfestellung dienen.

## Lernziele im Unterricht beobachten und beurteilen

| Unterrichtsabschnitt | Fokus | Geeigneter Nachweis |
| --- | --- | --- |
| [Baustein 1 – enaktiv](../unterricht/baustein1-enaktiv.md#lernziele) **oder** [lehrpersonenzentriert](../unterricht/baustein1-lehrpersonenzentriert.md#lernziele) | LZ1a; Vorbereitung LZ1b und LZ2 | Sichere und unsichere Stellungen begründen, Rot-Grün-Kombinationen ordnen und eine Regel in Worten ausdrücken |
| [Baustein 2](../unterricht/baustein2-logictraffic.md#lernziele) | LZ1a | Eine Tabellenzeile an der Kreuzung zeigen und die beiden Bedeutungen von `0`/`1` erklären |
| [Baustein 3](../unterricht/baustein3-wahrheitstabellen.md#lernziele) | LZ1b und LZ3a | Eine vollständige Tabelle erstellen und eine fehlerhafte Tabelle begründet korrigieren |
| [Baustein 4 – Basisteil](../unterricht/baustein4-boolesche-algebra.md#basisteil) | LZ1c, LZ2 und LZ3b | Eine Formel entwickeln, erläutern und vollständig prüfen |
| [Baustein 4 – Vertiefung](../unterricht/baustein4-boolesche-algebra.md#optionale-vertiefung) | LZ4 | Zwei äquivalente Darstellungen erklären und vergleichen |
| [Baustein 4 – Transfer](../unterricht/baustein4-boolesche-algebra.md#optionaler-transfer) | LZ2 und LZ3b auf höherem Anspruchsniveau | Die komplexere Kreuzung selbstständig modellieren und den Prüfweg begründen |

Die [Beurteilungsaufgaben](../unterricht/beurteilung.md) greifen diese Nachweise auf. Eine Abschlussaufgabe zum Basisteil verwendet eine neue, überschaubare Kreuzung mit zwei bis drei Variablen. Optionale Inhalte werden nur beurteilt, wenn sie zuvor erarbeitet und als Leistungserwartung angekündigt wurden.

## Lehrplanbezug und Einordnung

Für die 8.–9. Klasse dient der **Lehrplan 21** als Bezug zur obligatorischen Schulzeit; der **Rahmenlehrplan für gymnasiale Maturitätsschulen** beschreibt den weiterführenden Bildungsrahmen. Die konkrete Zuordnung zu Jahrgang und Fach richtet sich nach dem kantonalen bzw. schulischen Lehrplan. Die hier gewählte Progression ist eine didaktische Ausgestaltung für diese Unterrichtseinheit und keine schweizweit verbindliche Stoffverteilung für die 8.–9. Klasse.[^edk]

| Bezug | Beitrag dieser Unterrichtseinheit |
| --- | --- |
| **MI.2.1.b:** unterschiedliche Darstellungen für Daten nutzen | LZ1a greift diese bereits früher aufgebaute Kompetenz auf und verbindet Kreuzungsbild, Sprache und Tabelle.[^daten] |
| **MI.2.1.i, Zyklus 3:** logische Operatoren verwenden | LZ1c und LZ2 konkretisieren UND, ODER und NICHT an Sicherheitsregeln. Die Implikation wird als zusätzliche, kontextgebundene Schreibweise eingeführt.[^daten] |
| **MI.2.2:** Probleme analysieren und Lösungsverfahren beschreiben und umsetzen | LZ1b, LZ2 und LZ3 fördern systematisches Vorgehen, Modellieren und Prüfen. Die Einheit behandelt dabei keine vollständige Programmieraufgabe mit Schleifen oder Unterprogrammen.[^algorithmen] |
| **Anschluss an gymnasiale Informatik** | Der Weg von einem realitätsnahen Problem zu einem formalen Modell bereitet weiterführendes Arbeiten mit logischen Bedingungen vor. LZ4 bietet eine zusätzliche fachliche Vertiefung. Der Rahmenlehrplan ist dabei Orientierung für den weiteren Bildungsgang.[^rlp] |

[^daten]: D-EDK: [Lehrplan 21, MI.2.1 – Datenstrukturen](https://v-fe.lehrplan.ch/index.php?code=a%7C10%7C0%7C2%7C0%7C1), insbesondere Kompetenzstufen b und i, Fassung vom 29. Februar 2016.
[^algorithmen]: D-EDK: [Lehrplan 21, MI.2.2 – Algorithmen](https://v-fe.lehrplan.ch/MI.2.2.f), Fassung vom 29. Februar 2016. Die Zuordnung zur Unterrichtseinheit beschreibt einen Beitrag zum Kompetenzaufbau, nicht die vollständige Abdeckung aller Teilkompetenzen.
[^edk]: EDK: [Lehrpläne der verschiedenen Bildungsstufen](https://edk.ch/de/bildungssystem/beschreibung/lehrplaene?highlight=663dc543f3294fcb9dc63171456ee57d).
[^rlp]: EDK: [Rahmenlehrplan gymnasiale Maturitätsschulen vom 20. Juni 2024](https://edudoc.ch/record/232281). [Einordnung und Funktion des Rahmenlehrplans](https://edk.ch/de/die-edk/news/mm200624).
