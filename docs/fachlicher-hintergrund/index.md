## Grundidee von LogicTraffic

LogicTraffic simuliert eine Strassenkreuzung mit Ampeln für verschiedene Fahrspuren. Ziel ist es, eine logische Formel zu finden, die sicherstellt, dass kreuzende Spuren nie gleichzeitig grün haben und entsprechend keine Kollisionen möglich sind. Dadurch wird sichtbar, wie Aussagenlogik in einem alltagsnahen Steuerungsproblem angewendet werden kann.

In LogicTraffic wird jeder Fahrspur eine eigene boolsche Variable zugewiesen. Eine Ampel ist entweder rot (Variablenwert `0`) oder grün (Variablenwert `1`). Die Wahrheitstabelle listet alle möglichen Kombinationen dieser Ampelzustände auf. Die Formel beschreibt anschliessend, welche Kombinationen sicher sind.

## Zentrale Begriffe

| Begriff | Kurze Erklärung | Beispiel in LogicTraffic |
| --- | --- | --- |
| Aussage | Ein Sachverhalt, der eindeutig wahr oder falsch ist. | "Ampel A ist grün." |
| Wahrheitswert | Wert einer Aussage: wahr/`1` oder falsch/`0` | Die Aussage "Ampel A ist grün." stimmt. |
| Variable | Platzhalter für eine Aussage | `A`, `B`, `C` stehen für Fahrspuren bzw. Ampeln. |
| Junktor bzw. Operator | Logisches Verknüpfungszeichen, das Aussagen verbindet. Erzeugt aus Wahrheitswerten neue Wahrheitswerte.| `A ∧ B`, `A ∨ B`, `¬A` |
| Boolesche Funktion | Ordnet jeder Kombination von Eingabewerten genau einen Ausgabewert zu. | Eine Sicherheitsregel für eine Kreuzung |
| Wahrheitstabelle | Tabelle mit allen `2^n` Kombinationen von `n` Variablen.| Alle Rot-Grün-Kombinationen einer Verkehrssituation mit n Spuren |
| Normalform | Standardisierte Form einer booleschen Formel | DNF, KNF, KDNF, KKNF |

## Aussagenlogik in LogicTraffic

In der Aussagenlogik werden Aussagen mit genau zwei möglichen Wahrheitswerten betrachtet: wahr oder falsch. In LogicTraffic entspricht das dem Ampelzustand:

| Logischer Wert | Bedeutung in LogicTraffic | Praktische Bedeutung |
| --- | --- | --- |
| `1` | Ampel ist grün | Die entsprechende Spur ist befahrbar. |
| `0` | Ampel ist rot | Die entsprechende Spur ist nicht befahrbar. |

Eine einfache Aussage ist zum Beispiel:

| Schreibweise | Bedeutung |
| --- | --- |
| `A` | Spur A hat grün. |
| `¬A` | Spur A hat nicht grün, also rot. |
| `A ∧ ¬B` | Spur A hat grün und Spur B hat rot. |

Solche Aussagen werden zu Formeln verknüpft. Eine Formel beschreibt dann nicht mehr nur eine einzelne Ampel, sondern Sicherheitsbedingungen für die gegebene Kreuzung.