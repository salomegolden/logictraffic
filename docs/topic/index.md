# Zur Sache

Diese Seite gibt einen kompakten Überblick über die fachlichen Grundlagen von LogicTraffic. Für ausführlichere Erklärungen sind die Vertiefungsseiten verlinkt.

## Orientierung

| Bereich | Wofür ist er hilfreich? | Vertiefung |
| --- | --- | --- |
| Aussagelogik | Grundbegriffe verstehen: Aussage, Wahrheitswert, Variable, Junktor | diese Seite |
| Darstellungswechsel | Verstehen, wie Verkehrssituation, Sprache, Tabelle und Formel zusammenhängen | [Darstellungswechsel](darstellungswechsel.md) |
| Wahrheitstabellen | Systematisch alle Ampelzustände erfassen und Sicherheit prüfen | [Wahrheitstabellen](wahrheitstabellen.md) |
| Normalformen | Aus Wahrheitstabellen Formeln erzeugen und vergleichen | [Normalformen](normalformen.md) |
| Lernhürden | Typische Fehlvorstellungen erkennen und im Unterricht bearbeiten | [Lern- und Lehrherausforderungen](difficulties.md) |

## Grundidee von LogicTraffic

LogicTraffic simuliert eine Strassenkreuzung mit Ampeln für verschiedene Fahrspuren. Ziel ist es, eine logische Formel zu finden, die sicherstellt, dass kreuzende Spuren nie gleichzeitig grün haben. Dadurch wird sichtbar, wie Aussagenlogik in einem alltagsnahen Steuerungsproblem angewendet wird.[^11][^12]

In LogicTraffic wird jede Fahrspur durch eine Variable beschrieben. Eine Ampel ist entweder rot (`0`) oder grün (`1`). Die Wahrheitstabelle listet alle möglichen Kombinationen dieser Ampelzustände auf. Die Formel beschreibt anschliessend, welche Kombinationen sicher sind.

## Zentrale Begriffe

| Begriff | Kurze Erklärung | Beispiel in LogicTraffic |
| --- | --- | --- |
| Aussage | Ein Sachverhalt, der eindeutig wahr oder falsch ist.[^1][^7] | "Ampel A ist grün." |
| Wahrheitswert | Wert einer Aussage: wahr/`1` oder falsch/`0` | `A = 1` bedeutet: Spur A ist befahrbar. |
| Variable | Platzhalter für eine Aussage oder einen Zustand | `A`, `B`, `C` stehen für Fahrspuren bzw. Ampeln. |
| Junktor | Logisches Verknüpfungszeichen, das Aussagen verbindet.[^7] | `A ∧ B`, `A ∨ B`, `¬A` |
| Operator | Rechenzeichen der booleschen Logik; erzeugt aus Wahrheitswerten neue Wahrheitswerte.[^3][^9] | UND, ODER, NICHT |
| Boolesche Funktion | Ordnet jeder Kombination von Eingabewerten genau einen Ausgabewert zu.[^7] | Eine Sicherheitsregel für eine Kreuzung |
| Wahrheitstabelle | Tabelle mit allen `2^n` Kombinationen von `n` Variablen.[^2][^8] | Alle Rot-Grün-Kombinationen einer Situation |
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

Solche Aussagen werden zu Formeln verknüpft. Eine Formel beschreibt dann nicht mehr nur eine einzelne Ampel, sondern eine ganze Sicherheitsregel für die Kreuzung.[^10][^11]

## Operatoren

In dieser Unterrichtseinheit stehen drei grundlegende Operatoren im Zentrum. Die Implikation kann als zusätzlicher Operator eingeführt werden, ist aber didaktisch anspruchsvoller.

| Operator | Zeichen | Bedeutung | Wann ist der Ausdruck wahr? |
| --- | --- | --- | --- |
| Negation | `¬A` | nicht A | wenn `A` falsch ist |
| Konjunktion | `A ∧ B` | A und B | wenn beide Aussagen wahr sind |
| Disjunktion | `A ∨ B` | A oder B | wenn mindestens eine Aussage wahr ist |
| Implikation | `A → B` | wenn A, dann B | immer ausser bei `A = 1` und `B = 0` |

### Wahrheitstabellen der Operatoren

#### Negation

| `A` | `¬A` |
| --- | --- |
| 1 | 0 |
| 0 | 1 |

#### Konjunktion

| `A` | `B` | `A ∧ B` |
| --- | --- | --- |
| 1 | 1 | 1 |
| 1 | 0 | 0 |
| 0 | 1 | 0 |
| 0 | 0 | 0 |

#### Disjunktion

| `A` | `B` | `A ∨ B` |
| --- | --- | --- |
| 1 | 1 | 1 |
| 1 | 0 | 1 |
| 0 | 1 | 1 |
| 0 | 0 | 0 |

#### Implikation

Die Implikation entfernt sich am stärksten von der Alltagssprache. Formulierungen wie "Aus A folgt B" können missverständlich sein, weil sie schnell kausal verstanden werden. Präziser ist: `A` ist hinreichend für `B`, oder `B` ist notwendig für `A`.[^13]

| `A` | `B` | `A → B` |
| --- | --- | --- |
| 1 | 1 | 1 |
| 1 | 0 | 0 |
| 0 | 1 | 1 |
| 0 | 0 | 1 |

Gerade bei Operatoren treten häufig Fehlvorstellungen auf, besonders beim inklusiven Oder und bei der Implikation. Eine Übersicht dazu findet sich unter [Lern- und Lehrherausforderungen](difficulties.md).[^6]

## Darstellungen in LogicTraffic

LogicTraffic verbindet mehrere Darstellungsformen. Das ist didaktisch wichtig, weil Lernende nicht nur Formeln sehen, sondern zwischen Situation, Sprache, Tabelle und Formel wechseln müssen.

| Darstellung | In LogicTraffic | Lernfunktion |
| --- | --- | --- |
| ikonisch | Kreuzung, Spuren, Ampeln | Situation anschaulich erfassen |
| verbal | Beschreibung sicherer und unsicherer Zustände | Regeln in Alltagssprache formulieren |
| tabellarisch | Wahrheitstabelle | alle Fälle systematisch prüfen |
| symbolisch | boolesche Formel | Sicherheitsregel formal ausdrücken |

Der Wechsel zwischen diesen Darstellungen ist ein zentraler Lernschritt. Ausführlicher wird er auf der Seite [Darstellungswechsel](darstellungswechsel.md) erklärt.

## Weiterarbeiten

| Wenn Sie ... | Dann passt diese Seite |
| --- | --- |
| Wahrheitstabellen fachlich erklären oder im Unterricht einsetzen möchten | [Wahrheitstabellen](wahrheitstabellen.md) |
| Formeln aus Tabellen herleiten möchten | [Normalformen](normalformen.md) |
| typische Denkfehler vorbereiten möchten | [Lern- und Lehrherausforderungen](difficulties.md) |
| konkrete Aufgaben für den Unterricht suchen | [Unterrichtsplanung](../unterricht/index.md) |

[^1]: Hoffmann, A., Marx, B., & Vogt, W. (2005). _Mathematik für Ingenieure 1: Lineare Algebra, Analysis - Theorie und Numerik_. Pearson Deutschland.
[^2]: Junker, M. (2025). _Logik für die Informatik: Eine Einführung in die Aussagenlogik, Prädikatenlogik und Berechenbarkeitstheorie_. Springer Berlin Heidelberg. [https://doi.org/10.1007/978-3-662-70825-5](https://doi.org/10.1007/978-3-662-70825-5)
[^3]: Kreuzer, M., & Kühling, S. (2014). _Logik für Informatiker_. Pearson Deutschland. [https://elibrary.pearson.de/book/99.150005/9783863267391](https://elibrary.pearson.de/book/99.150005/9783863267391)
[^6]: Herman, G. L., Loui, M. C., Kaczmarczyk, L., & Zilles, C. (2012). Describing the What and Why of Students' Difficulties in Boolean Logic. ACM Transactions on Computing Education, 12(1), 1-28. https://doi.org/10.1145/2133797.2133800
[^7]: Boolesche Funktionen und ihre Normalformen. (2021, Juni 22). https://lehrerfortbildung-bw.de/u_matnatech/imp/gym/bp2016/fb2/m02_aug/1_hintergrund/4_grund/06_funktionen/
[^8]: Wahrheitstafeln - Theoretisches Material. Mathematik, 6. Schulstufe. (o. J.). Abgerufen 17. März 2026, von https://www.yaclass.at/p/mathematik/6-schulstufe/mengen-und-mengenoperationen-17080/aussagen-und-mengen-17463/re-519f4254-a9a1-457b-aa7e-38b6386d9b1c
[^9]: Hintergrund. (2021, Juni 22). https://lehrerfortbildung-bw.de/u_matnatech/imp/gym/bp2016/fb2/m02_aug/1_hintergrund/4_grund/
[^10]: Leitprogramm LogicTraffic [BZZ - Modulwiki]. (o. J.). Abgerufen 17. März 2026, von https://wiki.bzz.ch/modul/mathe/ma1/thema/lu04logik/aufgaben/leitprogramm/start
[^11]: Arnold, R., & Hartmann, W. (2007). LogicTraffic - Logik in der Allgemeinbildung. Informatik-Spektrum, 30(1), 19-26. https://doi.org/10.1007/s00287-006-0123-7
[^12]: Arnold, R., Amstalden, B., & Bader, J. (2022). Enhancing the Role of Computational Thinking in Primary and Secondary Education in Switzerland. Proceedings of the 17th Workshop in Primary and Secondary Computing Education, 1-2. https://doi.org/10.1145/3556787.3556874
[^13]: https://de.wikiversity.org/wiki/Aussagenlogik/Elementare_Einf%C3%BChrung/Textabschnitt
