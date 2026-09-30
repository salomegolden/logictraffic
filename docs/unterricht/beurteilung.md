# Beurteilung

Die Beurteilungsaufgaben knüpfen an die Unterrichtssequenz an und trennen bewusst zwischen Lernstand sichtbar machen und Leistung bilanzieren.

Für die **8.–9. Klasse am Gymnasium** beziehen sich die gemeinsamen Leistungserwartungen auf [LZ1–LZ3](../didaktik/lernziele.md): Zustände und Tabellen verstehen, Sicherheitsformeln entwickeln und Lösungen prüfen. Die beiden Einstiegsvarianten werden an denselben fachlichen Kriterien beurteilt. [LZ4](../didaktik/lernziele.md#lernziel-4-normalformen-und-minimierung-boolescher-ausdruecke) und der Transfer auf fünf Variablen werden nur dann zusätzlich beurteilt, wenn sie unterrichtet und vorher als Leistungserwartung angekündigt wurden.

## Überblick

| Form | Zweck | Geeignet für |
| --- | --- | --- |
| Formative Beurteilung | Lernstand erkennen, Rückmeldung geben, nächste Schritte planen | kurze Diagnose, Partnergespräch, Lernjournal, Tool-Demonstration |
| Summative Beurteilung | erreichte Kompetenzen nachweisen und bewerten | Test, Abgabe, mündliche Erklärung, kombinierte Anwendung |

# Formative Beurteilungsaufgaben

Formative Beurteilung soll während des Lernprozesses sichtbar machen, welche Vorstellungen tragfähig sind und wo noch Unterstützung nötig ist. Die Aufgaben sind kurz und lassen sich gut in Unterrichtsphasen einbauen.

## Aufgabenideen

| Aufgabe | Beobachtungsschwerpunkt | Durchführung |
| --- | --- | --- |
| Ampelzustand erklären | Verstehen von `0` und `1` im Kontext der Kreuzung | Lernende zeigen eine Situation in LogicTraffic und erklären die Werte in der Tabelle. |
| Sichere Zeile begründen | Zusammenhang zwischen Tabelle und Kollision | Eine Zeile wird ausgewählt; Lernende begründen, ob sie sicher ist. |
| Formel laut lesen | Verbindung zwischen Formel und natürlicher Sprache | Lernende übersetzen z.B. `A ∧ ¬B` in einen Satz. |
| Fehler finden | Debugging und systematisches Prüfen | Eine unsichere Tabelle wird vorgegeben; Lernende finden die problematische Zeile. |
| Darstellungswechsel | Wechsel zwischen Bild, Tabelle, Sprache und Formel | Lernende beschreiben dieselbe Situation in zwei Darstellungen. |

## Rückmeldefragen

- Welche Variable steht für welche Spur?
- Was bedeutet `1` in dieser Zeile?
- Warum ist diese Kombination sicher oder unsicher?
- Welche Zeile der Wahrheitstabelle passt zur aktuellen Ampelsituation?
- Welche Bedingung beschreibt die Formel in Alltagssprache?

## Auswertung

Formative Aufgaben müssen nicht benotet werden. Hilfreich ist eine kurze Einordnung:

| Beobachtung | Möglicher nächster Schritt |
| --- | --- |
| Werte `0` und `1` werden verwechselt | Noch einmal mit Ampelkarten oder Simulation arbeiten |
| Nur einzelne Fälle werden geprüft | Wahrheitstabelle als systematische Liste aller Fälle betonen |
| Formel wird nicht sprachlich verstanden | Formel in kurze Satzbausteine zerlegen |
| OR wird exklusiv verstanden | Beispiele mit `A = 1` und `B = 1` gezielt prüfen |

# Summative Beurteilungsaufgaben

Summative Aufgaben prüfen, ob Lernende zentrale Kompetenzen der Unterrichtssequenz selbstständig anwenden können: Zustände deuten, Wahrheitstabellen nutzen, Formeln verstehen und Ergebnisse begründen.

## Mögliche Abschlussaufgabe

Die Lernenden erhalten eine neue Verkehrssituation mit zwei oder drei Fahrspuren.

| Schritt | Auftrag | Erwartete Leistung / Lernziel |
| --- | --- | --- |
| 1 | Spuren benennen und Ampelzustände als Variablen festlegen | Variablen sinnvoll zuordnen; Ampelzustand und Sicherheitsbewertung unterscheiden – [LZ1a](../didaktik/lernziele.md#lz1a) |
| 2 | Wahrheitstabelle selbstständig erstellen und das Ordnungsmuster erläutern | Alle vier bzw. acht Belegungen ohne Wiederholungen erfassen; $2^n$ erklären – [LZ1b](../didaktik/lernziele.md#lz1b) |
| 3 | Sichere und unsichere Zeilen markieren | Kollisionen anhand der Fahrwege begründen – [LZ1a](../didaktik/lernziele.md#lz1a) |
| 4 | Eine passende Formel entwickeln und in Worten erklären | Teilregeln sinnvoll verbinden und Operatoren deuten – [LZ1c](../didaktik/lernziele.md#lz1c) und [LZ2](../didaktik/lernziele.md#lernziel-2-boolesche-formeln-aus-textbeschreibungen-ableiten) |
| 5 | Formel mit der vollständigen, begründet bewerteten Tabelle vergleichen | Alle sicheren und nur die sicheren Belegungen zulassen – [LZ3b](../didaktik/lernziele.md#lz3b) |
| 6 | Eine zusätzlich vorgegebene fehlerhafte Tabelle und eine fehlerhafte Formel untersuchen | Fehlende, doppelte oder falsch bewertete Zeilen sowie eine abweichende Formelbelegung benennen und korrigieren – [LZ3a](../didaktik/lernziele.md#lz3a) und [LZ3b](../didaktik/lernziele.md#lz3b) |

Für Schritt 6 genügen kurze Beispiele mit jeweils einem gezielten Fehler. Die Operatoren werden an konkreten Belegungen geprüft; eine einfache Implikation kann als Leseaufgabe ergänzt werden. Die selbst entwickelte Formel muss nicht alle Operatoren verwenden. Eine vorgegebene Formel nur zu interpretieren weist das selbstständige Entwickeln einer Formel (LZ2) noch nicht nach.

Wer eine teilweise ausgefüllte Tabelle oder vorgegebene Teilformeln benötigt, kann damit dieselben Zusammenhänge bearbeiten. Bei der Rückmeldung wird ausgewiesen, welche Schritte selbstständig und welche mit Unterstützung gelungen sind.

## Bewertungskriterien

| Kriterium | Sichtbare Leistung |
| --- | --- |
| Fachbegriffe | Variablen, Wahrheitswerte und Operatoren werden korrekt verwendet. |
| Systematik | Die Wahrheitstabelle ist vollständig und nachvollziehbar. |
| Sicherheit | sichere und unsichere Zustände werden begründet. |
| Formelverständnis | Formel, Tabelle und Situation werden sinnvoll aufeinander bezogen. |
| Erklärung | Die Lösung ist sprachlich klar und fachlich präzise. |

## Varianten

- Kurze Prüfung: Wahrheitstabelle und Begründung für eine vorgegebene Situation.
- Praktische Prüfung: Lernende zeigen ihre Lösung direkt in LogicTraffic.
- Kombinierte Aufgabe: Fehler in einer gegebenen Ampelsteuerung finden und korrigieren.
- Mündliche Ergänzung: Eine Formel erklären und mit einer Tabellenzeile verbinden.
