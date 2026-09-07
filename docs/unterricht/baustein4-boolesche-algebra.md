# Baustein 4 – Logische Formeln

In diesem Baustein lernen die Lernenden, Sicherheitsregeln einer Verkehrskreuzung mit aussagenlogischen Formeln zu beschreiben.

Ausgangspunkt ist die Erkenntnis aus Baustein 3: Wahrheitstabellen können alle möglichen Zustände vollständig darstellen, werden mit zunehmender Anzahl von Variablen jedoch schnell sehr umfangreich. Die Lernenden untersuchen deshalb, wie dieselbe Sicherheitsregel mit wenigen logischen Operatoren kompakter dargestellt werden kann.

Dabei wechseln sie zwischen Alltagssprache, Verkehrssituation, Wahrheitstabelle und Formel. In der optionalen Vertiefung vergleichen sie unterschiedliche, aber logisch äquivalente Formeln und lernen DNF und KNF als strukturierte Darstellungsformen kennen.

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
    LogicTraffic, Computer oder Tablets, Beamer oder Präsentationsbildschirm sowie die Arbeits- und Merkblätter zu Baustein 4

???+ note "Downloads zu Baustein 4"

    **Basisteil**

    - [:memo: 4a – Muss das wirklich so lang sein?](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4a_logische_operatoren.pdf)
    - [:memo: 4b – Von Worten zu Zeichen](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4b_einfuhrung_formelzeichen.pdf)
    - [:memo: 4c – Von Konflikten zur Formel](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4c_kreuzung_logisch_steuern.pdf)
    - [:material-image-outline: 4d – Logik auf einen Blick](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4d_merkblatt.pdf)

    **Erweiterter Baustein**

    - [:memo: 4e – Anders gebaut, gleich gemeint](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4e_knf_dnf.pdf)
    - [:memo: 4f – Von der Wahrheitstabelle zur Formel](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4f_kknf_kdnf.pdf)
    - [:memo: 4g – Lang, kurz, gleichwertig?](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4g_vergleich_gleichwertigkeit.pdf)
    - [:memo: 4h – Transferaufgabe](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4h_transfer.pdf)

## Lernziele

### Basisteil

Die Lernenden können …

- den Vorteil kompakter Formeln gegenüber umfangreichen Wahrheitstabellen beschreiben;
- die Operatoren `¬`, `∧`, `∨` und `→` in ihrem Verkehrskontext erklären;
- einfache Verkehrs- und Sicherheitsregeln in aussagenlogische Formeln übersetzen;
- einfache logische Formeln wieder in Alltagssprache übersetzen;
- logische Formeln in LogicTraffic syntaktisch korrekt eingeben;
- eine Formel anhand der zugehörigen Wahrheitstabelle überprüfen;
- zwischen einer konkreten Verkehrssituation, einer sprachlichen Regel, einer Wahrheitstabelle und einer Formel wechseln;
- erklären, dass unterschiedliche Formeln dieselbe Sicherheitsregel beschreiben können.

### Optionale Vertiefung

Die Lernenden können zusätzlich …

- DNF- und KNF-Formeln lesen und ihre Struktur beschreiben;
- DNF und KNF in einfachen Beispielen erkennen;
- logisch äquivalente Formeln anhand ihrer Wahrheitstabellen erkennen;
- einfache Anwendungen der De-Morgan-Regeln nachvollziehen;
- erklären, wie eine KDNF bzw. KKNF direkt aus einer Wahrheitstabelle erzeugt werden kann;
- kanonische und vereinfachte Formeln hinsichtlich Länge, Verständlichkeit und Verwendungszweck vergleichen.

??? note "Abgrenzung zu Baustein 3"

    In Baustein 3 stand die Frage im Zentrum:

    > Wie können wir **alle möglichen Zustände vollständig** darstellen?

    Baustein 4 verfolgt nun eine andere Frage:

    > Wie können wir **dieselbe Sicherheitsregel möglichst kompakt und eindeutig** beschreiben?

    Die Wahrheitstabelle verschwindet dabei nicht. Sie dient weiterhin zur Überprüfung, ob zwei Darstellungen tatsächlich dieselbe logische Funktion beschreiben.

## Vorbereitung

- LogicTraffic auf den Geräten öffnen und die Funktionsfähigkeit des Formeleditors prüfen.
- Für den Einstieg eine einfache Situation mit zwei Fahrspuren vorbereiten.
- Situation 3 für die selbstständige Modellierung bereithalten.
- Situation 4 für die Vertiefung zu DNF und KNF bereithalten.
- Falls die Vertiefung durchgeführt wird, die Auswahlmöglichkeiten für Normalformen im Formeleditor vorab prüfen.
- Situation 10 für den abschliessenden Transfer bereithalten.
- Die benötigten Arbeitsblätter ausdrucken oder digital bereitstellen.

??? info "Fachlicher Hintergrund – logische Operatoren"

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

    ??? warning "Die Implikation ist anspruchsvoller"

        Der Ausdruck `A → ¬B` wird im Alltag leicht anders verstanden als in der formalen Logik.

        Für die erste Einführung kann deshalb zunächst mit einem direkten Kollisionsverbot gearbeitet werden:

        `¬(A ∧ B)`

        Bedeutung:

        > A und B dürfen nicht gleichzeitig Grün haben.

        Die Implikation kann anschliessend als alternative Form derselben Sicherheitsidee eingeführt werden.

## Unterrichtsablauf – Überblick

| Phase | Inhalt | Material | Richtwert |
| --- | --- | --- | --- |
| **1. Problemstellung** | Skalierungsproblem aufgreifen und nach einer kompakteren Darstellung suchen | **AB 4a** | ca. 5–10 Min. |
| **2. Erarbeitung** | Logische Operatoren kennenlernen, lesen und erste Formeln bilden | **AB 4b** | ca. 15 Min. |
| **3. Modellierung** | Sicherheitsregeln für Situation 3 selbstständig formulieren und prüfen | **AB 4c**, ggf. **MB 4d** | ca. 20 Min. |
| **4. Vergleich** | Unterschiedliche korrekte Formeln vergleichen und Äquivalenz vorbereiten | **MB 4d** | ca. 10 Min. |
| **5. Sicherung** | Operatoren und Darstellungswechsel sichern | **MB 4d** | ca. 10 Min. |

## Durchführung

???+ abstract "Phase 1 – Von der Tabelle zur Regel"

    **Ziel:** Die Lernenden reaktivieren das Skalierungsproblem von Wahrheitstabellen und entwickeln das Bedürfnis nach einer kompakteren Darstellung.

    **Material:**  
    [:memo: AB 4a – Muss das wirklich so lang sein?](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4a_logische_operatoren.pdf)

    Die Lehrperson greift die Ergebnisse aus Baustein 3 auf:

    $$
    2^5 = 32
    $$

    mögliche Belegungen bei fünf Variablen und

    $$
    2^{10} = 1024
    $$

    Belegungen bei zehn Variablen.

    !!! question "Einstiegsfrage"

        Wahrheitstabellen können vollständig beschreiben, welche Ampelstellungen sicher sind.

        **Müssen wir dafür aber wirklich jede mögliche Kombination einzeln aufschreiben?**

        Oder können wir die Sicherheitsregel mit wenigen Zeichen ausdrücken?

    Die Lernenden bearbeiten anschliessend **AB 4a**. Im Zentrum steht noch nicht die formale Schreibweise, sondern die Frage, **warum eine kompakte Darstellung überhaupt hilfreich sein könnte**.

    ??? example "Mögliche Aussagen der Lernenden"

        > A und B dürfen nicht gleichzeitig Grün haben.

        > Wenn A Grün hat, muss B Rot haben.

        > Mindestens eine der beiden Ampeln muss Rot zeigen.

    ??? note "Didaktische Absicht"

        Die Formel entsteht aus einer bereits verstandenen Verkehrsregel.

        Dadurch wird die symbolische Darstellung nicht als isolierter Zeichenvorrat eingeführt, sondern als weitere Repräsentation einer bekannten Situation.

???+ abstract "Phase 2 – Von Worten zu Zeichen"

    **Ziel:** Die Lernenden ordnen sprachlichen Verknüpfungen logische Operatoren zu, lesen einfache Formeln und bilden erste eigene Ausdrücke.

    **Material:**  
    [:memo: AB 4b – Von Worten zu Zeichen](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4b_einfuhrung_formelzeichen.pdf)

    Die Operatoren `¬`, `∧`, `∨` und `→` werden schrittweise eingeführt. Die Lernenden übersetzen dabei bewusst **in beide Richtungen**:

    **Sprache → Formel**  
    und  
    **Formel → Sprache**

    Anschliessend wird eine einfache Sicherheitsregel in LogicTraffic geprüft, beispielsweise:

    `¬(A ∧ B)`

    > A und B dürfen nicht gleichzeitig Grün haben.

    ??? tip "Worauf beim Besprechen achten?"

        - Das logische `ODER` ist inklusiv: Mindestens eine Aussage ist wahr, beide dürfen ebenfalls wahr sein.
        - Klammern zeigen, welcher Teil einer Formel zusammengehört.
        - Die Lernenden sollen zuerst fachlich begründen und erst danach das Softwarefeedback zur Kontrolle verwenden.

    ??? warning "Klammern verändern die Bedeutung"

        Vergleichen Sie:

        `¬(A ∧ B)`

        mit

        `¬A ∧ B`

        Im ersten Fall wird die gesamte UND-Verknüpfung negiert. Im zweiten Fall nur `A`.

    ??? success "Mögliche Lösungen zu den ersten Übersetzungen"

        | Verkehrssituation / Regel | Logischer Ausdruck |
        | --- | --- |
        | Spur `B` muss anhalten. | `¬B` |
        | Spur `A` und Spur `B` haben gleichzeitig Grün. | `A ∧ B` |
        | Mindestens eine der beiden Spuren muss Rot haben. | `¬A ∨ ¬B` |
        | Wenn `A` Grün hat, muss `B` Rot haben. | `A → ¬B` |

???+ abstract "Phase 3 – Von Konflikten zur Formel"

    **Ziel:** Die Lernenden entwickeln für Situation 3 selbstständig aussagenlogische Sicherheitsregeln.

    **Material:**  
    [:memo: AB 4c – Von Konflikten zur Formel](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4c_kreuzung_logisch_steuern.pdf)  
    [:material-image-outline: MB 4d – Logik auf einen Blick](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4d_merkblatt.pdf)

    Die Lernenden öffnen **Situation 3** und bearbeiten AB 4c möglichst selbstständig.

    Der Modellierungsweg lautet:

    **Kreuzung → Konflikt → Sicherheitsregel in Worten → Teilformel → Gesamtformel → Prüfung**

    ??? tip "Denkhilfe"

        Statt sofort eine grosse Formel zu suchen, werden zunächst einzelne Konflikte beschrieben.

        Beispielsweise:

        > A und C dürfen nicht gleichzeitig Grün haben.

        Daraus wird:

        `¬(A ∧ C)`

        Für den zweiten Konflikt:

        `¬(B ∧ C)`

        Beide Regeln müssen gleichzeitig gelten. Deshalb können sie mit `∧` verbunden werden.

    ??? success "Mögliche korrekte Formeln für Situation 3"

        **Kollisionsverbote**

        `¬(A ∧ C) ∧ ¬(B ∧ C)`

        **Mit Implikationen**

        `(A → ¬C) ∧ (B → ¬C)`

        **Zusammengefasste Implikation**

        `C → (¬A ∧ ¬B)`

        **KNF**

        `(¬A ∨ ¬C) ∧ (¬B ∨ ¬C)`

        Die Formeln sehen unterschiedlich aus, erzeugen aber dieselbe Sicherheitsregel.

    ??? warning "Safe ist nicht automatisch optimal"

        Eine Formel kann alle Kollisionen verhindern und trotzdem unnötig viele sichere Zustände verbieten.

        Beispielsweise wäre eine Steuerung, bei der alle Ampeln immer Rot bleiben, zwar sicher, aber wenig sinnvoll.

        Für die Reflexion sind deshalb zwei Fragen wichtig:

        - Verhindert die Formel alle Kollisionen?
        - Erlaubt sie gleichzeitig die sicheren Kombinationen?

???+ abstract "Phase 4 – Verschieden geschrieben, gleich gemeint"

    **Ziel:** Die Lernenden erkennen, dass unterschiedlich aussehende Formeln dieselbe logische Funktion beschreiben können.

    **Material:**  
    [:material-image-outline: MB 4d – Logik auf einen Blick](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4d_merkblatt.pdf)

    Besonders geeignet ist der Vergleich:

    `¬(A ∧ C)`

    und

    `¬A ∨ ¬C`

    Die Lernenden geben beide Formeln nacheinander in LogicTraffic ein und vergleichen die Wahrheitstabellen.

    !!! question "Leitfragen"

        - Erzeugen beide Formeln bei jeder Belegung dieselben Wahrheitswerte?
        - Wie lassen sich beide Formeln in Alltagssprache lesen?
        - Warum beschreiben sie dieselbe Sicherheitsregel?

    Wenn zwei Formeln für jede mögliche Belegung denselben Wahrheitswert ergeben, sind sie **logisch äquivalent**:

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

???+ abstract "Phase 5 – Ergebnisse sichern"

    **Ziel:** Die Lernenden sichern die Operatoren sowie den Zusammenhang zwischen Verkehrssituation, Sprache, Wahrheitstabelle und Formel.

    **Material:**  
    [:material-image-outline: MB 4d – Logik auf einen Blick](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4d_merkblatt.pdf)

    Das Merkblatt kann gemeinsam besprochen und anschliessend als Nachschlagehilfe für die weiteren Arbeitsblätter verwendet werden.

    ??? example "Mögliche Ergebnissicherung"

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

    ??? success "Ich kann …"

        - die Operatoren `¬`, `∧`, `∨` und `→` erklären;
        - eine einfache Verkehrsregel in eine Formel übersetzen;
        - eine Formel wieder in Alltagssprache übersetzen;
        - mit der Wahrheitstabelle überprüfen, was eine Formel bewirkt;
        - erklären, warum zwei unterschiedlich aussehende Formeln logisch gleichwertig sein können.

## Optionale Vertiefung – DNF und KNF

Die Vertiefung kann direkt an den Basisteil angeschlossen oder in einer zusätzlichen Lektion durchgeführt werden.

| Schritt | Schwerpunkt | Material |
| --- | --- | --- |
| **1. DNF und KNF entdecken** | Normalformen lesen und ihre Struktur erkennen | **AB 4e** |
| **2. Von der Wahrheitstabelle zur Formel** | KDNF und KKNF systematisch erzeugen | **AB 4f** |
| **3. Lang, kurz, gleichwertig?** | Darstellungen vergleichen und beurteilen | **AB 4g** |

???+ abstract "Vertiefung 1 – DNF und KNF entdecken"

    **Ziele:** Die Lernenden lesen DNF- und KNF-Formeln, erkennen ihren Aufbau und beschreiben die Struktur.

    **Material:**  
    [:memo: AB 4e – Anders gebaut, gleich gemeint](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4e_knf_dnf.pdf)

    Für diese Vertiefung wird **Situation 4** verwendet.

    Eine Formel in **disjunktiver Normalform (DNF)** besteht aus UND-Termen, die mit ODER verbunden werden.

    Beispiel:

    `(A ∧ ¬B) ∨ (¬A ∧ C)`

    Eine Formel in **konjunktiver Normalform (KNF)** besteht aus ODER-Termen, die mit UND verbunden werden.

    Beispiel:

    `(¬A ∨ ¬C) ∧ (¬B ∨ ¬C)`

    Der Schwerpunkt liegt bewusst zunächst auf dem **Lesen und Erkennen**, bevor die Lernenden selbst Normalformen erzeugen.

    ??? info "DNF und KNF als Form – nicht als neue Funktion"

        DNF und KNF beschreiben keine grundsätzlich anderen logischen Funktionen.

        Sie sind bestimmte **Strukturen**, in denen eine Formel geschrieben werden kann.

        Dieselbe Funktion kann deshalb als freie Formel, DNF, KNF oder in einer anderen äquivalenten Form dargestellt werden.

???+ abstract "Vertiefung 2 – Von der Wahrheitstabelle zur Formel"

    **Ziele:** Die Lernenden erkennen, wie KDNF und KKNF nach einem festen Verfahren direkt aus einer Wahrheitstabelle entstehen.

    **Material:**  
    [:memo: AB 4f – Von der Wahrheitstabelle zur Formel](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4f_kknf_kdnf.pdf)

    Die kanonischen Formen dienen hier als **Brücke zwischen Wahrheitstabelle und Formel**.

    **KDNF**

    - Ausgangspunkt sind die Zeilen mit `sicher = 1`.
    - Für jede dieser Zeilen wird ein vollständiger UND-Term gebildet.
    - Die UND-Terme werden mit `∨` verbunden.

    **KKNF**

    - Ausgangspunkt sind die Zeilen mit `sicher = 0`.
    - Für jede dieser Zeilen wird ein ODER-Term gebildet, der genau diese Belegung ausschliesst.
    - Die ODER-Terme werden mit `∧` verbunden.

    ??? important "Warum dieser Zwischenschritt hilfreich sein kann"

        Die Formel muss nicht erraten werden. Sie kann **systematisch direkt aus der Wahrheitstabelle konstruiert werden**.

        Der Nachteil ist die Länge: Da jede relevante Tabellenzeile einzeln berücksichtigt wird, entstehen häufig sehr lange Formeln.

        Ein möglicher Lösungsweg lautet deshalb:

        **Wahrheitstabelle → KDNF/KKNF → vereinfachte Formel**

    ??? tip "Differenzierung mit den kanonischen Formen"

        **Direkter Weg**

        Verkehrssituation  
        → eigene kompakte Formel

        **Systematischer Weg**

        Wahrheitstabelle  
        → KDNF oder KKNF  
        → Struktur untersuchen  
        → Formel vereinfachen

        Beide Wege können zur gleichen logischen Funktion führen.

???+ abstract "Vertiefung 3 – Lang, kurz, gleichwertig?"

    **Ziel:** Die Lernenden vergleichen verschiedene Darstellungen derselben logischen Funktion und beurteilen ihre Eignung.

    **Material:**  
    [:memo: AB 4g – Lang, kurz, gleichwertig?](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4g_vergleich_gleichwertigkeit.pdf)

    Verglichen werden beispielsweise:

    - eine eigene Formel;
    - eine DNF oder KNF;
    - eine KDNF oder KKNF;
    - eine vereinfachte Darstellung aus LogicTraffic.

    Im Mittelpunkt steht nicht die Suche nach **der einen besten Formel**, sondern die Frage, welche Darstellung für welchen Zweck geeignet ist.

    ??? success "Zentrale Erkenntnis"

        Logisch äquivalente Formeln können sehr unterschiedlich aussehen.

        Eine kurze Formel ist oft leichter zu lesen. Eine kanonische Formel ist dagegen systematisch aus der Wahrheitstabelle erzeugbar und berücksichtigt sichtbar alle relevanten Fälle.

## Optionaler Transfer – Situation 10

???+ abstract "Transfer – Eine komplexe Kreuzung steuern"

    **Ziel:** Die Lernenden wenden ihre Kenntnisse auf eine Kreuzung mit fünf Variablen und damit 32 möglichen Belegungen an.

    **Material:**  
    [:memo: AB 4h – Transferaufgabe](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4h_transfer.pdf)

    Die Lernenden öffnen **Situation 10** und analysieren die Konflikte zwischen den Fahrspuren.

    Der Arbeitsweg orientiert sich an den vorherigen Aufgaben:

    **Kreuzung → Konflikte → sprachliche Regeln → Teilformeln → Gesamtformel → Prüfung**

    ??? tip "Alternative mit kanonischer Form"

        Falls der direkte Weg zur kompakten Formel schwierig ist:

        1. Ausgangspunkt ist die vollständige Wahrheitstabelle.
        2. Eine KDNF oder KKNF wird erzeugt.
        3. Die Lernenden untersuchen, wie die Tabellenzeilen in der Formel wiederzufinden sind.
        4. Anschliessend wird die lange kanonische Formel mit einer vereinfachten Darstellung verglichen.

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

???+ example "Unterstützende Massnahmen"

    - zunächst nur mit `¬`, `∧` und `∨` arbeiten;
    - die Implikation erst später ergänzen;
    - Verkehrsregeln zuerst vollständig in Alltagssprache formulieren lassen;
    - Satzstarter verwenden:

        > `¬A` bedeutet …

        > `A ∧ B` bedeutet …

        > Diese Formel verhindert die Kollision, weil …

    - einzelne Konfliktpaare markieren;
    - Formeln aus vorgegebenen Bausteinen zusammensetzen;
    - das Merkblatt 4d als Nachschlagehilfe nutzen;
    - die Wahrheitstabelle zur Überprüfung nutzen;
    - KDNF oder KKNF als systematischen Zwischenschritt von der Tabelle zur Formel verwenden.

??? example "Weiterführende Aufgaben"

    - mehrere logisch äquivalente Formeln für dieselbe Kreuzung finden;
    - Äquivalenz ohne LogicTraffic begründen;
    - De-Morgan-Regeln auf weitere Formeln anwenden;
    - eine Formel gezielt in DNF bzw. KNF umformen;
    - kanonische und nicht-kanonische Normalformen vergleichen;
    - eine möglichst kurze Formel für Situation 10 entwickeln;
    - erklären, warum zwei sehr unterschiedlich lange Formeln dieselbe Wahrheitstabelle erzeugen.

??? tip "Kooperative Durchführung"

    Eine mögliche Rollenverteilung im Tandem:

    - **Person 1:** formuliert die Verkehrsregel bzw. Formel;
    - **Person 2:** übersetzt sie zurück in Alltagssprache und überprüft sie an der Wahrheitstabelle.

    Danach werden die Rollen gewechselt.

    Dadurch steht nicht ausschliesslich die Bedienung der Software im Zentrum, sondern das gegenseitige Erklären der logischen Bedeutung.

## Didaktische Hinweise

LogicTraffic wurde gezielt dafür entwickelt, abstrakte Inhalte der Aussagenlogik über das konkrete Szenario einer Verkehrssteuerung zugänglich zu machen. Unterschiedliche Repräsentationen und eine hohe Interaktivität gehören zu den zentralen didaktischen Ideen der Lernumgebung.

Der vierte Baustein führt diese Progression konsequent weiter:

**Verkehrssituation → Alltagssprache → Wahrheitstabelle → Formel**

??? note "Warum der Wechsel zwischen Darstellungen wichtig ist"

    Die Formel sollte nicht lediglich als syntaktische Zeichenfolge behandelt werden.

    Schwierigkeiten beim Lernen boolescher Logik entstehen unter anderem beim Übersetzen zwischen sprachlichen Anforderungen und formalen Ausdrücken. Negation und Implikation gelten dabei als besonders anspruchsvoll.

    Deshalb wechseln die Lernenden wiederholt zwischen:

    - Verkehrssituation,
    - Alltagssprache,
    - Wahrheitstabelle,
    - logischer Formel.

??? note "Rolle der kanonischen Normalformen"

    Die kanonischen Normalformen können als Scaffold dienen.

    Ihr Wert liegt nicht in ihrer Kürze, sondern in der eindeutigen und mechanischen Beziehung zur Wahrheitstabelle. Lernende erhalten damit einen sicheren Weg von einer bereits verstandenen Repräsentation zu einer zunächst möglicherweise langen Formel.

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