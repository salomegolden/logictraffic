## Grundidee von LogicTraffic

LogicTraffic simuliert eine Strassenkreuzung mit Ampeln für verschiedene Fahrspuren. Ziel ist es, eine aussagenlogische Formel zu finden, die sicherstellt, dass kreuzende Spuren nie gleichzeitig grün haben. Dadurch wird sichtbar, wie Aussagenlogik in einem alltagsnahen Problem angewendet wird.

In LogicTraffic wird jeder Fahrspur eine eigene boolsche Variable zugewiesen. Eine Ampel ist entweder rot (Variablenwert `0`) oder grün (Variablenwert `1`). Die Wahrheitstabelle listet alle möglichen Kombinationen dieser Ampelzustände auf. Die Formel beschreibt anschliessend, welche Kombinationen sicher sind.

## Zentrale Begriffe

| Begriff | Kurze Erklärung | Beispiel in LogicTraffic |
| --- | --- | --- |
| Aussage | Ein Sachverhalt, der eindeutig wahr oder falsch ist. | "Ampel A ist grün." |
| Wahrheitswert | Wert einer Aussage: wahr/`1` oder falsch/`0` | `A = 1` bedeutet: Spur A ist befahrbar. |
| Aussagevariable | Platzhalter für eine Aussage oder einen Zustand | `A`, `B`, `C` stehen für Fahrspuren bzw. Ampeln. |
| Operator | Rechenzeichen der booleschen Logik; erzeugt aus Wahrheitswerten neue Wahrheitswerte.| UND, ODER, NICHT |
| Boolesche Funktion | Ordnet jeder möglichen Belegung genau einen Ausgabewert zu. | Die Zuordnung, ob eine Ampelkombination sicher (`1`) oder unsicher (`0`) ist |
| Sicherheitsregel | Sprachliche Beschreibung, welche Ampelstellungen sicher sind. | Zwei kreuzende Spuren dürfen nicht gleichzeitig Grün haben. |
| Aussagenlogische Formel | Formale Darstellung einer Regel mit Variablen und logischen Operatoren. | `¬(A ∧ B)` |
| Wahrheitstabelle | Tabelle mit allen `2^n` Kombinationen von `n` Variablen.| Alle Rot-Grün-Kombinationen einer Situation |
| Normalform | Standardisierte Form einer aussagenlogischen Formel | DNF, KNF, KDNF, KKNF |

* Bewusst Junktor und Operator nicht 

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

Solche Aussagen werden zu aussagenlogischen Formeln verknüpft. Eine Formel beschreibt dann nicht mehr nur eine einzelne Ampel, sondern eine ganze Sicherheitsregel für die Kreuzung.
