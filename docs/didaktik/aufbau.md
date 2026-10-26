# Aufbau der Unterrichtseinheit

Die Unterrichtseinheit führt von der Untersuchung vorgegebener Fahrwege über digitale und tabellarische Darstellungen zu aussagenlogischen Formeln. Eine Klasse wählt **einen von zwei aktiven Einstiegen** mit denselben fachlichen Lernzielen. Der gemeinsame Abschnitt [«Einstieg in die Logik»](../unterricht/baustein1-logikblock.md) ist eine freiwillige Ergänzung für beide Varianten ausserhalb der regulären Zeitplanung. Er ist keine Voraussetzung für Baustein 2. Die Bausteine 2–4 bilden den gemeinsamen weiteren Lernweg.

## Der Lernweg auf einen Blick

| Abschnitt | Was machen die Lernenden? | Materialien und Hinweise |
| --------- | ------------------------- | ------------------------ |
| **Alternative A:** [Baustein 1a – Enaktiver Einstieg](../unterricht/baustein1-enaktiv.md) | Sie fahren Fahrwege mit Fahrzeugen nach, untersuchen Konfliktpaare und prüfen Ampelbelegungen. Für drei Ampeln ordnen und bewerten sie alle acht Belegungen. | AB1a–AB1c im [Dossier](../downloads/baustein1/v1/baustein1-enaktiv-dossier.pdf); Materialset pro Lernpaar. **65–85 Min.** |
| **Alternative B:** [Baustein 1b – Kreuzungen anhand von Darstellungen untersuchen](../unterricht/baustein1-lehrpersonenzentriert.md) | Sie verfolgen Fahrwege in Kreuzungsbildern, bestimmen Konfliktpaare und beurteilen Ampelbelegungen. Sie erstellen eine vollständige Tabelle und formulieren eine sprachliche Sicherheitsregel. | AB1a–AB1d im [Dossier](../downloads/baustein1/v1/baustein1-darstellungen-dossier.pdf), Präsentation. **70–85 Min.**, aus den Einzelzeiten berechnet. |
| [Baustein 2 – LogicTraffic kennenlernen](../unterricht/baustein2-logictraffic.md) | Sie verändern Ampelbelegungen in LogicTraffic und ordnen Kreuzungsbild, Variablen, `0`/`1` und Tabellenzeilen einander zu. Sie unterscheiden Ampelwerte von der Sicherheitsbewertung. | AB2a zur Erkundung, danach MB2b als Nachschlagehilfe; AB2c und Tafelbild 2e zur Sicherung. **55–65 Min.** |
| [Baustein 3 – Wahrheitstabellen](../unterricht/baustein3-wahrheitstabellen.md) | Sie erstellen Tabellen für zwei und drei Variablen, erklären ihre Vollständigkeit und untersuchen fehlende, doppelte oder falsch bewertete Zeilen. | AB3a–AB3c; Tabellen zunächst auf Papier, danach mit LogicTraffic prüfen. **65–75 Min.** |
| [Baustein 4 – Aussagenlogische Formeln](../unterricht/baustein4-boolesche-algebra.md) | Sie formulieren Konfliktregeln in Worten, übersetzen sie in Teilformeln und verbinden diese zu einer Gesamtformel. Diese prüfen sie anhand aller Ampelbelegungen. | Basisteil: AB4a–AB4c und MB4d. **70 Min.** Vertiefung und Transfer werden separat gewählt. |

**Optional: [Einstieg in die Logik](../unterricht/baustein1-logikblock.md).** Mit AB1X unterscheiden die Lernenden Aussagen von Fragen und Aufforderungen. Der Abschnitt kann zu beiden Varianten ergänzt werden und ist weder eine dritte Einstiegsvariante noch ein verpflichtender nächster Schritt. Bei seinem Einsatz fallen einmal **10–15 Minuten zusätzlich** an. AB1X steht im Dossier zu 1a auf S. 12 und im Dossier zu 1b auf S. 7; hinzu kommt die Präsentation «Erweiterung Logik». Die Kommentare ordnen den Abschnitt dem gemeinsamen weiteren Unterricht nach dem gewählten Einstieg zu; die genauere Position ist nicht festgelegt. Wird er in beiden Varianten eingesetzt, sind derselbe Zeitpunkt und dieselbe Bearbeitungszeit vorgesehen.

[Unterricht vorbereiten](../unterricht/vorbereitung.md) · [Lernziele und Anforderungen](lernziele.md) · [Alle Unterrichtsmaterialien](../anhang/downloads.md)

## Darstellungen miteinander verbinden

Beide Einstiege führen zunächst zu begründeten Sicherheitsbeurteilungen und **sprachlichen Sicherheitsregeln**. Sie greifen auch schon die vollständige Sammlung von Ampelbelegungen auf. In Baustein 2 werden die Darstellungen in LogicTraffic gelesen und zugeordnet; Baustein 3 vertieft das selbstständige Erstellen und Prüfen vollständiger Wahrheitstabellen. Erst in Baustein 4 entwickeln die Lernenden selbst **aussagenlogische Formeln für die Sicherheitsbedingungen**.

Der [Darstellungswechsel](darstellungswechsel.md) bleibt in beide Richtungen wichtig: Eine Tabellenzeile wird als Ampelbelegung an der Kreuzung eingestellt, eine Formel in Alltagssprache zurückübersetzt und ihre Bewertung mit den Fahrwegen verglichen.

Bei zwei sich kreuzenden Fahrwegen lässt sich dieser Zusammenhang knapp zeigen:

| Darstellung | Sicherheitsbedingung |
| --- | --- |
| Fahrwege im Material oder Kreuzungsbild | Bei gleichzeitiger Freigabe ist eine Kollision möglich. |
| Sprachliche Regel | Die Ampeln A und B dürfen nicht gleichzeitig Grün zeigen. |
| Vollständige Wahrheitstabelle | `00`, `01` und `10` sind sicher; `11` ist unsicher. |
| Aussagenlogische Formel | $\neg(A \land B)$ ist genau für die sicheren Ampelbelegungen wahr. |

Bei den Ampelvariablen bedeutet `0` Rot und `1` Grün. In der Spalte **sicher** bedeutet `1` dagegen kollisionsfrei und `0` Kollisionsgefahr. Auch «alle Rot» ist ein sicherer Kreuzungszustand. Eine unsichere Ampelbelegung ermöglicht eine Kollision; diese muss nicht tatsächlich eintreten.

Das Ziel der Formelarbeit ist, **alle sicheren Ampelbelegungen zuzulassen und alle unsicheren auszuschliessen**. LogicTraffic modelliert statische Rot-Grün-Belegungen. Gelbphasen, Räumzeiten und zeitliche Verkehrssteuerung gehören nicht zu diesem Modell; Sicherheit und Verkehrsfluss sind unterschiedliche Fragen.

## Vertiefung und Transfer in Baustein 4

Der Basisteil endet mit dem Entwickeln und Überprüfen einfacher Sicherheitsformeln. Die folgenden Angebote bleiben Teile von Baustein 4 und benötigen zusätzliche Zeit:

- **Vertiefung, Phasen 4–6:** Mit AB4e–AB4g vergleichen die Lernenden gleichwertige Formeln, untersuchen De Morgan sowie DNF und KNF und nutzen KDNF/KKNF als systematischen Weg von der Tabelle zur Formel. **Zusätzlich 45 Minuten.** [Zur Vertiefung](../unterricht/baustein4-boolesche-algebra.md#phase-4-anders-gebaut-gleich-gemeint).
- **Transfer, Phase 7:** Mit AB4h analysieren sie Situation 10 mit fünf Variablen, verbinden Konfliktbedingungen und überprüfen ihre Formel mit LogicTraffic an allen 32 Belegungen. **Zusätzlich 20–30 Minuten.** [Zum Transfer](../unterricht/baustein4-boolesche-algebra.md#phase-7-transfer-situation-10).

## Zeit und Geräte planen

Für die gesamte Reihe bis zum Ende des Basisteils von Baustein 4 ergeben sich aus den aktuellen Modulseiten:

- **Mit Einstieg 1a:** 65–85 + 55–65 + 65–75 + 70 = **255–295 Minuten**.
- **Mit Einstieg 1b:** 70–85 + 55–65 + 65–75 + 70 = **260–295 Minuten**.

Jede reguläre Summe enthält **eine Einstiegsvariante sowie die Bausteine 2–4 mit Basisteil**. Der freiwillige Einstieg in die Logik ist nicht enthalten; bei seinem Einsatz werden separat 10–15 Minuten ergänzt. Einführung und Abschluss sind entsprechend den Modulseiten enthalten. Materialherstellung, optionale Erweiterungen, Vertiefung und Transfer kommen gegebenenfalls hinzu.

Beim Darstellungseinstieg nennt der Kommentar unterschiedliche Gesamtzeiten. Die hier verwendeten 70–85 Minuten sind die Summe seiner Einzelzeiten; die Abweichungen sind unter [Zeitplanung zu Baustein 1b](../unterricht/baustein1-lehrpersonenzentriert.md#zeitplanung) dokumentiert. Für Baustein 3 ist die vollständige Durchführung mit AB3c eingerechnet; bei einer Kürzung verändert sich die Gesamtdauer.

**Geräte:** Für Einstieg 1a benötigen die Lernenden keinen Computer. Einstieg 1b und, bei seinem Einsatz, der optionale Logikteil benötigen einen Computer mit Beamer oder Präsentationsbildschirm für die Lehrperson. Für **Bausteine 2–4 ist ein Computer oder Tablet mit LogicTraffic pro Zweiergruppe** vorgesehen. In Baustein 3 werden die Tabellen zunächst möglichst auf Papier bearbeitet und anschliessend digital kontrolliert.

## Lernfortschritte sichtbar machen

Kurze formative Lernkontrollen zeigen, ob eine Darstellung verstanden wurde oder eine Rückkehr zum Kreuzungsbild beziehungsweise Material hilfreich ist:

- **Nach dem gewählten Einstieg:** Eine sichere und eine unsichere Ampelbelegung anhand der Fahrwege begründen und eine sprachliche Sicherheitsregel formulieren.
- **Nach Baustein 3:** Die Vollständigkeit einer Tabelle erklären und fehlende, doppelte oder falsch bewertete Zeilen korrigieren.
- **Nach dem Basisteil von Baustein 4:** Eine Formel in Worten erläutern und zeigen, wie sie anhand aller Ampelbelegungen geprüft wurde.

Weitere Hinweise: [Beurteilungsaufgaben und Kriterien](../unterricht/beurteilung.md), [typische Lernschwierigkeiten](lernschwierigkeiten.md) und [fachlicher Hintergrund zu Wahrheitstabellen](../fachlicher-hintergrund/wahrheitstabellen.md).
