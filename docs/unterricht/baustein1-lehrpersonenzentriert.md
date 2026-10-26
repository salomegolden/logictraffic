# Baustein 1b – Kreuzungen anhand von Darstellungen untersuchen

??? example "Lehrpersonenkommentar als Download"

    [Kommentar für die Lehrperson (PDF)](../downloads/baustein1/v1/baustein1-darstellungen-lehrpersonenkommentar.pdf)

Die Lernenden untersuchen anhand statischer Kreuzungsbilder, welche Fahrwege miteinander im Konflikt stehen und welche Ampelbelegungen sicher sind. Die Lehrperson erläutert die Modellannahmen und führt ein Verfahren zur Sicherheitsbeurteilung vor. Anschliessend wenden die Lernenden dieses Verfahren selbst an, erfassen alle acht Ampelbelegungen einer Kreuzung mit drei Ampeln und begründen ihre Ergebnisse.

Dieser Baustein ist eine Alternative zum [enaktiven Einstieg (Baustein 1a)](baustein1-enaktiv.md). Beide Einstiege verfolgen dieselben fachlichen Kernziele und bereiten die anschliessende Arbeit mit LogicTraffic vor. Hier arbeiten die Lernenden mit Bildern, sprachlichen Erklärungen und Tabellen. Fahrzeuge und Ampelplättchen werden nicht bewegt.

Die Einträge werden zunächst mit **Rot** und **Grün** bezeichnet. Die systematische Verwendung von `0` und `1`, formale Operatoren und aussagenlogische Formeln folgen in den gemeinsamen Folgebausteinen.

??? abstract "Auf einen Blick"

    **:busts_in_silhouette: Zielgruppe:** Gymnasiale Klassen der 8.–9. Schulstufe ohne Vorkenntnisse in Aussagenlogik

    **:stopwatch: Dauer:** Die Einzelzeiten des Kommentars ergeben **70–85 Minuten**, einschliesslich Einführung und Abschluss. Der Kommentar enthält abweichende Gesamtangaben; siehe [Zeitplanung](#zeitplanung). Der gemeinsame Logikblock benötigt zusätzlich 10–15 Minuten.

    **:computer: Computer:** Nur für die Präsentation durch die Lehrperson; keine Bedienung von LogicTraffic durch die Lernenden

    **:brain: Vorwissen:** Kein Vorwissen erforderlich

    **:package: Material:** Präsentation mit statischen Kreuzungsbildern, ein Dossier pro Person, Schreibzeug sowie Tafel oder Visualizer

??? example "Materialhinweise und Downloads"

    - [:memo: Dossier für Lernende (PDF)](../downloads/baustein1/v1/baustein1-darstellungen-dossier.pdf)
    - [:ledger: Kommentar für die Lehrperson (PDF)](../downloads/baustein1/v1/baustein1-darstellungen-lehrpersonenkommentar.pdf)
    - [:film_projector: Präsentation (PDF)](../downloads/baustein1/v1/baustein1-darstellungen-praesentation.pdf)

    Das Dossier enthält **AB1a auf S. 2**, **AB1b auf S. 3**, **AB1c auf S. 4–5**, **AB1d auf S. 6** und **AB1X auf S. 7**. Die Präsentation für AB1X ist auf der [gemeinsamen Unterseite](baustein1-logikblock.md#material) verlinkt.

    **Baustein 1b** bezeichnet diese Einstiegsvariante. **AB1b** ist das Arbeitsblatt «Ampelbelegungen beurteilen» innerhalb dieses Dossiers. Die gleich nummerierten Arbeitsblätter des enaktiven Einstiegs gehören zu dessen eigener Materialvariante.

## Lernziele

??? success "Bezug zur Unterrichtseinheit"

    **LZ1a · Verkehrssituationen und Darstellungen deuten:** Die Lernenden erkennen Fahrwege und Konfliktpaare und unterscheiden sichere von unsicheren Ampelbelegungen begründet.

    **Vorbereitung auf LZ1b · Alle möglichen Ampelbelegungen systematisch erfassen:** Die Lernenden ordnen Belegungen für zwei und drei Ampeln vollständig und ohne Wiederholungen, bewerten sie anhand der Fahrwege und erläutern ihr Ordnungsmuster. Im Dossier erfassen sie alle acht Belegungen für drei Ampeln.

    **Vorbereitung auf LZ2 · Sicherheitsregeln entwickeln & in Formeln übersetzen:** Die Lernenden beschreiben die Konflikte einer einfachen Kreuzung mit bis zu drei unabhängig schaltbaren Ampeln in eigenen Worten.

??? success "Gemeinsame Lernziele beider Einstiege"

    Die Lernenden können …

    - vorgegebene Fahrwege in einem Kreuzungsbild verfolgen und Konfliktpaare erkennen;
    - erklären, dass eine Ampelbelegung für jede betrachtete Ampel Rot oder Grün festlegt;
    - sichere und unsichere Ampelbelegungen anhand der gleichzeitig freigegebenen Fahrwege begründet unterscheiden;
    - erklären, weshalb mehrere grüne Ampeln sicher sein können und weshalb «alle Rot» sicher ist;
    - alle acht Ampelbelegungen einer Kreuzung mit drei unabhängig schaltbaren Ampeln vollständig und ohne Wiederholungen erfassen;
    - jede dieser Ampelbelegungen als sicher oder unsicher beurteilen;
    - erklären, wie ihre Ordnung das Vergessen und doppelte Erfassen von Belegungen verhindert;
    - für ein Konfliktpaar eine Sicherheitsregel in eigenen Worten formulieren.

    **Lernnachweis:** Jede Person hält die Konfliktpaare fest, beurteilt Ampelbelegungen mit Begründung, vervollständigt die Tabelle mit allen acht Belegungen und deren Sicherheitsbeurteilung und formuliert eine sprachliche Sicherheitsregel.

## Vorbereitung

??? example "Präsentation und Unterrichtsmaterial vorbereiten"

    Das [Dossier](../downloads/baustein1/v1/baustein1-darstellungen-dossier.pdf) für jede Person ausdrucken. Die [Präsentation](../downloads/baustein1/v1/baustein1-darstellungen-praesentation.pdf) öffnen und die Lesbarkeit der Ampelbezeichnungen vom hinteren Teil des Unterrichtsraums aus prüfen.

    Als Grundsituation dient die Kreuzung mit drei festgelegten Fahrwegen:

    - **C:** von links geradeaus nach rechts;
    - **D:** von unten geradeaus nach oben;
    - **E:** von rechts geradeaus nach links.

    C und E verlaufen auf getrennten Fahrspuren. D kreuzt die Fahrwege von C und E. Die Konfliktpaare sind **C–D** und **D–E**; **C–E ist konfliktfrei**. Diese Zuordnung bleibt in Dossier und Präsentation unverändert.

    Die Fahrwegfarben unterscheiden die Fahrwege. Ob ein Fahrweg freigegeben ist, zeigt ausschliesslich die zugehörige Ampel. Die Lehrperson hält die [Lösungsvorlage](#losungen-und-ergebnissicherung) bereit und zeigt Lösungen erst nach der jeweiligen Bearbeitungszeit.

??? tip "Modellannahmen für beide Einstiege"

    - Jeder betrachtete Fahrweg besitzt eine eigene Ampel. Die drei Ampeln können unabhängig voneinander Rot oder Grün zeigen.
    - Grün bedeutet: Der zugehörige Fahrweg ist freigegeben. Rot bedeutet: Der zugehörige Fahrweg ist gesperrt.
    - Innerhalb einer untersuchten Situation bleiben die Fahrwege unverändert.
    - Zwei Fahrwege stehen im Konflikt, wenn bei gleichzeitiger Freigabe eine Kollision möglich ist. Dazu können auch Fahrwege gehören, die in dieselbe Fahrspur zusammenführen.
    - Die zufällige Anwesenheit von Fahrzeugen, zeitliche Abstände, zusätzliche Vortrittsregeln und Ausweichmanöver werden nicht berücksichtigt.
    - Eine **Ampelbelegung** legt für jede betrachtete Ampel Rot oder Grün fest. Ein **sicherer Kreuzungszustand** liegt vor, wenn bei dieser Ampelbelegung zwischen den gleichzeitig freigegebenen Fahrwegen keine Kollision möglich ist.
    - «Alle Rot» ist sicher, obwohl kein Fahrzeug fahren darf. Sicherheit und Verkehrsfluss sind unterschiedliche Fragen.

## Unterrichtsablauf – Übersicht

Alle Verweise auf die Präsentation nennen die **PDF-Seite einschliesslich Titelseite**. So lassen sich die Inhalte trotz abweichender Folienverweise im Kommentar eindeutig finden.

| Abschnitt | Inhalt | Richtzeit |
| --- | --- | --- |
| Einführung | Dossier ausgeben und Arbeitsweise erläutern; Präsentation S. 1–2 | 3 Min. |
| 1. Fahrwege untersuchen | AB1a, Aufgaben 1–3, Dossier S. 2; Präsentation S. 3–6 | 15–20 Min. |
| 2. Sichere Ampelbelegungen beurteilen | AB1b, Aufgabe 1, Beispiele 1 und 2, Dossier S. 3; Präsentation S. 7–13 | 20 Min. |
| 3. Alle Möglichkeiten erfassen | AB1c, Aufgabe 1 auf S. 4, Aufgaben 2–4 auf S. 5; Präsentation S. 14–19 | 20–25 Min. |
| 4. Ergebnisse sichern und Ausblick | AB1d, Aufgaben 1–4, Dossier S. 6; Präsentation S. 20–22 | 10–15 Min. |
| Abschluss | Materialien versorgen | 2 Min. |
| **Gesamt** | **Summe der Einzelzeiten; abweichende Angaben im Kommentar siehe unten** | **70–85 Min.** |

Zusätzlich im gemeinsamen weiteren Unterricht:

| Abschnitt | Inhalt | Richtzeit |
| --- | --- | --- |
| [Gemeinsamer Logikblock](baustein1-logikblock.md) | AB1X, Aufgabe 1, Dossier S. 7; Präsentation «Erweiterung Logik», S. 1–5 | zusätzlich 10–15 Min. |

Der Logikblock und die optionalen Erweiterungen der Differenzierung sind nicht in der Gesamtzeit enthalten.

### Zeitplanung

??? info "Abweichende Gesamtangaben im Kommentar"

    Die Einzelzeiten auf **S. 3** des [Kommentars](../downloads/baustein1/v1/baustein1-darstellungen-lehrpersonenkommentar.pdf#page=3) ergeben **70–85 Minuten**: 3 + (15–20) + 20 + (20–25) + (10–15) + 2.

    Die dort gedruckte Gesamtzeile nennt **60–85 Minuten**, «Auf einen Blick» auf **S. 1** nennt **70–90 Minuten**, und die Abgrenzung zum Logikblock auf **S. 9** nennt **70–85 Minuten**. Die Tabelle dieser Seite weist die berechnete Summe ausdrücklich aus; die widersprüchlichen Gesamtangaben bleiben damit nachvollziehbar. Die einzelnen Phasenzeiten wurden nicht verändert.

## Durchführung

### Einführung

??? info "Organisation"

    **Sozialform:** Plenum

    **Benötigte Zeit:** 3 Minuten

    Die Lehrperson gibt die Dossiers aus, erläutert die Arbeitsweise mit Bildern und Tabellen und öffnet die Präsentation auf **S. 1–2**. Die Frage nach der Aufgabe von Ampeln führt zum Kreuzungsproblem.

### Phase 1 – Fahrwege untersuchen

??? success "Ziele der Einheit"

    Die Lernenden verfolgen die drei vorgegebenen Fahrwege und bestimmen, welche Fahrwegpaare miteinander im Konflikt stehen.

??? example "Material"

    - Präsentation, PDF-S. 3–6
    - AB1a «Ampelbelegungen kennenlernen», Aufgaben 1–3, Dossier S. 2
    - Schreibzeug

??? info "Organisation"

    **Sozialform:** Gemeinsame Einführung im Plenum, anschliessend Einzelarbeit mit kurzem Partnervergleich

    **Benötigte Zeit:** 15–20 Minuten

??? abstract "Verlaufsplanung"

    **1. Problem erläutern – 2 Minuten:** Das Kreuzungsbild auf **Präsentation S. 3** zeigen und fragen: «Welche Fahrwege dürfen gleichzeitig freigegeben sein, ohne dass eine Kollision möglich ist?»

    **2. Modell klären – 4 Minuten:** Mit **S. 4** die Ampeln und Modellannahmen erklären. Einen Fahrweg gemeinsam von der Zufahrt bis zur Ausfahrt verfolgen. Die Konfliktpaare noch nicht vorgeben.

    **3. Fahrwege untersuchen – 6–9 Minuten:** Die Lernenden bearbeiten **AB1a, Aufgaben 1–3, Dossier S. 2**, zunächst allein. Sie beschreiben C, D und E, prüfen alle drei Fahrwegpaare, markieren Konfliktstellen und begründen ein Konfliktpaar. Danach kurzer Partnervergleich. **Präsentation S. 5** mit dem Arbeitsauftrag bleibt sichtbar.

    **4. Ergebnisse besprechen – 3–5 Minuten:** Beurteilungen sammeln und mit **S. 6** auswerten. Die Konfliktstellen im Bild markieren: C–D und D–E stehen im Konflikt; C–E ist konfliktfrei.

??? tip "Didaktische Hinweise"

    Die Lernenden sollen die Fahrwege selbst nachvollziehen. Die Lehrperson gibt das Modell vor, nimmt ihnen aber nicht die gesamte Sicherheitsanalyse ab. Ein geometrischer Schnittpunkt ist relevant, wenn sich die Fahrwege im Modell auf derselben Ebene begegnen.

??? question "Differenzierung"

    === "Vereinfachungen"

        - Fahrwege einzeln hervorheben.
        - Satzstarter anbieten: «Der Fahrweg C führt von … nach …».

    === "Erweiterungen"

        - Begründen lassen, weshalb entgegengesetzte Fahrtrichtungen auf getrennten Spuren nicht automatisch einen Konflikt bilden.

### Phase 2 – Sichere Ampelbelegungen beurteilen

??? success "Ziele der Einheit"

    Die Lernenden beurteilen vollständige Ampelbelegungen und begründen ihre Entscheidung anhand der freigegebenen Fahrwege.

??? example "Material"

    - Präsentation, PDF-S. 7–13
    - AB1b «Ampelbelegungen beurteilen», Aufgabe 1, Beispiele 1 und 2, Dossier S. 3
    - Schreibzeug

??? info "Organisation"

    **Sozialform:** Kurze Demonstration im Plenum, Einzelarbeit und gemeinsame Auswertung

    **Benötigte Zeit:** 20 Minuten

??? abstract "Verlaufsplanung"

    **1. Vorgehen vormachen – 5 Minuten:** Mit **Präsentation S. 7–9** den Begriff Ampelbelegung und vier Prüfschritte erläutern: Welche Ampeln zeigen Grün? Welche Fahrwege sind freigegeben? Stehen diese Fahrwege im Konflikt? Ist die Ampelbelegung sicher oder unsicher?

    Auf **S. 8** ist nur C freigegeben: C = Grün, D = Rot, E = Rot. Auf **S. 9** sind **C und D** freigegeben: C = Grün, D = Grün, E = Rot. Diese Ampelbelegung ist unsicher, weil C und D im Konflikt stehen.

    **2. Zwei Beispiele beurteilen – 7 Minuten:** Jede Person bearbeitet **AB1b, Aufgabe 1, Beispiele 1 und 2, Dossier S. 3**, selbstständig. Die Lehrperson unterstützt bei der Zuordnung von Ampeln und Fahrwegen. **Präsentation S. 10** zeigt den Arbeitsauftrag.

    **3. Lösungen vergleichen – 5 Minuten:** Mit **S. 11** die Begründungen besprechen. Beispiel 1: D und E zeigen Grün; eine Kollision ist möglich. Beispiel 2: Alle Ampeln zeigen Rot; kein Fahrweg ist freigegeben, die Ampelbelegung ist sicher.

    **4. Mehrere grüne Ampeln prüfen – 3 Minuten:** Auf **S. 12** die Ampelbelegung C = Grün, D = Rot, E = Grün beurteilen lassen und mit **S. 13** auswerten. C und E verlaufen auf getrennten Spuren. Entscheidend sind die Konflikte, nicht allein die Anzahl grüner Ampeln.

??? tip "Didaktische Hinweise"

    Eine unsichere Ampelbelegung ermöglicht eine Kollision; sie bedeutet nicht, dass in jedem konkreten Moment eine Kollision stattfinden muss.

    **Quellenhinweis zu Präsentation S. 9:** Der Satz «Nur der Fahrweg C ist freigegeben» widerspricht dort den Ampelwerten und der richtigen Erklärung rechts. Freigegeben sind **C und D**. Die Originaldatei bleibt unverändert; bei der Präsentation wird dieser Satz richtiggestellt.

??? question "Differenzierung"

    === "Vereinfachungen"

        - Die vier Prüfschritte sichtbar lassen.
        - Satzstarter anbieten: «Die Ampelbelegung ist …, weil …».

    === "Erweiterungen"

        - Die Behauptung «Zwei grüne Ampeln sind immer gefährlich» anhand eines Gegenbeispiels widerlegen.

### Phase 3 – Alle Möglichkeiten erfassen

??? success "Ziele der Einheit"

    Die Lernenden erfassen alle acht Ampelbelegungen vollständig und ohne Wiederholungen, beurteilen jede Belegung und erklären ihre Ordnung.

??? example "Material"

    - Präsentation, PDF-S. 14–19
    - AB1c «Sichere Ampelbelegungen finden», Dossier S. 4–5
    - Schreibzeug

??? info "Organisation"

    **Sozialform:** Kurzes Unterrichtsgespräch, Einzelarbeit mit Partnervergleich und gemeinsame Auswertung

    **Benötigte Zeit:** 20–25 Minuten

??? abstract "Verlaufsplanung"

    **1. Vollständigkeit als Problem aufgreifen – 5 Minuten:** Mit **Präsentation S. 14** nur **AB1c, Aufgabe 1, Dossier S. 4**, bearbeiten lassen. Die Lernenden vermuten die Anzahl möglicher Ampelbelegungen und begründen ihre Überlegung. **Dossier S. 5 bleibt geschlossen.** Anschliessend Vorschläge sammeln, wie sich Wiederholungen und Auslassungen vermeiden lassen.

    **2. Alle Belegungen eintragen – 5–10 Minuten:** Mit **Präsentation S. 15** Dossier S. 5 öffnen lassen. Jede Person trägt für **AB1c, Aufgabe 2**, alle acht Ampelbelegungen in die leere Tabelle ein. Eine nachvollziehbare eigene Ordnung ist zulässig. Bei Bedarf das Verfahren zunächst für zwei Ampeln erläutern und auf drei Ampeln übertragen lassen.

    **3. Sicherheit beurteilen – 5 Minuten:** **AB1c, Aufgabe 3, Dossier S. 5**, mit **Präsentation S. 16** bearbeiten lassen. Jede Tabellenzeile prüfen und «sicher» oder «unsicher» ankreuzen. Bei unsicheren Belegungen mindestens ein gleichzeitig freigegebenes Konfliktpaar notieren; bei sicheren Belegungen einen Strich eintragen.

    **4. Vergleichen und begründen – 5 Minuten:** Mit **Präsentation S. 17** kurz zu zweit vergleichen und **AB1c, Aufgabe 4, Dossier S. 5**, bearbeiten. Erst danach die Lösungstabelle auf **S. 18** zeigen und Abweichungen am Kreuzungsbild klären. Mit **S. 19** erläutern lassen, weshalb die Ordnung vollständig ist.

??? tip "Didaktische Hinweise"

    Zuerst werden die möglichen Ampelbelegungen erfasst, anschliessend wird deren Sicherheit beurteilt. Acht ausgefüllte Zeilen allein belegen keine Vollständigkeit: Es dürfen keine Belegungen doppelt vorkommen.

??? question "Differenzierung"

    === "Vereinfachungen"

        - Zunächst C auf Rot festhalten und alle vier Belegungen von D und E erfassen.
        - Danach C auf Grün setzen und dieselben vier Belegungen wiederholen.

    === "Erweiterungen"

        - Erklären lassen, wie viele Belegungen bei einer vierten unabhängig schaltbaren Ampel hinzukommen und weshalb sich die Anzahl verdoppelt.

### Phase 4 – Ergebnisse sichern und Ausblick

??? success "Ziele der Einheit"

    Die Lernenden erklären die Sicherheitsbeurteilung, formulieren eine Sicherheitsregel und erläutern den Nutzen einer systematischen Ordnung.

??? example "Material"

    - Präsentation, PDF-S. 20–22
    - AB1d «Was hast du verstanden?», Aufgaben 1–4, Dossier S. 6
    - Ausgefülltes AB1c auf Dossier S. 5

??? info "Organisation"

    **Sozialform:** Einzelarbeit und gemeinsame Auswertung im Plenum

    **Benötigte Zeit:** 10–15 Minuten

??? abstract "Verlaufsplanung"

    **1. Individuelle Sicherung – etwa 5 Minuten:** **Präsentation S. 20** zeigt den Arbeitsauftrag. Die Lernenden bearbeiten **AB1d, Aufgaben 1–4, Dossier S. 6**, zunächst allein. Sie dürfen das Kreuzungsbild und ihre Tabelle auf S. 5 verwenden. Sie erklären Sicherheit, begründen eine unsichere Ampelbelegung, formulieren eine Regel zu einem Konfliktpaar und erklären die Vollständigkeit ihrer Ordnung. Kurze, fachlich treffende Antworten genügen.

    **2. Ergebnisse sichern – etwa 5 Minuten:** Mit **Präsentation S. 21** ausgewählte Antworten besprechen. Gesichert werden die acht Ampelbelegungen, die Konfliktpaare, die Sicherheit von «alle Rot», das Beispiel mit zwei sicheren Grünfreigaben und eine sprachliche Sicherheitsregel.

    **3. Ausblick – 1–2 Minuten:** Mit **Präsentation S. 22** erläutern, dass die Kreuzungen im nächsten Baustein mit LogicTraffic am Computer untersucht werden.

??? tip "Didaktische Hinweise"

    Die individuelle Bearbeitung erfolgt vor der gemeinsamen Besprechung, damit erkennbar wird, welche Zusammenhänge die Lernenden bereits selbst erklären können.

??? question "Differenzierung"

    === "Vereinfachungen"

        - Satzstarter anbieten: «Die Ampeln … und … dürfen nicht gleichzeitig Grün zeigen, weil …».

    === "Erweiterungen"

        - Beide Konfliktpaare in einer gemeinsamen sprachlichen Regel berücksichtigen.

### Abschluss

??? info "Organisation"

    **Benötigte Zeit:** 2 Minuten

    Die Lernenden versorgen die Materialien.

## Gemeinsamer Logikblock

!!! info "Gemeinsamer Logikblock – zusätzlich"

    Wird der Block eingesetzt, findet er nach dem jeweiligen Einstieg im gemeinsamen weiteren Unterricht statt; beide Varianten erhalten denselben Inhalt und dieselbe Bearbeitungszeit. Er benötigt **10–15 Minuten zusätzlich** und ist nicht in der Gesamtzeit des Einstiegs enthalten. Benötigt werden **AB1X im jeweiligen Dossier** und die **Präsentation «Erweiterung Logik»**. [Zum Ablauf, zu den Seitenangaben und Materialien](baustein1-logikblock.md).

## Lösungen und Ergebnissicherung

??? success "Lösungen zu AB1a und AB1b"

    **AB1a, Aufgaben 1–3, Dossier S. 2:** C führt von links nach rechts, D von unten nach oben und E von rechts nach links. C–D und D–E sind Konfliktpaare; C–E ist konfliktfrei.

    **AB1b, Aufgabe 1, Dossier S. 3:** Beispiel 1 ist unsicher, weil D und E Grün zeigen und ihre Fahrwege im Konflikt stehen. Beispiel 2 ist sicher, weil alle Ampeln Rot zeigen und kein Fahrweg freigegeben ist.

??? success "Lösungstabelle zu AB1c"

    Die Tabelle entspricht **Kommentar S. 8** und **Präsentation S. 18**; sie gehört zu **AB1c, Aufgaben 2–4, Dossier S. 5**.

    | C | D | E | Beurteilung | Gleichzeitig freigegebenes Konfliktpaar |
    | --- | --- | --- | --- | --- |
    | Rot | Rot | Rot | sicher | – |
    | Rot | Rot | Grün | sicher | – |
    | Rot | Grün | Rot | sicher | – |
    | Rot | Grün | Grün | unsicher | D–E |
    | Grün | Rot | Rot | sicher | – |
    | Grün | Rot | Grün | sicher | – |
    | Grün | Grün | Rot | unsicher | C–D |
    | Grün | Grün | Grün | unsicher | C–D und D–E |

    Es gibt **fünf sichere und drei unsichere Ampelbelegungen**. Mögliche Sicherheitsregel: «Wenn D Grün zeigt, müssen C und E Rot zeigen.» Diese Lösung gilt für die hier festgelegten geraden Fahrwege; bei einer anderen Kreuzung wird die Sicherheit erneut geprüft.

??? success "Hinweise zur Sicherung mit AB1d"

    Für **AB1d, Aufgabe 3, Dossier S. 6**, genügt eine Regel zu einem Konfliktpaar, beispielsweise: «C und D dürfen nicht gleichzeitig Grün zeigen, weil sich ihre Fahrwege kreuzen.» Die vollständige Regel für beide Konfliktpaare ist eine Erweiterung.

## Didaktische Hinweise

??? tip "Geprüfte Präsentationsverweise"

    Der Kommentar nennt in der Übersicht auf **S. 3** und in den Phasen auf **S. 4–7** unterschiedliche Folienbereiche. Diese Seite verwendet deshalb ausschliesslich die tatsächlichen PDF-Seiten der aktuellen Präsentation. Die auf **Kommentar S. 6** erwähnte **Hilfefolie H1** ist darin nicht enthalten; die dort beschriebene Hilfe mit zunächst zwei Ampeln kann mündlich gegeben werden. Es wird kein fehlendes Material vorausgesetzt.

    Die zusätzliche Abschlussübersicht auf **Präsentation S. 23** enthält bereits Begriffe aus dem gemeinsamen Logikblock. Dessen ausführlicher Ablauf wird ausschliesslich auf der [gemeinsamen Unterseite](baustein1-logikblock.md) beschrieben.

    Die Erweiterungen der Differenzierung sind optional und haben keine eigenen Richtzeiten im Kommentar. Sie werden nicht zusätzlich in die Pflichtzeit eingerechnet.

## Übergang zum gemeinsamen Unterricht

Nach dem jeweiligen Einstieg bearbeiten beide Gruppen [Baustein 2 – LogicTraffic](baustein2-logictraffic.md) und die weiteren gemeinsamen Bausteine. Die Codierung mit `0` und `1`, formale Wahrheitstabellen und Operatoren werden dort eingeführt.
