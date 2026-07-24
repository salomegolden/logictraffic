# Normalformen

Normalformen sind standardisierte Darstellungen boolescher Funktionen. Sie helfen, aus einer Wahrheitstabelle systematisch eine Formel zu erzeugen und verschiedene Formeln miteinander zu vergleichen.[^1]

## Überblick

| Form | Grundidee | Blick auf die Wahrheitstabelle |
| --- | --- | --- |
| DNF | ODER von UND-Bausteinen | beschreibt Zeilen mit Ergebnis `1` |
| KNF | UND von ODER-Bausteinen | beschreibt Zeilen mit Ergebnis `0` |
| KDNF | vollständige DNF | jede wahre Zeile wird vollständig beschrieben |
| KKNF | vollständige KNF | jede falsche Zeile wird vollständig beschrieben |

## Kanonische disjunktive Normalform

Die kanonische disjunktive Normalform entsteht aus allen Zeilen, in denen die Funktion wahr ist. Jede dieser Zeilen wird zu einem vollständigen UND-Baustein. Alle Bausteine werden anschliessend mit ODER verbunden.[^1][^2]

Merksatz für Lernende:

| Schritt | Beschreibung |
| --- | --- |
| 1 | Suche alle Zeilen mit Ergebnis `1`. |
| 2 | Baue aus jeder dieser Zeilen einen vollständigen UND-Baustein. |
| 3 | Verbinde alle Bausteine mit ODER. |

Beispiel:

`(¬A ∧ ¬B ∧ C) ∨ (A ∧ ¬B ∧ C)`

Diese Formel sagt: Die Funktion ist wahr, wenn eine der beschriebenen Zeilen eintritt.

## Konjunktive Normalform

Die konjunktive Normalform arbeitet mit den Zeilen, in denen die Funktion falsch ist. Jede dieser Zeilen wird zu einem ODER-Baustein. Alle Bausteine werden anschliessend mit UND verbunden.[^1][^3]

Merksatz für Lernende:

| Schritt | Beschreibung |
| --- | --- |
| 1 | Suche alle Zeilen mit Ergebnis `0`. |
| 2 | Baue aus jeder dieser Zeilen einen vollständigen ODER-Baustein. |
| 3 | Verbinde alle Bausteine mit UND. |

Beispiel:

`(A ∨ ¬B ∨ C) ∧ (¬A ∨ B ∨ C)`

Diese Formel sagt: Alle Bedingungen müssen erfüllt sein, damit die ganze Formel wahr ist.

## Didaktische Hinweise

| Schwierigkeit | Unterstützung |
| --- | --- |
| Lernende verwechseln DNF und KNF | konsequent mit `1`-Zeilen bzw. `0`-Zeilen markieren |
| Negationen werden vergessen | jede Tabellenzeile Variable für Variable übersetzen |
| Formeln wirken zu lang | zuerst kanonisch vollständig arbeiten, erst danach vereinfachen |
| Bedeutung bleibt abstrakt | Formel wieder in Alltagssprache übersetzen lassen |

## Fachübergreifende Anschlüsse

| Fachbereich | Anschluss |
| --- | --- |
| Mathematik | Mengenlehre, Venn-Diagramme, algebraische Strukturen |
| Informatik | Schaltnetze, Logikgatter, Bedingungen in Programmen |
| Physik/Technik | digitale Schaltungen und Steuerungslogik |

## Weiterarbeiten

| Ziel | Seite |
| --- | --- |
| Grundlagen zu Wahrheitstabellen auffrischen | [Wahrheitstabellen](wahrheitstabellen.md) |
| typische Fehlvorstellungen vorbereiten |  |
| Aufgaben mit LogicTraffic einsetzen | |

[^1]: Boolesche Funktionen und ihre Normalformen. (2021, Juni 22). https://lehrerfortbildung-bw.de/u_matnatech/imp/gym/bp2016/fb2/m02_aug/1_hintergrund/4_grund/06_funktionen/
[^2]: Inf-schule | Schaltnetze: Fachkonzept disjunktive Normalform. Abgerufen 17. März 2026, von https://inf-schule.de/rechner/digitaltechnik/Schaltnetze/Fachkonzept_Normalform
[^3]: Konjunktive Normalform: Umwandlung & Beispiel. StudySmarter. Abgerufen 17. März 2026, von https://www.studysmarter.de/schule/informatik/theoretische-informatik/konjunktive-normalform/
