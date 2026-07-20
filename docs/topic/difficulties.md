# Lern- und Lehrherausforderungen

Boolesche Logik ist fachlich grundlegend, aber für Lernende oft anspruchsvoll. Schwierigkeiten entstehen besonders dort, wo Alltagssprache, Tabellenlogik und formale Symbole nicht deckungsgleich sind.[^1][^2]

## Warum das Thema wichtig ist

Logisches Denken verbindet Sprache, Erfahrung und Fachwissen. Es unterstützt Problemlösen, Modellieren und Entscheiden. Gerade alltagsnahe Beispiele wie Ampelsteuerungen helfen, abstrakte Logik verständlicher zu machen.[^3]

## Typische Fehlvorstellungen

| Fehlvorstellung | Woran man sie erkennt | Unterrichtlicher Fokus |
| --- | --- | --- |
| Implikation wird als UND gelesen | Lernende deuten "Wenn A, dann B" als "A und B müssen beide gelten" | Wahrheitstabelle der Implikation gezielt prüfen |
| ODER wird exklusiv verstanden | `A ∨ B` gilt für Lernende nur, wenn genau eine Aussage wahr ist | Fall `A = 1`, `B = 1` sichtbar machen |
| Komplexe Operatoren werden vereinfacht | Implikation wird zu AND oder OR umgedeutet | vollständige Wahrheitsbedingungen vergleichen |
| Negierte Variablen werden übersehen | Formeln enthalten nur positive Fälle | jede Tabellenzeile vollständig übersetzen |

## Fehlvorstellung: Implikation als UND

Lernende glauben häufig, dass eine Aussage der Form `A -> B` nur wahr ist, wenn `A` und `B` gleichzeitig wahr sind. Das ist fachlich falsch: Eine Implikation ist nur dann falsch, wenn `A` wahr und `B` falsch ist.

| A | B | A -> B |
| --- | --- | --- |
| 1 | 1 | 1 |
| 1 | 0 | 0 |
| 0 | 1 | 1 |
| 0 | 0 | 1 |

Hilfreicher Merksatz: Eine Implikation beschreibt keine Kausalität, sondern eine logische Bedingung.

## Fehlvorstellung: ODER als exklusives Oder

Im Alltag meint "oder" oft: entweder das eine oder das andere. In der Aussagenlogik ist `A ∨ B` aber inklusiv. Die Aussage ist wahr, wenn mindestens eine Bedingung erfüllt ist, also auch dann, wenn beide wahr sind.

| A | B | A ∨ B |
| --- | --- | --- |
| 1 | 1 | 1 |
| 1 | 0 | 1 |
| 0 | 1 | 1 |
| 0 | 0 | 0 |

Hilfreicher Merksatz: OR bedeutet mindestens eine Bedingung, nicht genau eine Bedingung.

## Fehlvorstellung: Unvollständige Fälle

Beim Bilden von Normalformen werden negierte Variablen oft vergessen. Lernende notieren dann nur, was sichtbar "vorhanden" ist, und übersehen Fälle wie `¬A` oder Kombinationen, in denen mehrere Variablen falsch sind.

| Problem | Gegenmassnahme |
| --- | --- |
| Variable fehlt im Baustein | jede Zeile Spalte für Spalte übersetzen |
| nur positive Variablen werden notiert | bewusst nach roten Ampeln bzw. `0`-Werten fragen |
| Formel wird aus Intuition gebildet | zuerst Tabelle vollständig machen, danach Formel ableiten |

## Praktische Diagnosefragen

- Was bedeutet `0` in dieser Spalte?
- Darf bei `A ∨ B` auch beides wahr sein?
- Welche Tabellenzeile macht die Implikation falsch?
- Kommt jede Variable in diesem Normalform-Baustein genau einmal vor?
- Welche Verkehrssituation passt zu dieser Formel?

[^1]: Fehér, Z., Jaruska, L., Szarka, K., & Tóthová Tarová, E. (2023). Students' propositional logic thinking in higher education from the perspective of disciplines. Frontiers in Education, 8. https://doi.org/10.3389/feduc.2023.1247653
[^2]: Herman, G. L., Loui, M. C., Kaczmarczyk, L., & Zilles, C. (2012). Describing the What and Why of Students' Difficulties in Boolean Logic. ACM Transactions on Computing Education, 12(1), 1-28. https://doi.org/10.1145/2133797.2133800
[^3]: Milbou, L., Deprez, J., & Laenens, E. A study on the Reintroduction of Logic in Secondary Schools.
