## Grundidee von LogicTraffic

LogicTraffic simuliert eine Strassenkreuzung mit Ampeln für verschiedene Fahrspuren. Ziel ist es, eine logische Formel zu finden, die sicherstellt, dass kreuzende Spuren nie gleichzeitig grün haben. Dadurch wird sichtbar, wie Aussagenlogik in einem alltagsnahen Steuerungsproblem angewendet wird.

In LogicTraffic wird jede Fahrspur durch eine Variable beschrieben. Eine Ampel ist entweder rot (`0`) oder grün (`1`). Die Wahrheitstabelle listet alle möglichen Kombinationen dieser Ampelzustände auf. Die Formel beschreibt anschliessend, welche Kombinationen sicher sind.

## Zentrale Begriffe

| Begriff | Kurze Erklärung | Beispiel in LogicTraffic |
| --- | --- | --- |
| Aussage | Ein Sachverhalt, der eindeutig wahr oder falsch ist. | "Ampel A ist grün." |
| Wahrheitswert | Wert einer Aussage: wahr/`1` oder falsch/`0` | `A = 1` bedeutet: Spur A ist befahrbar. |
| Variable | Platzhalter für eine Aussage oder einen Zustand | `A`, `B`, `C` stehen für Fahrspuren bzw. Ampeln. |
| Junktor | Logisches Verknüpfungszeichen, das Aussagen verbindet. | `A ∧ B`, `A ∨ B`, `¬A` |
| Operator | Rechenzeichen der booleschen Logik; erzeugt aus Wahrheitswerten neue Wahrheitswerte.| UND, ODER, NICHT |
| Boolesche Funktion | Ordnet jeder Kombination von Eingabewerten genau einen Ausgabewert zu. | Eine Sicherheitsregel für eine Kreuzung |
| Wahrheitstabelle | Tabelle mit allen `2^n` Kombinationen von `n` Variablen.| Alle Rot-Grün-Kombinationen einer Situation |
| Normalform | Standardisierte Form einer booleschen Formel | DNF, KNF, KDNF, KKNF |

## Aussagenlogik in LogicTraffic

In der Aussagenlogik werden Aussagen mit genau zwei möglichen Wahrheitswerten betrachtet: wahr oder falsch. In LogicTraffic entspricht das dem Ampelzustand:

| Logischer Wert | Bedeutung in LogicTraffic | Alltagssprache |
| --- | --- | --- |
| `1` | Ampel ist grün | Die Spur ist befahrbar. |
| `0` | Ampel ist rot | Die Spur ist gesperrt. |

Eine einfache Aussage ist zum Beispiel:

| Schreibweise | Bedeutung |
| --- | --- |
| `A` | Spur A hat grün. |
| `¬A` | Spur A hat nicht grün, also rot. |
| `A ∧ ¬B` | Spur A hat grün und Spur B hat rot. |

Solche Aussagen werden zu Formeln verknüpft. Eine Formel beschreibt dann nicht mehr nur eine einzelne Ampel, sondern eine ganze Sicherheitsregel für die Kreuzung.