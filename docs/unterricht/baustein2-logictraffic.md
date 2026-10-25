# Baustein 2 – LogicTraffic kennenlernen

??? example "Lehrpersonenkommentar als Download"

    [Lehrpersonenkommentar Baustein 2 - Einführung LogicTraffic](https://canva.link/mos333l78usz4xj)


In diesem Baustein übertragen die Lernenden die bereits bekannte Idee einer sicheren Verkehrskreuzung in die digitale Lernumgebung **LogicTraffic**. Sie lernen die Oberfläche kennen und untersuchen schrittweise, wie Fahrspuren, Ampelbelegungen, Variablen, die Werte `0` und `1` sowie die Wahrheitstabelle miteinander zusammenhängen.

Im Zentrum steht noch **nicht** das systematische Erstellen von Wahrheitstabellen und auch noch **nicht** das Arbeiten mit aussagenlogischen Formeln. Entscheidend ist zunächst der Darstellungswechsel: Die Lernenden sollen verstehen, wie eine konkrete Verkehrssituation in LogicTraffic digital und symbolisch dargestellt wird.

Die Progression des Bausteins lautet:

**reale bzw. enaktive Kreuzung → digitale Kreuzung → Fahrspur und Variable → Rot/Grün und `0`/`1` → Tabellenzeile → Sicherheit → Darstellungen zusammenführen**

Die aussagenlogische Formel wird am Ende lediglich als weitere Darstellung der **Sicherheitsregel** sichtbar gemacht. Wie vollständige Wahrheitstabellen selbstständig aufgebaut werden, folgt in [Baustein 3 – Wahrheitstabellen](baustein3-wahrheitstabellen.md). Das eigentliche Arbeiten mit aussagenlogischen Formeln folgt erst in [Baustein 4 – Aussagenlogische Formeln](baustein4-boolesche-algebra.md).

??? abstract "Auf einen Blick"

    **:busts_in_silhouette: Zielgruppe:** Gymnasiale Klassen der 8.–9. Schulstufe

    **:stopwatch: Dauer:** ca. **45–55 Minuten**  

    **:computer: Computer:**  Ein Computer oder Tablet mit LogicTraffic pro Zweiergruppe

    **:brain: Vorwissen:** 

    - Die Lernenden können grundsätzlich zwischen sicheren und unsicheren Verkehrssituationen unterscheiden.
    - Begriffe wie Wahrheitstabelle, Variable oder Formel müssen noch nicht formal beherrscht werden.

    **:package: Material:** LogicTraffic, Computer oder Tablets, Beamer oder Präsentationsbildschirm sowie die Materialien [2a](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2a_orientierung_logictraffic.pdf)–[2e](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2e_tafelbild_ergebnissicherung.pdf)

??? example "Materialhinweise und Downloads"

    - [:memo: Gesamtdossier Baustein 2 – Materialien 2a–2c für die Lernenden (PDF)](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/Baustein_2_Dossier.pdf)

    **Für die Lernenden**

    - [:memo: 2a – Orientierung in LogicTraffic](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2a_orientierung_logictraffic.pdf)
    - [:material-image-outline: 2b – Merkblatt Orientierung](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2b_merkblatt_orientierung.pdf)
    - [:memo: 2c – Ergebnissicherung LogicTraffic](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2c_ergebnissicherungLT.pdf)

    **Für die Lehrperson**

    - [:material-image-outline: 2e – Tafelbild zur Ergebnissicherung](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2e_tafelbild_ergebnissicherung.pdf)

    Die PDFs stellen die Materialien in druckbarer Form bereit.

## Lernziele

??? success "Lernziele"

    **Bezug zur Unterrichtseinheit:** [LZ1a – Verkehrssituationen und Darstellungen deuten](../didaktik/lernziele.md#lz1a). Der Schwerpunkt liegt auf dem Lesen und Zuordnen; das selbstständige Erstellen vollständiger Tabellen folgt in Baustein 3, die Arbeit mit Operatoren in Baustein 4.

    Die Lernenden können …

    - sich in den zentralen Bereichen von LogicTraffic orientieren;
    - erklären, dass die bereits mit `A`, `B`, `C` usw. bezeichneten Fahrspuren als Variablen in weiteren Darstellungen wieder auftauchen;
    - erklären, wie die Ampelfarben Rot und Grün mit `0` und `1` dargestellt werden;
    - zwischen `0` und `1` bei einer Fahrspur und `0` und `1` in der Spalte `sicher` unterscheiden;
    - zu einer konkreten Ampelbelegung die passende Tabellenzeile finden und eine vorgegebene Tabellenzeile wieder als Ampelbelegung lesen;
    - sichere und unsichere Ampelbelegungen anhand der Fahrwege begründen;
    - erklären, dass die Kreuzung jeweils eine konkrete Ampelbelegung zeigt, während die Wahrheitstabelle alle möglichen Ampelbelegungen mit ihrer Sicherheitsbewertung umfasst;
    - die Bereiche Kreuzung, Variablen bzw. `0`/`1`, Wahrheitstabelle, `sicher` und Formel in ihrer jeweiligen Funktion unterscheiden;
    - beschreiben, dass diese Darstellungen unterschiedliche Aspekte derselben modellierten Kreuzung bzw. Sicherheitsregel sichtbar machen;
    - die Frage formulieren, wie eine vollständige Wahrheitstabelle auch ohne Vorgabe durch LogicTraffic systematisch erstellt werden könnte.

    **Lernnachweis:** Mit AB2c ordnen die Lernenden die Darstellungen ihren Funktionen zu. Sie stellen eine vorgegebene Tabellenzeile an der Kreuzung ein und erklären getrennt die Ampelbelegungen und die Sicherheitsbewertung.

    ??? tip "Einordnung zwischen Baustein 1 und Baustein 3"

        **Baustein 1** arbeitet vor allem mit der konkreten Verkehrssituation:

        > Welche Ampelbelegungen sind sicher und warum?

        **Baustein 2** führt dieselbe Grundidee in die digitale Lernumgebung über:

        > Wie stellt LogicTraffic Fahrspuren, Ampelbelegungen und Sicherheit dar?

        **Baustein 3** verschiebt den Schwerpunkt anschliessend auf die Systematik:

        > Wie können wir selbst alle möglichen Ampelbelegungen vollständig aufschreiben, ohne eine zu vergessen?

        Dadurch erhält jeder Baustein eine eigene Funktion und die Wahrheitstabelle wird in Baustein 2 bewusst **nur gelesen und gedeutet**, noch nicht systematisch konstruiert.

## Vorbereitung

- Die Materialien 2a–2c einzeln oder als [Gesamtdossier Baustein 2 (PDF)](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/Baustein_2_Dossier.pdf) bereitstellen.

- [LogicTraffic](https://logictraffic.ch/) auf allen Geräten öffnen und die Funktionsfähigkeit prüfen.
- Für die gemeinsame Einführung vorzugsweise **Situation 2** bereithalten. Sie besitzt zwei Variablen und ermöglicht einen überschaubaren Einstieg.
- Dieselbe Situation über den Beamer öffnen, damit alle Lernenden dieselben Veränderungen beobachten können.
- **[2e](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2e_tafelbild_ergebnissicherung.pdf)** für die gemeinsame Auswertung von [2c](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2c_ergebnissicherungLT.pdf) projizieren oder ausdrucken.
- Den Formelbereich in LogicTraffic sichtbar lassen, aber noch nicht fachlich vertiefen.

??? info "Fachlicher Hintergrund – was zeigt LogicTraffic?"

    LogicTraffic verbindet mehrere Repräsentationen miteinander. Für Baustein 2 ist wichtig, diese Darstellungen **nicht vorschnell gleichzusetzen**, sondern ihre jeweilige Funktion zu unterscheiden.

    | Bereich | Bedeutung in diesem Baustein |
    | --- | --- |
    | **Kreuzung** | Zeigt die Fahrwege und jeweils eine konkrete Ampelbelegung. |
    | **Fahrspuren / Variablen** | Die bereits beschrifteten Fahrspuren `A`, `B`, `C` … werden als Variablen verwendet. |
    | **`0` und `1` bei den Variablen** | Beschreiben den Zustand einer Ampel: `0 = Rot`, `1 = Grün`. |
    | **Wahrheitstabelle** | Enthält alle möglichen Ampelbelegungen mit ihrer Sicherheitsbewertung. |
    | **Spalte `sicher`** | Bewertet, ob die jeweilige Ampelbelegung kollisionsfrei ist. |
    | **Formel** | Beschreibt die Sicherheitsregel kompakt und gilt für alle möglichen Belegungen. Sie wird in Baustein 2 nur als Ausblick betrachtet. |
    | **Einzelne Ampel** | Zeigt Rot oder Grün |
    | **Ampelbelegung** | Legt für jede betrachtete Ampel Rot oder Grün fest. |

    Für den Darstellungswechsel ist besonders hilfreich, zwischen **einer einzelnen Tabellenzeile** und der **gesamten Wahrheitstabelle** zu unterscheiden:

    **konkrete Ampelbelegung** ↔ **Kombination der Werte in den Ampelspalten einer Zeile**

    Die vollständige Tabellenzeile enthält zusätzlich die Sicherheitsbewertung in der Spalte `sicher`.

    **alle möglichen Ampelbelegungen** ↔ **gesamte Wahrheitstabelle**

??? tip "Zwei verschiedene Bedeutungen von 0 und 1"

    In LogicTraffic begegnen den Lernenden `0` und `1` auf zwei Ebenen.

    **Bei einer Fahrspur:**

    - `0` = Ampel Rot
    - `1` = Ampel Grün

    **In der Spalte `sicher`:**

    - `0` = Kombination unsicher
    - `1` = Kombination sicher

    Deshalb sollte im Unterricht möglichst präzise gesprochen werden:

    > „Bei `A = 1` ist die Ampel der Spur A grün.“

    bzw.

    > „Bei dieser Tabellenzeile ist `sicher = 0`, weil sich die grünen Fahrwege kreuzen.“

## Unterrichtsablauf – Überblick

| Phase | Schwerpunkt | Material | Richtwert |
| --- | --- | --- | ---: |
| **1. Von der Kreuzung zur digitalen Darstellung** | Vorwissen aktivieren und die Frage vorbereiten, wie eine Kreuzung am Computer dargestellt werden kann | Rückbezug auf Baustein 1 | ca. 5' |
| **2. LogicTraffic erkunden und Ampelbelegungen lesen** | Oberfläche, Variablen, `0`/`1`, Tabellenzeilen sowie sichere und unsichere Ampelbelegungen untersuchen | **[AB 2a](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2a_orientierung_logictraffic.pdf)**, anschliessend **[MB 2b](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2b_merkblatt_orientierung.pdf)**, LogicTraffic | ca. 25–30' |
| **3. Darstellungen zusammenführen und sichern** | Funktionen der verschiedenen Darstellungen ordnen und den Übergang zu Baustein 3 vorbereiten | **[AB 2c](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2c_ergebnissicherungLT.pdf)**, **[Tafelbild 2e](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2e_tafelbild_ergebnissicherung.pdf)** | ca. 15–20' |


## Durchführung

### Phase 1 – Von der Kreuzung zur digitalen Darstellung

??? success "Ziele der Einheit"

    Die Lernenden aktivieren ihr Verständnis von Fahrspuren, Ampeln und Verkehrssicherheit und entwickeln die Frage, wie eine reale Kreuzung in einer digitalen Lernumgebung dargestellt werden kann.

    Dabei werden die späteren Begriffe `Variable`, `Wahrheitstabelle` und `Formel` noch nicht vorausgesetzt oder erklärt.

??? example "Material"

    **Wenn Baustein 1 durchgeführt wurde:**

    - die dort verwendete oder eine vergleichbare Verkehrssituation
    - Beamer oder Präsentationsbildschirm

??? info "Organisation"

    **Sozialform:** Kurzes **Plenumsgespräch**. Die Lernenden beobachten eine bekannte bzw. reale Kreuzung und formulieren zunächst in Alltagssprache, welche Informationen für eine sichere Ampelsteuerung relevant sind.

    **Benötigte Zeit:** nach Baustein 1: ca. **5 Minuten**  

??? abstract "Verlaufsplanung"

    **1. Rückbezug herstellen**

    Wenn Baustein 1 durchgeführt wurde, greift die Lehrperson eine bekannte Kreuzung bzw. eine bereits untersuchte Ampelbelegung auf.

    **Inputfragen:**

    > Woran habt ihr erkannt, ob eine Ampelbelegung sicher oder unsicher ist?

    **Erwartete Antworten:**

    - Man muss betrachten, welche Fahrspuren gleichzeitig Grün haben.
    - Entscheidend ist, ob sich die Fahrwege dieser Spuren kreuzen.
    - Entscheidend ist die Ampelbelegung, also welche der betrachteten Ampeln gleichzeitig Grün zeigen.

    **3. Übergang zu LogicTraffic**

    Die Lehrperson schliesst mit der Frage:

    > Wie könnte ein Computer eine solche Kreuzung so darstellen, dass wir verschiedene Ampelbelegungen untersuchen können?

    Die Vermutungen werden kurz gesammelt. Erst danach wird LogicTraffic geöffnet.

??? tip "Didaktische Hinweise"

    Diese Phase soll **kein zweiter Theorieeinstieg** werden. Ihr Zweck ist ausschliesslich, einen verständlichen Ausgangspunkt für die digitale Darstellung zu schaffen.

    Fachbegriffe sollten in dieser Phase noch nicht vorweggenommen werden. Besonders `0`, `1` und Wahrheitstabelle werden erst an beobachtbaren Veränderungen in LogicTraffic aufgebaut.

??? question "Differenzierung"

    === "Vereinfachungen"

        - Nur eine übersichtliche Kreuzung betrachten.
        - Mit konkreten Fragen arbeiten:  
          > „Welche beiden Fahrwege könnten sich schneiden?“  
          > „Was könnte passieren, wenn beide gleichzeitig Grün haben?“

    === "Erweiterungen"

        - Mehrere mögliche Ampelbelegungen gedanklich vergleichen lassen.
        - Begründen lassen, welche Informationen eine digitale Darstellung mindestens enthalten müsste.
        - Zwischen Informationen über die **Geometrie der Kreuzung** und Informationen über die **aktuelle Ampelbelegung** unterscheiden lassen.

<span id="phase-2-logictraffic-erkunden-und-zustande-lesen"></span>

### Phase 2 – LogicTraffic erkunden und Ampelbelegungen lesen

??? success "Ziele der Einheit"

    Die Lernenden orientieren sich in LogicTraffic und können Fahrspuren, Variablen und Ampelbelegungen miteinander verknüpfen.

    Sie übersetzen zwischen Rot/Grün und `0`/`1`, ordnen eine konkrete Ampelbelegung einer Tabellenzeile zu und begründen anhand der Fahrwege, ob eine Kombination sicher oder unsicher ist.

??? example "Material"

    - [:memo: AB 2a – Orientierung in LogicTraffic](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2a_orientierung_logictraffic.pdf)
    - [:material-image-outline: MB 2b – Merkblatt Orientierung](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2b_merkblatt_orientierung.pdf)
    - [LogicTraffic](https://logictraffic.ch/), vorzugsweise **Situation 2**
    - Computer oder Tablet pro Zweiergruppe
    - Beamer oder Präsentationsbildschirm

??? info "Organisation"

    **Sozialform:** Kurze gemeinsame Orientierung im **Plenum**, danach **Partnerarbeit** mit [AB 2a](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2a_orientierung_logictraffic.pdf).
    Im Tandem übernimmt eine Person die Bedienung von LogicTraffic, während die andere Person beobachtet, liest und begründet. Spätestens beim Wechsel von Seite 1 zu Seite 2 des Arbeitsblatts werden die Rollen getauscht.

    **Benötigte Zeit:** ca. **25–30 Minuten**

??? abstract "Verlaufsplanung"

    **1. Oberfläche gemeinsam öffnen**

    Die Lehrperson öffnet Situation 2 über den Beamer und gibt zunächst einen kurzen Orientierungsauftrag:

    > Schaut euch LogicTraffic an. Welche Teile der Darstellung kennt ihr bereits von einer echten Kreuzung – und welche Teile sind neu?

    Im Plenum werden nur die für diesen Baustein relevanten Bereiche lokalisiert:

    - Kreuzung und Fahrwege;
    - die bereits beschrifteten Fahrspuren `A`, `B` usw.;
    - Ampeln;
    - Wahrheitstabelle;
    - Spalte `sicher`;
    - Formelbereich als sichtbarer, aber noch nicht zu erklärender Bereich.

    **Wichtig:** Die Fahrspuren werden **nicht nochmals beschriftet**. Die Bezeichnungen `A`, `B`, `C` … sind in LogicTraffic bereits vorhanden. Die Aufgabe besteht darin, zu erkennen, dass dieselben Variablen in anderen Bereichen der Lernumgebung wieder auftauchen.

    **2. [AB 2a](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2a_orientierung_logictraffic.pdf) – Aufgabe 1: Wo ist was?**

    Die Lernenden orientieren sich direkt in der Lernumgebung und identifizieren die zentralen Bereiche.

    Die Lehrperson verzichtet auf eine lange Vorführung. Die Orientierung soll möglichst durch eigenes Beobachten und Anklicken erfolgen.

    **3. [AB 2a](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2a_orientierung_logictraffic.pdf) – Aufgabe 2: Fahrspur und Variable gehören zusammen**

    Die Lernenden verfolgen beispielsweise die bereits beschriftete Spur `A` und suchen, wo `A` in der Wahrheitstabelle wieder auftaucht.

    **Inputfrage:**

    > Was bleibt gleich, obwohl die Fahrspur einmal in der Kreuzung und einmal in der Tabelle dargestellt wird?

    **Erwartete Antwort:**

    > Die Bezeichnung bzw. Variable `A` steht in beiden Darstellungen für dieselbe Fahrspur.

    **4. [AB 2a](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2a_orientierung_logictraffic.pdf) – Aufgabe 3: Rot und Grün werden zu 0 und 1**

    Die Lernenden verändern eine Ampel und beobachten gleichzeitig die zugehörige Variable bzw. Tabellenzeile.

    Gemeinsam wird gesichert:

    - Rot → `0`
    - Grün → `1`

    **Inputfragen:**

    > Was bedeutet `A = 1` in dieser Verkehrssituation?

    **Erwartete Antwort:** Die Ampel der Spur `A` zeigt Grün.

    > Was bedeutet `A = 0`?

    **Erwartete Antwort:** Die Ampel der Spur `A` zeigt Rot.

    **5. [Merkblatt 2b](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2b_merkblatt_orientierung.pdf) gezielt einführen**

    Erst **nach diesen ersten eigenen Beobachtungen** wird das [Merkblatt 2b](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2b_merkblatt_orientierung.pdf) ausgeteilt bzw. geöffnet.

    Es dient ab diesem Zeitpunkt als Nachschlagehilfe zu:

    - den Bereichen der Oberfläche;
    - der Bedeutung von `0` und `1`;
    - dem Zusammenhang der verschiedenen Darstellungen.

    Das Merkblatt ist **kein zusätzliches Arbeitsblatt** und wird nicht mit weiteren Aufgaben versehen.

    **6. [AB 2a](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2a_orientierung_logictraffic.pdf) – Aufgabe 4: Von der Kreuzung zur Tabellenzeile**

    Die Lernenden stellen unterschiedliche Ampelbelegungen ein und suchen jeweils die entsprechende Zeile.

    Der Darstellungswechsel soll bewusst in beide Richtungen erfolgen:

    **Kreuzung → Tabellenzeile**

    und

    **Tabellenzeile → Kreuzung**

    **Inputfrage:**

    > Zeigt die Wahrheitstabelle nur die Ampelbelegung, die wir gerade sehen?

    **Erwartete Antwort:** Nein. Die Kreuzung zeigt gerade eine Ampelbelegung; die Tabelle enthält alle möglichen Ampelbelegungen mit ihrer Sicherheitsbewertung.

    Wie diese vollständige Tabelle systematisch entsteht, wird noch nicht thematisiert.

    **7. [AB 2a](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2a_orientierung_logictraffic.pdf) – Aufgabe 5: Sicher oder unsicher?**

    Für mehrere Ampelbelegungen entscheiden die Lernenden zuerst anhand der Fahrwege:

    - Welche Spuren haben Grün?
    - Schneiden sich diese Fahrwege?
    - Kann eine Kollision entstehen?

    Erst danach wird der Wert in der Spalte `sicher` betrachtet bzw. zur Kontrolle verwendet.

    **Inputfrage:**

    > Was bewertet die Spalte `sicher`: eine einzelne Ampel oder die ganze Kombination?

    **Erwartete Antwort:** Die gesamte Ampelbelegung.

    **8. [AB 2a](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2a_orientierung_logictraffic.pdf) – Aufgaben 6 und 7: Darstellungen unterscheiden**

    Zum Abschluss des Arbeitsblatts wird bewusst zwischen den Darstellungen unterschieden:

    - Die **Kreuzung** zeigt Fahrwege und eine konkrete Ampelbelegung.
    - Die **Ampelspalten einer Tabellenzeile** beschreiben diese Ampelbelegung mit `0` und `1`; die vollständige Zeile enthält zusätzlich die Sicherheitsbewertung.
    - Die **gesamte Wahrheitstabelle** enthält verschiedene mögliche Ampelbelegungen.
    - Die Spalte **`sicher`** bewertet die jeweiligen Kombinationen.
    - Die **Formel** wird nur als kompakte Darstellung der Sicherheitsregel benannt; sie muss noch nicht gelesen oder gebildet werden.

??? tip "Didaktische Hinweise"

    Der Baustein soll nicht zu einer technischen Bedienungsanleitung für LogicTraffic werden. Die Oberfläche ist nur dann didaktisch relevant, wenn ein sichtbares Element mit einer fachlichen Bedeutung verknüpft wird.

    Besonders wichtig sind drei Abgrenzungen:

    **1. Fahrspurbezeichnungen nicht doppelt erzeugen**  
    `A`, `B`, `C` … sind in LogicTraffic bereits eingetragen. Ein erneutes Beschriften würde eher Verwirrung erzeugen. Die Lernleistung besteht im **Zuordnen derselben Variable über mehrere Darstellungen hinweg**.

    **2. `0` und `1` nicht als „falsch“ und „richtig“ einführen**  
    In dieser Phase werden sie konkret als Ampelfarben gelesen: `0 = Rot`, `1 = Grün`.

    **3. Formel nicht vorwegnehmen**  
    Der Formelbereich darf sichtbar sein und auf dem Merkblatt vorkommen. Inhaltlich genügt jedoch die Aussage, dass die Formel später die Sicherheitsregel kompakt beschreiben wird.

    Das [Merkblatt 2b](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2b_merkblatt_orientierung.pdf) wird bewusst **nach** der ersten Erkundung eingesetzt. Würde es vor [AB 2a](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2a_orientierung_logictraffic.pdf) ausgeteilt, nähme es einen Teil der Beobachtungsleistung vorweg.

??? question "Differenzierung"

    === "Vereinfachungen"

        - Ausschliesslich mit Situation 2 und zwei Variablen arbeiten.
        - Das [Merkblatt 2b](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2b_merkblatt_orientierung.pdf) nach Aufgabe 3 offen verwenden lassen.
        - Immer nur **eine** Veränderung an der Kreuzung vornehmen und danach beschreiben lassen, was sich an anderer Stelle mitverändert.
        - Satzstarter anbieten:  
          > „`A = 1` bedeutet …“  
          > „Diese Tabellenzeile passt, weil …“  
          > „Die Kombination ist unsicher, weil …“
        - Bei der Suche nach einer Tabellenzeile zuerst nur die Variablenspalten betrachten und die Spalte `sicher` danach ergänzen.

    === "Erweiterungen"

        - Eine Tabellenzeile vorgeben und die zugehörige Ampelbelegung ohne Ausprobieren einstellen lassen.
        - Eine Ampelbelegung kurz zeigen, wieder verändern und die ursprüngliche Tabellenzeile aus dem Gedächtnis notieren lassen.
        - Begründen lassen, weshalb zwei gleichzeitig grüne Ampeln nicht automatisch eine unsichere Situation bedeuten.
        - Bereits eine Situation mit drei Variablen erkunden, ohne die vollständige Tabelle systematisch aufzubauen.
        - Beobachten lassen, dass der Formelbereich auf Änderungen reagiert, ohne die Formel bereits fachlich zu analysieren.

### Phase 3 – Darstellungen zusammenführen und sichern

??? success "Ziele der Einheit"

    Die Lernenden ordnen die verschiedenen Darstellungen in LogicTraffic nach ihrer Funktion und sichern die zentralen Erkenntnisse des Bausteins.

    Sie unterscheiden insbesondere zwischen einer konkreten Ampelbelegung, ihrer symbolischen Beschreibung, der vollständigen Menge möglicher Ampelbelegungen und der Sicherheitsregel. Daraus entwickeln sie die Anschlussfrage für Baustein 3.

??? example "Material"

    - [:memo: AB 2c – Ergebnissicherung LogicTraffic](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2c_ergebnissicherungLT.pdf)
    - [:material-image-outline: 2e – Tafelbild zur Ergebnissicherung](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2e_tafelbild_ergebnissicherung.pdf)
    - [:material-image-outline: MB 2b – Merkblatt Orientierung](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2b_merkblatt_orientierung.pdf) als Nachschlagehilfe
    - LogicTraffic und Beamer

??? info "Organisation"

    **Sozialform:** Zunächst kurze **Einzelarbeit** mit [2c](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2c_ergebnissicherungLT.pdf), danach **Partnervergleich**. Die gemeinsame Sicherung erfolgt im **Plenum** mit [Tafelbild 2e](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2e_tafelbild_ergebnissicherung.pdf).

    **Benötigte Zeit:** ca. **15–20 Minuten**

??? abstract "Verlaufsplanung"

    **1. [AB 2c](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2c_ergebnissicherungLT.pdf) zunächst individuell bearbeiten**

    Die Lernenden sichern die Ergebnisse der Erkundung auf dem Blatt **„Dieselbe Situation – verschiedene Darstellungen“**.

    Die Aufgaben bündeln die zuvor untersuchten Zusammenhänge:

    - **Was zeigt welche Darstellung?**
    - **Kreuzung oder Wahrheitstabelle?**
    - **Was bedeutet `sicher`?**
    - **Welche Idee verbindet die verschiedenen Darstellungen?**

    Das [Merkblatt 2b](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2b_merkblatt_orientierung.pdf) darf bei Bedarf als Nachschlagehilfe verwendet werden.

    **2. Ergebnisse im Tandem vergleichen**

    Die Lernenden vergleichen ihre Zuordnungen und korrigieren Unterschiede nicht nur formal, sondern mit einer kurzen Begründung.

    **Leitfragen:**

    > Welche Darstellung zeigt nur eine aktuelle Ampelbelegung?

    **Erwartete Antwort:** Die Kreuzung.

    > Wo finden wir dieselbe aktuelle Ampelbelegung mit `0` und `1` wieder?

    **Erwartete Antwort:** In einer passenden Zeile der Wahrheitstabelle.

    > Was umfasst die gesamte Wahrheitstabelle darüber hinaus?

    **Erwartete Antwort:** Verschiedene bzw. alle möglichen Kombinationen der Variablenwerte.

    > Was sagt `sicher` aus?

    **Erwartete Antwort:** Ob die jeweilige Ampelbelegung kollisionsfrei ist.

    **3. [Tafelbild 2e](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2e_tafelbild_ergebnissicherung.pdf) zur gemeinsamen Sicherung einsetzen**

    Die Lehrperson projiziert [2e](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2e_tafelbild_ergebnissicherung.pdf) und ordnet die Begriffe gemeinsam mit der Klasse.

    Fachlich präzise kann die Beziehung so gesichert werden:

    **Kreuzung**  
    → zeigt Fahrwege und eine konkrete Ampelbelegung

    **Variablen und `0`/`1`**  
    → beschreiben die Ampelbelegung symbolisch

    **eine Tabellenzeile**  
    → enthält genau eine Ampelbelegung und deren Sicherheitsbewertung

    **Wahrheitstabelle**  
    → umfasst die möglichen Belegungen und ihre Sicherheitsbewertung

    **`sicher`**  
    → bewertet die jeweilige Belegung

    **Formel**  
    → beschreibt die Sicherheitsregel kompakt für alle Belegungen; dies ist zunächst nur ein Ausblick

    **4. Gemeinsamen Merksatz formulieren**

    Ein geeigneter Merksatz lautet:

    > LogicTraffic zeigt dasselbe Kreuzungsproblem auf verschiedenen Ebenen: anschaulich in der Kreuzung, symbolisch mit Variablen und `0`/`1`, vollständig in der Wahrheitstabelle und später kompakt als Formel.

    Dadurch wird vermieden, Kreuzung, einzelne Tabellenzeile, gesamte Wahrheitstabelle und Formel als völlig identische Darstellungen zu behandeln.

    **5. Übergang zu Baustein 3 erzeugen**

    Die Lehrperson zeigt nochmals die Wahrheitstabelle und fragt:

    > Bisher liefert LogicTraffic uns die möglichen Kombinationen bereits. Wie könnten wir diese Tabelle selbst erstellen und sicher sein, dass keine Kombination fehlt oder doppelt vorkommt?

    Diese Frage bildet den direkten Ausgangspunkt für [Baustein 3 – Wahrheitstabellen](baustein3-wahrheitstabellen.md).

??? tip "Didaktische Hinweise"

    [2c](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2c_ergebnissicherungLT.pdf) und [2e](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2e_tafelbild_ergebnissicherung.pdf) erfüllen bewusst **verschiedene Rollen**:

    - **[2c](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2c_ergebnissicherungLT.pdf)** ist die aktive Ergebnissicherung der Lernenden.
    - **[2e](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2e_tafelbild_ergebnissicherung.pdf)** unterstützt die gemeinsame Auswertung durch die Lehrperson.

    Dadurch sollte [2e](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2e_tafelbild_ergebnissicherung.pdf) nicht vor der Bearbeitung von [2c](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2c_ergebnissicherungLT.pdf) gezeigt werden, da es sonst die eigentliche Sicherungsleistung vorwegnimmt.

    Fachlich ist zudem eine kleine Präzisierung wichtig: Eine konkrete Ampelbelegung und eine gesamte Wahrheitstabelle sind nicht einfach „dieselbe Darstellung in anderer Form“. Die **Ampelspalten einer Zeile** beschreiben eine konkrete Ampelbelegung; die **vollständige Zeile** enthält zusätzlich die Sicherheitsbewertung. Die **gesamte Tabelle** umfasst alle möglichen Ampelbelegungen mit ihrer Bewertung. Die **Formel** beschreibt wiederum die übergeordnete Sicherheitsregel. Gerade diese Unterscheidung erleichtert später den Übergang zu Baustein 3 und 4.

    Die Formel bleibt hier ein **Ausblick**. Lernende müssen weder Operatoren kennen noch die angezeigte Formel erklären können.

??? question "Differenzierung"

    === "Vereinfachungen"

        - [2b](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2b_merkblatt_orientierung.pdf) beim Ausfüllen von [2c](https://github.com/salomegolden/logictraffic/releases/download/ab2_v2/2c_ergebnissicherungLT.pdf) offen verwenden lassen.
        - Nur die vier Kernbereiche Kreuzung, Variablen/`0`–`1`, Wahrheitstabelle und `sicher` sichern; die Formel anschliessend gemeinsam ergänzen.
        - Satzstarter anbieten:  
          > „Die Kreuzung zeigt …“  
          > „Eine Tabellenzeile zeigt …“  
          > „Die ganze Wahrheitstabelle zeigt …“  
          > „`sicher = 1` bedeutet …“
        - Das Tafelbild Schritt für Schritt aufdecken bzw. besprechen.

    === "Erweiterungen"

        - Den Unterschied zwischen **einer Tabellenzeile** und der **gesamten Wahrheitstabelle** in eigenen Worten erklären lassen.
        - Begründen lassen, weshalb die Formel eher zur ganzen Sicherheitsregel als zu einer einzelnen Ampelbelegung gehört.
        - Eine eigene grafische Darstellung der Repräsentationswechsel entwickeln lassen.
        - Bereits vermuten lassen, wie viele Zeilen eine vollständige Wahrheitstabelle mit drei Fahrspuren enthalten könnte, ohne die allgemeine Regel vorwegzunehmen.


## Abschluss des Bausteins

Am Ende von Baustein 2 können die Lernenden die digitale Lernumgebung nicht nur bedienen, sondern zentrale Elemente **fachlich deuten**:

1. Fahrspuren werden als Variablen `A`, `B`, `C` … bezeichnet.
2. `0` und `1` beschreiben bei den Variablen die Ampelfarben Rot und Grün.
3. Die Ampelspalten einer Zeile beschreiben eine konkrete Ampelbelegung; die vollständige Zeile enthält zusätzlich die Sicherheitsbewertung.
4. Die Wahrheitstabelle umfasst verschiedene mögliche Ampelbelegungen.
5. Die Spalte `sicher` bewertet, ob eine Kombination kollisionsfrei ist.
6. Die Formel ist eine weitere, kompakte Darstellung der Sicherheitsregel und wird erst später vertieft.

??? success "Von der konkreten Kreuzung zur symbolischen Darstellung"

    Baustein 2 schafft die Brücke von der anschaulichen Verkehrssituation zur symbolischen Darstellung in LogicTraffic.

    Die nächste offene Frage lautet:

    > **Wie können wir selbst eine vollständige Wahrheitstabelle erstellen, ohne eine Kombination zu vergessen?**

    Genau diese Frage wird in [Baustein 3 – Wahrheitstabellen](baustein3-wahrheitstabellen.md) bearbeitet.
