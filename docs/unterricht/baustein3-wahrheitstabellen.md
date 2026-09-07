# Baustein 3 – Wahrheitstabellen

In diesem Baustein lernen die Lernenden, Wahrheitstabellen nicht nur in LogicTraffic zu lesen, sondern selbstständig und systematisch aufzubauen.

Ausgangspunkt ist eine einfache Kreuzung mit zwei Fahrspuren. Die Lernenden klären zunächst, was eine Wahrheitstabelle überhaupt darstellt und wie die Werte `0` und `1` in den Variablenspalten sowie in der Spalte `sicher` zu lesen sind. Anschliessend entwickeln sie für drei Variablen ein systematisches Verfahren, mit dem alle möglichen Belegungen vollständig und ohne Wiederholungen erzeugt werden können.

Zum Abschluss prüfen sie ihr Verständnis an einer fehlerhaften Wahrheitstabelle. Dabei unterscheiden sie zwischen **strukturellen Fehlern** – etwa fehlenden oder doppelten Kombinationen – und **inhaltlichen Fehlern** bei der Beurteilung der Sicherheit.

Die Progression des Bausteins lautet:

**Verkehrssituation → einzelne Ampelstellung → Tabellenzeile → vollständige Wahrheitstabelle → Systematik $2^n$ → Fehleranalyse → Skalierungsproblem**

Damit bereitet Baustein 3 den Übergang zu [Baustein 4 – Logische Formeln](baustein4-boolesche-algebra.md) vor: Wahrheitstabellen bilden alle Zustände vollständig ab, werden mit wachsender Variablenzahl jedoch schnell sehr umfangreich.

!!! abstract "Auf einen Blick"

    **:stopwatch: Dauer:**  
    ca. **50–60 Minuten**

    **:busts_in_silhouette: Sozialform:**  
    Plenum, Partnerarbeit und kurze Einzelphasen

    **:computer: Computer:**  
    Ein Computer oder Tablet mit LogicTraffic pro Zweiergruppe

    **:brain: Vorwissen:**  
    - [Baustein 2 – LogicTraffic kennenlernen](baustein2-logictraffic.md) wurde idealerweise abgeschlossen.
    - Die Lernenden kennen Variablen als Bezeichnungen für Fahrspuren.
    - `0 = Rot` und `1 = Grün` sind bei den Fahrspuren bekannt.
    - Die Lernenden können eine konkrete Ampelstellung einer Darstellung in LogicTraffic zuordnen.
    - Die Bedeutung der Spalte `sicher` ist grundsätzlich bekannt.

    **:package: Material:**  
    LogicTraffic, Computer oder Tablets, Beamer oder Präsentationsbildschirm sowie die Arbeitsblätter zu Baustein 3

??? note "Downloads zu Baustein 3"

    - [:memo: 3a – Wahrheitstabellen verstehen](https://github.com/salomegolden/logictraffic/releases/download/ab3_v1/3a_wahrheitstabellen_verstehen.pdf)
    - [:memo: 3b – Wahrheitstabellen systematisch erstellen](https://github.com/salomegolden/logictraffic/releases/download/ab3_v1/3b_wahrheitstabellen_systematisch_erstellen.pdf)
    - [:memo: 3c – Herausforderung: Fehler finden](https://github.com/salomegolden/logictraffic/releases/download/ab3_v1/3c_herausforderung_fehler.pdf)

## Lernziele

Die Lernenden können …

- eine Wahrheitstabelle als vollständige Darstellung aller möglichen Kombinationen von Variablenwerten erklären;
- eine konkrete Ampelstellung einer Tabellenzeile zuordnen und umgekehrt;
- zwischen den Werten der Fahrspuren (`0 = Rot`, `1 = Grün`) und den Werten der Spalte `sicher` unterscheiden;
- für zwei und drei Variablen alle möglichen Belegungen systematisch und lückenlos aufschreiben;
- ein Ordnungsmuster zum Erzeugen aller Kombinationen beschreiben;
- erklären, warum bei $n$ Variablen $2^n$ mögliche Belegungen entstehen;
- für jede Ampelkombination begründet entscheiden, ob die Verkehrssituation sicher oder unsicher ist;
- fehlende, doppelte und inhaltlich falsch bewertete Zeilen in einer Wahrheitstabelle erkennen und korrigieren;
- erkennen, dass Wahrheitstabellen bei zunehmender Anzahl von Variablen schnell sehr umfangreich werden;
- daraus die Notwendigkeit einer kompakteren Darstellung ableiten.

## Vorbereitung

- LogicTraffic auf allen Geräten öffnen und die Funktionsfähigkeit prüfen.
- **Situation 2** für Phase 1 bereithalten.
- **Situation 3** für Phase 2 bereithalten.
- **Situation 4** für Phase 3 bereithalten.
- Die Arbeitsblätter 3a, 3b und 3c ausdrucken oder digital bereitstellen.
- Wenn möglich, Wahrheitstabellen zunächst **ausserhalb von LogicTraffic** bearbeiten lassen. Die Lernumgebung wird anschliessend als Kontroll- und Rückmeldewerkzeug eingesetzt.
- Für den Abschluss eine Situation mit fünf Variablen oder die entsprechende Zeilenanzahl `32` bereithalten.

??? tip "Abgrenzung zu Baustein 2"

    In Baustein 2 haben die Lernenden die Wahrheitstabelle bereits als Darstellung in LogicTraffic kennengelernt.

    In Baustein 3 steht eine neue Frage im Zentrum:

    > **Wie können wir selbst alle möglichen Ampelzustände vollständig und systematisch aufschreiben, ohne eine Kombination zu vergessen?**

    Der Schwerpunkt liegt deshalb nicht mehr auf der Bedienung der Lernumgebung, sondern auf der **Struktur, Vollständigkeit und Bedeutung einer Wahrheitstabelle**.

??? info "Fachlicher Hintergrund – Wahrheitstabellen"

    Eine Wahrheitstabelle enthält alle möglichen Belegungen der verwendeten Variablen.

    In LogicTraffic besitzt jede Fahrspur genau zwei Zustände:

    - `0` = Rot
    - `1` = Grün

    Bei $n$ Variablen entstehen deshalb:

    $$
    2^n
    $$

    verschiedene Belegungen.

    | Anzahl Variablen | Anzahl möglicher Zustände |
    | ---: | ---: |
    | 1 | $2^1 = 2$ |
    | 2 | $2^2 = 4$ |
    | 3 | $2^3 = 8$ |
    | 4 | $2^4 = 16$ |
    | 5 | $2^5 = 32$ |
    | 10 | $2^{10} = 1024$ |

    Eine systematische Reihenfolge kann wie beim binären Zählen aufgebaut werden.

    Für drei Variablen lautet eine mögliche Reihenfolge:

    `000`, `001`, `010`, `011`, `100`, `101`, `110`, `111`

??? warning "Zwei verschiedene Bedeutungen von 0 und 1"

    In LogicTraffic werden `0` und `1` auf zwei verschiedenen Ebenen verwendet.

    **Bei den Fahrspuren:**

    - `0` = Die Ampel ist rot.
    - `1` = Die Ampel ist grün.

    **In der Spalte `sicher`:**

    - `0` = Die Kombination ist unsicher.
    - `1` = Die Kombination ist sicher.

    Diese Bedeutungen sollten sprachlich konsequent getrennt werden.

    Statt nur zu sagen

    > „Hier steht eine Eins.“

    sollte möglichst präzisiert werden:

    > „Bei Spur A bedeutet `1`, dass die Ampel Grün zeigt.“

    bzw.

    > „In der Spalte `sicher` bedeutet `1`, dass diese Kombination kollisionsfrei ist.“

## Unterrichtsablauf – Überblick

| Phase | Schwerpunkt | Material | Richtwert |
| --- | --- | --- | ---: |
| **1. Wahrheitstabellen verstehen** | Einzelne Ampelstellungen lesen, Tabellenzeilen deuten und die vollständige Tabelle für zwei Variablen verstehen | **AB 3a**, Situation 2 | ca. 15 Min. |
| **2. Wahrheitstabellen systematisch erstellen** | Drei Variablen vollständig erfassen, Ordnungsmuster erkennen und $2^n$ herleiten | **AB 3b**, Situation 3 | ca. 25 Min. |
| **3. Herausforderung – Fehler finden** | Fehlende, doppelte und falsch bewertete Zeilen diagnostizieren; Wissen sichern und Skalierungsproblem reflektieren | **AB 3c**, Situation 4 | ca. 15–20 Min. |

Die drei Phasen bilden gemeinsam den vollständigen Baustein. Bei knappem Zeitbudget kann Phase 3 als Vertiefung eingesetzt werden; die inhaltliche Brücke zu Baustein 4 sollte jedoch in jedem Fall am Ende kurz gesichert werden.

## Durchführung

### Phase 1 - Wahrheitstabellen verstehen

??? success "Ziele der Einheit"

    Die Lernenden verstehen, dass **jede Tabellenzeile genau eine mögliche Ampelstellung** beschreibt.

    Sie können die Werte der Fahrspuren korrekt als Rot bzw. Grün lesen, den Wert der Spalte `sicher` davon unterscheiden und erklären, weshalb eine Wahrheitstabelle alle möglichen Zustände enthalten muss.

??? example "Material"

    - [:memo: AB 3a – Wahrheitstabellen verstehen](https://github.com/salomegolden/logictraffic/releases/download/ab3_v1/3a_wahrheitstabellen_verstehen.pdf)
    - LogicTraffic, **Situation 2**
    - Computer oder Tablet pro Zweiergruppe
    - Beamer oder Präsentationsbildschirm

??? info "Sozialformen"

    Kurzer Einstieg im **Plenum**, anschliessend **Partnerarbeit** mit AB 3a. Die Ergebnisse werden am Ende gemeinsam gesichert.

    Im Tandem kann jeweils eine Person eine Tabellenzeile lesen, während die andere Person die entsprechende Ampelstellung beschreibt oder in LogicTraffic einstellt. Danach werden die Rollen gewechselt.

??? tip "benötigte Zeit"

    ca. **15 Minuten**

??? abstract "Verlaufsplanung"

    **1. Eine konkrete Ampelstellung als Ausgangspunkt**

    Die Lehrperson öffnet Situation 2 und stellt eine konkrete Ampelkombination ein.

    **Inputfragen:**

    > Welche Spur ist Grün, welche ist Rot?

    > Wie könnten wir genau diese Ampelstellung mit `0` und `1` aufschreiben?

    Die Lernenden ordnen die konkrete Situation einer Tabellenzeile zu.

    Dabei wird nochmals gesichert:

    - `0` bei einer Fahrspur bedeutet **Rot**.
    - `1` bei einer Fahrspur bedeutet **Grün**.

    **2. Von einer Zeile zur Tabelle**

    Die Lehrperson zeigt bzw. thematisiert eine zweite Ampelstellung.

    **Leitfrage:**

    > Reichen diese beiden Zustände schon aus, um alle Möglichkeiten zu beschreiben?

    **Erwartete Antwort:** Nein. Beide Ampeln können jeweils Rot oder Grün sein.

    Bei zwei Variablen `A` und `B` gibt es insgesamt:

    $$
    2 \cdot 2 = 4 = 2^2
    $$

    Kombinationen.

    Eine vollständige Tabelle enthält:

    | `A` | `B` |
    | :---: | :---: |
    | `0` | `0` |
    | `0` | `1` |
    | `1` | `0` |
    | `1` | `1` |

    **3. AB 3a bearbeiten**

    Die Lernenden lesen und ergänzen die Tabelle auf AB 3a.

    Dabei sollen sie wiederholt zwischen drei Darstellungen wechseln:

    **Verkehrssituation**

    ↔ **Ampelstellung mit Rot/Grün**

    ↔ **Tabellenzeile mit `0` und `1`**

    Anschliessend wird die Spalte `sicher` betrachtet.

    **Inputfrage:**

    > Bedeutet `1` in der Spalte `sicher` ebenfalls, dass eine Ampel Grün ist?

    **Erwartete Antwort:** Nein.

    Gemeinsam wird unterschieden:

    **Variablenspalten:**

    - `0` = Rot
    - `1` = Grün

    **Spalte `sicher`:**

    - `0` = unsicher
    - `1` = sicher

    **4. Sicherheit beurteilen**

    Die Lernenden beurteilen die Kombinationen zunächst anhand der Kreuzung.

    Hilfsfragen:

    - Welche Spuren sind gleichzeitig Grün?
    - Schneiden sich deren Fahrwege?
    - Kann eine Kollision entstehen?
    - Welchen Wert erhält deshalb `sicher`?

    Erst danach wird mit LogicTraffic kontrolliert.

    **5. Zentrale Erkenntnis sichern**

    **Abschlussfrage:**

    > Was muss eine Wahrheitstabelle enthalten, damit sie wirklich vollständig ist?

    **Erwartete Antwort:**

    > Jede mögliche Kombination der Variablenwerte muss genau einmal vorkommen.

??? note "Didaktische Hinweise"

    Die zentrale Herausforderung dieser Phase ist weniger das Erstellen der Tabelle als das **Verstehen der Repräsentation**.

    Besonders wichtig ist die konsequente Trennung der beiden Bedeutungen von `0` und `1`. Lernende können sonst fälschlicherweise annehmen, dass `sicher = 0` bedeute, eine bestimmte Ampel sei Rot.

    Ein weiterer typischer Stolperstein ist die Kombination, bei der **alle Ampeln Rot** sind. Diese ist möglicherweise ineffizient, aber nicht automatisch unsicher. In diesem Baustein bedeutet `sicher` ausschliesslich:

    > Bei dieser Ampelstellung kann keine Kollision entstehen.

    LogicTraffic sollte auch hier erst **nach einer eigenen Begründung** verwendet werden.

??? bug "Differenzierung"

    === "Vereinfachungen"

        - Nur zwei Variablen verwenden.
        - Rot und Grün zusätzlich mit farbigen Punkten oder Ampelsymbolen markieren.
        - Satzstarter anbieten:  
          > „Bei `A = 1` ist …“  
          > „Die Zeile `01` bedeutet …“  
          > „`sicher = 1` bedeutet …“
        - Eine Tabellenzeile gemeinsam vollständig deuten.
        - Die Lernenden die Ampelstellung zuerst in LogicTraffic einstellen und erst danach die Zeile notieren lassen.

    === "Erweiterungen"

        - Die Lernenden selbst eine Tabellenzeile vorgeben und vom Partner in LogicTraffic darstellen lassen.
        - Begründen lassen, weshalb bei zwei Variablen genau vier und nicht beispielsweise sechs Kombinationen möglich sind.
        - Eine unvollständige Zweivariablen-Tabelle vorgeben und die fehlende Kombination ohne Ausprobieren bestimmen lassen.
        - Bereits eine Vermutung formulieren lassen, wie viele Kombinationen bei drei Variablen entstehen müssten.

### Phase 2 - Wahrheitstabellen systematisch erstellen

??? success "Ziele der Einheit"

    Die Lernenden können eine vollständige Wahrheitstabelle mit drei Variablen **selbstständig und nach einem erkennbaren Muster** aufbauen.

    Sie erklären, weshalb bei drei Variablen acht Kombinationen entstehen, leiten daraus die allgemeine Regel $2^n$ ab und erkennen, dass die Zeilenzahl mit jeder zusätzlichen Variable stark wächst.

??? example "Material"

    - [:memo: AB 3b – Wahrheitstabellen systematisch erstellen](https://github.com/salomegolden/logictraffic/releases/download/ab3_v1/3b_wahrheitstabellen_systematisch_erstellen.pdf)
    - LogicTraffic, **Situation 3**
    - Computer oder Tablet pro Zweiergruppe
    - Beamer oder Präsentationsbildschirm
    - optional: Notizpapier für einen ersten eigenen Tabellenentwurf

??? info "Sozialformen"

    Überwiegend **Partnerarbeit**. Der Einstieg und die Herleitung von $2^n$ werden kurz im **Plenum** gesichert.

    Die Lernenden sollen zuerst selbst eine Ordnungsidee entwickeln. Erst danach werden verschiedene Strategien verglichen und das binär geordnete Muster als zuverlässige Möglichkeit festgehalten.

??? tip "benötigte Zeit"

    ca. **25 Minuten**

??? abstract "Verlaufsplanung"

    **1. Problem erweitern**

    Situation 3 besitzt drei Variablen:

    `A`, `B` und `C`.

    Bevor eine Tabelle gezeichnet wird, fragt die Lehrperson:

    > Wie viele verschiedene Ampelstellungen müsste es jetzt insgesamt geben?

    Die Lernenden können zunächst schätzen oder aus der Zweivariablen-Situation argumentieren.

    Gemeinsam wird hergeleitet:

    $$
    2 \cdot 2 \cdot 2 = 8 = 2^3
    $$

    **2. Vollständigkeit als Problem formulieren**

    **Leitfrage:**

    > Wie können wir acht Kombinationen so aufschreiben, dass garantiert keine fehlt und keine doppelt vorkommt?

    Zunächst dürfen eigene Strategien entstehen.

    Mögliche Ideen:

    - bereits verwendete Kombinationen abhaken;
    - immer nur einen Wert verändern;
    - nach einem regelmässigen Wechselmuster vorgehen;
    - die Kombinationen wie Binärzahlen ordnen.

    **3. AB 3b bearbeiten**

    Die Lernenden erstellen die vollständige Tabelle selbstständig.

    Ein mögliches systematisches Ergebnis ist:

    | `A` | `B` | `C` |
    | :---: | :---: | :---: |
    | `0` | `0` | `0` |
    | `0` | `0` | `1` |
    | `0` | `1` | `0` |
    | `0` | `1` | `1` |
    | `1` | `0` | `0` |
    | `1` | `0` | `1` |
    | `1` | `1` | `0` |
    | `1` | `1` | `1` |

    Die Lernenden untersuchen das Wechselmuster:

    **Variable `C`:**

    `0, 1, 0, 1, 0, 1, 0, 1`

    **Variable `B`:**

    `0, 0, 1, 1, 0, 0, 1, 1`

    **Variable `A`:**

    `0, 0, 0, 0, 1, 1, 1, 1`

    **Inputfrage:**

    > Warum können wir mit diesem Muster sicher sein, dass jede Kombination genau einmal vorkommt?

    **Erwartete Antwort:**

    Die Werte wechseln nach einem festen System. Dadurch werden nacheinander alle unterschiedlichen Dreierkombinationen erzeugt, ohne dass eine wiederholt oder übersprungen wird.

    **4. Spalte `sicher` ergänzen**

    Die Lernenden untersuchen Situation 3 und bewerten jede Zeile.

    Da `A` und `B` parallel verlaufen und `C` beide kreuzt, sind diejenigen Kombinationen unsicher, bei denen `C` gleichzeitig mit `A` oder `B` Grün hat.

    Eine korrekte Tabelle lautet:

    | `A` | `B` | `C` | `sicher` |
    | :---: | :---: | :---: | :---: |
    | `0` | `0` | `0` | `1` |
    | `0` | `0` | `1` | `1` |
    | `0` | `1` | `0` | `1` |
    | `0` | `1` | `1` | `0` |
    | `1` | `0` | `0` | `1` |
    | `1` | `0` | `1` | `0` |
    | `1` | `1` | `0` | `1` |
    | `1` | `1` | `1` | `0` |

    Die Tabelle wird anschliessend mit LogicTraffic kontrolliert.

    **5. Von drei Variablen zu $2^n$**

    Die bisherigen Ergebnisse werden verglichen:

    | Variablen | Kombinationen |
    | ---: | ---: |
    | 1 | $2$ |
    | 2 | $4$ |
    | 3 | $8$ |
    | 4 | $16$ |
    | 5 | $32$ |

    **Inputfrage:**

    > Was passiert jedes Mal, wenn eine weitere Variable hinzukommt?

    **Erwartete Antwort:** Die Zahl der möglichen Kombinationen verdoppelt sich.

    Daraus wird die Regel gesichert:

    $$
    \text{Anzahl der möglichen Belegungen} = 2^n
    $$

    **6. Skalierungsproblem erzeugen**

    Abschliessend wird gemeinsam berechnet:

    Bei fünf Variablen:

    $$
    2^5 = 32
    $$

    Bei zehn Variablen:

    $$
    2^{10} = 1024
    $$

    **Leitfrage:**

    > Wahrheitstabellen sind vollständig – aber sind sie bei sehr vielen Variablen noch eine praktische Darstellung?

    Die Lernenden halten erste Vor- und Nachteile fest.

??? note "Didaktische Hinweise"

    Die entscheidende Leistung besteht nicht darin, die Reihenfolge `000` bis `111` auswendig zu lernen. Die Lernenden sollen verstehen, **weshalb ein systematisches Muster Vollständigkeit garantiert**.

    Unterschiedliche korrekte Reihenfolgen der Zeilen sind grundsätzlich zulässig. Entscheidend ist, dass:

    - jede mögliche Kombination genau einmal vorkommt;
    - keine Kombination fehlt;
    - keine Kombination doppelt vorkommt.

    Das binäre Zählmuster ist deshalb als besonders gut überprüfbare Strategie zu vermitteln, nicht als einzig erlaubte Reihenfolge.

    Die Regel $2^n$ sollte aus der konkreten Situation heraus entwickelt werden:

    Jede weitere Variable besitzt zwei mögliche Werte und verdoppelt deshalb die Zahl der Kombinationen.

    LogicTraffic bleibt ein **Kontrollwerkzeug**. Die Tabelle sollte möglichst zuerst von den Lernenden selbst konstruiert werden.

??? bug "Differenzierung"

    === "Vereinfachungen"

        - Die acht Tabellenzeilen bereits vorzeichnen und nur die Werte eintragen lassen.
        - Das Wechselmuster für `C` vorgeben und `B` sowie `A` ergänzen lassen.
        - Die Zweivariablen-Tabelle daneben sichtbar lassen.
        - Mit der Frage unterstützen:  
          > „Wie oft muss sich der Wert in dieser Spalte ändern?“
        - Die Spalte `sicher` erst nach einer vollständigen Variablentabelle ergänzen.
        - Die Herleitung zunächst als `2 · 2 · 2 = 8` notieren und erst danach `2^3` einführen.

    === "Erweiterungen"

        - Eine vollständige Tabelle für vier Variablen ohne Vorlage beginnen lassen.
        - Vorhersagen lassen, welches Wechselmuster eine vierte Variable besitzt.
        - Für `n = 6`, `8`, `10` oder `12` die Zeilenzahl berechnen lassen.
        - Verschiedene korrekte Ordnungssysteme vergleichen und hinsichtlich Fehlersicherheit beurteilen.
        - Erklären lassen, weshalb das binäre Zählmuster auch bei beliebig vielen Variablen funktioniert.

### Phase 3 - Herausforderung – Fehler finden

??? success "Ziele der Einheit"

    Die Lernenden wenden ihr Wissen über Vollständigkeit, Ordnung und Sicherheit auf eine fehlerhafte Wahrheitstabelle an.

    Sie können zwischen **strukturellen Fehlern** und **inhaltlichen Fehlern** unterscheiden, eine Tabelle korrigieren und ihre Korrekturen fachlich begründen.

    Zum Abschluss erkennen sie die Wahrheitstabelle als zuverlässiges, aber bei vielen Variablen umfangreiches Werkzeug und formulieren damit die Ausgangsfrage für Baustein 4.

??? example "Material"

    - [:memo: AB 3c – Herausforderung: Fehler finden](https://github.com/salomegolden/logictraffic/releases/download/ab3_v1/3c_herausforderung_fehler.pdf)
    - LogicTraffic, **Situation 4**
    - Computer oder Tablet pro Zweiergruppe
    - Ergebnisse bzw. Merksätze aus Phase 2

??? info "Sozialformen"

    Zunächst kurze **Einzelarbeit**, damit jede Person die Tabelle selbst untersucht. Anschliessend **Partnervergleich** und gemeinsame Sicherung im **Plenum**.

    Die Kontrolle mit LogicTraffic erfolgt erst nach der eigenen Fehlersuche.

??? tip "benötigte Zeit"

    ca. **15–20 Minuten**

??? abstract "Verlaufsplanung"

    **1. Situation 4 analysieren**

    Situation 4 besitzt die Variablen:

    `B`, `C` und `D`.

    `B` und `C` verlaufen parallel, während `D` beide Fahrwege kreuzt.

    Vor der Fehlersuche wird kurz geklärt:

    - `B` und `C` dürfen grundsätzlich gleichzeitig Grün haben.
    - `D` darf nicht gleichzeitig mit `B` oder `C` Grün haben.

    **2. Fehlerhafte Tabelle auf AB 3c untersuchen**

    Die Tabelle enthält bewusst verschiedene Fehlertypen.

    Die Lernenden erhalten den Auftrag, nicht einfach nur „falsche Zeilen“ zu markieren, sondern systematisch zwei Fragen zu prüfen:

    **Vollständigkeit**

    > Kommt jede mögliche Kombination genau einmal vor?

    **Sicherheit**

    > Ist der Wert in der Spalte `sicher` fachlich korrekt?

    In der vorbereiteten Fehlertabelle sind insbesondere folgende Probleme enthalten:

    - die Kombination `101` kommt doppelt vor;
    - die Kombination `110` fehlt;
    - `011` ist fälschlicherweise als sicher markiert;
    - `111` ist fälschlicherweise als sicher markiert.

    **3. Fehler kategorisieren**

    Die Lernenden ordnen die Fehler zwei Kategorien zu.

    **Strukturelle Fehler:**

    - doppelte Kombination;
    - fehlende Kombination.

    **Inhaltliche Fehler:**

    - falscher Wert in der Spalte `sicher`.

    **Inputfrage:**

    > Warum reicht es nicht, nur zu zählen, ob die Tabelle acht Zeilen besitzt?

    **Erwartete Antwort:**

    Auch eine Tabelle mit acht Zeilen kann unvollständig sein, wenn eine Kombination doppelt vorkommt und dafür eine andere fehlt.

    **4. Tabelle korrigieren**

    Die korrekte Wahrheitstabelle für Situation 4 lautet:

    | `B` | `C` | `D` | `sicher` |
    | :---: | :---: | :---: | :---: |
    | `0` | `0` | `0` | `1` |
    | `0` | `0` | `1` | `1` |
    | `0` | `1` | `0` | `1` |
    | `0` | `1` | `1` | `0` |
    | `1` | `0` | `0` | `1` |
    | `1` | `0` | `1` | `0` |
    | `1` | `1` | `0` | `1` |
    | `1` | `1` | `1` | `0` |

    Die Lernenden begründen mindestens zwei ihrer Korrekturen.

    **Mögliche Begründung für `011`:**

    > `C = 1` und `D = 1`. Beide Spuren haben Grün und ihre Fahrwege kreuzen sich. Deshalb ist die Kombination unsicher und `sicher = 0`.

    **Mögliche Begründung für `110`:**

    > Diese Kombination fehlte. Sie muss enthalten sein, weil bei drei Variablen alle acht möglichen Belegungen genau einmal in der Tabelle vorkommen müssen.

    **5. Mit LogicTraffic überprüfen**

    Erst nach der Korrektur wird Situation 4 in LogicTraffic verwendet.

    Die Lernenden vergleichen:

    - Sind alle acht Kombinationen vorhanden?
    - Stimmen die Werte der Spalte `sicher`?
    - Falls noch eine Abweichung besteht: Handelt es sich um einen Struktur- oder einen Sicherheitsfehler?

    **6. Baustein sichern**

    Gemeinsam werden drei Kernregeln formuliert:

    **1. Vollständigkeit**

    Bei $n$ Variablen gibt es $2^n$ mögliche Belegungen.

    **2. Systematik**

    Jede mögliche Belegung muss genau einmal vorkommen.

    **3. Bedeutung**

    Die Spalte `sicher` bewertet die gesamte Ampelkombination und nicht eine einzelne Fahrspur.

    **7. Ausblick auf Baustein 4**

    Die Lehrperson greift nochmals das Wachstum auf:

    $$
    2^5 = 32
    $$

    und

    $$
    2^{10} = 1024
    $$

    **Abschlussfrage:**

    > Können wir dieselbe Sicherheitsregel vielleicht ausdrücken, ohne dafür jede mögliche Kombination einzeln aufzuschreiben?

    Diese Frage bildet den direkten Übergang zu [Baustein 4 – Logische Formeln](baustein4-boolesche-algebra.md).

??? note "Didaktische Hinweise"

    AB 3c ist besonders geeignet, um sichtbar zu machen, ob die Lernenden eine Wahrheitstabelle **verstanden** haben oder lediglich ein Muster reproduzieren können.

    Die Fehlersuche sollte deshalb nicht mit LogicTraffic beginnen. Sonst reduziert sich die Aufgabe auf einen blossen Abgleich mit einer fertigen Tabelle.

    Die Unterscheidung zwischen Struktur- und Inhaltsfehlern ist didaktisch besonders wertvoll:

    - Ein **Strukturfehler** betrifft die vollständige Erfassung des Zustandsraums.
    - Ein **Inhaltsfehler** betrifft die Bewertung einer konkreten Verkehrssituation.

    Bei Situation 4 ist zudem darauf zu achten, dass `B` und `C` parallel verlaufen. Die Kombination `110` ist deshalb **sicher**. Entscheidend ist nicht, wie viele Ampeln gleichzeitig Grün zeigen, sondern ob sich die grünen Fahrwege tatsächlich kreuzen.

    Der Ausblick auf Baustein 4 sollte die Wahrheitstabelle nicht abwerten. Sie bleibt ein sehr wichtiges Werkzeug zur vollständigen Beschreibung und später zur Überprüfung logischer Formeln. Das Problem ist ausschliesslich ihre mangelnde Kompaktheit bei vielen Variablen.

??? bug "Differenzierung"

    === "Vereinfachungen"

        - Die Fehlersuche in zwei Schritte trennen: zuerst nur die Variablenspalten, danach die Spalte `sicher`.
        - Eine Checkliste bereitstellen:  
          1. Gibt es acht Zeilen?  
          2. Kommt jede Kombination genau einmal vor?  
          3. Stimmen die Sicherheitswerte?
        - Die Kombinationen `000` bis `111` als Referenz danebenlegen.
        - Nur zwei der vier eingebauten Fehler suchen lassen und die übrigen gemeinsam besprechen.
        - Die Kreuzung von Situation 4 während der Sicherheitsprüfung sichtbar lassen.

    === "Erweiterungen"

        - Eine eigene fehlerhafte Wahrheitstabelle erstellen und mit einem anderen Tandem austauschen.
        - Die Fehler so wählen, dass die Tabelle weiterhin acht Zeilen besitzt und der Strukturfehler deshalb nicht durch blosses Zählen auffällt.
        - Ohne LogicTraffic begründen, welche Zeilen in Situation 4 zwingend `sicher = 0` sein müssen.
        - Erklären, weshalb `110` trotz zweier grüner Ampeln sicher ist.
        - Eine Strategie formulieren, mit der eine beliebige Wahrheitstabelle systematisch auf Vollständigkeit geprüft werden kann.

## Abschluss des Bausteins

Am Ende des Bausteins haben die Lernenden Wahrheitstabellen auf drei Ebenen untersucht:

1. **lesen und deuten** – Was beschreibt eine Tabellenzeile?
2. **systematisch erzeugen** – Wie erfassen wir alle möglichen Zustände vollständig?
3. **prüfen und korrigieren** – Wie erkennen wir strukturelle und inhaltliche Fehler?

!!! success "Von einzelnen Zuständen zur vollständigen Darstellung"

    Eine Wahrheitstabelle ist eine systematische Methode, um den vollständigen Zustandsraum eines Problems darzustellen.

    Für $n$ Variablen mit jeweils zwei möglichen Werten enthält sie:

    $$
    2^n
    $$

    Zeilen.

    Diese Vollständigkeit ist ihre grosse Stärke. Gleichzeitig führt genau sie bei vielen Variablen zu sehr grossen Tabellen.

    Daraus entsteht die Anschlussfrage für Baustein 4:

    > **Wie können wir dieselbe logische Funktion kompakter beschreiben?**