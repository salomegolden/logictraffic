# Aussagenlogische Formeln und Boolsche Algebra

Die formale Logik bildet eine der zentralen Fundamentalen Ideen der Informatik (nach Schwill sowie Hartmann et al. [^1]): Sie spannt das Fundament von der mathematischen Modellierung realer Systeme über Algorithmen bis hin zum Hardware- und Datenbankentwurf.  

In LogicTraffic repräsentieren Formeln das Formalisieren. Während [Wahrheitstabellen](../anhang/glossar.md#wahrheitstabelle) der vollständigen Erfassung aller Zustände dienen (Strukturieren), ermöglichen Formeln eine kompakte, deklarative und rechenbare Steuerung der Lichtsignalanlage. [^1], [^2].

## Didaktischer Sinn: Vom Tabellenumweg zur Steuerungsregel

In komplexeren Verkehrssituationen (z. B. Situation 10 mit 5 Spuren und 32 Zeilen) stösst die manuelle Tabellenpflege an ihre Grenzen. An dieser Stelle motiviert der Lehrerkommentar den Wechsel zur Formel:

Lernende erkennen, dass eine Ampelsteuerung nicht den gesamten Tabellenverlauf im Speicher halten muss, sondern anhand einer handlungsorientierten Regel wie z. B. $C \rightarrow (\neg A \land \neg B)$ in Echtzeit prüft, ob die Schaltung kollisionsfrei ist.  

## Der Zeichenvorrat im LogicTraffic-Formeleditor

Im Formeleditor von LogicTraffic stehen ausschliesslich die folgenden Symbole und Operatoren zur Verfügung [^4]:

| Symbol | Bezeichnung | Verkehrsbedeutung in LogicTraffic |
| --- | --- | --- |
| $A, B, C, D, E$ | Fahrspuren (Variablen) | Repräsentieren die einzelnen Spuren bzw. Signalgeber der Kreuzung. |
| $1$ | Wahrheitswert 1 (true) | Grün: Freie Fahrt für die entsprechende Spur. |
| $0$ | Wahrheitswert 0 (false) | Rot: Haltegebot für die entsprechende Spur. |
| $\neg$ | Negation (NICHT) | $\neg A$ bedeutet: „Spur $A$ hat Rot (kein Grün)“. |
| $\land$ | Konjunktion (UND) | $A \land B$ bedeutet: „Spur $A$ und $B$ haben gleichzeitig Grün“ (Kollisionszustand bei schneidenden Spuren). |
| $\lor$ | Disjunktion (ODER) | $\neg A \lor \neg B$ bedeutet: „Mindestens eine der Spuren $A$ oder $B$ muss Rot haben“ (Kollisionsvermeidung). |
| $\rightarrow$ | Implikation (WENN ... DANN) | $A \rightarrow \neg B$ bedeutet: „Wenn Spur $A$ Grün hat, dann muss Spur $B$ Rot haben“. |
| $( \quad )$ | Klammern | Legen die Auswertungsreihenfolge verbindlich fest. |

!!! tip "Vorrangregeln der Operatoren"

    Wird auf Klammern verzichtet, wertet LogicTraffic streng nach Priorität aus:

    $$\neg \quad \text{vor} \quad \land \quad \text{vor} \quad \lor \quad \text{vor} \quad \rightarrow$$

    ??? example "Beispiel" 
        $\neg A \lor B \land C$ wird ausgewertet als $(\neg A) \lor (B \land C)$. Zur Vermeidung von Schülerfehlern empfiehlt sich im Unterricht das explizite Setzen von Klammern.  

## Rechenregeln der Booleschen Algebra im Verkehrsbezug 

Mithilfe der Booleschen Algebra können Steuerungsformeln formal vereinfacht werden, ohne die Kollisionsfreiheit der Kreuzung zu verändern (logische Gleichwertigkeit $\equiv$) [^2], [^3].

| Gesetz |  Formel | Bedeutung an der Kreuzung in LogicTraffic |
| --- | --- | --- |
| De Morgan | $\neg (A \land B) \equiv \neg A \lor \neg B$ | Wandelt das Verbot eines gemeinsamen Unfalls ($\neg(A \land B)$) direkt in eine steuerungstechnische Regel um: Mindestens eine Spur muss zwingend Rot zeigen. |
| Absorption | $A \land (A \lor B) \equiv A$  $\neg A \land (\neg A \lor \neg B) \equiv \neg A$ | Streicht überflüssige Zusatzbedingungen: Schreibt eine übergeordnete Regel bereits strikt Rot für Spur $A$ vor ($\neg A$), ist die weichere Kollisionsbedingung mit Nachbarspur $B$ automatisch mitabgedeckt und fällt weg. |
| Komplement | $A \land \neg A \equiv 0$  $A \lor \neg A \equiv 1$ | Eine Ampel kann nicht gleichzeitig Grün und Rot zeigen ($0$). Zu jedem Zeitpunkt gilt: Eine Spur ist entweder Grün oder Rot ($1$). |
| Doppelnegation | $\neg \neg A \equiv A$ | Das Aufheben eines Haltegebots entspricht der Freigabe (Grün). |

## Die 6 Formel-Formen in LogicTraffic

Über das Dropdown-Menü oberhalb des Formelfelds generiert LogicTraffic aus der Wahrheitstabelle automatisch sechs standardisierte Formeldarstellungen:

=== "KDNF"

    --8<-- "code/includes/begriffe.md:kdnf"

=== "KKNF"

    --8<-- "code/includes/begriffe.md:kknf"

=== "KNF"

    --8<-- "code/includes/begriffe.md:knf"

=== "DNF"

    --8<-- "code/includes/begriffe.md:dnf"

=== "Implikationsform"

    --8<-- "code/includes/begriffe.md:implikationsformel"

=== "Einfachste Form"

    --8<-- "code/includes/begriffe.md:einfachste_form"

Mehr dazu [hier](normalformen.md).

## Typische Hürden und didaktische Hinweise

??? warning "Didaktischer Hinweis: Das Verständnis der Implikation ($A \rightarrow \neg B$)"

    * Schwierigkeit: Lernende verstehen oft nicht, warum die Formel $A \rightarrow \neg B$ wahr ($1$) ist, wenn Spur $A$ Rot hat ($A=0$). Im Alltag wird vermutet, dass dann auch $B$ nicht fahren darf.
    * Erklärungshilfe im Unterricht: Die Regel lautet: „WENN $A$ Grün hat, dann muss $B$ Rot sein.“ Wenn $A$ an der roten Ampel wartet ($A=0$), droht von Spur $A$ gar keine Gefahr. Die Bedingung ist somit nicht verletzt, und Spur $B$ darf problemlos Grün erhalten.

??? note "Didaktischer Hinweis: Einsatz des Parsebaums"

    Über die Schaltfläche Parsebaum zeigt LogicTraffic die Formel wahlweise als binären oder $n$-ären Strukturbaum an. Dies hilft insbesondere Schülerinnen und Schülern mit Schwierigkeiten bei der Klammersetzung zu erkennen, welche Teilformeln zuerst ausgewertet werden.

[^1]: Hartmann, W., Jäckel, S., Näf, M., & Reichert, R. (2026). Informatikunterricht planen und durchführen. Springer. https://doi.org/10.1007/978-3-662-72786-7
[^2]: Arnold, R., & Hartmann, W. (2007). LogicTraffic – Logik in der Allgemeinbildung. Informatik-Spektrum, 30(1), 19–26. https://doi.org/10.1007/s00287-006-0123-7
[^3]: Junker, M. (2025). Logik für die Informatik: Eine Einführung in die Aussagenlogik, Prädikatenlogik und Berechenbarkeitstheorie. Springer Berlin Heidelberg. https://doi.org/10.1007/978-3-662-70825-5
[^4]: Arnold, R., Langheinrich, M., & Hartmann, W. (2007). InfoTrafﬁc – Teaching Important Concepts of Computer Science and Math through Real-World Examples.
