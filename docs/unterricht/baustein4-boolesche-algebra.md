# Baustein 4 – Logische Formeln

In diesem Baustein lernen die Lernenden, Sicherheitsregeln einer Verkehrskreuzung mit aussagenlogischen Formeln zu beschreiben.

Ausgangspunkt ist die Erkenntnis aus [Baustein 3 – Wahrheitstabellen](baustein3-wahrheitstabellen.md): Wahrheitstabellen können alle möglichen Zustände vollständig darstellen, werden mit zunehmender Anzahl von Variablen jedoch schnell sehr umfangreich. Baustein 4 greift genau dieses Problem auf. Die Lernenden entwickeln aus bereits verstandenen Verkehrssituationen schrittweise kompakte logische Regeln und überprüfen diese anschliessend wieder an der Wahrheitstabelle.

Die Progression des Bausteins lautet:

**Verkehrssituation → sprachliche Regel → logische Formel → Wahrheitstabelle → Vergleich und Reflexion**

In der optionalen Vertiefung untersuchen die Lernenden logisch äquivalente Formeln sowie DNF und KNF. KDNF und KKNF werden dabei nicht als eigentliches Lernziel in den Vordergrund gestellt, sondern als systematischer Zwischenschritt von der Wahrheitstabelle zur Formel genutzt.

!!! abstract "Auf einen Blick"

    **:stopwatch: Dauer:**  
    Basisteil: ca. **60 Minuten**  
    optionale Vertiefung: zusätzlich ca. **45 Minuten**  
    optionaler Transfer: zusätzlich ca. **20–30 Minuten**

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

??? note "Downloads zu Baustein 4"

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

- logisch äquivalente Formeln anhand ihrer Wahrheitstabellen erkennen;
- einfache Anwendungen der De-Morgan-Regeln nachvollziehen;
- DNF- und KNF-Formeln lesen und ihre Struktur beschreiben;
- DNF und KNF in einfachen Beispielen erkennen;
- erklären, wie eine KDNF bzw. KKNF systematisch aus einer Wahrheitstabelle erzeugt werden kann;
- kanonische, freie und vereinfachte Formeln hinsichtlich Länge, Verständlichkeit und Verwendungszweck vergleichen.

### Optionaler Transfer

Die Lernenden können zusätzlich …

- eine komplexere Kreuzung systematisch in Teilprobleme zerlegen;
- mehrere Konfliktbedingungen zu einer Gesamtformel verbinden;
- ihre Lösung mit LogicTraffic fachlich begründet überprüfen;
- verschiedene Lösungswege vergleichen und die Rolle der Wahrheitstabelle als Kontrollinstrument erklären.

??? note "Abgrenzung zu Baustein 3"

    In Baustein 3 stand die Frage im Zentrum:

    > Wie können wir **alle möglichen Zustände vollständig** darstellen?

    Baustein 4 verfolgt nun eine andere Frage:

    > Wie können wir **dieselbe Sicherheitsregel kompakt und eindeutig** beschreiben?

    Die Wahrheitstabelle verschwindet dabei nicht. Sie erhält eine neue Rolle: Sie dient vor allem dazu, Formeln zu **überprüfen und zu vergleichen**.

## Vorbereitung

- LogicTraffic auf allen Geräten öffnen und den Formeleditor kurz testen.
- Für Phase 1 Situation 10 oder das entsprechende Abschlussbild aus Baustein 3 bereithalten.
- Für Phase 2 eine einfache Situation mit zwei Fahrspuren vorbereiten.
- Situation 3 für Phase 3 bereithalten.
- Situation 4 für die optionale Vertiefung vorbereiten.
- Situation 10 für den abschliessenden Transfer bereithalten.
- Falls die Vertiefung durchgeführt wird, die Anzeige bzw. Erzeugung verschiedener Normalformen in LogicTraffic vorab prüfen.
- Die benötigten Arbeitsblätter ausdrucken oder digital bereitstellen.
- Das [Merkblatt 4d](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4d_merkblatt.pdf) so bereithalten, dass es ab Phase 2 bei Bedarf als Nachschlagehilfe eingesetzt werden kann.

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

    Besonders die **Negation** und die **Implikation** benötigen eine sorgfältige sprachliche Begleitung. Die Lernenden sollen deshalb wiederholt in beide Richtungen übersetzen:

    **Sprache → Formel**  
    und  
    **Formel → Sprache**

??? info "Fachlicher Hintergrund – Normalformen"

    Eine Formel in **disjunktiver Normalform (DNF)** besteht aus UND-Termen, die mit ODER verbunden werden.

    Beispiel:

    `(A ∧ ¬B) ∨ (¬A ∧ C)`

    Eine Formel in **konjunktiver Normalform (KNF)** besteht aus ODER-Klauseln, die mit UND verbunden werden.

    Beispiel:

    `(¬A ∨ ¬C) ∧ (¬B ∨ ¬C)`

    DNF und KNF sind keine neuen logischen Funktionen, sondern bestimmte **Strukturen**, in denen eine Funktion dargestellt werden kann.

    **KDNF und KKNF** sind kanonische Sonderformen. Ihr didaktischer Wert liegt vor allem darin, dass sie sich nach einem festen Verfahren direkt aus einer Wahrheitstabelle konstruieren lassen. Sie sind deshalb ein hilfreiches Scaffold, wenn der direkte Weg zu einer kompakten Formel schwierig ist.

## Unterrichtsablauf – Überblick

| Phase | Schwerpunkt | Material | Richtwert |
| --- | --- | --- | ---: |
| **1. Von der Tabelle zur Regel** | Skalierungsproblem reaktivieren und Bedarf nach einer kompakten Darstellung erzeugen | **[AB 4a](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4a_logische_operatoren.pdf)** | ca. 10 Min. |
| **2. Von Worten zu Zeichen** | Operatoren kennenlernen, Formeln lesen und erste Regeln formal ausdrücken | **[AB 4b](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4b_einfuhrung_formelzeichen.pdf)**, **[MB 4d](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4d_merkblatt.pdf)** | ca. 20 Min. |
| **3. Von Konflikten zur Formel** | Situation 3 modellieren, Teilregeln verbinden und Lösung überprüfen | **[AB 4c](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4c_kreuzung_logisch_steuern.pdf)**, **[MB 4d](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4d_merkblatt.pdf)** | ca. 30 Min. |
| **4. Anders gebaut, gleich gemeint** | Äquivalenz, De Morgan sowie DNF und KNF entdecken | **[AB 4e](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4e_knf_dnf.pdf)** | ca. 15 Min. |
| **5. Von der Wahrheitstabelle zur Formel** | KDNF/KKNF als systematischen Zwischenschritt kennenlernen | **[AB 4f](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4f_kknf_kdnf.pdf)** | ca. 15 Min. |
| **6. Lang, kurz, gleichwertig?** | Verschiedene äquivalente Darstellungen vergleichen und beurteilen | **[AB 4g](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4g_vergleich_gleichwertigkeit.pdf)** | ca. 15 Min. |
| **7. Transfer – Situation 10** | Vorgehen auf eine komplexe Kreuzung mit fünf Variablen übertragen | **[AB 4h](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4h_transfer.pdf)** | ca. 20–30 Min. |

Die **Phasen 1–3 bilden den Basisteil**. Die **Phasen 4–6 sind eine optionale Vertiefung** und können in einer zusätzlichen Lektion durchgeführt werden. **Phase 7 ist ein zusätzlicher Transfer** und kann je nach verfügbarem Zeitgefäss angeschlossen oder später eingesetzt werden.

## Durchführung

### Phase 1 - Von der Tabelle zur Regel

??? success "Ziele der Einheit"

    Die Lernenden erkennen das Skalierungsproblem von Wahrheitstabellen wieder und können erklären, warum bei komplexeren Kreuzungen eine kompaktere Darstellung sinnvoll ist.

    Sie formulieren eine bereits verstandene Sicherheitsbedingung zunächst bewusst in Alltagssprache. Die formalen Zeichen werden in dieser Phase noch nicht systematisch eingeführt.

??? example "Material"

    - [:memo: AB 4a – Muss das wirklich so lang sein?](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4a_logische_operatoren.pdf)
    - Beamer oder Präsentationsbildschirm
    - LogicTraffic mit Situation 10 oder die entsprechende Darstellung aus Baustein 3
    - optional: Notizpapier oder Begleitportfolio

??? info "Sozialformen"

    Kurzer Einstieg im **Plenum**, anschliessend eine kurze **Partnerphase** zur Formulierung einer Sicherheitsregel und gemeinsame Sicherung im **Plenum**.

??? tip "benötigte Zeit"

    ca. **10 Minuten**

??? abstract "Verlaufsplanung"

    **1. Rückbezug auf Baustein 3**

    Die Lehrperson zeigt erneut eine komplexere Kreuzung mit fünf Variablen.

    Gemeinsam wird erinnert:

    $$
    2^5 = 32
    $$

    mögliche Belegungen.

    Als gedankliche Steigerung wird gefragt, wie viele Zeilen bei zehn Variablen notwendig wären:

    $$
    2^{10} = 1024
    $$

    **Inputfrage:**

    > Was ist an einer Wahrheitstabelle praktisch, und was wird bei vielen Variablen problematisch?

    **Erwartete Antworten:**

    - Alle möglichen Zustände sind vollständig enthalten.
    - Man kann nichts vergessen, wenn die Tabelle korrekt aufgebaut ist.
    - Die Tabelle wird schnell sehr lang und unübersichtlich.
    - Das manuelle Erstellen und Prüfen wird zeitaufwendig und fehleranfällig.

    **2. Bearbeitung von [AB 4a](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4a_logische_operatoren.pdf)**

    Die Lernenden bearbeiten den Einstieg auf [AB 4a](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4a_logische_operatoren.pdf). Im Zentrum steht die Frage, ob eine bekannte Sicherheitsbedingung auch **ohne vollständige Auflistung aller Zustände** beschrieben werden kann.

    **Zentrale Leitfrage:**

    > Müssen wir wirklich jede mögliche Kombination einzeln aufschreiben, oder können wir die Sicherheitsregel mit einer kurzen Regel ausdrücken?

    In der Partnerphase werden mögliche sprachliche Regeln formuliert.

    **Mögliche Aussagen der Lernenden:**

    > A und B dürfen nicht gleichzeitig Grün haben.

    > Wenn A Grün hat, muss B Rot haben.

    > Mindestens eine der beiden Spuren muss Rot zeigen.

    **3. Gemeinsame Überleitung**

    Die Lehrperson sammelt zwei bis drei Formulierungen und stellt die Anschlussfrage:

    > Wie könnten wir eine solche Regel so schreiben, dass sie kurz, eindeutig und auch von einem Computer ausgewertet werden kann?

    Diese Frage führt direkt zu Phase 2.

??? note "Didaktische Hinweise"

    Die formale Schreibweise sollte hier noch **nicht vorweggenommen** werden. Entscheidend ist zunächst, dass die Lernenden selbst einen Bedarf für eine kompaktere Repräsentation erleben.

    Der Übergang aus Baustein 3 bleibt dadurch inhaltlich nachvollziehbar: Die Wahrheitstabelle wird nicht als „schlechtes“ Verfahren abgewertet, sondern als vollständige Darstellung gewürdigt, deren Skalierungsgrenzen nun eine neue Repräsentationsform motivieren.

    Die sprachlichen Lösungen müssen an dieser Stelle noch nicht fachsprachlich perfekt sein. Sie bilden das Ausgangsmaterial für die Formalisierung in Phase 2.

??? bug "Differenzierung"

    === "Vereinfachungen"

        - Eine einfache Kreuzung mit nur zwei Fahrspuren verwenden.
        - Satzstarter anbieten:  
          > „A und B dürfen nicht …“  
          > „Wenn A Grün hat, dann …“
        - Die Zahlen $2^5$ und $2^{10}$ bereits vorgeben und nur die Bedeutung diskutieren lassen.
        - Die Lernenden zunächst nur eine einzige Sicherheitsregel formulieren lassen.

    === "Erweiterungen"

        - Die Lernenden berechnen lassen, wie viele Tabellenzeilen bei 6, 8, 12 oder 15 Variablen entstehen.
        - Zwei Darstellungen vergleichen lassen: vollständige Tabelle versus kurze sprachliche Regel.
        - Diskutieren lassen, welche Eigenschaften eine gute formale Darstellung haben sollte: kurz, eindeutig, überprüfbar und maschinenlesbar.

### Phase 2 - Von Worten zu Zeichen

??? success "Ziele der Einheit"

    Die Lernenden können die Operatoren `¬`, `∧`, `∨` und `→` im Verkehrskontext lesen und einfachen sprachlichen Regeln zuordnen.

    Sie übersetzen einfache Aussagen in beide Richtungen zwischen Alltagssprache und Formel und überprüfen erste Formeln in LogicTraffic.

??? example "Material"

    - [:memo: AB 4b – Von Worten zu Zeichen](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4b_einfuhrung_formelzeichen.pdf)
    - [:material-image-outline: MB 4d – Logik auf einen Blick](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4d_merkblatt.pdf)
    - LogicTraffic
    - Computer oder Tablet pro Zweiergruppe
    - Beamer oder Präsentationsbildschirm

??? info "Sozialformen"

    Kurzer **fragend-entwickelnder Input im Plenum**, anschliessend **Partnerarbeit** mit [AB 4b](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4b_einfuhrung_formelzeichen.pdf). Die erste Überprüfung in LogicTraffic erfolgt ebenfalls im Tandem. Abschliessend kurze gemeinsame Sicherung.

??? tip "benötigte Zeit"

    ca. **20 Minuten**

??? abstract "Verlaufsplanung"

    **1. Sprachliche Regeln aus Phase 1 aufgreifen**

    Die Lehrperson greift eine bekannte Aussage auf:

    > A und B dürfen nicht gleichzeitig Grün haben.

    Die Aussage wird zunächst in kleinere logische Bausteine zerlegt.

    **Inputfragen:**

    > Wie können wir ausdrücken, dass A Grün hat?

    **Erwartete Antwort:** `A`

    > Wie können wir ausdrücken, dass A nicht Grün hat?

    **Erwartete Antwort:** `¬A`

    Anschliessend werden die vier Operatoren schrittweise eingeführt:

    | Alltagssprache | Symbol | Beispiel |
    | --- | :---: | --- |
    | NICHT | `¬` | `¬A` |
    | UND | `∧` | `A ∧ B` |
    | ODER | `∨` | `A ∨ B` |
    | WENN … DANN | `→` | `A → ¬B` |

    **2. [AB 4b](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4b_einfuhrung_formelzeichen.pdf) bearbeiten**

    Die Lernenden übersetzen bewusst in **beide Richtungen**:

    **Sprache → Formel**  
    und  
    **Formel → Sprache**

    Eine sinnvolle Rollenverteilung im Tandem ist:

    - Person 1 übersetzt die Aussage in eine Formel.
    - Person 2 liest die Formel wieder in Alltagssprache zurück.
    - Danach werden die Rollen gewechselt.

    **Mögliche Übersetzungen:**

    | Verkehrssituation / Regel | Logischer Ausdruck |
    | --- | --- |
    | Spur `B` muss anhalten. | `¬B` |
    | Spur `A` und Spur `B` haben gleichzeitig Grün. | `A ∧ B` |
    | Mindestens eine der beiden Spuren muss Rot haben. | `¬A ∨ ¬B` |
    | Wenn `A` Grün hat, muss `B` Rot haben. | `A → ¬B` |

    **3. Erste Formel in LogicTraffic überprüfen**

    Als gut zugänglicher Einstieg wird verwendet:

    `¬(A ∧ B)`

    **Inputfragen:**

    > Welche Belegung soll diese Formel verbieten?

    **Erwartete Antwort:** Genau die Belegung, bei der `A = 1` und `B = 1` gilt.

    > Welche Belegungen sollen erlaubt bleiben?

    **Erwartete Antwort:** `00`, `01` und `10`, sofern die beiden Spuren tatsächlich miteinander kollidieren.

    Die Formel wird eingegeben und die erzeugte Wahrheitstabelle mit der fachlichen Erwartung verglichen.

    **4. Klammern und Bedeutung sichern**

    Gemeinsam werden zwei Formeln verglichen:

    `¬(A ∧ B)`

    und

    `¬A ∧ B`

    **Inputfrage:**

    > Was wird jeweils negiert?

    **Erwartete Antwort:**

    - Bei `¬(A ∧ B)` wird die gesamte UND-Verknüpfung negiert.
    - Bei `¬A ∧ B` wird nur `A` negiert.

    Das [Merkblatt 4d](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4d_merkblatt.pdf) kann ab jetzt als Nachschlagehilfe verwendet werden.

??? note "Didaktische Hinweise"

    Die Lernenden sollen die Operatoren nicht als isolierte Zeichentabelle auswendig lernen, sondern ihre Bedeutung jeweils an einer bekannten Verkehrssituation aufbauen.

    Für die erste aktive Verwendung empfiehlt es sich, den Schwerpunkt zunächst auf `¬`, `∧` und `∨` zu legen. Die Implikation `→` kann eingeführt und gelesen werden, ist sprachlich jedoch anspruchsvoller und muss nicht sofort die bevorzugte Schreibweise der Lernenden sein.

    Beim logischen `ODER` ist auf die inklusive Bedeutung hinzuweisen. Zudem darf die Implikation nicht als zeitliche Abfolge verstanden werden.

    LogicTraffic dient zur **Überprüfung**, nicht als Ersatz für die Begründung. Eine Aussage wie „Die Formel stimmt, weil LogicTraffic `Optimal` anzeigt“ reicht fachlich nicht aus.

??? bug "Differenzierung"

    === "Vereinfachungen"

        - Zunächst nur mit `¬`, `∧` und `∨` arbeiten; `→` erst am Schluss ergänzen.
        - Das [Merkblatt 4d](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4d_merkblatt.pdf) von Beginn der Partnerarbeit an offen verwenden.
        - Formeln aus vorgegebenen Bausteinen zusammensetzen lassen.
        - Satzstarter anbieten:  
          > „`¬A` bedeutet …“  
          > „`A ∧ B` bedeutet …“  
          > „Die Formel verbietet …“
        - Vor der Eingabe in LogicTraffic die erwarteten Wahrheitswerte markieren lassen.

    === "Erweiterungen"

        - Mehrere sprachliche Formulierungen für dieselbe Formel finden lassen.
        - `¬(A ∧ B)` und `A → ¬B` in LogicTraffic vergleichen lassen, ohne die Äquivalenz bereits formal zu benennen.
        - Eigene Beispiele für korrekt geklammerte und falsch interpretierte Formeln entwickeln lassen.
        - Begründen lassen, weshalb `A ∨ B` auch dann wahr ist, wenn beide Variablen wahr sind.

### Phase 3 - Von Konflikten zur Formel

??? success "Ziele der Einheit"

    Die Lernenden können eine Verkehrssituation systematisch analysieren, einzelne Konflikte als sprachliche Sicherheitsregeln formulieren und daraus eine Gesamtformel entwickeln.

    Sie überprüfen ihre Formel in LogicTraffic und können fachlich begründen, welche Belegungen erlaubt bzw. ausgeschlossen werden.

??? example "Material"

    - [:memo: AB 4c – Von Konflikten zur Formel](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4c_kreuzung_logisch_steuern.pdf)
    - [:material-image-outline: MB 4d – Logik auf einen Blick](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4d_merkblatt.pdf)
    - LogicTraffic, **Situation 3**
    - Computer oder Tablet pro Zweiergruppe

??? info "Sozialformen"

    Überwiegend **Partnerarbeit**. Kurzer gemeinsamer Start zur Klärung des Arbeitswegs und eine gemeinsame Ergebnissicherung am Schluss.

    Im Tandem kann eine Person die Konflikte bzw. Formeln entwickeln, während die andere Person jede Teilformel in Alltagssprache zurückübersetzt und an der Wahrheitstabelle kontrolliert. Die Rollen werden zwischendurch gewechselt.

??? tip "benötigte Zeit"

    ca. **30 Minuten**

??? abstract "Verlaufsplanung"

    **1. Modellierungsweg transparent machen**

    Vor Beginn wird der Arbeitsweg sichtbar gemacht:

    **Kreuzung → Konflikte → Regeln in Worten → Teilformeln → Gesamtformel → Prüfung**

    Die Lernenden öffnen Situation 3 und bearbeiten [AB 4c](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4c_kreuzung_logisch_steuern.pdf) möglichst selbstständig.

    **2. Konflikte identifizieren**

    **Inputfrage:**

    > Welche Fahrspuren können tatsächlich miteinander kollidieren?

    In Situation 3 verlaufen `A` und `B` parallel, während `C` beide kreuzt.

    **Erwartete Konfliktpaare:**

    - `A` und `C`
    - `B` und `C`

    `A` und `B` bilden dagegen kein Konfliktpaar.

    **3. Konflikte zunächst sprachlich formulieren**

    Mögliche Regeln:

    > A und C dürfen nicht gleichzeitig Grün haben.

    > B und C dürfen nicht gleichzeitig Grün haben.

    **4. Teilformeln bilden**

    Aus den beiden Regeln entstehen beispielsweise:

    `¬(A ∧ C)`

    und

    `¬(B ∧ C)`

    **Inputfrage:**

    > Müssen nur eine oder beide Regeln gleichzeitig erfüllt sein?

    **Erwartete Antwort:** Beide Regeln müssen gelten.

    Daraus ergibt sich als Gesamtformel:

    `¬(A ∧ C) ∧ ¬(B ∧ C)`

    **5. Formel in LogicTraffic prüfen**

    Vor dem Test formulieren die Lernenden eine Erwartung:

    - Welche Belegungen müssen auf jeden Fall `sicher = 0` ergeben?
    - Welche Kombinationen sollten erlaubt bleiben?

    Erst danach wird die Formel eingegeben.

    Bei einer Abweichung wird nicht sofort eine neue Formel geraten. Stattdessen wird geprüft:

    1. Ist ein Konflikt vergessen worden?
    2. Wurde eine Negation falsch gesetzt?
    3. Fehlt eine Klammer?
    4. Wurden die Teilregeln korrekt miteinander verbunden?

    **6. Unterschiedliche korrekte Darstellungen kurz vergleichen**

    Im Plenum können zwei oder drei korrekte Lösungen gesammelt werden, beispielsweise:

    **Kollisionsverbote**

    `¬(A ∧ C) ∧ ¬(B ∧ C)`

    **Mit Implikationen**

    `(A → ¬C) ∧ (B → ¬C)`

    **Zusammengefasste Implikation**

    `C → (¬A ∧ ¬B)`

    Die Formeln werden an dieser Stelle noch nicht formal umgeformt. Entscheidend ist zunächst die Beobachtung:

    > Verschiedene Formeln können dieselben sicheren und unsicheren Zustände beschreiben.

    **7. Basisteil sichern**

    Zum Abschluss wird der Repräsentationswechsel gemeinsam festgehalten:

    **Verkehrssituation**

    → `A` und `C` dürfen nicht gleichzeitig Grün haben.

    **sprachliche Regel**

    → Mindestens eine der beiden Spuren muss Rot haben.

    **Formel**

    → `¬(A ∧ C)`

    **Wahrheitstabelle**

    → Die Formel ist genau dann `0`, wenn `A` und `C` gleichzeitig Grün haben.

    Das [Merkblatt 4d](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4d_merkblatt.pdf) dient anschliessend als Nachschlagehilfe.

??? note "Didaktische Hinweise"

    Die wichtigste Strategie dieser Phase ist die **Zerlegung des Gesamtproblems in einzelne Konflikte**. Die Lernenden sollen nicht versuchen, sofort eine grosse Formel zu erraten.

    Ebenso wichtig ist die Unterscheidung zwischen **sicher** und **optimal**. Eine Formel kann Kollisionen verhindern und trotzdem unnötig viele sichere Zustände ausschliessen. Deshalb sollten immer beide Fragen gestellt werden:

    - Verhindert die Formel alle Kollisionen?
    - Erlaubt sie gleichzeitig die eigentlich sicheren Kombinationen?

    Das Softwarefeedback ist formativ zu nutzen. Die Lernenden sollen erklären, **warum** eine Lösung stimmt oder nicht stimmt.

    Die kurze Gegenüberstellung verschiedener korrekter Formeln bereitet die optionale Vertiefung vor, ohne den Basisteil bereits mit Normalformen oder Umformungsregeln zu überladen.

??? bug "Differenzierung"

    === "Vereinfachungen"

        - Die beiden Konfliktpaare in der Kreuzung bereits farblich oder mit Pfeilen markieren.
        - Die Lernenden zuerst nur **eine** Teilregel vollständig formulieren lassen.
        - Ein Schema vorgeben:  
          `¬(___ ∧ ___)`
        - Die erste Teilformel gemeinsam entwickeln und nur die zweite selbstständig ergänzen lassen.
        - Das [Merkblatt 4d](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4d_merkblatt.pdf) offen verwenden.
        - Die Gesamtformel aus zwei vorgegebenen Teilformeln zusammensetzen lassen.

    === "Erweiterungen"

        - Mindestens zwei unterschiedliche korrekte Gesamtformeln entwickeln lassen.
        - Jede alternative Formel vollständig in Alltagssprache zurückübersetzen lassen.
        - Ohne Software vorhersagen lassen, ob zwei Formeln dieselbe Wahrheitstabelle erzeugen.
        - Eine möglichst gut lesbare und eine möglichst kurze Formel entwickeln und die beiden Varianten vergleichen.
        - Begründen lassen, weshalb eine lediglich „sichere“, aber zu restriktive Formel keine optimale Steuerung ist.

### Phase 4 - Anders gebaut, gleich gemeint

??? success "Ziele der Einheit"

    Die Lernenden erkennen, dass unterschiedlich aussehende Formeln dieselbe logische Funktion beschreiben können.

    Sie überprüfen logische Äquivalenz über Wahrheitstabellen, lernen ein De-Morgan-Muster kennen und können DNF und KNF anhand ihrer äusseren Struktur unterscheiden.

??? example "Material"

    - [:memo: AB 4e – Anders gebaut, gleich gemeint](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4e_knf_dnf.pdf)
    - [:material-image-outline: MB 4d – Logik auf einen Blick](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4d_merkblatt.pdf)
    - LogicTraffic, **Situation 4**
    - Computer oder Tablet pro Zweiergruppe

??? info "Sozialformen"

    **Partnerarbeit** mit kurzen gemeinsamen Zwischenstopps. Die Begriffe Äquivalenz, DNF und KNF werden im **Plenum** gesichert.

??? tip "benötigte Zeit"

    ca. **15 Minuten**

??? abstract "Verlaufsplanung"

    **1. Äquivalenz aus einer bekannten Sicherheitsregel entwickeln**

    Als Einstieg werden zwei Formeln verglichen:

    `¬(A ∧ C)`

    und

    `¬A ∨ ¬C`

    **Inputfragen:**

    > Wie lassen sich beide Formeln in Alltagssprache lesen?

    **Erwartete Antworten:**

    - `¬(A ∧ C)`: A und C dürfen nicht gleichzeitig Grün haben.
    - `¬A ∨ ¬C`: Mindestens eine der beiden Spuren muss Rot haben.

    > Erzeugen beide Formeln für jede Belegung denselben Wahrheitswert?

    Die Lernenden prüfen dies mit der Wahrheitstabelle.

    Wenn zwei Formeln bei jeder möglichen Belegung denselben Wahrheitswert erzeugen, sind sie **logisch äquivalent**:

    $$
    \neg(A \land C) \equiv \neg A \lor \neg C
    $$

    **2. De-Morgan-Muster benennen**

    Aus der Beobachtung wird das Muster festgehalten:

    $$
    \neg(A \land B) \equiv \neg A \lor \neg B
    $$

    Das zweite Gesetz kann ergänzend gezeigt werden:

    $$
    \neg(A \lor B) \equiv \neg A \land \neg B
    $$

    **3. Mit [AB 4e](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4e_knf_dnf.pdf) DNF und KNF entdecken**

    Für die weiteren Aufgaben wird Situation 4 verwendet.

    Die Lernenden untersuchen verschiedene Formeln und achten zunächst auf die **äussere Struktur**, nicht auf ein Umformungsverfahren.

    **DNF:**

    UND-Terme werden mit ODER verbunden.

    Beispiel:

    `(A ∧ ¬B) ∨ (¬A ∧ C)`

    **KNF:**

    ODER-Klauseln werden mit UND verbunden.

    Beispiel:

    `(¬A ∨ ¬C) ∧ (¬B ∨ ¬C)`

    **Inputfragen:**

    > Was ist bei einer DNF der äussere Verknüpfungsoperator?

    **Erwartete Antwort:** ODER (`∨`).

    > Was ist bei einer KNF der äussere Verknüpfungsoperator?

    **Erwartete Antwort:** UND (`∧`).

    > Beschreiben DNF und KNF grundsätzlich andere Sicherheitsfunktionen?

    **Erwartete Antwort:** Nein. Es sind unterschiedliche Formen, in denen dieselbe logische Funktion dargestellt werden kann.

??? note "Didaktische Hinweise"

    Äquivalenz sollte zunächst **beobachtet und überprüft** werden, bevor Umformungsregeln formalisiert werden. Dadurch bleibt der Zusammenhang mit der bereits bekannten Wahrheitstabelle erhalten.

    DNF und KNF werden in dieser Phase bewusst als **Formen** eingeführt. Die Lernenden müssen noch kein allgemeines Verfahren zur Umformung beliebiger Formeln beherrschen.

    Die De-Morgan-Regeln sind hier eine Brücke zwischen zwei äquivalenten Schreibweisen. Sie sollen nicht zu einer isolierten Sammlung von Rechenregeln werden.

??? bug "Differenzierung"

    === "Vereinfachungen"

        - Den äussersten Operator einer Formel zuerst markieren lassen.
        - DNF- und KNF-Beispiele sortieren lassen, bevor eigene Begründungen verlangt werden.
        - Nur das erste De-Morgan-Gesetz verwenden.
        - Äquivalenz immer zuerst mit einer vollständigen Wahrheitstabelle überprüfen.
        - Satzstarter anbieten:  
          > „Die Formel ist eine DNF, weil …“  
          > „Die Formeln sind äquivalent, weil …“

    === "Erweiterungen"

        - Das zweite De-Morgan-Gesetz selbstständig mit einer Wahrheitstabelle überprüfen lassen.
        - Eine einfache Formel gezielt in eine äquivalente Form umschreiben lassen.
        - Eine DNF und eine KNF für dieselbe Funktion suchen und vergleichen lassen.
        - Äquivalenz zunächst ohne LogicTraffic begründen und danach erst kontrollieren.

### Phase 5 - Von der Wahrheitstabelle zur Formel

??? success "Ziele der Einheit"

    Die Lernenden verstehen, dass eine Formel nicht immer erraten oder durch geschicktes Umformen gefunden werden muss.

    Sie können nachvollziehen, wie KDNF bzw. KKNF nach einem festen Verfahren direkt aus einer Wahrheitstabelle konstruiert werden und erkennen den Nutzen dieser Formen als systematischen Zwischenschritt.

??? example "Material"

    - [:memo: AB 4f – Von der Wahrheitstabelle zur Formel](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4f_kknf_kdnf.pdf)
    - LogicTraffic, **Situation 4**
    - Computer oder Tablet pro Zweiergruppe
    - optional: [:material-image-outline: MB 4d – Logik auf einen Blick](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4d_merkblatt.pdf)

??? info "Sozialformen"

    **Partnerarbeit** mit einem kurzen gemeinsamen Beispiel zu Beginn. Die Lernenden ordnen einzelne Tabellenzeilen den zugehörigen Termen bzw. Klauseln zu.

??? tip "benötigte Zeit"

    ca. **15 Minuten**

??? abstract "Verlaufsplanung"

    **1. Ausgangspunkt: eine bereits verstandene Wahrheitstabelle**

    Die Lehrperson zeigt eine Wahrheitstabelle aus Situation 4.

    **Leitfrage:**

    > Können wir aus der Tabelle nach einem festen Verfahren eine Formel bauen, ohne zuerst eine kurze Lösung erraten zu müssen?

    **2. KDNF aus den Zeilen mit `sicher = 1`**

    Für jede Zeile mit `sicher = 1` wird ein vollständiger UND-Term gebildet.

    Beispiel für eine Belegung:

    | A | B | C | sicher |
    | :---: | :---: | :---: | :---: |
    | 1 | 0 | 1 | 1 |

    Daraus entsteht:

    `A ∧ ¬B ∧ C`

    **Regel:**

    - Wert `1` → Variable wird nicht negiert.
    - Wert `0` → Variable wird negiert.
    - Alle Literale der Zeile werden mit `∧` verbunden.
    - Die vollständigen Zeilenterme mit `sicher = 1` werden anschliessend mit `∨` verbunden.

    **Inputfrage:**

    > Warum beschreibt ein vollständiger UND-Term genau eine Tabellenzeile?

    **Erwartete Antwort:** Weil für jede Variable genau festgelegt ist, ob sie `0` oder `1` sein muss.

    **3. KKNF aus den Zeilen mit `sicher = 0`**

    Für jede Zeile mit `sicher = 0` wird eine ODER-Klausel gebildet, die **genau diese Belegung ausschliesst**.

    Für eine Zeile gilt deshalb:

    - Tabellenwert `1` → Variable wird in der Klausel negiert.
    - Tabellenwert `0` → Variable wird in der Klausel nicht negiert.
    - Die Literale werden mit `∨` verbunden.
    - Die vollständigen Klauseln werden mit `∧` verbunden.

    **Inputfrage:**

    > Warum müssen die Vorzeichen bei der KKNF gegenüber der Tabellenzeile gerade so gewählt werden?

    **Erwartete Antwort:** Damit die Klausel genau bei dieser einen unerwünschten Belegung falsch wird.

    **4. [AB 4f](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4f_kknf_kdnf.pdf) bearbeiten**

    Die Lernenden ordnen Tabellenzeilen zu Termen bzw. Klauseln und verfolgen in LogicTraffic, wie eine kanonische Form aus der Tabelle entsteht.

    **5. Rolle der kanonischen Formen reflektieren**

    **Leitfrage:**

    > Was ist der Vorteil und was ist der Nachteil dieses Verfahrens?

    **Erwartete Antworten:**

    **Vorteil:**
    - systematisch;
    - vollständig;
    - direkt aus der Wahrheitstabelle erzeugbar;
    - eine Formel muss nicht erraten werden.

    **Nachteil:**
    - die Formel kann sehr lang werden;
    - die eigentliche Verkehrsbedeutung ist oft schwerer zu erkennen.

    Als möglicher Lösungsweg wird festgehalten:

    **Wahrheitstabelle → KDNF/KKNF → vereinfachte bzw. gut lesbare Formel**

??? note "Didaktische Hinweise"

    KDNF und KKNF sind in diesem Baustein bewusst **Scaffolds** und nicht das zentrale Endziel. Der Schwerpunkt der gesamten Reihe bleibt auf DNF/KNF, Äquivalenz, Modellierung und dem Wechsel zwischen Repräsentationen.

    Das mechanische Verfahren kann Lernenden Sicherheit geben, die beim direkten Formulieren einer Formel Schwierigkeiten haben. Für stärkere Lernende darf der direkte Weg von der Verkehrssituation zu einer kompakten Formel weiterhin gleichwertig bestehen bleiben.

    Wichtig ist, dass die Lernenden den Zusammenhang zwischen **einer Tabellenzeile** und **einem vollständigen Term bzw. einer vollständigen Klausel** verstehen. Reines Kopieren einer automatisch erzeugten Formel reicht nicht aus.

??? bug "Differenzierung"

    === "Vereinfachungen"

        - Nur KDNF bearbeiten und KKNF zunächst weglassen.
        - Eine Tabellenzeile und den zugehörigen Term vollständig vormachen.
        - In den nächsten Termen bereits einzelne Literale vorgeben.
        - Die relevanten Zeilen mit `sicher = 1` bzw. `sicher = 0` markieren lassen.
        - Eine Checkliste für das Verfahren bereitstellen.

    === "Erweiterungen"

        - KDNF und KKNF für dieselbe Wahrheitstabelle vollständig gegenüberstellen.
        - Für eine beliebige Tabellenzeile ohne Software den zugehörigen KDNF-Term und die KKNF-Klausel bilden.
        - Begründen lassen, warum beide kanonischen Formen dieselbe Funktion beschreiben.
        - Eine kanonische Formel schrittweise vereinfachen und jede Vereinfachung auf Äquivalenz prüfen.

### Phase 6 - Lang, kurz, gleichwertig?

??? success "Ziele der Einheit"

    Die Lernenden vergleichen verschiedene Formeln, die dieselbe logische Funktion beschreiben, und beurteilen deren Eignung nach nachvollziehbaren Kriterien.

    Sie unterscheiden dabei zwischen **logischer Korrektheit** und Eigenschaften wie Länge, Lesbarkeit, systematischer Erzeugbarkeit oder Nähe zur Verkehrssituation.

??? example "Material"

    - [:memo: AB 4g – Lang, kurz, gleichwertig?](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4g_vergleich_gleichwertigkeit.pdf)
    - LogicTraffic, **Situation 4**
    - Computer oder Tablet pro Zweiergruppe
    - Ergebnisse aus [AB 4e](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4e_knf_dnf.pdf) und [AB 4f](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4f_kknf_kdnf.pdf)

??? info "Sozialformen"

    **Partnerarbeit** zum Vergleichen und Bewerten der Formeln, anschliessend kurze **Plenumsdiskussion** zur Frage, ob es eine „beste“ Darstellung gibt.

??? tip "benötigte Zeit"

    ca. **15 Minuten**

??? abstract "Verlaufsplanung"

    **1. Mehrere Darstellungen nebeneinanderstellen**

    Verglichen werden – soweit vorhanden – beispielsweise:

    - eine selbst entwickelte freie Formel;
    - eine DNF;
    - eine KNF;
    - eine KDNF oder KKNF;
    - eine vereinfachte Darstellung aus LogicTraffic.

    **2. Zuerst die Äquivalenz prüfen**

    Bevor über Länge oder Schönheit gesprochen wird, klären die Lernenden:

    > Beschreiben die Formeln tatsächlich dieselbe Funktion?

    Als Kriterium gilt:

    > Zwei Formeln sind logisch äquivalent, wenn sie bei **jeder** Belegung denselben Wahrheitswert erzeugen.

    Die Wahrheitstabelle dient als Prüfinstrument.

    **3. [AB 4g](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4g_vergleich_gleichwertigkeit.pdf) bearbeiten**

    Die Formeln werden nach mehreren Kriterien beurteilt:

    - Ist die Formel korrekt?
    - Wie lang ist sie?
    - Kann man ihre Verkehrsbedeutung gut erkennen?
    - Lässt sie sich systematisch aus der Wahrheitstabelle erzeugen?
    - Wie leicht lässt sie sich erklären?
    - Für welchen Zweck ist sie besonders geeignet?

    **Inputfrage:**

    > Ist die kürzeste Formel automatisch die beste Formel?

    **Erwartete Antwort:** Nein. Das hängt vom Verwendungszweck ab.

    Eine kurze Formel kann leicht lesbar sein, während eine kanonische Formel den systematischen Bezug zur vollständigen Wahrheitstabelle besonders deutlich macht.

    **4. Gemeinsame Sicherung**

    Als zentrale Erkenntnis wird festgehalten:

    > Logisch äquivalente Formeln können sehr unterschiedlich aussehen.

    > Welche Darstellung besonders geeignet ist, hängt davon ab, wofür sie verwendet wird.

??? note "Didaktische Hinweise"

    Diese Phase soll keine Suche nach einer vermeintlich einzig richtigen oder einzig „schönen“ Formel werden.

    Die Lernenden sollen zwei Ebenen konsequent trennen:

    **1. Semantik:** Beschreibt die Formel die richtige Funktion?  
    **2. Darstellung:** Wie geeignet ist diese Form für einen bestimmten Zweck?

    Gerade sehr lange KDNF- oder KKNF-Formeln sind didaktisch wertvoll, weil sichtbar wird, dass Länge kein Kriterium für logische Korrektheit ist.

    Gleichzeitig bietet der Vergleich Gelegenheit für anspruchsvollere Denkprozesse: erklären, begründen, beurteilen und zwischen Darstellungen wechseln.

??? bug "Differenzierung"

    === "Vereinfachungen"

        - Nur zwei Formeln miteinander vergleichen.
        - Eine Kriterienliste mit Ankreuzfeldern verwenden.
        - Die Äquivalenz bereits vorgeben und nur Lesbarkeit und Aufbau untersuchen lassen.
        - Jede Formel zuerst vollständig in Alltagssprache übersetzen lassen.

    === "Erweiterungen"

        - Die Äquivalenz zweier Formeln ohne LogicTraffic begründen.
        - Eine möglichst kurze äquivalente Formel entwickeln.
        - Zwei Formeln gezielt für unterschiedliche Zwecke empfehlen und die Wahl begründen.
        - Untersuchen, ob eine Vereinfachung die Verkehrsbedeutung leichter oder schwerer erkennbar macht.
        - Eine eigene Bewertungsdimension ergänzen und begründen.

### Phase 7 - Transfer – Situation 10

??? success "Ziele der Einheit"

    Die Lernenden übertragen den vollständigen Modellierungsweg auf eine komplexere Kreuzung mit fünf Variablen und 32 möglichen Belegungen.

    Sie analysieren die Konfliktstruktur, entwickeln eine Gesamtformel, überprüfen diese systematisch und reflektieren, welchen Vorteil die kompakte Formel gegenüber der vollständigen Wahrheitstabelle bietet.

??? example "Material"

    - [:memo: AB 4h – Transferaufgabe](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4h_transfer.pdf)
    - LogicTraffic, **Situation 10**
    - Computer oder Tablet pro Zweiergruppe
    - [:material-image-outline: MB 4d – Logik auf einen Blick](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4d_merkblatt.pdf)
    - bei Bedarf [AB 4f](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4f_kknf_kdnf.pdf) als Hilfestellung für den systematischen Weg über die Wahrheitstabelle

??? info "Sozialformen"

    Überwiegend **Partnerarbeit**. Die Paare arbeiten möglichst selbstständig und vergleichen ihre Lösungsstrategien zum Schluss mit einem anderen Tandem oder im Plenum.

??? tip "benötigte Zeit"

    ca. **20–30 Minuten**

??? abstract "Verlaufsplanung"

    **1. Ausgangslage klären**

    Die Lernenden öffnen Situation 10.

    Die Kreuzung besitzt fünf Variablen:

    `A`, `B`, `C`, `D` und `E`.

    Die vollständige Wahrheitstabelle enthält:

    $$
    2^5 = 32
    $$

    Zeilen.

    **Leitfrage:**

    > Wie können wir diese Kreuzung steuern, ohne 32 Tabellenzeilen einzeln als Regel aufzuschreiben?

    **2. Konfliktstruktur systematisch analysieren**

    Die Lernenden markieren bzw. notieren alle Fahrspurpaare, bei denen tatsächlich eine Kollision möglich ist.

    Dabei steht nicht das blosse Formulieren der immer gleichen Aussage „X und Y dürfen nicht gleichzeitig Grün haben“ im Zentrum, sondern die **vollständige und begründete Analyse der Kreuzung**:

    - Welche Paare bilden echte Konflikte?
    - Welche Paare können gleichzeitig Grün haben?
    - Wurde ein Konflikt vergessen?
    - Wurde ein Paar fälschlich als Konflikt eingestuft?

    **3. Teilregeln entwickeln und bündeln**

    Für jedes echte Konfliktpaar kann zunächst eine Teilregel der Form

    `¬(X ∧ Y)`

    oder eine logisch äquivalente Form entwickelt werden.

    Anschliessend werden die Teilregeln so verbunden, dass **alle** Sicherheitsbedingungen gleichzeitig gelten.

    **Inputfrage:**

    > Mit welchem Operator müssen unabhängige Sicherheitsbedingungen verbunden werden, wenn alle gleichzeitig erfüllt sein müssen?

    **Erwartete Antwort:** Mit UND (`∧`).

    **4. Vor dem Test eine Erwartung formulieren**

    Bevor die Gesamtformel in LogicTraffic eingegeben wird, wählen die Lernenden mehrere charakteristische Belegungen aus:

    - mindestens eine offensichtlich kollidierende Belegung;
    - mindestens eine offensichtlich sichere Belegung;
    - wenn möglich eine Belegung mit mehreren gleichzeitig grünen, aber nicht kollidierenden Spuren.

    Für jede Belegung wird vorhergesagt, ob `sicher = 0` oder `sicher = 1` gelten muss.

    **5. Gesamtformel überprüfen und überarbeiten**

    Die Formel wird in LogicTraffic getestet.

    Bei Abweichungen erfolgt die Fehlersuche systematisch:

    1. Konfliktanalyse prüfen.
    2. Teilformeln prüfen.
    3. Klammern und Negationen prüfen.
    4. Verbindung der Teilformeln prüfen.
    5. Erst danach die Formel verändern.

    **6. Alternativer systematischer Weg bei Bedarf**

    Falls der direkte Weg zur Gesamtformel schwierig ist, kann die Wahrheitstabelle als Scaffold eingesetzt werden:

    **Wahrheitstabelle → KDNF oder KKNF → Struktur untersuchen → kompaktere Formel**

    Die kanonische Form dient dabei bewusst als **Zwischenschritt**, nicht als verpflichtendes Endprodukt.

    **7. Transfer reflektieren**

    **Abschlussfrage:**

    > Was können wir mit einer Formel ausdrücken, wofür wir in Baustein 3 noch 32 Tabellenzeilen benötigt haben?

    **Erwartete Antworten:**

    - Die Konfliktstruktur kann mit wenigen Regeln beschrieben werden.
    - Die Formel ist kompakter als die vollständige Tabelle.
    - Die Wahrheitstabelle bleibt nützlich, um die Formel zu kontrollieren.
    - Eine komplexe Aufgabe kann in kleinere Konfliktbedingungen zerlegt und anschliessend wieder zusammengesetzt werden.

??? note "Didaktische Hinweise"

    Der Transfer sollte nicht zu einer repetitiven Aufgabe werden, in der für bereits vorgegebene Spurpaare nur immer wieder `¬(X ∧ Y)` eingesetzt wird. Der eigentliche Anspruch liegt in der **Modellierung des Gesamtsystems**:

    **analysieren → relevante Konflikte auswählen → Teilprobleme formulieren → Gesamtregel konstruieren → gezielt überprüfen**

    Die Lehrperson sollte deshalb möglichst nicht alle Konfliktpaare vorgeben. Unterstützt wird nur so weit, wie es für den jeweiligen Lernstand notwendig ist.

    Die 32-zeilige Wahrheitstabelle erhält im Transfer eine wichtige neue Funktion: Sie ist nicht mehr der primäre Lösungsweg, sondern ein mächtiges Instrument zur **Verifikation**.

    Für die Auswertung lohnt es sich, unterschiedliche korrekte Formeln nebeneinanderzustellen. Dadurch wird sichtbar, dass dieselbe Sicherheitsfunktion verschieden modelliert werden kann.

??? bug "Differenzierung"

    === "Vereinfachungen"

        - Das erste Konfliktpaar gemeinsam identifizieren und formulieren.
        - Eine teilweise ausgefüllte Konfliktliste bereitstellen.
        - Die Kreuzung schrittweise untersuchen: zuerst nur drei, danach alle fünf Variablen berücksichtigen.
        - Die Struktur der Gesamtformel vorgeben:  
          `Teilregel 1 ∧ Teilregel 2 ∧ …`
        - Das [Merkblatt 4d](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4d_merkblatt.pdf) offen verwenden.
        - Bei Bedarf über [AB 4f](https://github.com/salomegolden/logictraffic/releases/download/arbeitsbl%C3%A4tter/4f_kknf_kdnf.pdf) und eine kanonische Form von der Wahrheitstabelle zur Formel gelangen.

    === "Erweiterungen"

        - Mehrere logisch äquivalente Gesamtformeln entwickeln.
        - Eine möglichst kompakte Formel suchen und mit einer konfliktsweisen Darstellung vergleichen.
        - Eine Lösung ohne LogicTraffic begründen und erst danach überprüfen.
        - Die Äquivalenz zweier Lösungen anhand ausgewählter Belegungen und anschliessend vollständig über die Wahrheitstabelle untersuchen.
        - Begründen, welche Darstellung sich für Menschen und welche sich für ein systematisches Erzeugungsverfahren besonders gut eignet.

## Abschluss des Bausteins

Am Ende des Bausteins haben die Lernenden dieselbe grundlegende Sicherheitsidee auf mehreren Ebenen betrachtet:

1. **konkret bzw. visuell** als Verkehrssituation;
2. **sprachlich** als Sicherheitsregel;
3. **tabellarisch** als Wahrheitstabelle;
4. **symbolisch** als aussagenlogische Formel.

!!! success "Von der Kreuzung zur Logik"

    Eine reale Problemsituation kann schrittweise analysiert, abstrahiert und formal beschrieben werden.

    Wahrheitstabellen und Formeln stehen dabei nicht in Konkurrenz zueinander:

    - Die **Wahrheitstabelle** beschreibt alle möglichen Zustände vollständig.
    - Die **Formel** beschreibt dieselbe logische Funktion kompakt.
    - Der Wechsel zwischen beiden Darstellungen ermöglicht es, Lösungen zu entwickeln, zu überprüfen und miteinander zu vergleichen.