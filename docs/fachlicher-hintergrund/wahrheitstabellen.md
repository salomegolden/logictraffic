# Wahrheitstabellen

Wahrheitstabellen sind ein zentrales Werkzeug in LogicTraffic. Sie halten systematisch alle möglichen Zustände einer Verkehrskreuzung fest und zeigen, welche Kombinationen sicher sind.[^1]

## Definition

Eine Wahrheitstabelle listet alle Kombinationen der Wahrheitswerte aller Variablen auf. Bei `n` Variablen enthält sie `2^n` Zeilen.[^2]

| Anzahl Variablen | Anzahl Tabellenzeilen |
| --- | --- |
| 1 | 2 |
| 2 | 4 |
| 3 | 8 |
| 4 | 16 |

## Bedeutung in LogicTraffic

| Tabellenteil | Bedeutung |
| --- | --- |
| Variablenspalten | Ampelzustände der Spuren, z.B. `A`, `B`, `C` |
| Wert `1` | Spur hat grün bzw. ist befahrbar |
| Wert `0` | Spur hat rot bzw. ist gesperrt |
| Spalte "sicher" | Bewertung der gesamten Ampelkombination |

### Wahrheitstabellen der Operatoren

#### Negation

Die Negation kehrt den Wahrheitswert einer Aussage um. Wenn `A` wahr ist, ist `¬A` falsch; wenn `A` falsch ist, ist `¬A` wahr.

| `A` | `¬A` |
| --- | --- |
| 1 | 0 |
| 0 | 1 |

#### Konjunktion

Die Konjunktion entspricht dem logischen UND. `A ∧ B` ist nur dann wahr, wenn beide Teilaussagen wahr sind.

| `A` | `B` | `A ∧ B` |
| --- | --- | --- |
| 1 | 1 | 1 |
| 1 | 0 | 0 |
| 0 | 1 | 0 |
| 0 | 0 | 0 |

#### Disjunktion

Die Disjunktion entspricht dem inklusiven ODER. `A ∨ B` ist wahr, sobald mindestens eine der beiden Aussagen wahr ist; auch beide dürfen wahr sein.

| `A` | `B` | `A ∨ B` |
| --- | --- | --- |
| 1 | 1 | 1 |
| 1 | 0 | 1 |
| 0 | 1 | 1 |
| 0 | 0 | 0 |

#### Implikation

Die Implikation entfernt sich am stärksten von der Alltagssprache. Formulierungen wie "Aus A folgt B" können missverständlich sein, weil sie schnell kausal verstanden werden. Präziser ist: `A` ist hinreichend für `B`, oder `B` ist notwendig für `A`.[^13]

`A → B` ist nur dann falsch, wenn die Voraussetzung `A` wahr ist, die Schlussfolgerung `B` aber falsch ist.

| `A` | `B` | `A → B` |
| --- | --- | --- |
| 1 | 1 | 1 |
| 1 | 0 | 0 |
| 0 | 1 | 1 |
| 0 | 0 | 1 |


## Sicher oder unsicher

| Wert in der Spalte "sicher" | Bedeutung |
| --- | --- |
| `1` | Diese Ampelkombination lässt keine Kollision zu. |
| `0` | Diese Ampelkombination kann zu einer Kollision führen. |

Die Werte können in LogicTraffic verändert werden. Dadurch passt sich die automatisch erzeugte Formel an. So wird sichtbar, dass die Formel genau die markierten sicheren Zeilen beschreibt.

## Didaktischer Nutzen

| Funktion | Nutzen im Unterricht |
| --- | --- |
| Visualisierung | Lernende sehen Ampelzustände und Sicherheitsstatus nebeneinander. |
| Systematisierung | Keine Kombination wird vergessen. |
| Interaktion | Klicks auf Ampeln oder Tabellenwerte verändern die Situation. |
| Formelbrücke | Aus sicheren Zeilen kann eine boolesche Formel entstehen. |


[^1]: Arnold, R., & Hartmann, W. (2007). LogicTraffic - Logik in der Allgemeinbildung. Informatik-Spektrum, 30(1), 19-26. https://doi.org/10.1007/s00287-006-0123-7
[^2]: Junker, M. (2025). _Logik für die Informatik: Eine Einführung in die Aussagenlogik, Prädikatenlogik und Berechenbarkeitstheorie_. Springer Berlin Heidelberg. https://doi.org/10.1007/978-3-662-70825-5