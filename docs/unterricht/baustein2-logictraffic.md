# Baustein 2 – LogicTraffic kennenlernen

In diesem Baustein übertragen die Lernenden die bereits bekannte Idee einer sicheren Verkehrskreuzung in die digitale Lernumgebung **LogicTraffic**. Sie lernen die Oberfläche kennen und untersuchen schrittweise, wie Fahrspuren, Ampelzustände, Variablen, die Werte `0` und `1` sowie die Wahrheitstabelle miteinander zusammenhängen.

Im Zentrum steht noch **nicht** das systematische Erstellen von Wahrheitstabellen und auch noch **nicht** das Arbeiten mit logischen Formeln. Entscheidend ist zunächst der Darstellungswechsel: Die Lernenden sollen verstehen, wie eine konkrete Verkehrssituation in LogicTraffic digital und symbolisch dargestellt wird.

Die Progression des Bausteins lautet:

**reale bzw. enaktive Kreuzung → digitale Kreuzung → Fahrspur und Variable → Rot/Grün und `0`/`1` → Tabellenzeile → Sicherheit → Darstellungen zusammenführen**

Die Formel wird am Ende lediglich als weitere Darstellung der **Sicherheitsregel** sichtbar gemacht. Wie vollständige Wahrheitstabellen selbstständig aufgebaut werden, folgt in [Baustein 3 – Wahrheitstabellen](baustein3-wahrheitstabellen.md). Das eigentliche Arbeiten mit logischen Formeln folgt erst in [Baustein 4 – Logische Formeln](baustein4-boolesche-algebra.md).

!!! abstract "Auf einen Blick"

    **:stopwatch: Dauer:**  
    nach Baustein 1: ca. **45–55 Minuten**  
    ohne Baustein 1: zusätzlich ca. **5–10 Minuten** für den Einstieg mit [2d](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2d_prasentation_lp_kreuzungen.pdf)

    **:busts_in_silhouette: Sozialform:**  
    Plenum, Partnerarbeit und kurze Einzelphasen

    **:computer: Computer:**  
    Ein Computer oder Tablet mit LogicTraffic pro Zweiergruppe

    **:brain: Vorwissen:**  
    - Die Lernenden können grundsätzlich zwischen sicheren und unsicheren Verkehrssituationen unterscheiden.
    - Idealerweise wurde zuvor [Baustein 1 – Enaktiver Einstieg](baustein1-enaktiv.md) durchgeführt.
    - Falls Baustein 1 ausgelassen wird, übernimmt die Präsentation **[2d](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2d_prasentation_lp_kreuzungen.pdf)** die Aktivierung einer realen Verkehrssituation.
    - Begriffe wie Wahrheitstabelle, Variable oder Formel müssen noch nicht formal beherrscht werden.

    **:package: Material:**  
    LogicTraffic, Computer oder Tablets, Beamer oder Präsentationsbildschirm sowie die Materialien [2a](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2a_orientierung_logictraffic.pdf)–[2e](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2e_tafelbild_ergebnissicherung.pdf)

??? note "Downloads zu Baustein 2"

    **Für die Lernenden**

    - [:memo: 2a – Orientierung in LogicTraffic](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2a_orientierung_logictraffic.pdf)
    - [:material-image-outline: 2b – Merkblatt Orientierung](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2b_merkblatt_orientierung.pdf)
    - [:memo: 2c – Ergebnissicherung LogicTraffic](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2c_ergebnissicherungLT.pdf)

    **Für die Lehrperson**

    - [:film_projector: 2d – Präsentation: Kreuzungen](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2d_prasentation_lp_kreuzungen.pdf) – **optional**, wenn Baustein 1 nicht durchgeführt wurde
    - [:material-image-outline: 2e – Tafelbild zur Ergebnissicherung](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2e_tafelbild_ergebnissicherung.pdf)

## Lernziele

Die Lernenden können …

- sich in den zentralen Bereichen von LogicTraffic orientieren;
- erklären, dass die bereits mit `A`, `B`, `C` usw. bezeichneten Fahrspuren als Variablen in weiteren Darstellungen wieder auftauchen;
- erklären, wie die Ampelzustände Rot und Grün mit `0` und `1` dargestellt werden;
- zwischen `0` und `1` bei einer Fahrspur und `0` und `1` in der Spalte `sicher` unterscheiden;
- zu einer konkreten Ampelstellung die passende Tabellenzeile finden und eine vorgegebene Tabellenzeile wieder als Ampelstellung lesen;
- sichere und unsichere Ampelkombinationen anhand der Fahrwege begründen;
- erklären, dass die Kreuzung jeweils einen konkreten Zustand zeigt, während die Wahrheitstabelle verschiedene mögliche Zustände umfasst;
- die Bereiche Kreuzung, Variablen bzw. `0`/`1`, Wahrheitstabelle, `sicher` und Formel in ihrer jeweiligen Funktion unterscheiden;
- beschreiben, dass diese Darstellungen unterschiedliche Aspekte derselben modellierten Kreuzung bzw. Sicherheitsregel sichtbar machen;
- die Frage formulieren, wie eine vollständige Wahrheitstabelle auch ohne Vorgabe durch LogicTraffic systematisch erstellt werden könnte.

??? note "Einordnung zwischen Baustein 1 und Baustein 3"

    **Baustein 1** arbeitet vor allem mit der konkreten Verkehrssituation:

    > Welche Ampelstellungen sind sicher und warum?

    **Baustein 2** führt dieselbe Grundidee in die digitale Lernumgebung über:

    > Wie stellt LogicTraffic Fahrspuren, Ampelzustände und Sicherheit dar?

    **Baustein 3** verschiebt den Schwerpunkt anschliessend auf die Systematik:

    > Wie können wir selbst alle möglichen Zustände vollständig aufschreiben, ohne einen zu vergessen?

    Dadurch erhält jeder Baustein eine eigene Funktion und die Wahrheitstabelle wird in Baustein 2 bewusst **nur gelesen und gedeutet**, noch nicht systematisch konstruiert.

## Vorbereitung

- [LogicTraffic](https://logictraffic.ch/) auf allen Geräten öffnen und die Funktionsfähigkeit prüfen.
- Für die gemeinsame Einführung vorzugsweise **Situation 2** bereithalten. Sie besitzt zwei Variablen und ermöglicht einen überschaubaren Einstieg.
- Dieselbe Situation über den Beamer öffnen, damit alle Lernenden dieselben Veränderungen beobachten können.
- Falls Baustein 1 durchgeführt wurde, zu Beginn kurz an die dort untersuchten sicheren und unsicheren Ampelstellungen anknüpfen.
- Falls Baustein 1 **nicht** durchgeführt wurde, die Präsentation **[2d](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2d_prasentation_lp_kreuzungen.pdf)** als alternativen Einstieg bereithalten.
- **[2a](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2a_orientierung_logictraffic.pdf)** als zentrales Arbeitsblatt für die Erkundung bereitstellen.
- **[2b](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2b_merkblatt_orientierung.pdf)** noch nicht zu Beginn austeilen: Das Merkblatt enthält bereits zentrale Orientierungsinformationen und eignet sich besser als Nachschlagehilfe **nach der ersten eigenen Erkundung**.
- **[2c](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2c_ergebnissicherungLT.pdf)** für die abschliessende Ergebnissicherung bereitstellen.
- **[2e](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2e_tafelbild_ergebnissicherung.pdf)** für die gemeinsame Auswertung von [2c](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2c_ergebnissicherungLT.pdf) projizieren oder ausdrucken.
- Den Formelbereich in LogicTraffic sichtbar lassen, aber noch nicht fachlich vertiefen.

??? info "Fachlicher Hintergrund – was zeigt LogicTraffic?"

    LogicTraffic verbindet mehrere Repräsentationen miteinander. Für Baustein 2 ist wichtig, diese Darstellungen **nicht vorschnell gleichzusetzen**, sondern ihre jeweilige Funktion zu unterscheiden.

    | Bereich | Bedeutung in diesem Baustein |
    | --- | --- |
    | **Kreuzung** | Zeigt die Fahrwege und jeweils eine konkrete Ampelstellung. |
    | **Fahrspuren / Variablen** | Die bereits beschrifteten Fahrspuren `A`, `B`, `C` … werden als Variablen verwendet. |
    | **`0` und `1` bei den Variablen** | Beschreiben den Zustand einer Ampel: `0 = Rot`, `1 = Grün`. |
    | **Wahrheitstabelle** | Enthält verschiedene mögliche Kombinationen der Variablenwerte. |
    | **Spalte `sicher`** | Bewertet, ob die jeweilige Ampelkombination kollisionsfrei ist. |
    | **Formel** | Beschreibt die Sicherheitsregel kompakt und gilt für alle möglichen Belegungen. Sie wird in Baustein 2 nur als Ausblick betrachtet. |

    Für den Darstellungswechsel ist besonders hilfreich, zwischen **einer einzelnen Tabellenzeile** und der **gesamten Wahrheitstabelle** zu unterscheiden:

    **konkrete Ampelstellung** ↔ **eine Tabellenzeile**

    **alle möglichen Ampelstellungen** ↔ **gesamte Wahrheitstabelle**

??? warning "Zwei verschiedene Bedeutungen von 0 und 1"

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
| **1. Von der Kreuzung zur digitalen Darstellung** | Vorwissen aktivieren und die Frage vorbereiten, wie eine Kreuzung am Computer dargestellt werden kann | Rückbezug auf Baustein 1; alternativ **[2d](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2d_prasentation_lp_kreuzungen.pdf)** | ca. 5 Min.; ohne Baustein 1 ca. 10–15 Min. |
| **2. LogicTraffic erkunden und Zustände lesen** | Oberfläche, Variablen, `0`/`1`, Tabellenzeilen sowie sichere und unsichere Zustände untersuchen | **[AB 2a](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2a_orientierung_logictraffic.pdf)**, anschliessend **[MB 2b](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2b_merkblatt_orientierung.pdf)**, LogicTraffic | ca. 25–30 Min. |
| **3. Darstellungen zusammenführen und sichern** | Funktionen der verschiedenen Darstellungen ordnen und den Übergang zu Baustein 3 vorbereiten | **[AB 2c](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2c_ergebnissicherungLT.pdf)**, **[Tafelbild 2e](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2e_tafelbild_ergebnissicherung.pdf)** | ca. 15–20 Min. |

Die Materialien sind damit eindeutig zugeordnet: **[2a](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2a_orientierung_logictraffic.pdf)** trägt die eigentliche Erkundung, **[2b](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2b_merkblatt_orientierung.pdf)** dient danach als Nachschlagehilfe, **[2c](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2c_ergebnissicherungLT.pdf)** sichert die Ergebnisse, **[2e](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2e_tafelbild_ergebnissicherung.pdf)** unterstützt die gemeinsame Auswertung und **[2d](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2d_prasentation_lp_kreuzungen.pdf)** ersetzt nur dann den realen bzw. enaktiven Rückbezug, wenn Baustein 1 nicht stattgefunden hat.

## Durchführung

### Phase 1 - Von der Kreuzung zur digitalen Darstellung

??? success "Ziele der Einheit"

    Die Lernenden aktivieren ihr Verständnis von Fahrspuren, Ampeln und Verkehrssicherheit und entwickeln die Frage, wie eine reale Kreuzung in einer digitalen Lernumgebung dargestellt werden kann.

    Dabei werden die späteren Begriffe `Variable`, `Wahrheitstabelle` und `Formel` noch nicht vorausgesetzt oder erklärt.

??? example "Material"

    **Wenn Baustein 1 durchgeführt wurde:**

    - die dort verwendete oder eine vergleichbare Verkehrssituation
    - Beamer oder Präsentationsbildschirm

    **Wenn Baustein 1 nicht durchgeführt wurde:**

    - [:film_projector: 2d – Präsentation: Kreuzungen](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2d_prasentation_lp_kreuzungen.pdf)
    - Beamer oder Präsentationsbildschirm

??? info "Sozialformen"

    Kurzes **Plenumsgespräch**. Die Lernenden beobachten eine bekannte bzw. reale Kreuzung und formulieren zunächst in Alltagssprache, welche Informationen für eine sichere Ampelsteuerung relevant sind.

??? tip "benötigte Zeit"

    nach Baustein 1: ca. **5 Minuten**  
    ohne Baustein 1 mit [Präsentation 2d](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2d_prasentation_lp_kreuzungen.pdf): ca. **10–15 Minuten**

??? abstract "Verlaufsplanung"

    **1. Rückbezug herstellen**

    Wenn Baustein 1 durchgeführt wurde, greift die Lehrperson eine bekannte Kreuzung bzw. eine bereits untersuchte Ampelstellung auf.

    **Inputfragen:**

    > Woran habt ihr erkannt, ob eine Ampelstellung sicher oder unsicher ist?

    **Erwartete Antworten:**

    - Man muss betrachten, welche Fahrspuren gleichzeitig Grün haben.
    - Entscheidend ist, ob sich die Fahrwege dieser Spuren kreuzen.
    - Nicht die einzelne Ampel, sondern die Kombination der Ampelstellungen ist relevant.

    **2. Alternative ohne Baustein 1**

    Wurde Baustein 1 ausgelassen, verwendet die Lehrperson **[2d](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2d_prasentation_lp_kreuzungen.pdf)**. Die Präsentation dient bewusst nur dazu, eine reale Kreuzung zu beobachten und das Sicherheitsproblem zu aktivieren. Sie ist **keine Einführung in die Oberfläche von LogicTraffic**.

    Die Lernenden beschreiben beispielsweise:

    - welche Fahrwege sie erkennen;
    - welche Bewegungen gleichzeitig möglich erscheinen;
    - wo mögliche Konflikte entstehen;
    - welche Informationen eine Ampelsteuerung berücksichtigen muss.

    **Leitfrage:**

    > Welche Informationen braucht eine Ampelsteuerung, damit eine Kreuzung sicher funktioniert?

    **3. Übergang zu LogicTraffic**

    Die Lehrperson schliesst mit der Frage:

    > Wie könnte ein Computer eine solche Kreuzung so darstellen, dass wir verschiedene Ampelstellungen untersuchen können?

    Die Vermutungen werden kurz gesammelt. Erst danach wird LogicTraffic geöffnet.

??? note "Didaktische Hinweise"

    Diese Phase soll **kein zweiter Theorieeinstieg** werden. Ihr Zweck ist ausschliesslich, einen verständlichen Ausgangspunkt für die digitale Darstellung zu schaffen.

    Wenn Baustein 1 bereits stattgefunden hat, ist die [Präsentation 2d](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2d_prasentation_lp_kreuzungen.pdf) nicht zusätzlich nötig. Dadurch werden Wiederholungen vermieden und der Baustein bleibt kompakt.

    Ohne Baustein 1 ersetzt [2d](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2d_prasentation_lp_kreuzungen.pdf) nicht den enaktiven Zugang vollständig, schafft aber einen konkreten Alltagsbezug, bevor mit der digitalen Lernumgebung gearbeitet wird.

    Fachbegriffe sollten in dieser Phase noch nicht vorweggenommen werden. Besonders `0`, `1` und Wahrheitstabelle werden erst an beobachtbaren Veränderungen in LogicTraffic aufgebaut.

??? bug "Differenzierung"

    === "Vereinfachungen"

        - Nur eine übersichtliche Kreuzung betrachten.
        - Mit konkreten Fragen arbeiten:  
          > „Welche beiden Fahrwege könnten sich schneiden?“  
          > „Was könnte passieren, wenn beide gleichzeitig Grün haben?“
        - Bei Baustein-1-Erfahrungen direkt auf eine bekannte Ampelstellung zurückgreifen.

    === "Erweiterungen"

        - Mehrere mögliche Ampelstellungen gedanklich vergleichen lassen.
        - Begründen lassen, welche Informationen eine digitale Darstellung mindestens enthalten müsste.
        - Zwischen Informationen über die **Geometrie der Kreuzung** und Informationen über den **aktuellen Ampelzustand** unterscheiden lassen.

### Phase 2 - LogicTraffic erkunden und Zustände lesen

??? success "Ziele der Einheit"

    Die Lernenden orientieren sich in LogicTraffic und können Fahrspuren, Variablen und Ampelzustände miteinander verknüpfen.

    Sie übersetzen zwischen Rot/Grün und `0`/`1`, ordnen eine konkrete Ampelstellung einer Tabellenzeile zu und begründen anhand der Fahrwege, ob eine Kombination sicher oder unsicher ist.

??? example "Material"

    - [:memo: AB 2a – Orientierung in LogicTraffic](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2a_orientierung_logictraffic.pdf)
    - [:material-image-outline: MB 2b – Merkblatt Orientierung](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2b_merkblatt_orientierung.pdf)
    - [LogicTraffic](https://logictraffic.ch/), vorzugsweise **Situation 2**
    - Computer oder Tablet pro Zweiergruppe
    - Beamer oder Präsentationsbildschirm

??? info "Sozialformen"

    Kurze gemeinsame Orientierung im **Plenum**, danach **Partnerarbeit** mit [AB 2a](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2a_orientierung_logictraffic.pdf).

    Im Tandem übernimmt eine Person die Bedienung von LogicTraffic, während die andere Person beobachtet, liest und begründet. Spätestens beim Wechsel von Seite 1 zu Seite 2 des Arbeitsblatts werden die Rollen getauscht.

??? tip "benötigte Zeit"

    ca. **25–30 Minuten**

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

    **2. [AB 2a](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2a_orientierung_logictraffic.pdf) – Aufgabe 1: Wo ist was?**

    Die Lernenden orientieren sich direkt in der Lernumgebung und identifizieren die zentralen Bereiche.

    Die Lehrperson verzichtet auf eine lange Vorführung. Die Orientierung soll möglichst durch eigenes Beobachten und Anklicken erfolgen.

    **3. [AB 2a](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2a_orientierung_logictraffic.pdf) – Aufgabe 2: Fahrspur und Variable gehören zusammen**

    Die Lernenden verfolgen beispielsweise die bereits beschriftete Spur `A` und suchen, wo `A` in der Wahrheitstabelle wieder auftaucht.

    **Inputfrage:**

    > Was bleibt gleich, obwohl die Fahrspur einmal in der Kreuzung und einmal in der Tabelle dargestellt wird?

    **Erwartete Antwort:**

    > Die Bezeichnung bzw. Variable `A` steht in beiden Darstellungen für dieselbe Fahrspur.

    **4. [AB 2a](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2a_orientierung_logictraffic.pdf) – Aufgabe 3: Rot und Grün werden zu 0 und 1**

    Die Lernenden verändern eine Ampel und beobachten gleichzeitig die zugehörige Variable bzw. Tabellenzeile.

    Gemeinsam wird gesichert:

    - Rot → `0`
    - Grün → `1`

    **Inputfragen:**

    > Was bedeutet `A = 1` in dieser Verkehrssituation?

    **Erwartete Antwort:** Die Ampel der Spur `A` zeigt Grün.

    > Was bedeutet `A = 0`?

    **Erwartete Antwort:** Die Ampel der Spur `A` zeigt Rot.

    **5. [Merkblatt 2b](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2b_merkblatt_orientierung.pdf) gezielt einführen**

    Erst **nach diesen ersten eigenen Beobachtungen** wird das [Merkblatt 2b](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2b_merkblatt_orientierung.pdf) ausgeteilt bzw. geöffnet.

    Es dient ab diesem Zeitpunkt als Nachschlagehilfe zu:

    - den Bereichen der Oberfläche;
    - der Bedeutung von `0` und `1`;
    - dem Zusammenhang der verschiedenen Darstellungen.

    Das Merkblatt ist **kein zusätzliches Arbeitsblatt** und wird nicht mit weiteren Aufgaben versehen.

    **6. [AB 2a](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2a_orientierung_logictraffic.pdf) – Aufgabe 4: Von der Kreuzung zur Tabellenzeile**

    Die Lernenden stellen unterschiedliche Ampelstellungen ein und suchen jeweils die entsprechende Zeile.

    Der Darstellungswechsel soll bewusst in beide Richtungen erfolgen:

    **Kreuzung → Tabellenzeile**

    und

    **Tabellenzeile → Kreuzung**

    **Inputfrage:**

    > Zeigt die Wahrheitstabelle nur die Ampelstellung, die wir gerade sehen?

    **Erwartete Antwort:** Nein. Die Kreuzung zeigt gerade einen Zustand; die Tabelle enthält verschiedene mögliche Zustände.

    Wie diese vollständige Tabelle systematisch entsteht, wird noch nicht thematisiert.

    **7. [AB 2a](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2a_orientierung_logictraffic.pdf) – Aufgabe 5: Sicher oder unsicher?**

    Für mehrere Ampelkombinationen entscheiden die Lernenden zuerst anhand der Fahrwege:

    - Welche Spuren haben Grün?
    - Schneiden sich diese Fahrwege?
    - Kann eine Kollision entstehen?

    Erst danach wird der Wert in der Spalte `sicher` betrachtet bzw. zur Kontrolle verwendet.

    **Inputfrage:**

    > Was bewertet die Spalte `sicher`: eine einzelne Ampel oder die ganze Kombination?

    **Erwartete Antwort:** Die gesamte Kombination der Ampelzustände.

    **8. [AB 2a](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2a_orientierung_logictraffic.pdf) – Aufgaben 6 und 7: Darstellungen unterscheiden**

    Zum Abschluss des Arbeitsblatts wird bewusst zwischen den Darstellungen unterschieden:

    - Die **Kreuzung** zeigt Fahrwege und eine konkrete Ampelstellung.
    - Eine **Tabellenzeile** beschreibt diese Ampelstellung mit `0` und `1`.
    - Die **gesamte Wahrheitstabelle** enthält verschiedene mögliche Ampelstellungen.
    - Die Spalte **`sicher`** bewertet die jeweiligen Kombinationen.
    - Die **Formel** wird nur als kompakte Darstellung der Sicherheitsregel benannt; sie muss noch nicht gelesen oder gebildet werden.

??? note "Didaktische Hinweise"

    Der Baustein soll nicht zu einer technischen Bedienungsanleitung für LogicTraffic werden. Die Oberfläche ist nur dann didaktisch relevant, wenn ein sichtbares Element mit einer fachlichen Bedeutung verknüpft wird.

    Besonders wichtig sind drei Abgrenzungen:

    **1. Fahrspurbezeichnungen nicht doppelt erzeugen**  
    `A`, `B`, `C` … sind in LogicTraffic bereits eingetragen. Ein erneutes Beschriften würde eher Verwirrung erzeugen. Die Lernleistung besteht im **Zuordnen derselben Variable über mehrere Darstellungen hinweg**.

    **2. `0` und `1` nicht als „falsch“ und „richtig“ einführen**  
    In dieser Phase werden sie konkret als Ampelzustände gelesen: `0 = Rot`, `1 = Grün`.

    **3. Formel nicht vorwegnehmen**  
    Der Formelbereich darf sichtbar sein und auf dem Merkblatt vorkommen. Inhaltlich genügt jedoch die Aussage, dass die Formel später die Sicherheitsregel kompakt beschreiben wird.

    Das [Merkblatt 2b](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2b_merkblatt_orientierung.pdf) wird bewusst **nach** der ersten Erkundung eingesetzt. Würde es vor [AB 2a](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2a_orientierung_logictraffic.pdf) ausgeteilt, nähme es einen Teil der Beobachtungsleistung vorweg.

??? bug "Differenzierung"

    === "Vereinfachungen"

        - Ausschliesslich mit Situation 2 und zwei Variablen arbeiten.
        - Das [Merkblatt 2b](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2b_merkblatt_orientierung.pdf) nach Aufgabe 3 offen verwenden lassen.
        - Immer nur **eine** Veränderung an der Kreuzung vornehmen und danach beschreiben lassen, was sich an anderer Stelle mitverändert.
        - Satzstarter anbieten:  
          > „`A = 1` bedeutet …“  
          > „Diese Tabellenzeile passt, weil …“  
          > „Die Kombination ist unsicher, weil …“
        - Bei der Suche nach einer Tabellenzeile zuerst nur die Variablenspalten betrachten und die Spalte `sicher` danach ergänzen.

    === "Erweiterungen"

        - Eine Tabellenzeile vorgeben und die zugehörige Ampelstellung ohne Ausprobieren einstellen lassen.
        - Eine Ampelstellung kurz zeigen, wieder verändern und die ursprüngliche Tabellenzeile aus dem Gedächtnis notieren lassen.
        - Begründen lassen, weshalb zwei gleichzeitig grüne Ampeln nicht automatisch eine unsichere Situation bedeuten.
        - Bereits eine Situation mit drei Variablen erkunden, ohne die vollständige Tabelle systematisch aufzubauen.
        - Beobachten lassen, dass der Formelbereich auf Änderungen reagiert, ohne die Formel bereits fachlich zu analysieren.

### Phase 3 - Darstellungen zusammenführen und sichern

??? success "Ziele der Einheit"

    Die Lernenden ordnen die verschiedenen Darstellungen in LogicTraffic nach ihrer Funktion und sichern die zentralen Erkenntnisse des Bausteins.

    Sie unterscheiden insbesondere zwischen einer konkreten Ampelstellung, ihrer symbolischen Beschreibung, der vollständigen Menge möglicher Zustände und der Sicherheitsregel. Daraus entwickeln sie die Anschlussfrage für Baustein 3.

??? example "Material"

    - [:memo: AB 2c – Ergebnissicherung LogicTraffic](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2c_ergebnissicherungLT.pdf)
    - [:material-image-outline: 2e – Tafelbild zur Ergebnissicherung](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2e_tafelbild_ergebnissicherung.pdf)
    - [:material-image-outline: MB 2b – Merkblatt Orientierung](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2b_merkblatt_orientierung.pdf) als Nachschlagehilfe
    - LogicTraffic und Beamer

??? info "Sozialformen"

    Zunächst kurze **Einzelarbeit** mit [2c](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2c_ergebnissicherungLT.pdf), danach **Partnervergleich**. Die gemeinsame Sicherung erfolgt im **Plenum** mit [Tafelbild 2e](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2e_tafelbild_ergebnissicherung.pdf).

??? tip "benötigte Zeit"

    ca. **15–20 Minuten**

??? abstract "Verlaufsplanung"

    **1. [AB 2c](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2c_ergebnissicherungLT.pdf) zunächst individuell bearbeiten**

    Die Lernenden sichern die Ergebnisse der Erkundung auf dem Blatt **„Dieselbe Situation – verschiedene Darstellungen“**.

    Die Aufgaben bündeln die zuvor untersuchten Zusammenhänge:

    - **Was zeigt welche Darstellung?**
    - **Kreuzung oder Wahrheitstabelle?**
    - **Was bedeutet `sicher`?**
    - **Welche Idee verbindet die verschiedenen Darstellungen?**

    Das [Merkblatt 2b](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2b_merkblatt_orientierung.pdf) darf bei Bedarf als Nachschlagehilfe verwendet werden.

    **2. Ergebnisse im Tandem vergleichen**

    Die Lernenden vergleichen ihre Zuordnungen und korrigieren Unterschiede nicht nur formal, sondern mit einer kurzen Begründung.

    **Leitfragen:**

    > Welche Darstellung zeigt nur eine aktuelle Ampelstellung?

    **Erwartete Antwort:** Die Kreuzung.

    > Wo finden wir dieselbe aktuelle Ampelstellung mit `0` und `1` wieder?

    **Erwartete Antwort:** In einer passenden Zeile der Wahrheitstabelle.

    > Was umfasst die gesamte Wahrheitstabelle darüber hinaus?

    **Erwartete Antwort:** Verschiedene bzw. alle möglichen Kombinationen der Variablenwerte.

    > Was sagt `sicher` aus?

    **Erwartete Antwort:** Ob die jeweilige Kombination der Ampelzustände kollisionsfrei ist.

    **3. [Tafelbild 2e](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2e_tafelbild_ergebnissicherung.pdf) zur gemeinsamen Sicherung einsetzen**

    Die Lehrperson projiziert [2e](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2e_tafelbild_ergebnissicherung.pdf) und ordnet die Begriffe gemeinsam mit der Klasse.

    Fachlich präzise kann die Beziehung so gesichert werden:

    **Kreuzung**  
    → zeigt Fahrwege und einen konkreten Ampelzustand

    **Variablen und `0`/`1`**  
    → beschreiben den Ampelzustand symbolisch

    **eine Tabellenzeile**  
    → beschreibt genau eine mögliche Belegung

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

??? note "Didaktische Hinweise"

    [2c](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2c_ergebnissicherungLT.pdf) und [2e](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2e_tafelbild_ergebnissicherung.pdf) erfüllen bewusst **verschiedene Rollen**:

    - **[2c](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2c_ergebnissicherungLT.pdf)** ist die aktive Ergebnissicherung der Lernenden.
    - **[2e](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2e_tafelbild_ergebnissicherung.pdf)** unterstützt die gemeinsame Auswertung durch die Lehrperson.

    Dadurch sollte [2e](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2e_tafelbild_ergebnissicherung.pdf) nicht vor der Bearbeitung von [2c](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2c_ergebnissicherungLT.pdf) gezeigt werden, da es sonst die eigentliche Sicherungsleistung vorwegnimmt.

    Fachlich ist zudem eine kleine Präzisierung wichtig: Eine konkrete Ampelstellung und eine gesamte Wahrheitstabelle sind nicht einfach „dieselbe Darstellung in anderer Form“. Eine **Tabellenzeile** entspricht einer konkreten Belegung; die **gesamte Tabelle** umfasst mehrere bzw. alle Belegungen. Die **Formel** beschreibt wiederum die übergeordnete Sicherheitsregel. Gerade diese Unterscheidung erleichtert später den Übergang zu Baustein 3 und 4.

    Die Formel bleibt hier ein **Ausblick**. Lernende müssen weder Operatoren kennen noch die angezeigte Formel erklären können.

??? bug "Differenzierung"

    === "Vereinfachungen"

        - [2b](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2b_merkblatt_orientierung.pdf) beim Ausfüllen von [2c](https://github.com/salomegolden/logictraffic/releases/download/ab2_v1/2c_ergebnissicherungLT.pdf) offen verwenden lassen.
        - Nur die vier Kernbereiche Kreuzung, Variablen/`0`–`1`, Wahrheitstabelle und `sicher` sichern; die Formel anschliessend gemeinsam ergänzen.
        - Satzstarter anbieten:  
          > „Die Kreuzung zeigt …“  
          > „Eine Tabellenzeile zeigt …“  
          > „Die ganze Wahrheitstabelle zeigt …“  
          > „`sicher = 1` bedeutet …“
        - Das Tafelbild Schritt für Schritt aufdecken bzw. besprechen.

    === "Erweiterungen"

        - Den Unterschied zwischen **einer Tabellenzeile** und der **gesamten Wahrheitstabelle** in eigenen Worten erklären lassen.
        - Begründen lassen, weshalb die Formel eher zur ganzen Sicherheitsregel als zu einer einzelnen Ampelstellung gehört.
        - Eine eigene grafische Darstellung der Repräsentationswechsel entwickeln lassen.
        - Bereits vermuten lassen, wie viele Zeilen eine vollständige Wahrheitstabelle mit drei Fahrspuren enthalten könnte, ohne die allgemeine Regel vorwegzunehmen.

## Abschluss des Bausteins

Am Ende von Baustein 2 können die Lernenden die digitale Lernumgebung nicht nur bedienen, sondern zentrale Elemente **fachlich deuten**:

1. Fahrspuren werden als Variablen `A`, `B`, `C` … bezeichnet.
2. `0` und `1` beschreiben bei den Variablen die Ampelzustände Rot und Grün.
3. Eine Tabellenzeile kann eine konkrete Ampelstellung symbolisch beschreiben.
4. Die Wahrheitstabelle umfasst verschiedene mögliche Ampelstellungen.
5. Die Spalte `sicher` bewertet, ob eine Kombination kollisionsfrei ist.
6. Die Formel ist eine weitere, kompakte Darstellung der Sicherheitsregel und wird erst später vertieft.

!!! success "Von der konkreten Kreuzung zur symbolischen Darstellung"

    Baustein 2 schafft die Brücke von der anschaulichen Verkehrssituation zur symbolischen Darstellung in LogicTraffic.

    Die nächste offene Frage lautet:

    > **Wie können wir selbst eine vollständige Wahrheitstabelle erstellen, ohne eine Kombination zu vergessen?**

    Genau diese Frage wird in [Baustein 3 – Wahrheitstabellen](baustein3-wahrheitstabellen.md) bearbeitet.