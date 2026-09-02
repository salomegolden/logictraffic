# Formeln verstehen

Diese Seite führt in logische Verknüpfungen und den Formeleditor ein. Ziel ist, dass Lernende Formeln nicht nur eingeben, sondern mit Wahrheitstabellen und Verkehrssituationen verbinden. Am Ende der Tabellen-Lektion wurde gezeigt, dass eine Kreuzung mit 5 Spuren bereits $2^5 = 32$ Zeilen benötigt und 10 Spuren sogar $2^{10} = 1024$ Zeilen erfordern würden.

Die fundamentale Leitidee: „Ein Steuerungscomputer speichert keine endlose Tabelle, sondern prüft Regeln!“ Eine Ampelsteuerung benötigt eine handlungsorientierte Bedingung, die in Echtzeit entscheidet, ob ein Signalzustand erlaubt ist.

!!! info "Von der Alltagssprache zur Formelsprache"

    Von der Alltagssprache zur Formelsprache (Scaffolding):Umgangssprache: „Wenn Spur A grün ist, muss Spur B rot sein.“Logische Bausteine zuordnen: „Spur A grün“ ($A$), „Spur B rot / Halt“ ($\neg B$), „Wenn … dann …“ ($\rightarrow$).Formel: $A \rightarrow \neg B$.

!!! abstract "Auf einen Blick"

    **:stopwatch: Dauer:**  
    45 Minuten (Basis: Junktoren $\neg, \land, \lor, \rightarrow$, Syntax & Modellierung von Situation 2 und 3) 
    90 Minuten (inkl. Vertiefung zu semantischen Äquivalenzen, Optimierung und kanonischen Normalformen)

    **:busts_in_silhouette: Sozialform:**  
    Kooperatives Arbeiten im Schüler-Tandem; Plenumsphasen für Konfrontation und Ergebnissicherung

    **:computer: Computer:**  
    Ein Rechner, Laptop oder Tablet mit Zugriff auf *LogicTraffic* pro Zweiergruppe (Nutzung des integrierten Formeleditors mit Bildschirmtastatur)

    **:brain: Vorwissen:**  
    * [Baustein 3 (Wahrheitstabellen)](baustein3-wahrheitstabellen.md) wurde abgeschlossen 
    * Variablen als Fahrspuren ($A, B, C$) sowie Wahrheitswerte ($1 = \text{Grün}$, $0 = \text{Rot/Halt}$) sind bekannt
    * Die Ergebnisspalte `sicher` ($1 = \text{kollisionsfrei}$, $0 = \text{Kollision}$) ist vertraut
    * Der kognitive Konflikt bezüglich der Skalierungsgrenzen von Wahrheitstabellen bei wachsender Spurenanzahl ($2^n$ Zeilen, z. B. 32 Zeilen bei Situation 10) ist präsent

    **:package: Material:**  
    * Webanwendung *LogicTraffic*  
    * Lehrpersonen-PC mit Beamer oder Präsentationsbildschirm zur Demonstration.  
    * Arbeitsblatt xx
    * Arbeitsblatt xy
    * Übersichtsblatt yy 
    * Notizpapier / Begleitportfolio zur formalen Ergebnissicherung.

!!! note "Downloads zu Baustein 4"

    [link]

## Lernziele

Die Lernenden

* …übersetzen umgangssprachliche Verkehrs- und Sicherheitsregeln schrittweise in aussagenlogische Ausdrücke.
* nutzen den Zeichenvorrat von LogicTraffic ($A, B, C, \dots$, $\neg, \land, \lor, \rightarrow$, Klammern) syntaktisch korrekt.
* verstehen die logische Bedeutung der Operatoren anhand des Verkehrsgeschehens (z. B. $A \land B =$ Kollision, $\neg A =$ Halt).
* interpretieren das Feedbacksystem (Not safe, Safe, Optimal) und iterieren ihre Formeln bis zur semantischen Äquivalenz.

## Vorbereitung

## Unterrichtsablauf - Überblick

### 1. Basisversion (45 Minuten): Formeln & Steuerung

| Phase | Inhalt & Aktivität | Sozialform / Medien | Richtwert |
| :--- | :--- | :--- | :--- |
| **1. Einstieg & Konflikt** | • Grenzen der Tabelle an *Situation 8* aufzeigen (32 Zeilen).<br>• Leitfrage: Wie steuern wir die Kreuzung mit einer einzigen Regel? | **Plenum**<br>Beamer (*Situation 10*) | **ca. 10'** |
| **2. Erarbeitung** | • Junktoren ($\neg, \land, \lor, \rightarrow$) an *Situation 2* ableiten ($A \rightarrow \neg B$).<br>• Eingabe im Formeleditor und Parsebaum demonstrieren[cite: 2, 4]. | **Plenum**<br>Tafel, *LogicTraffic* | **ca. 10'** |
| **3. Übung** | • Tandems steuern *Situation 3* [3 Spuren](cite: 1, 4).<br>• Formeloptimierung über den Polizisten-Status (`Not safe`, `Safe`, `Optimal`). | **Pair Learning**<br>Schüler-PCs [*LogicTraffic*](cite: 1, 12) | **ca. 30'** |
| **4. Sicherung** | • Lösungsvergleich ($A \rightarrow \neg C$ vs. $\neg(A \land C)$)[cite: 2].<br>• Vorrangregeln ($\neg$ vor $\land$ vor $\lor$ vor $\rightarrow$) festhalten[cite: 2]. | **Plenum**<br>Merkheft / Portfolio | **ca. 10'** |

---

### 2. Erweiterte Version (90 Minuten): Inkl. Äquivalenzen & Normalformen

| Phase | Inhalt & Aktivität | Sozialform / Medien | Richtwert |
| :--- | :--- | :--- | :--- |
| **1. Einstieg & Konflikt** | • Skalierungsgrenzen von Tabellen an *Situation 8* rekapitulieren.<br>• Impuls: Steuerungsrechner prüfen kompakte Regeln in Echtzeit. | **Plenum**<br>Beamer (*Situation 10*) | **ca. 10'** |
| **2. Erarbeitung I** | • Junktoren ($\neg, \land, \lor, \rightarrow$) an *Situation 2* einführen.<br>• Formeleditor und Parsebaum erproben. | **Plenum**<br>Tafel, *LogicTraffic* | **ca. 15'** |
| **3. Übung I** | • Steuerungsformeln für *Situation 3* im Tandem entwickeln.<br>• Iterative Fehlerbehebung mit Polizisten-Feedback (`Optimal`). | **Pair Learning**<br>Schüler-PCs (*LogicTraffic*) | **ca. 30'** |
| **4. Erarbeitung II** | • Semantische Äquivalenzen vergleichen (z. B. De Morgan).<br>• Automatische Generierung von KDNF und KKNF demonstrieren. | **Plenum**<br>Beamer, *LogicTraffic* | **ca. 15'** |
| **5. Übung II** | • Transfer: Steuerung von *Situation 10* (5 Spuren) via Formeln oder *Simplest Form*. | **Pair Learning**<br>Schüler-PCs [*LogicTraffic*](cite: 1, 12) | **ca. 30'** |
| **6. Sicherung** | • Gegenüberstellung: Tabelle vs. Formel vs. Normalformen.<br>• Dokumentation der Rechenregeln im Portfolio. | **Plenum**<br>Merkheft / Portfolio | **ca. 15'** |

## Durchführung

### Phase 1 - Konfrontationsaufgabe - Die Grenzen der Tabelle

??? question "Aufgabe 1: Der Speicherüberlauf an Grosskreuzungen (Situation 8)"

    Phase: Einstieg & Konfrontation | Modus: Plenum & Tandem | Zeit: ca. 7 Min. | Situation: Situation 8

Didaktische Absicht: Reaktivierung des kognitiven Konflikts aus Baustein 3: Wahrheitstabellen skalieren exponentiell ($2^n$) und sind für reale Steuerungsrechner ungeeignet. Es entsteht das Bedürfnis nach einer kompakten Bedingungsprüfung in Echtzeit.

Ablauf: Die Lehrperson projiziert die 5-Spuren-Kreuzung (Situation 10) an die Wand und lässt die Schüler/innen kurz per Handnotiz versuchen, das Verkehrsgeschehen in einem Satz zusammenzufassen.

**Kontext:**  
An der Kreuzung mit 3 Spuren (*Situation 3*) reichte uns eine Tabelle mit $2^3 = 8$ Zeilen. Nun stehen wir vor einer klassischen 4-Wege-Kreuzung (*Situation 8* mit den Spuren $A, B, C, D$). Eine lückenlose Wahrheitstabelle würde hier bereits $2^4 = 16$ Zeilen umfassen. Der Steuerungscomputer der Ampelanlage soll jedoch nicht jedes Mal 16 Zeilen durchforsten müssen, sondern anhand einer handlungsorientierten Regel schalten.

!!! quote "Arbeitsauftrag"

    1. Öffnet in *LogicTraffic* die **Situation 8**.
    2. Beobachtet kurz die vier Fahrspuren $A, B, C$ und $D$.
    3. Notiert zu zweit auf einem Schmierzettel **genau einen verständlichen deutschen Satz**, der unmissverständlich festlegt, wer wann fahren darf (oder wer warten muss), damit es *niemals* kracht.
    4. *Reflexionsfrage:* Warum ist dieser deutsche Satz für einen Programmierer oder Computer immer noch zu ungenau?

??? tip "Denkhilfe"

    Orientiert euch an den Fahrtrichtungen: Welche Richtungen schneiden sich im Zentrum und dürfen niemals gleichzeitig Grün erhalten?

??? success "Didaktischer Erwartungshorizont"

    * **Schülersatz (Beispiel):** *„Die Spuren der Querstrasse dürfen niemals gleichzeitig grün sein mit den Spuren der Hauptstrasse.“* oder *„Wenn A oder B fahren, müssen C und D zwingend rot haben.“*
    * **Kern-Erkenntnis:** Alltagssprache verwendet Sammelbegriffe („Querstrasse“, „Hauptstrasse“) oder lange Nebensätze. Der Mikrocontroller einer Ampel kennt jedoch nur Einzelsignale ($0$ und $1$) und benötigt exakte, berechenbare Bedingungen.

??? tip "Sprachhilfe: Satzbausteine für deine Ampelregel"
    **1. Wortspeicher (Wichtige Begriffe):**

    * *Spuren:* Spur $A$, Spur $B$ (Verkehrsachse 1) | Spur $C$, Spur $D$ (Querachse 2)[cite: 1, 11]
    * *Signale:* hat Grün / freie Fahrt ($1$) | hat Rot / muss anhalten ($0$)
    * *Gefahr:* gleichzeitig, kreuzen sich, schneiden sich, Unfall / Kollision

    **2. Satzbau-Schablonen (Wähle eine Variante):**

    * **Variante A (Wenn-Dann-Form):**  
      *„Wenn Spur _____ (oder Spur _____) Grün hat, dann müssen Spur _____ und Spur _____ zwingend Rot haben.“*
    * **Variante B (Kollisionsverbot):**  
      *„Spur _____ und Spur _____ dürfen niemals gleichzeitig mit Spur _____ oder _____ fahren.“*
    * **Variante C (Achsen-Regel):**  
      *„Solange auf der Hauptstrasse ($A$ und $B$) gefahren wird, muss die Querstrasse ($C$ und $D$) komplett stehen.“*

??? example "Mögliche Ergebnisse und Lösungen"

    Je nach Sprachniveau und Abstraktionsgrad der Schülerpaare treten typischerweise drei Formulierungsebenen auf:
    
    * Alltagssprachliche Schülerformulierung (Einstiegsniveau): *„Die Autos von oben und unten dürfen niemals gleichzeitig mit den Autos von links und rechts fahren, sonst kracht es in der Mitte.“ Didaktischer Kommentar: Intuitiv richtig, fasst Spuren jedoch noch zu Richtungen zusammen.
    * Strukturierte Steuerungsregel (Zielformulierung für den Transfer): *„Wenn Spur $A$ oder Spur $B$ Grün hat, müssen die Spuren $C$ und $D$ Rot haben – und umgekehrt.“* (Didaktischer Kommentar: Eignet sich didaktisch ideal, da die Wenn-Dann-Struktur unmittelbar die Implikation vorstrukturiert).
    * Kollisionsorientierte Negationsregel (Vorbereitung De Morgan): *„Es darf niemals passieren, dass $A$ oder $B$ gleichzeitig mit $C$ oder $D$ Grün haben.“* 
    (Didaktischer Kommentar: Bereitet das Verbot von Konjunktionen $\neg(\dots \land \dots)$ vor).D
    
    Didaktische Brücke zur Formalisierung: Anhand der Zielformulierung lässt sich der Schritt zur Formel im Unterrichtsgespräch nahtlos anschliessen:
    $$\underbrace{\text{Wenn } A \text{ oder } B \text{ Grün hat}}_{(A \lor B)}, \quad \underbrace{\text{dann müssen}}_{ \rightarrow } \quad \underbrace{C \text{ und } D \text{ Rot sein}}_{(\neg C \land \neg D)}$$
    
    Dies verdeutlicht der Klasse, dass die logische Formel $(A \lor B) \rightarrow (\neg C \land \neg D)$ keine willkürliche Mathematik ist, sondern eine exakte 1:1-Übersetzung ihrer eigenen deutschen Verkehrsregel.

### Phase 2 - Erarbeitungsaufgabe - Das Übersetzungsbüro (Situation 2 / Syntax, Junktoren & Editor)

Ein Ampelcomputer versteht keine langen deutschen Sätze, sondern verarbeitet mathematisch exakte Rechenzeichen. An einer einfachen Kreuzung mit zwei schneidenden Spuren ($A$ und $B$) übersetzt ihr typische Verkehrssituationen Schritt für Schritt in die Maschinensprache von *LogicTraffic*.

Didaktische Absicht:

* Erarbeitung der formalen Junktoren ($\neg, \land, \lor, \rightarrow$) direkt aus dem realen Verkehrsgeschehen.
* Einführung der materialen Implikation ($A \rightarrow \neg B$) als intuitive Schaltungsregel („Wenn A fährt, muss B halten“).
* Kennenlernen des Formeleditors und der Bildschirmtastatur in LogicTraffic ohne Syntaxfrust.
* Unmittelbare Verifikation von Formeleingaben über die automatisierte Synchronisation mit der Wahrheitstabelle und das Polizisten-Feedback.

!!! quote "Arbeitsauftrag 1"
    1. Übertragt die Bedeutungen in eure Notizen und ergänzt die fehlenden Formeln mithilfe des **Wort- und Symbolspeichers**:

        | Nr. | Verkehrssituation / Regel | Logische Bedeutung | LogicTraffic-Ausdruck |
        | :-: | :--- | :--- | :--- |
        | **1** | Spur $B$ muss anhalten. | Spur $B$ hat kein Grün (also Rot). | `¬B` |
        | **2** | Spur $A$ und Spur $B$ fahren gleichzeitig los. | Spur $A$ hat Grün **und** Spur $B$ hat Grün (Crash!). | `...` |
        | **3** | Kollisionsvermeidung: Mindestens eine Spur steht. | Spur $A$ hat Rot **oder** Spur $B$ hat Rot (oder beide). | `...` |
        | **4** | Schaltungsregel: *„Wenn A grün ist, muss B rot sein.“* | **Wenn** Spur $A$ gilt, **dann** folgt daraus $\neg B$. | `...` |

    2. Öffnet in *LogicTraffic* die **Situation 2**.
    3. Klickt im Formeleditor auf die Tasten der Bildschirmtastatur, um die Schaltformel `A → ¬B` einzugeben[cite: 2, 6].
    4. Klickt auf **In Wahrheitstabelle laden** (bzw. **prüfen**):
        
        * Welches Feedback-Icon zeigt der Polizist neben dem Formelfeld an?
        * Was hat sich in der Spalte `sicher` der Wahrheitstabelle verändert?

??? tip "Wort- und Symbolspeicher für den Formeleditor"

    * `¬` (**Negation / NICHT**): Kehrt den Wert um (`¬A` = Rot für Spur $A$).
    * `∧` (**Konjunktion / UND**): Beide Spuren fahren gleichzeitig (`A ∧ B`).
    * `∨` (**Disjunktion / ODER**): Mindestens eine Bedingung ist erfüllt (`¬A ∨ ¬B`).
    * `→` (**Implikation / WENN-DANN**): Schaltungsbedingung (`A → ¬B`).
    * `Del`: Letztes eingegebenes Zeichen löschen.

??? success "Musterlösung & Fachbegriffe"

    * **Ergänzte Tabelle:**
        * Zeile 2: `A ∧ B` *(Konjunktion / Beschreibung des Crash-Zustands)*
        * Zeile 3: `¬A ∨ ¬B` *(Disjunktion / De Morgan'sche Kollisionsvermeidung)*
        * Zeile 4: `A → ¬B` *(Materiale Implikation / direkte Schaltungsregel)*
    * **Polizisten-Status:** Der Polizist salutiert (**Optimal**).
    * **Auswirkung in der Tabelle:** In der Spalte `sicher` werden alle unfallfreien Belegungen ($00, 01, 10$) mit einer $1$ belegt, während der Kollisionszustand ($11$) zuverlässig auf $0$ gesperrt wird.

??? warning "Entlastung von Syntaxhürden"

    Anfängliche Frustration bei Programmier- und Logikwerkzeugen entsteht meist durch Syntaxfehler oder das mühsame Suchen von Sonderzeichen ($\neg, \land, \lor, \rightarrow$) auf der Computertastatur. Die ausschliessliche Nutzung der On-Screen-Tastatur im LogicTraffic-Editor nimmt diese Hürde vollständig weg, sodass die Aufmerksamkeit ganz auf der logischen Bedeutung verbleibt. 

??? warning "Implikation im Verkehrsmodell"

    Das klassische logische Missverständnis bei der materialen Implikation („Warum ist $0 \rightarrow \dots$ wahr?“) klärt sich über den situativen Kontext zwanglos auf: Wenn Spur $A$ an der roten Ampel wartet ($A = 0$), geht von ihr physikalisch keine Gefahr aus. Die Regel $A \rightarrow \neg B$ wird dadurch nicht verletzt, und Spur $B$ darf vollkommen gefahrlos schalten.

??? info "Synchroner Darstellungswechsel:"

    Der Klick auf In Wahrheitstabelle laden verdeutlicht den Zusammenhang zwischen der kompakten Formelzeile und der vollständigen 4-Zeilen-Matrix. Die Lernenden sehen unmittelbar, wie eine einzige Rechenregel denselben Zweck erfüllt wie das manuelle Pflegen mehrerer Tabellenzeilen.

### Phase 3 - Übungsaufgabe - Die Kreuzungs-Steuerung (Situation 3 / 3 Spuren & Feedback)

Phase: Übung & Anwendung | Modus: Pair Learning oder Einzelarbeit am PC | Zeit: ca. 30 Min. | Situation: Situation 3

Didaktische Absicht:

* Selbstständiges Modellieren einer mehrspurigen Kreuzung mit mehreren Konfliktpunkten mittels aussagenlogischer Formeln.  
* Zusammensetzen mehrerer Teilbedingungen über Konjunktionen (∧) und Klammern.  
* Nutzung des formativen Polizisten-Feedbacks (Not safe, Safe, Optimal) zur eigenständigen Fehlerdiagnose und schrittweisen Lösungsoptimierung (Trial and Error mit unmittelbarer Verstärkung).  

**Kontext:**  
Ihr übernehmt als Verkehrsingenieure die Steuerung von **Situation 3** (3 Spuren: $A, B, C$).  
*Spur $A$ und Spur $B$ verlaufen nebeneinander und können gefahrlos gleichzeitig fahren. Spur $C$ biegt links ab und kreuzt dabei beide Spuren ($A$ und $B$)*.

!!! quote "Arbeitsauftrag 1"
    1. Öffnet in *LogicTraffic* die **Situation 3**
    2. Analysiert die Kreuzung gemeinsam im Tandem:
        *Welche Spuren dürfen gleichzeitig fahren?
        * Zwischen welchen Spuren droht ein Unfall, wenn beide Grün haben?
    3. Formuliert im Formeleditor eine logische Formel, welche die Kreuzung unfallfrei und flüssig steuert, und klickt auf **In Wahrheitstabelle laden** (oder **prüfen**)
    4. Lest die Rückmeldung des Polizisten ab und verbessert eure Formel schrittweise:
        ***nicht sicher:** Klickt auf *simulieren* – bei welchen Autos kracht es? Ergänzt die fehlende Sicherheitsbedingung!
        * **nicht optimal:** Eure Kreuzung ist zwar unfallsicher, aber ihr sperrt Spuren unnötig auf Rot. Prüft, ob ihr Spuren verriegelt habt, die sich gar nicht behindern
        * **optimal:** Voller Verkehrsfluss bei 100 % garantierter Kollisionsfreiheit!
    5. Tragt eure finale, optimale Formel in euer Begleitportfolio ein.

??? tip "Denkhilfe: Konfliktstellen einzeln sichern"

    Spur $C$ hat **zwei** unabhängige Konfliktgegner: Spur $A$ und Spur $B$ 
    * Formuliert zuerst die Regel für Spur $A$ und $C$  
    * Formuliert danach die Regel für Spur $B$ und $C$ 
    * Verknüpft beide Bedingungen mit einem logischen UND (`∧`) und setzt zur Übersicht Klammern: `(...) ∧ (...)`.

??? success "Musterlösungen & didaktischer Erwartungshorizont"

    In *LogicTraffic* führen mehrere unterschiedliche Modellierungsansätze zum Status **Optimal**:
    * **Schaltregeln mit Implikation:**  
      `(A → ¬C) ∧ (B → ¬C)`  
      *Oder kompakter zusammengefasst:*  
      `C → (¬A ∧ ¬B)` bzw. `C → ¬(A ∨ B)`[cite: 1, 2]
    * **Kollisionsverbote (UND-Ansatz):**  
      `¬(A ∧ C) ∧ ¬(B ∧ C)`[cite: 1, 3]
    * **ODER-Bedingungen (Klauselform / De Morgan):**  
      `(¬A ∨ ¬C) ∧ (¬B ∨ ¬C)`[cite: 1, 2, 3]
    * **Tabellenergebnis:** Exakt die 5 sicheren Zustände ($000, 001, 010, 100, 110$) erhalten eine $1$, während die 3 Kollisionen ($011, 101, 111$) zuverlässig gesperrt werden ($0$)

??? warning "Klammerregeln"

    Sobald mehrere logische Bedingungen mit ∧ zusammengefügt werden, wird die korrekte Klammerung bedeutsam[cite: 1, 2]. Ohne Klammern bindet das logische UND stärker als die Implikation ($\land \succ \rightarrow$). Die Schreibweise A → ¬C ∧ B → ¬C führt daher zu syntaktischen Fehlinterpretationen. Die Lehrperson erinnert die Gruppen bei Bedarf an die Faustregel: „Jede Einzelregel kommt in ihre eigene Klammer.“

??? info "Pair Learning und Kooperativer Diskurs"

    Obwohl die Erarbeitung im Schüler-Tandem (Pair Learning) empfohlen wird, ist eine Bearbeitung in Einzelarbeit problemlos möglich. Den Lernenden kann hierbei bewusst die Wahlfreiheit überlassen werden. Dies entspricht dem Prinzip des personalisierten Lernens und kommt Schülerinnen und Schülern entgegen, die Aufgaben lieber im eigenen Tempo ohne sozialen Abstimmungsdruck bearbeiten möchten. Fachdidaktische Befunde zur gendersensiblen Informatikdidaktik zeigen, dass insbesondere Mädchen von sozialen, kooperativen Lernformen wie Pair Learning oder Teamarbeit profitieren. Kollaborative Settings schaffen ein unterstützendes, sicheres Lernumfeld mit reduzierten Wettbewerbsaspekten, stärken das Zugehörigkeitsgefühl und bauen Hemmschwellen sowie stereotype Barrieren im Umgang mit formal-abstrakten Themen ab.

### Phase 4 - Abschluss in der Basislektion

**Kontext:**  
Beim Steuern von *Situation 3* (Spur $A$ und $B$ parallel, Spur $C$ kreuzt beide) haben verschiedene Teams ganz unterschiedliche Formeln eingereicht. Im ersten Schritt vergleichen wir eure Ergebnisse. Im zweiten Schritt haltet ihr die universellen Regeln der Logik auf eurem Merkblatt fest.

!!! quote "Arbeitsauftrag 1"
    **Teil A: Der Lösungsvergleich im Plenum (5 Min.)**
    Betrachtet die gesammelten Formeln an der Tafel:

    * **Team Rot:** `(A → ¬C) ∧ (B → ¬C)` *(„Wenn A fährt, muss C halten UND wenn B fährt, muss C halten“)*
    * **Team Blau:** `C → (¬A ∧ ¬B)` *(„Wenn C fährt, müssen A und B gleichzeitig halten“)*
    * **Team Gelb:** `¬(A ∧ C) ∧ ¬(B ∧ C)` *(„Kein Crash zwischen A und C UND kein Crash zwischen B und C“)*
    * **Team Schwarz:** `¬A ∧ ¬B ∧ ¬C` *(„Alle Spuren haben dauerhaft Rot“)*

    1. Diskutiert: Warum stuft *LogicTraffic* die Teams **Rot, Blau und Gelb** alle als 🫡 **Optimal** ein, obwohl die Formeln völlig unterschiedlich aussehen?
    2. Welchen Status erhält **Team Schwarz** und warum ist diese Lösung für eine echte Kreuzung unbrauchbar?

---

!!! quote "Arbeitsauftrag 2"

    Füllt auf eurem Merkblatt (Begleitportfolio) die folgenden drei Abschnitte aus:

    1. **Das Logik-Lexikon:** Ordnet den vier Verkehrsbedeutungen das korrekte Rechenzeichen zu (`¬`, `∧`, `∨`, `→`).
    2. **Die Rangfolge der Operatoren:** Welche Operation bindet am stärksten, wenn keine Klammern gesetzt sind?
    3. **Beispiel für Formelgleichheit (Äquivalenz):** Notiert zwei verschiedene Formeln aus dem Unterricht, die genau dieselbe Ampelschaltung bewirken.

??? tip "Hinweis zu Teil A (Warum verschiedene Formeln klappen)"

    Denkt an die Wahrheitstabelle aus Baustein 3: Entscheidend für den Computer ist nur, was am Ende in der Spalte `sicher` steht. Wenn zwei Formeln bei allen 8 Zeilen exakt dieselben Einsen und Nullen erzeugen, sind sie für die Ampelsteuerung **vollkommen gleichwertig** (logisch äquivalent).

??? success "Musterlösung & Tafelbild (Inhalt des Merkblatts)"

    Merkblatt: Aussagenlogische Formeln & Regeln

    1. Die Grundoperatoren (Junktoren):
    ┌──────────────┬─────────┬──────────────────────┬───────────────────────────────────────────┐
    │ Operator     │ Symbol  │ Logischer Name       │ Verkehrsbedeutung                         │
    ├──────────────┼─────────┼──────────────────────┼───────────────────────────────────────────┤
    │ NICHT        │    ¬    │ Negation             │ Halt / Rotlicht auf dieser Spur           │
    │ UND          │    ∧    │ Konjunktion          │ Gleichzeitiges Grün (Kollisionszustand)   │
    │ ODER         │    ∨    │ Disjunktion          │ Mindestens eine Bedingung ist erfüllt     │
    │ WENN..., DANN│    →    │ Materiale Implikation│ Schaltungsregel (Wenn Spur A, dann ...)   │
    └──────────────┴─────────┴──────────────────────┴───────────────────────────────────────────┘

    2. Rangfolge der Operatoren (Priorität ohne Klammern):
       1. ¬ (bindet am stärksten)
       2. ∧
       3. ∨
       4. → (bindet am schwächsten)
       Faustregel: Setze bei zusammengesetzten Regeln immer Klammern: (...) ∧ (...)!

    3. Semantische Äquivalenz (Formelgleichheit):
       Zwei Formeln sind logisch äquivalent (≡), wenn sie bei jeder Belegung 
       denselben Wahrheitswertverlauf (dieselben Zeilen in der Tabelle) erzeugen.
       
       Beispiel Situation 3:
       (A → ¬C) ∧ (B → ¬C)   ≡   C → (¬A ∧ ¬B)   ≡   ¬(A ∧ C) ∧ ¬(B ∧ C)
       (Alle drei Schaltungen sind sicher UND lassen den Verkehr optimal fliessen = 🫡 Optimal)

    4. "Safe" ist nicht gleich "Optimal":
       • Safe: Verhindert Unfälle (kann aber auch bedeuten: alle Ampeln bleiben ewig Rot).
       • Optimal: Maximale Sicherheit bei maximalem Verkehrsfluss (kein unnötiges Warten).

## Erweiterungsaufgaben für die vertiefte Versions

### Phase 5 - Erarbeitung 2 - Äquivalenzen & Kanonische Normalformen

**Sozialform / Medien:** Gelenktes Unterrichtsgespräch mit Demonstration an der Beamer-Projektion, anschliessend entdeckende Partnerarbeit im Tandem (*Pair Learning*); Schüler-PCs mit *LogicTraffic* (*Situation 3*), Begleitportfolio / Notizen.

**Didaktische Absicht:**  

* Verständnis der **semantischen Äquivalenz** über De Morgans Gesetze ($\neg(A \land C) \equiv \neg A \lor \neg C$).
* Didaktischer Brückenschlag zwischen Baustein 3 (Wahrheitstabelle) und Baustein 4 (Formeln): Erkennen, wie ein Algorithmus aus Tabellenzeilen vollautomatisch formale Ausdrücke ableitet.
* Dekonstruktion der **Kanonisch Disjunktiven Normalform (CDNF)** als Summe aller erlaubten Zustände (Minterme) und der **Kanonisch Konjunktiven Normalform (CCNF)** als Produkt aller verbotenen Kollisionen (Maxterme).
* Erkennen des Skalierungsproblems von Normalformen als Motivation für logische Minimierungsverfahren (*Simplest Form*).

??? note "Ablauf und Unterrichtsgeschehen"

    1. **Problemimpuls & De Morgan (ca. 10'):**
        Die Lehrperson projiziert zwei optimale Lösungen aus Phase 3 an die Wand: `¬(A ∧ C)` und `¬A ∨ ¬C`. *Leitfrage:* „Warum führen diese beiden völlig unterschiedlich aussehenden Formeln im Strassenverkehr zum exakt identischen Ampelverhalten?“ Die Klasse stellt fest: *„Es darf nicht sein, dass beide fahren“* ist logisch identisch mit *„Mindestens einer muss anhalten“*.
    2. **Werkzeugdemonstration: Die Formelmaschine in *LogicTraffic* (ca. 5'):**  
        Die Lehrperson lenkt den Blick auf das Dropdown-Menü oberhalb des Formelfeldes (standardmässig auf `scrollen` eingestellt). Sie wählt `CDNF` und danach `CCNF` aus: Riesige Formelketten erscheinen automatisch im Textfeld.  
        *Impuls:* „Woher kennt der Computer diese Formeln, ohne dass wir eine einzige Taste getippt haben?“
    3. **Entdeckende Tandemarbeit (ca. 10'):**  
        Die Schülerpaare bearbeiten **Aufgabe 4** an ihren Geräten. Sie zählen die Klammern in der CDNF und CCNF und vergleichen die Anzahl gezielt mit den Zeilen mit `sicher = 1` bzw. `sicher = 0` in ihrer Wahrheitstabelle.
    4. **Kurze Zwischensynthese im Plenum (ca. 2'):**  
        Zusammenfassung an der Tafel:  

        * Jede Zeile mit `sicher = 1` erzeugt einen **Minterm** (UND-Klammer mit allen Variablen). Alle sicheren Zustände werden mit ODER (`∨`) verknüpft $\rightarrow$ **CDNF**  
        * Jede Zeile mit `sicher = 0` erzeugt einen **Maxterm** (ODER-Klammer, die den Crash verbietet). Alle Verbote werden mit UND (`∧`) verknüpft $\rightarrow$ **CCNF**

!!! quote "Einstieg" 

    **Kontext:**  
    Ihr habt gesehen, dass es mehrere Wege gibt, eine Kreuzung fehlerfrei zu steuern[cite: 3, 4]. Doch was macht ein Computer, wenn kein Mensch da ist, um eine schlaue Regel zu erfinden? Er nutzt ein rein mechanisches Verfahren, um direkt aus der Wahrheitstabelle eine Formel zu bauen: sogenannte **kanonische Normalformen**.

!!! quote "Teil A: De Morgan & Formelgleichheit"
    1. Gebt in *LogicTraffic* bei **Situation 3** nacheinander folgende zwei Formeln ein und klickt jeweils auf **In Wahrheitstabelle laden**:

       * Formel 1: `¬(A ∧ C)`
       * Formel 2: `¬A ∨ ¬C`

    2. Prüft die Spalte `sicher`: Unterscheiden sich die beiden Tabellen in einer einzigen Zeile?
    3. Formuliert den Bedeutungsunterschied im Alltag: *Warum bedeutet „Es dürfen nicht beide fahren“ dasselbe wie „Mindestens einer muss stehen“*?

!!! quote "Teil B: Das Geheimnis des Dropdown-Menüs (KDNF & KKNF)

    1. Stellt sicher, dass bei Situation 3 die Spalte `sicher` korrekt ausgefüllt ist (5 sichere Zeilen mit `1`, 3 Kollisionszeilen mit `0`).
    2. Öffnet das Dropdown-Menü oberhalb des Formelfeldes und wählt **KDNF** aus:

       * Wie viele grosse Klammerblöcke (durch `∨` getrennt) wurden erzeugt?
       * Vergleicht diese Zahl mit den Zeilen mit `sicher = 1` in der Wahrheitstabelle. Was fällt euch auf?
       * Schaut euch einen Block genau an (z. B. `A ∧ B ∧ ¬C`). Welcher Tabellenzeile entspricht dieser Zustand?

    3. Wählt nun im Menü **KKNF** aus:

       * Wie viele Klammern (durch `∧` verbunden) seht ihr jetzt?
       * Welcher Zeilenart in der Tabelle (`sicher = 1` oder `sicher = 0`) entspricht diese Anzahl?

    4. Klickt auf **Simplest**: Was macht *LogicTraffic* mit dem Bandwurm-Ausdruck?

??? tip "Hinweis zum Lesen der Normalformen"

    * **KDNF (Disjunktive Normalform):** Listet alle *erlaubten Kombinationen* auf.  
          *Übersetzung:* „Die Ampel schaltet grün, WENN Zustand 1 vorliegt ODER Zustand 2 ODER Zustand 3 ...“
    * **KKNF (Konjunktive Normalform):** Listet alle *verbotenen Unfälle* auf.  
          *Übersetzung:* „Die Ampel schaltet grün, WENN Crash 1 nicht auftritt UND Crash 2 nicht auftritt ...“

??? success "Musterlösungen und Fachbegriffe"

    * **Teil A (De Morgan):** Beide Formeln erzeugen eine identische Belegung in der Spalte `sicher` (Status 🫡 `Optimal`)[cite: 4]. Die Gesetze von De Morgan besagen: $\neg(X \land Y) \equiv \neg X \lor \neg Y$[cite: 4].
    * **Teil B (Normalformen bei Situation 3):**
        * **KDNF:** Besteht aus genau **5 Konjunktionen (Mintermen)**, verbunden durch `∨`. Jede Klammer beschreibt exakt eine der 5 grünen Zeilen (`sicher = 1`), z. B. `(¬A ∧ ¬B ∧ ¬C) ∨ ... ∨ (A ∧ B ∧ ¬C)`.
        * **KKNF:** Besteht aus genau **3 Disjunktionen (Maxtermen)**, verbunden durch `∧`. Jede Klammer sperrt exakt eine der 3 roten Zeilen (`sicher = 0`), an denen $A$ und $C$ kollidieren.
        * **Simplest:** LogicTraffic wendet Minimierungsalgorithmen an (z. B. Quine-McCluskey / Karnaugh-Veitch) und kürzt den langen Normalform-Ausdruck automatisch auf die kompakte Form `¬A ∨ ¬C` bzw. `A → ¬C` zusammen.

??? info "Didaktischer Kommentar"

    Diese Phase bildet den methodischen Kern des gymnasialen Informatikunterrichts: Sie verknüpft die tabellarische Zustandserfassung (ikonisch-strukturell) direkt mit der algebraischen Logik (symbolisch-formal). Die Schülerinnen und Schüler begreifen, dass eine aussagenlogische Formel nicht erraten werden muss, sondern dass eine mathematisch deterministische Beziehung zwischen Tabelle und Normalform existiert.

    **KDNF vs. KKNF aus verkehrstechnischer Sicht:**  
    
    * Die **KDNF** entspricht dem *Zulassungsprinzip* (Positivliste): Man zählt alle erlaubten Fahrzustände auf. Bei wenigen Spuren ist dies anschaulich, skaliert bei grossen Netzen mit vielen sicheren Zuständen jedoch extrem schlecht.
    * Die **KKNF** entspricht dem *Sicherheitsprinzip* (Verbotsliste): Man identifiziert lediglich die Schnittpunkte der Fahrspuren und formuliert für jeden potenziellen Unfall ein Ausschlusskriterium. Dies entspricht der intuitiven Denkweise von Verkehrsingenieuren und führt in der Praxis meist zu deutlich kompakteren Regelwerken.
    
??? info "Vorbereitung auf den Transfer (Phase 5 & 6):"

    Das Verständnis der softwaregestützten Minimierung (`Simplest Form`) entlastet die Lernenden für die nachfolgende Transferphase an der komplexen 5-Spuren-Kreuzung (*Situation 10*): Sie haben verstanden, dass der Computer selbst riesige Tabellen über Normalformen formalisieren und anschliessend auf winzige Schaltterme reduzieren kann.

### Phase 5 - Übungs- und Sicherungsaufgabe 

**Sozialform / Medien:** Vertiefendes Arbeiten im Schüler-Tandem (*Pair Learning* am Rechner, offene Wahl für Einzelarbeit); Schüler-PCs mit *LogicTraffic* (*Situation 10*), Begleitportfolio / Arbeitsblatt.

**Didaktische Absicht:**

* **Komplexer Transfer:** Anwendung der Modellierungskompetenz und des Normalform-Verständnisses auf eine Grosskreuzung mit 5 Spuren ($A, B, C, D, E$) und einem Zustandsraum von $2^5 = 32$ Zeilen.
* **Repräsentationsvergleich:** Direkter Vergleich zwischen algorithmisch erzeugten Normalformen (CDNF, CCNF), automatischer Minimierung (*Simplest Form*) und menschlich konstruierter Implikationslogik.
* **Effizienzerlebnis:** Erkennen des enormen praktischen Nutzens von Minimierungsverfahren in der Informatik (von einer 32-Zeilen-Matrix über meterlange Normalform-Bandwürmer hin zu 3–4 kompakten Schalttermen).

---

#### Ablauf & Unterrichtsgeschehen

1. **Auftragserteilung & Zielklarheit (ca. 10'):** Die Lehrperson verweist auf den Einstieg der Doppelstunde: *„Zu Beginn schien Situation 10 mit 32 Zeilen unbezwingbar. Jetzt besitzt ihr das mathematische und werkzeugbasierte Rüstzeug, um diese Grosskreuzung vollständig zu steuern.“* Der Arbeitsauftrag für Übung II wird freigegeben.
2. **Exploration & Analyse im Tandem (ca. 30'):** Die Schülerpaare bearbeiten **Aufgabe 5**. Sie erforschen zunächst das Verhalten von *LogicTraffic* bei der automatischen Generierung von KDNF und KKNF an 16 resp. 32 Zeilen. Anschliessend nutzen sie die Funktion *Simplest* und versuchen im Team, eine eigene kompakte Implikationsformel (`→`) zu konstruieren, die vom Polizisten mit 🫡 `Optimal` bewertet wird.
3. **Didaktische Zwischenbegleitung:** Die Lehrperson unterstützt leistungsschwächere Gruppen bei der Identifikation der Konfliktachsen in *Situation 10* (Spur $E$ kollidiert mit $A, B, C$; Spur $A$ kollidiert mit $C, D$). Schnellere Tandems werden herausgefordert, ihre eigene Implikationsformel zeichenweise mit der *Simplest Form* der Software zu messen.
4. **Ergebnissicherung im Tandem (ca. 15'):**  
    Die Schülerpaare tragen ihre finalen Formelausdrücke und die Erkenntnisse zum Unterschied zwischen CDNF, CCNF und minimierter Form in ihr Portfolio ein.

---

!!! quote "Einstieg"

    Nun kehren wir zu den grossen Kreuzungen zurück: **Situation 10** besitzt 5 Fahrspuren ($A, B, C, D, E$) und eine Wahrheitstabelle mit $2^5 = 32$ Zeilen. Die manuelle Eingabe jeder Zeile wäre fehleranfällig und zeitraubend. Ihr nutzt nun die kanonischen Normalformen und logische Minimierungsverfahren, um die Signalanlage fehlerfrei und optimal zu programmieren.

!!! quote "Aufgabe 1"

    1. Öffnet in *LogicTraffic* die **Situation 10**.
    2. Stellt sicher, dass die Spalte `sicher` vollständig ausgefüllt ist.
    3. Erkundung der Normalformen: Öffnet das Dropdown-Menü oberhalb des Formelfeldes und vergleicht die Formeln:

       * Wählt **KDNF**: Wie viele Konjunktions-Klammern (`∧`) werden mit ODER (`∨`) aneinandergereiht? Welcher Anzahl an Tabellenzeilen entspricht dies?
       * Wählt **KKNF**: Wie viele Disjunktions-Klammern (`∨`) werden mit UND (`∧`) verknüpft? Warum ist die KKNF bei Situation 10 deutlich kürzer als die KDNF?
       * Klickt auf **In Wahrheitstabelle laden**: Welchen Status zeigt der Polizist bei beiden Formen an?

!!! quote "Aufgabe 2"

    Die Minimierungs-Maschine: Wählt im Menü die Option **Simplest**:
       
       * Wie drastisch verkürzt *LogicTraffic* den Ausdruck?
       * Testet die Formel mit einem Klick auf **prüfen**.

!!! quote "Aufgabe 3"

    Versucht nun, selbst eine kurze, lesbare Formel mit Implikationen (`→`) zu verfassen, die Situation 10 steuert:
       * *Schritt 1:* Welche Spuren schneidet die Querspur $E$? Schreibt die Bedingung: `E → (...)`
       * *Schritt 2:* Welche Spuren schneidet Spur $A$? Schreibt die Bedingung: `A → (...)`
       * *Schritt 3:* Verknüpft beide Bedingungen mit `∧` und klammert sauber: `(...) ∧ (...)`
       * Erreicht eure eigene Formel ebenfalls den Status 🫡 **Optimal**?

??? tip "Hinweis zu den Konflikten in Situation 10"

    Analysiert die Geometrie der Kreuzung genau:

    * Spur $E$ kreuzt die Spuren $A$, $B$ und $C$. Wenn $E$ fährt, müssen also alle drei stehen: `E → (¬A ∧ ¬B ∧ ¬C)`.
    * Spur $A$ kreuzt neben $E$ auch die Spur $C$ und die Spur $D$: `A → (¬C ∧ ¬D)`.
    * Prüft, ob damit bereits alle Konfliktpunkte der Kreuzung abgesichert sind!

??? success "Musterlösung & didaktischer Erwartungshorizont"

    * Vergleich CDNF vs. CCNF bei Situation 10:  

        * Die **KDNF** besteht aus vielen Mintermen (erlaubte Kombinationen), was zu einem extrem langen Bandwurm-Ausdruck führt.  
        * Die **KKNF** ist deutlich kompakter, da es auf dieser Kreuzung verhältnismässig wenige verbotene Kollisionspaare gibt.  
        * Beide Normalformen führen nach dem Laden zum Status Optimal.

    * Simplest Form: *LogicTraffic* reduziert den Ausdruck auf wenige verknüpfte Terme (oft in Form optimierter Disjunktionen nach dem Quine-McCluskey-Verfahren), z. B.: `¬E ∧ ¬A ∨ ¬E ∧ ¬C ∨ ...`
    * Selbst erstellte Implikationsformel (Musterlösung): `(E → ¬A ∧ ¬B ∧ ¬C) ∧ (A → ¬C ∧ ¬D)`
        *Ergebnis:* Der Polizist salutiert (Optimal).  
        *Fazit:* Mit nur zwei überschaubaren Implikations-Klammern lässt sich die gesamte 32-Zeilen-Kreuzung mathematisch perfekt und ohne Sicherheitslücken beherrschen.

??? info "Didaktischer Kommentar"

    In dieser Übungsphase schliesst sich der motivationale Kreis der Unterrichtseinheit. Die Schülerinnen und Schüler erleben die Überlegenheit der formalen Logik gegenüber der Datenmatrix: Wo eine Wahrheitstabelle 32 Zeilen verlangt und eine CDNF unlesbar lang wird, genügt eine präzise formulierte Implikationsregel aus zwei geklammerten Bedingungen. Dies vermittelt ein tiefes Verständnis für Abstraktion als Problemlösewerkzeug der Informatik.

    * CDNF vs. CCNF als Entwurfsentscheidung: An *Situation 10* erkennen die Lernenden, warum Ingenieure Sicherheitsanforderungen fast immer als **CCNF (Verbotsliste / Maxterme)** oder als **Implikationen** modellieren: In sicherheitskritischen Systemen gibt es meist wesentlich weniger verbotene Ausnahmezustände (Crashes) als erlaubte Betriebszustände. Die Verbotslogik skaliert im Strassenverkehr daher um ein Vielfaches besser als die Aufzählung aller erlaubten Kombinationen.

??? info "Differenzierung in der Transferphase:"

    * *Basisanforderung:* Nutzung der Dropdown-Werkzeuge (CDNF, CCNF, Simplest), Laden in die Tabelle und Interpretation der Statusmeldung des Polizisten.  
    * *Erweiterte Anforderung:* Eigenständiges Aufstellen der Implikationsformel `(E → ¬A ∧ ¬B ∧ ¬C) ∧ (A → ¬C ∧ ¬D)` und Verifikation der Vollständigkeit über das Simulations-Feedback.

### Phase 6: Sicherung, Bilanzierung & Abschlussaufgabe

**Sozialform / Medien:** Moderierte Bilanzierung im Plenum, anschliessend Einzelarbeit zur individuellen Portfolio-Sicherung; Beamer / Tafel, Begleitportfolio / Merkheft.

**Didaktische Absicht:**

* **Gesamtsynthese** Reflexion des Weges vom ikonischen Handeln über die Wahrheitstabelle (Stufe *Strukturieren*) bis zur formalen Aussagenlogik und den Normalformen (Stufe *Formalisieren*).
* **Repräsentationsvergleich:** Systematische Gegenüberstellung von *Wahrheitstabelle*, *KDNF*, *KKNF* und *minimierter Form* hinsichtlich Skalierung, Lesbarkeit und Maschinentauglichkeit.
*  **Festigung von Konzeptwissen:** Verbindliche Dokumentation von De Morgans Gesetzen, der Normalformen-Definitionen und der Rangfolge der Junktoren als überdauerndes Informatikwissen.

---

#### Ablauf & Unterrichtsgeschehen

1. **Plenumsbilanzierung & Repräsentationsvergleich (ca. 10'):**  
    Die Lehrperson projiziert nebeneinander die drei Lösungsformen für *Situation 10* an die Wand:  

    * Die 32-Zeilen-Wahrheitstabelle.  
    * Die automatisch generierte CDNF / CCNF (Bandwurm-Ausdrücke).  
    * Die handoptimierte Implikationsregel `(E → ¬A ∧ ¬B ∧ ¬C) ∧ (A → ¬C ∧ ¬D)`.

    *Impulsfrage:* „Wenn ihr Chef-Entwickler/in für ein autonomes Verkehrsleitsystem wärt: Welche dieser Darstellungen baut ihr in den Steuerungs-Chip ein – und warum?“

2. **Fachlicher Diskurs im Plenum (ca. 3'):**  
    Die Klasse arbeitet die Stärken und Schwächen der Repräsentationen heraus: Tabellen sind lückenlos, explodieren aber speichertechnisch ($2^n$); Normalformen lassen sich mechanisch vom Computer erzeugen, sind aber unlesbar; optimierte logische Regeln benötigen minimalen Speicher und sind in Echtzeit berechenbar.

3. **Individuelle Abschlussaufgabe & Portfolio-Eintrag (ca. 15'):**  
    Die Lernenden bearbeiten die abschliessende Experten-Synthese (Aufgabe 6) in Einzelarbeit und vervollständigen ihr erweitertes Merkblatt im Begleitportfolio.

---

**Phase:** Abschluss & Synthese | **Modus:** Einzelarbeit / Portfolio | **Zeit:** ca. 10 Min. | **Fokus:** Konzeptwissen & Repräsentationsvergleich[cite: 3, 5]
!!! quote "Kontext:"

    Ihr habt den gesamten Weg gemeistert: Von der visuellen Simulation über die Wahrheitstabelle bis hin zu den mathematischen Normalformen und kompakten Schaltregeln. Zum Abschluss vergleichen wir die Werkzeuge der Informatik und sichern das Gelernte für euer Portfolio.

!!! quote "Teil A: Der Grosse Repräsentationsvergleich"

    Vergleicht die vier Darstellungsformen, die ihr in *LogicTraffic* kennengelernt habt, und füllt die Tabelle in euren Notizen aus:

    | Darstellungsform | Wie entsteht sie? | Vorteil | Nachteil / Grenze |
    | :--- | :--- | :--- | :--- |
    | **Wahrheitstabelle** | Manuelles Durchtesten aller Zustände[cite: 5]. | Lückenlos und sehr übersichtlich bei 2–3 Spuren. | ... *(Tipp: Zeilen bei 10 Spuren?)* |
    | **CDNF** (Disjunktive Normalform) | Automatisch aus allen Zeilen mit `sicher = 1`. | Vollautomatisch erzeugbar (Positivliste aller Fahrzustände). | ... *(Tipp: Länge des Ausdrucks?)* |
    | **CCNF** (Konjunktive Normalform) | Automatisch aus allen Zeilen mit `sicher = 0`. | ... *(Tipp: Anzahl der Crashes im Verkehr)* | Für Menschen schwer zu lesen; benötigt Klammern. |
    | **Optimierte Regel** (Implikationen `→`) | Logisches Zerlegen der Konfliktachsen im Kopf. | Extrem kompakt, schnell auf dem Chip berechenbar[cite: 5]. | Erfordert Denkaufwand beim Menschen (nicht rein mechanisch). |


!!! quote "Teil B: Das Experten-Merkblatt (Portfolio)"

    Ergänzt euer Merkblatt im Begleitportfolio um die formalen Gesetze der Logik:
    
    1. **De Morgan'sche Gesetze:** Notiert die beiden Umformungsregeln für die Verkehrslogik:
       
       * `¬(A ∧ B) ≡ ...` *(„Beide dürfen nicht gleichzeitig fahren ist identisch mit ...“)*
       * `¬(A ∨ B) ≡ ...` *(„Weder A noch B dürfen fahren ist identisch mit ...“)*
    
    2. **Normalformen auf den Punkt gebracht:**
       
       * Was ist ein **Minterm** (CDNF) und wofür steht er im Strassenverkehr?
       * Was ist ein **Maxterm** (CCNF) und wovor schützt er im Strassenverkehr?
    
    3. **Abschlussreflexion:** Warum sind logische Formeln die universelle Grundlage für jede spätere Computerprogrammierung (z. B. in Python, Java oder C)?


??? tip "Denkhilfe zu Teil B"
    
    * Denkt an die Bausteine: Ein Minterm verknüpft Variablen mit UND (`A ∧ B ∧ ¬C`) und beschreibt eine exakte Schaltung.
    * Maxterme verknüpfen negierte Variablen mit ODER (`¬A ∨ ¬C`) und schliessen eine konkrete Crash-Gefahr aus.

??? success "Musterlösung & Tafelbild (Inhalt des erweiterten Merkblatts)"

        1. Repräsentationsvergleich:

           * Wahrheitstabelle: Vollständig, aber skaliert exponentiell (2^n Zeilen; unbrauchbar ab ca. 5–6 Spuren).
           * KDNF (Disjunktive Normalform): ODER-Verknüpfung aller erlaubten Minterme (Positivliste; oft extrem lang).
           * KKNF (Konjunktive Normalform): UND-Verknüpfung aller verbotenen Maxterme (Sicherheitsliste; im Verkehr oft kompakter als CDNF).
           * Minimierte Regel: Logische Vereinfachung (z. B. via Implikation A → ¬B); ideal für Steuerungs-Chips.

        2. Die Gesetze von De Morgan:
           
           * `¬(A ∧ B) ≡ ¬A ∨ ¬B` („Es dürfen nicht beide grün haben“ ≡ „Mindestens einer muss rot haben“)
           * `¬(A ∨ B) ≡ ¬A ∧ ¬B`  („Weder A noch B dürfen grün haben“ ≡ „Sowohl A als auch B müssen rot haben“)

        3. Normalformen im Verkehrskontext:
           
           * Minterm (in KDNF): Eine UND-Klammer über alle Spuren, die genau eine sichere Verkehrskombination freigibt.
           * Maxterm (in KKNF): Eine ODER-Klammer über alle Spuren, die genau eine tödliche Kollision zuverlässig sperrt.

        4. Fazit für die Informatik:
           Aussagenlogische Bedingungen steuern jeden Algorithmus: Jede if-Abfrage in Programmiersprachen (Python, Java) und jedes Transistor-Schaltnetz in Computerprozessoren basiert exakt auf diesen Gesetzmässigkeiten.

#### Fachdidaktischer Kommentar für Lehrpersonen

* **Synthese und 'Kollation' nach Zendler:**  
    Der Phasenabschluss folgt dem didaktischen Prinzip der Kollation und Erweiterung der Wissensbasis nach Zendler: Die Schülerinnen und Schüler vergleichen ihre handlungsorientierten Teillösungen systematisch mit den idealtypischen, standardisierten Strukturen der Fachwissenschaft (Kanonische Normalformen, De Morgan).
* **Förderung von Selbsterklärungen (*Self-Explanation-Effekt* nach Chi et al.):**  
    Das synoptische Gegenüberstellen von Wahrheitstabelle, CDNF, CCNF und Implikationsformel regt gezielte Selbsterklärungen an. Die Lernenden begreifen nicht nur rein rezeptiv *wie* man umformt, sondern *warum* unterschiedliche Repräsentationen existieren und wann welche Form informatikpraktisch überlegen ist (Trade-Off zwischen Rechenaufwand, Speicherbedarf und Wartbarkeit).
* **Nachhaltige Sicherung von 'Konzeptwissen':**  
    Die Erarbeitung der Normalformen und der De Morgan'schen Gesetze verhindert, dass die Doppelstunde als reine „Software-Schulung“ für *LogicTraffic* wahrgenommen wird. Der Ausblick auf Programmiersprachen (Verzweigungen, Boolean Logic) und Hardware-Entwurf (Schaltnetze) schlägt die Brücke zu den Kernkompetenzen gymnasialer und sekundarer Informatiklehrpläne.