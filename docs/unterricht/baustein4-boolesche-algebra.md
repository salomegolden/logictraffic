# Baustein 4 – Logische Formeln

In diesem Baustein lernen die Lernenden, Sicherheitsregeln einer Verkehrskreuzung mit aussagenlogischen Formeln zu beschreiben.

Ausgangspunkt ist die Erkenntnis aus Baustein 3: Wahrheitstabellen können alle möglichen Zustände vollständig darstellen, werden mit zunehmender Anzahl von Variablen jedoch schnell sehr umfangreich. Die Lernenden untersuchen deshalb, wie dieselbe Sicherheitsregel mit wenigen logischen Operatoren kompakter dargestellt werden kann.

Dabei wechseln sie zwischen Alltagssprache, Verkehrssituation, Wahrheitstabelle und Formel. In einer optionalen Vertiefung vergleichen sie unterschiedliche, aber logisch äquivalente Formeln und lernen DNF und KNF als strukturierte Darstellungsformen kennen.

!!! abstract "Auf einen Blick"

    **:stopwatch: Dauer:**  
    ca. 60 Minuten für den Basisteil  
    zusätzlich ca. 30–45 Minuten für die Vertiefung zu Äquivalenzen, DNF und KNF

    **:busts_in_silhouette: Sozialform:**  
    Plenum, Partnerarbeit und kurze Einzelphasen

    **:computer: Computer:**  
    Ein Computer oder Tablet mit LogicTraffic pro Zweiergruppe

    **:brain: Vorwissen:**  
    - [Baustein 3 – Wahrheitstabellen](baustein3-wahrheitstabellen.md) wurde idealerweise abgeschlossen.
    - Die Lernenden kennen Variablen als Bezeichnungen für Fahrspuren.
    - `0 = Rot` und `1 = Grün` sind bekannt.
    - Die Bedeutung der Spalte `sicher` ist bekannt.
    - Die Lernenden können einfache Wahrheitstabellen lesen und erstellen.
    - Die Regel $2^n$ und das Skalierungsproblem von Wahrheitstabellen sind bekannt.

    **:package: Material:**  
    LogicTraffic, Computer oder Tablets, Beamer oder Präsentationsbildschirm, Arbeitsblatt bzw. Heft oder Begleitportfolio

!!! note "Downloads zu Baustein 4"

    - [:memo: Arbeitsblatt zu logischen Formeln](LINK_ERGÄNZEN)
    - [:material-image-outline: Übersicht zu den logischen Operatoren](LINK_ERGÄNZEN)
    - [:material-image-outline: Merkblatt zu DNF und KNF](LINK_ERGÄNZEN)

## Lernziele

### Basisteil

Die Lernenden können …

- einfache Verkehrs- und Sicherheitsregeln in aussagenlogische Formeln übersetzen;
- die Operatoren `¬`, `∧`, `∨` und `→` in ihrem Verkehrskontext erklären;
- logische Formeln in LogicTraffic syntaktisch korrekt eingeben;
- eine Formel anhand der zugehörigen Wahrheitstabelle überprüfen;
- erklären, dass unterschiedliche Formeln dieselbe Sicherheitsregel beschreiben können;
- zwischen einer konkreten Verkehrssituation, einer sprachlichen Regel, einer Wahrheitstabelle und einer Formel wechseln;
- den Vorteil kompakter Formeln gegenüber umfangreichen Wahrheitstabellen beschreiben.

### Optionale Vertiefung

Die Lernenden können zusätzlich …

- logisch äquivalente Formeln anhand ihrer Wahrheitstabellen erkennen;
- einfache Anwendungen der De-Morgan-Regeln nachvollziehen;
- den Aufbau einer disjunktiven Normalform (DNF) und einer konjunktiven Normalform (KNF) beschreiben;
- DNF und KNF in einfachen Beispielen erkennen;
- erklären, wie eine kanonische DNF bzw. KNF direkt aus einer Wahrheitstabelle erzeugt werden kann;
- kanonische und vereinfachte Formeln hinsichtlich Länge und Verständlichkeit vergleichen.

## Vorbereitung

- LogicTraffic auf den Geräten öffnen und die Funktionsfähigkeit des Formeleditors prüfen.
- Für die Einführung eine einfache Situation mit zwei Fahrspuren vorbereiten, beispielsweise Situation 2.
- Für die selbstständige Erarbeitung Situation 3 bereitstellen.
- Falls die Vertiefung durchgeführt wird, die Auswahlmöglichkeiten für Normalformen im Formeleditor vorab prüfen.
- Die 5-Spuren-Kreuzung aus Baustein 3 für den abschliessenden Transfer bereithalten.
- Arbeitsblatt bzw. Begleitportfolio bereitstellen.

??? tip "Abgrenzung zu Baustein 3"

    In Baustein 3 stand die Frage im Zentrum:

    > Wie können wir **alle möglichen Zustände vollständig** darstellen?

    Baustein 4 verfolgt nun eine andere Frage:

    > Wie können wir **dieselbe Sicherheitsregel möglichst kompakt und eindeutig** beschreiben?

    Die Wahrheitstabelle verschwindet dabei nicht. Sie dient weiterhin zur Überprüfung, ob zwei Darstellungen tatsächlich dieselbe logische Funktion beschreiben.

## Fachlicher Hintergrund

### Logische Operatoren

In LogicTraffic werden Aussagen über Fahrspuren mit logischen Operatoren miteinander verbunden.

| Alltagssprache | Symbol | Fachbegriff | Beispiel |
| --- | :---: | --- | --- |
| NICHT | `¬` | Negation | `¬A` |
| UND | `∧` | Konjunktion | `A ∧ B` |
| ODER | `∨` | Disjunktion | `A ∨ B` |
| WENN … DANN | `→` | Implikation | `A → ¬B` |

Im Verkehrskontext können diese Ausdrücke beispielsweise so gelesen werden:

- `¬A`: Spur `A` hat nicht Grün, also Rot.
- `A ∧ B`: Spur `A` und Spur `B` haben gleichzeitig Grün.
- `¬A ∨ ¬B`: Mindestens eine der beiden Spuren hat Rot.
- `A → ¬B`: Wenn Spur `A` Grün hat, muss Spur `B` Rot haben.

!!! info "Von der Alltagssprache zur Formel"

    Eine Sicherheitsregel kann schrittweise formalisiert werden.

    **Alltagssprache:**

    > Wenn Spur A grün ist, muss Spur B rot sein.

    **Logische Bausteine:**

    - Spur A ist grün: `A`
    - Spur B ist rot: `¬B`
    - Wenn … dann …: `→`

    **Formel:**

    `A → ¬B`

!!! warning "Die Implikation ist anspruchsvoller"

    Der Ausdruck `A → ¬B` wird im Alltag leicht anders verstanden als in der formalen Logik.

    Für die erste Einführung kann deshalb zunächst mit einem direkten Kollisionsverbot gearbeitet werden:

    `¬(A ∧ B)`

    Bedeutung:

    > A und B dürfen nicht gleichzeitig Grün haben.

    Die Implikation kann anschliessend als alternative Form derselben Sicherheitsidee eingeführt werden.

## Unterrichtsablauf – Überblick

| Phase | Inhalt | Sozialform / Medien | Richtwert |
| --- | --- | --- | --- |
| **1. Problemstellung** | Skalierungsproblem aus Baustein 3 aufgreifen und nach einer kurzen Sicherheitsregel suchen | Plenum, LogicTraffic / Beamer | ca. 5–10 Min. |
| **2. Erarbeitung** | Logische Operatoren aus Verkehrsregeln entwickeln und erste Formeln bilden | Plenum, LogicTraffic | ca. 15 Min. |
| **3. Modellierung** | Sicherheitsregeln für Situation 3 selbstständig formulieren und prüfen | Partnerarbeit, LogicTraffic | ca. 20 Min. |
| **4. Formeln vergleichen** | Verschiedene korrekte Formeln vergleichen und Äquivalenz vorbereiten | Plenum / Partnerarbeit | ca. 10 Min. |
| **5. Sicherung** | Operatoren, Darstellungswechsel und zentrale Erkenntnisse festhalten | Plenum / Einzelarbeit | ca. 10 Min. |

## Durchführung

### Phase 1 – Von der Tabelle zur Regel

**Ziel der Phase:**  
Die Lernenden reaktivieren das Skalierungsproblem von Wahrheitstabellen und entwickeln das Bedürfnis nach einer kompakteren Darstellung.

Die Lehrperson greift die Ergebnisse aus Baustein 3 auf.

Bei fünf Variablen entstehen bereits:

$$
2^5 = 32
$$

mögliche Belegungen.

Bei zehn Variablen wären es:

$$
2^{10} = 1024
$$

Belegungen.

!!! question "Einstiegsfrage"

    Wahrheitstabellen können vollständig beschreiben, welche Ampelstellungen sicher sind.

    **Müssen wir dafür aber wirklich jede mögliche Kombination einzeln aufschreiben?**

    Oder können wir die Sicherheitsregel mit wenigen Zeichen ausdrücken?

Die Lehrperson zeigt anschliessend eine einfache Kreuzung mit zwei Fahrspuren.

Die Lernenden formulieren zunächst in Alltagssprache, was gelten muss.

??? example "Mögliche Aussagen:"

    > A und B dürfen nicht gleichzeitig Grün haben.
    > Wenn A Grün hat, muss B Rot haben.
    > Mindestens eine der beiden Ampeln muss Rot zeigen.



Die verschiedenen Formulierungen werden zunächst gesammelt, ohne sie sofort formal zu bewerten.

??? note "Didaktische Absicht"

    Die Formel entsteht aus einer bereits verstandenen Verkehrsregel.

    Dadurch wird die symbolische Darstellung nicht als isolierter Zeichenvorrat eingeführt, sondern als weitere Repräsentation einer bekannten Situation.

### Phase 2 – Logische Bausteine kennenlernen

**Ziel der Phase:**  
Die Lernenden ordnen sprachlichen Verknüpfungen logische Operatoren zu und bilden erste einfache Formeln.

Die Lehrperson führt die Operatoren schrittweise ein.

!!! quote "Lernauftrag 1 – Von der Sprache zur Formel"

    Ergänzt die fehlenden Formeln.

    | Verkehrssituation / Regel | Logischer Ausdruck |
    | --- | --- |
    | Spur `B` muss anhalten. | `¬B` |
    | Spur `A` und Spur `B` haben gleichzeitig Grün. | |
    | Mindestens eine der beiden Spuren muss Rot haben. | |
    | Wenn `A` Grün hat, muss `B` Rot haben. | |

??? success "Mögliche Lösung"

    | Verkehrssituation / Regel | Logischer Ausdruck |
    | --- | --- |
    | Spur `B` muss anhalten. | `¬B` |
    | Spur `A` und Spur `B` haben gleichzeitig Grün. | `A ∧ B` |
    | Mindestens eine der beiden Spuren muss Rot haben. | `¬A ∨ ¬B` |
    | Wenn `A` Grün hat, muss `B` Rot haben. | `A → ¬B` |

Nun wird eine der Formeln in LogicTraffic eingegeben.

Besonders anschaulich ist zunächst:

`¬(A ∧ B)`

Die Formel bedeutet:

> Es darf nicht gleichzeitig gelten, dass `A` und `B` Grün haben.

Die Lernenden laden die Formel in die Wahrheitstabelle und beobachten, welche Belegungen als sicher markiert werden.

!!! quote "Beobachtungsauftrag"

    Vergleicht die Formel mit der Wahrheitstabelle.

    - Welche Tabellenzeile wird durch die Formel ausgeschlossen?
    - Welche Kombinationen bleiben erlaubt?
    - Passt das zur Verkehrssituation?

!!! tip "Nicht das Softwarefeedback erklären lassen"

    LogicTraffic kann zur Überprüfung verwendet werden.

    Die fachliche Begründung sollte jedoch zuerst von den Lernenden kommen.

    Nicht:

    > Die Formel stimmt, weil LogicTraffic `Optimal` anzeigt.

    Sondern:

    > Die Formel stimmt, weil genau die Kombination ausgeschlossen wird, bei der sich die beiden grünen Fahrspuren kreuzen.

??? warning "Klammern"

    Klammern helfen dabei, zusammengesetzte Formeln eindeutig zu lesen.

    Für den Einstieg ist es sinnvoll, lieber eine Klammer zu viel als eine zu wenig zu setzen.

    Beispiel:

    `¬(A ∧ B)`

    oder bei mehreren Regeln:

    `(A → ¬C) ∧ (B → ¬C)`

### Phase 3 – Sicherheitsregeln selbst formulieren

**Ziel der Phase:**  
Die Lernenden entwickeln für eine komplexere Verkehrssituation selbstständig aussagenlogische Formeln.

Die Lernenden öffnen Situation 3.

Die Fahrspuren `A` und `B` verlaufen parallel, während `C` beide kreuzt.

!!! quote "Lernauftrag 2 – Situation 3 steuern"

    Untersucht die Kreuzung genau.

    1. Welche Fahrspuren können miteinander kollidieren?
    2. Formuliert zunächst in Alltagssprache mindestens zwei Sicherheitsregeln.
    3. Übersetzt eure Regeln anschliessend in logische Formeln.
    4. Gebt die Formel in LogicTraffic ein.
    5. Vergleicht die erzeugte Spalte `sicher` mit eurer Erwartung.
    6. Verbessert eure Formel, falls nötig.

??? tip "Denkhilfe"

    Statt sofort eine grosse Formel zu suchen, können zunächst einzelne Konflikte beschrieben werden.

    Beispielsweise:

    > A und C dürfen nicht gleichzeitig Grün haben.

    Daraus wird:

    `¬(A ∧ C)`

    Für den zweiten Konflikt:

    `¬(B ∧ C)`

    Beide Regeln müssen gleichzeitig gelten. Deshalb können sie mit `∧` verbunden werden.

??? success "Mögliche korrekte Formeln"

    Für Situation 3 sind beispielsweise folgende Darstellungen möglich:

    **Kollisionsverbote:**

    `¬(A ∧ C) ∧ ¬(B ∧ C)`

    **Mit Implikationen:**

    `(A → ¬C) ∧ (B → ¬C)`

    **Zusammengefasste Implikation:**

    `C → (¬A ∧ ¬B)`

    **Klauselform:**

    `(¬A ∨ ¬C) ∧ (¬B ∨ ¬C)`

    Die Formeln sehen unterschiedlich aus, erzeugen aber dieselbe Sicherheitsregel.

!!! warning "Safe ist nicht automatisch eine optimale Steuerung"

    Eine Formel kann alle Kollisionen verhindern und trotzdem unnötig viele sichere Zustände verbieten.

    Beispielsweise wäre eine Steuerung, bei der alle Ampeln immer Rot bleiben, zwar sicher, aber wenig sinnvoll.

    Das Feedback von LogicTraffic kann deshalb zur Reflexion genutzt werden:

    - Verhindert unsere Formel alle Kollisionen?
    - Erlaubt sie gleichzeitig die sicheren Kombinationen?

    Der Status selbst ersetzt jedoch nicht die fachliche Begründung.

### Phase 4 – Unterschiedliche Formeln vergleichen

**Ziel der Phase:**  
Die Lernenden erkennen, dass unterschiedlich aussehende Formeln dieselbe logische Funktion beschreiben können.

Die Lehrperson sammelt verschiedene Lösungen der Gruppen.

Besonders geeignet sind:

`¬(A ∧ C)`

und

`¬A ∨ ¬C`

Die Lernenden geben beide Formeln nacheinander in LogicTraffic ein und laden sie in die Wahrheitstabelle.

!!! quote "Lernauftrag 3 – Zwei Formeln, eine Bedeutung?"

    Vergleicht:

    `¬(A ∧ C)`

    und

    `¬A ∨ ¬C`

    1. Erzeugen beide Formeln dieselben Werte in der Wahrheitstabelle?
    2. Beschreibt beide Formeln in Alltagssprache.
    3. Warum passen beide Beschreibungen zur gleichen Verkehrssituation?

Mögliche sprachliche Übersetzungen:

> `¬(A ∧ C)`: A und C dürfen nicht beide gleichzeitig Grün haben.

> `¬A ∨ ¬C`: Mindestens eine der beiden Spuren muss Rot haben.

Wenn beide Formeln für jede mögliche Belegung denselben Wahrheitswert ergeben, sind sie **logisch äquivalent**.

Man schreibt:

$$
\neg(A \land C) \equiv \neg A \lor \neg C
$$

??? info "De Morgan"

    Das beobachtete Muster ist ein Beispiel für ein De-Morgan-Gesetz:

    $$
    \neg(A \land B) \equiv \neg A \lor \neg B
    $$

    Das zweite De-Morgan-Gesetz lautet:

    $$
    \neg(A \lor B) \equiv \neg A \land \neg B
    $$

    Im Basisteil muss nicht zwingend mit beiden Regeln formal gearbeitet werden.

### Phase 5 – Ergebnisse sichern

**Ziel der Phase:**  
Die Lernenden sichern die zentralen logischen Operatoren und den Zusammenhang zwischen den verschiedenen Darstellungen.

??? example "Mögliche Ergebnissicherung"

    **Logische Operatoren**

    | Symbol | Bedeutung | Beispiel |
    | :---: | --- | --- |
    | `¬` | NICHT | `¬A` |
    | `∧` | UND | `A ∧ B` |
    | `∨` | ODER | `A ∨ B` |
    | `→` | WENN … DANN | `A → ¬B` |

    **Eine Sicherheitsregel kann unterschiedlich dargestellt werden:**

    **Verkehrssituation**

    → A und C dürfen nicht gleichzeitig Grün haben.

    **Alltagssprache**

    → Mindestens eine der beiden Spuren muss Rot haben.

    **Formel**

    → `¬(A ∧ C)`

    oder

    → `¬A ∨ ¬C`

    **Wahrheitstabelle**

    → Beide Formeln erzeugen dieselben Wahrheitswerte.

!!! success "Ich kann …"

    - die Operatoren `¬`, `∧`, `∨` und `→` erklären;
    - eine einfache Verkehrsregel in eine Formel übersetzen;
    - eine Formel wieder in Alltagssprache übersetzen;
    - mit der Wahrheitstabelle überprüfen, was eine Formel bewirkt;
    - erklären, warum zwei unterschiedlich aussehende Formeln logisch gleichwertig sein können.

## Optionale Vertiefung – DNF und KNF

Die folgende Vertiefung kann direkt an den Basisteil angeschlossen oder in einer zusätzlichen Lektion durchgeführt werden.

### Vertiefungsziele

Die Lernenden …

- untersuchen verschiedene strukturierte Darstellungen derselben logischen Funktion;
- erkennen den Aufbau von DNF und KNF;
- vergleichen lange und kurze äquivalente Formeln;
- nutzen die Wahrheitstabelle weiterhin als Referenz für semantische Äquivalenz.

### Vertiefung 1 – DNF und KNF entdecken

Eine Formel in **disjunktiver Normalform (DNF)** besteht aus UND-Termen, die mit ODER verbunden werden.

Beispiel:

`(A ∧ ¬B) ∨ (¬A ∧ C)`

Struktur:

> UND-Term **ODER** UND-Term **ODER** …

Eine Formel in **konjunktiver Normalform (KNF)** besteht aus ODER-Klauseln, die mit UND verbunden werden.

Beispiel:

`(¬A ∨ ¬C) ∧ (¬B ∨ ¬C)`

Struktur:

> ODER-Klausel **UND** ODER-Klausel **UND** …

!!! quote "Lernauftrag 4 – Welche Struktur erkennt ihr?"

    Betrachtet:

    `¬(A ∧ C) ∧ ¬(B ∧ C)`

    und

    `(¬A ∨ ¬C) ∧ (¬B ∨ ¬C)`

    1. Prüft mit LogicTraffic, ob beide Formeln dieselbe Wahrheitstabelle erzeugen.
    2. Welche der beiden Formeln besitzt bereits die typische Struktur einer KNF?
    3. Wie ist diese Formel aufgebaut?
    4. Welche Darstellung findet ihr leichter zu lesen? Begründet.

Die Lernenden erkennen:

`(¬A ∨ ¬C) ∧ (¬B ∨ ¬C)`

ist eine KNF.

??? info "DNF und KNF als Form – nicht als neue Funktion"

    DNF und KNF beschreiben keine grundsätzlich anderen logischen Funktionen.

    Sie sind bestimmte **Strukturen**, in denen eine Formel geschrieben werden kann.

    Dieselbe Funktion kann deshalb häufig

    - als freie logische Formel,
    - als DNF,
    - als KNF
    - oder in einer anderen äquivalenten Form

    dargestellt werden.

### Vertiefung 2 – Von der Wahrheitstabelle zur Formel

!!! important "Kanonische Formen als möglicher Zwischenschritt"

    Eine Wahrheitstabelle lässt sich immer nach einem festen Verfahren in eine Formel übertragen.

    Dafür können die **kanonische disjunktive Normalform (KDNF)** und die **kanonische konjunktive Normalform (KKNF)** verwendet werden.

    **KDNF**

    Für jede Zeile mit `sicher = 1` wird ein UND-Term gebildet, der die Belegung dieser Zeile vollständig beschreibt.

    Diese Terme werden anschliessend mit ODER (`∨`) verbunden.

    **KKNF**

    Für jede Zeile mit `sicher = 0` wird eine ODER-Klausel gebildet, die genau diese Belegung ausschliesst.

    Diese Klauseln werden anschliessend mit UND (`∧`) verbunden.

    Der grosse Vorteil:

    > Die Formel muss nicht erraten werden. Sie kann **systematisch direkt aus der Wahrheitstabelle konstruiert werden**.

    Dadurch können die kanonischen Formen für einige Lernende eine hilfreiche **Brücke zwischen Wahrheitstabelle und Formel** darstellen.

    Der Nachteil:

    > Da jede relevante Tabellenzeile einzeln berücksichtigt wird, entstehen häufig sehr lange Formeln.

    Die kanonische Form ist deshalb nicht unbedingt die Form, mit der man am Ende arbeiten möchte. Sie bietet aber einen sicheren Ausgangspunkt, der anschliessend vereinfacht werden kann.

    Für Lernende, die bereits selbstständig eine kompakte Formel aus der Verkehrssituation entwickeln können, ist dieser Zwischenschritt nicht zwingend erforderlich.

    In LogicTraffic können die kanonischen Formen über die entsprechende Auswahl automatisch erzeugt werden. Je nach Bezeichnung der Oberfläche werden sie als `CDNF` bzw. `CCNF` angezeigt.

!!! tip "Differenzierung mit den kanonischen Formen"

    Die kanonischen Formen eignen sich gut für eine natürliche Differenzierung.

    **Möglicher Weg 1**

    Verkehrssituation  
    → eigene kompakte Formel

    **Möglicher Weg 2**

    Wahrheitstabelle  
    → KDNF oder KKNF  
    → Struktur untersuchen  
    → Formel vereinfachen

    Beide Wege führen zur gleichen logischen Funktion.

    Entscheidend ist nicht, welcher Weg benutzt wird, sondern ob die Lernenden erklären können, warum die resultierende Formel dieselbe Wahrheitstabelle erzeugt.

### Vertiefung 3 – KDNF untersuchen

Für Situation 3 wird zunächst die vollständige Wahrheitstabelle betrachtet.

!!! quote "Lernauftrag 5 – Von den Einsen zur Formel"

    Lasst euch in LogicTraffic die kanonische DNF anzeigen.

    Untersucht die Formel.

    1. Wie viele grosse UND-Terme enthält sie?
    2. Wie viele Zeilen besitzen in der Wahrheitstabelle `sicher = 1`?
    3. Wählt einen UND-Term aus.
    4. Findet die Tabellenzeile, die genau diesem Term entspricht.
    5. Warum werden die einzelnen Terme mit `∨` verbunden?

??? info "Grundidee der KDNF"

    Ein vollständiger UND-Term beschreibt genau **eine** Belegung.

    Beispiel:

    `A ∧ ¬B ∧ C`

    bedeutet:

    - `A = 1`
    - `B = 0`
    - `C = 1`

    Werden alle Belegungen mit `sicher = 1` durch ODER miteinander verbunden, entsteht eine Formel, die genau diese sicheren Zustände zulässt.

### Vertiefung 4 – KKNF untersuchen

!!! quote "Lernauftrag 6 – Von den Nullen zur Formel"

    Lasst euch nun die kanonische KNF anzeigen.

    1. Wie viele ODER-Klauseln enthält die Formel?
    2. Wie viele Zeilen besitzen `sicher = 0`?
    3. Wählt eine Klausel aus.
    4. Findet die Tabellenzeile, die dadurch ausgeschlossen wird.
    5. Warum werden die Klauseln mit `∧` verbunden?

??? info "Grundidee der KKNF"

    Während die KDNF die Belegungen mit `sicher = 1` einzeln auflistet, konstruiert die KKNF Bedingungen aus den Belegungen mit `sicher = 0`.

    Beide Verfahren liefern eine Formel, die exakt dieselbe Wahrheitstabelle beschreibt.

### Vertiefung 5 – Lang oder kurz?

Die Lernenden vergleichen nun mehrere Darstellungen derselben Funktion:

- KDNF;
- KKNF;
- eine gewöhnliche DNF oder KNF;
- eine selbst entwickelte kompakte Formel;
- die automatisch vereinfachte Darstellung von LogicTraffic.

!!! quote "Lernauftrag 7 – Welche Formel ist die beste?"

    Vergleicht verschiedene Formeln für dieselbe Kreuzung.

    Beurteilt sie nach folgenden Kriterien:

    - Ist die Formel korrekt?
    - Wie lang ist sie?
    - Kann man ihre Bedeutung noch gut erkennen?
    - Lässt sie sich direkt aus der Wahrheitstabelle erzeugen?
    - Wie leicht lässt sie sich erklären?

    Gibt es überhaupt **eine** beste Darstellung?

Die zentrale Erkenntnis lautet:

> Logisch äquivalente Formeln können sehr unterschiedlich aussehen.

> Welche Darstellung besonders geeignet ist, hängt davon ab, wofür sie verwendet wird.

## Optionaler Transfer – Situation 10

**Ziel:**  
Die Lernenden wenden ihre Kenntnisse auf eine Kreuzung an, deren Wahrheitstabelle bereits $32$ Zeilen besitzt.

!!! quote "Transferauftrag"

    Öffnet Situation 10.

    Die Kreuzung besitzt fünf Variablen:

    `A`, `B`, `C`, `D` und `E`.

    Die vollständige Wahrheitstabelle enthält:

    $$
    2^5 = 32
    $$

    Zeilen.

    1. Analysiert die Konflikte zwischen den Fahrspuren.
    2. Formuliert zunächst einzelne Sicherheitsregeln in Alltagssprache.
    3. Übersetzt sie in logische Formeln.
    4. Verknüpft die Einzelregeln zu einer Gesamtregel.
    5. Prüft eure Formel mit LogicTraffic.
    6. Vergleicht eure Formel anschliessend mit einer automatisch erzeugten bzw. vereinfachten Darstellung.

??? tip "Alternative mit kanonischer Form"

    Falls der direkte Weg zur kompakten Formel schwierig ist:

    1. Ausgangspunkt ist die vollständige Wahrheitstabelle.
    2. Lasst eine KDNF oder KKNF erzeugen.
    3. Prüft, wie die Tabellenzeilen in der Formel wiederzufinden sind.
    4. Vergleicht die lange kanonische Formel anschliessend mit einer vereinfachten Darstellung.

    Die kanonische Form dient hier bewusst als **Zwischenschritt**, nicht als Endprodukt.

## Typische Lernschwierigkeiten

??? warning "Alltagssprache und formale Logik werden gleichgesetzt"

    Besonders `oder` und `wenn … dann …` können in der Alltagssprache anders verwendet werden als in der formalen Aussagenlogik.

    Übersetzen Sie deshalb konsequent in beide Richtungen:

    **Sprache → Formel**

    und

    **Formel → Sprache**.

??? warning "Die Negation wird auf den falschen Ausdruck angewendet"

    Vergleichen Sie beispielsweise:

    `¬A ∧ B`

    mit

    `¬(A ∧ B)`.

    Die Klammer entscheidet darüber, welcher Ausdruck negiert wird.

??? warning "Implikation wird als zeitlicher Ablauf verstanden"

    `A → ¬B` bedeutet nicht:

    > Erst wird A grün und danach B rot.

    Sondern:

    > Für jede zulässige Belegung gilt: Wenn A grün ist, darf B nicht grün sein.

??? warning "Eine richtige Formel wird nur am Status erkannt"

    LogicTraffic liefert hilfreiches Feedback.

    Die Lernenden sollten jedoch erklären können, **welche Belegungen ihre Formel erlaubt bzw. verbietet und warum**.

??? warning "Lange Formeln werden automatisch für schlechter gehalten"

    Eine lange Formel kann logisch vollkommen korrekt sein.

    KDNF und KKNF zeigen dies besonders deutlich.

    Die Länge einer Formel und ihre logische Korrektheit sind zwei unterschiedliche Kriterien.

## Differenzierung

=== "Unterstützende Massnahmen"

    - zunächst nur mit `¬`, `∧` und `∨` arbeiten;
    - die Implikation erst später ergänzen;
    - Verkehrsregeln zuerst vollständig in Alltagssprache formulieren lassen;
    - Satzstarter verwenden:

        > `¬A` bedeutet …

        > `A ∧ B` bedeutet …

        > Diese Formel verhindert die Kollision, weil …

    - einzelne Konfliktpaare markieren;
    - Formeln aus vorgegebenen Bausteinen zusammensetzen;
    - die Wahrheitstabelle zur Überprüfung nutzen;
    - KDNF oder KKNF als systematischen Zwischenschritt von der Tabelle zur Formel verwenden.

=== "Weiterführende Aufgaben"

    - mehrere logisch äquivalente Formeln für dieselbe Kreuzung finden;
    - Äquivalenz ohne LogicTraffic begründen;
    - De-Morgan-Regeln auf weitere Formeln anwenden;
    - eine Formel gezielt in DNF bzw. KNF umformen;
    - kanonische und nicht-kanonische Normalformen vergleichen;
    - eine möglichst kurze Formel für Situation 10 entwickeln;
    - erklären, warum zwei sehr unterschiedlich lange Formeln dieselbe Wahrheitstabelle erzeugen.

!!! tip "Kooperative Durchführung"

    Eine mögliche Rollenverteilung im Tandem:

    - **Person 1:** formuliert die Verkehrsregel bzw. Formel;
    - **Person 2:** übersetzt sie zurück in Alltagssprache und überprüft sie an der Wahrheitstabelle.

    Danach werden die Rollen gewechselt.

    Dadurch steht nicht ausschliesslich die Bedienung der Software im Zentrum, sondern das gegenseitige Erklären der logischen Bedeutung.

## Didaktische Hinweise

LogicTraffic wurde gezielt dafür entwickelt, abstrakte Inhalte der Aussagenlogik über das konkrete Szenario einer Verkehrssteuerung zugänglich zu machen. Unterschiedliche Repräsentationen und eine hohe Interaktivität gehören zu den zentralen didaktischen Ideen der Lernumgebung.

Der vierte Baustein führt diese Progression konsequent weiter:

**Verkehrssituation → Alltagssprache → Wahrheitstabelle → Formel**

Dabei ist wichtig, die Formel nicht lediglich als syntaktische Zeichenfolge zu behandeln. Schwierigkeiten beim Lernen boolescher Logik entstehen unter anderem gerade beim Übersetzen zwischen sprachlichen Anforderungen und formalen Ausdrücken. Auch Negation und Implikation gelten als besonders anspruchsvolle Bereiche.

Die kanonischen Normalformen können dabei als Scaffold dienen. Ihr Wert liegt nicht in ihrer Kürze, sondern in der eindeutigen und mechanischen Beziehung zur Wahrheitstabelle. Lernende erhalten damit einen sicheren Weg von einer bereits verstandenen Repräsentation zu einer zunächst möglicherweise langen Formel.

Für den gymnasialen Anspruch sollte die Arbeit jedoch nicht bei diesem Verfahren enden. Anspruchsvollere Denkprozesse entstehen insbesondere beim Vergleichen, Begründen und Vereinfachen verschiedener äquivalenter Darstellungen.

## Abschluss des Bausteins

Am Ende der Unterrichtsreihe haben die Lernenden dieselbe grundlegende Sicherheitsregel auf mehreren Abstraktionsebenen betrachtet:

1. **handelnd** mit Fahrzeugen und Ampeln;
2. **digital und visuell** in LogicTraffic;
3. **tabellarisch** als Wahrheitstabelle;
4. **symbolisch** als aussagenlogische Formel.

!!! success "Von der Kreuzung zur Logik"

    Eine reale Problemsituation kann schrittweise abstrahiert und formal beschrieben werden.

    Dabei geht keine Information über die Sicherheitsregel verloren – lediglich ihre Darstellung verändert sich.
