# Baustein 2 – LogicTraffic kennenlernen

In diesem Baustein lernen die Lernenden die digitale Lernumgebung LogicTraffic kennen. Sie untersuchen, wie die dargestellte Verkehrssituation, die Wahrheitstabelle und boolesche Formeln miteinander verbunden sind.

Im Zentrum steht zunächst nicht das formale Arbeiten mit Formeln. Die Lernenden sollen verstehen, welche Informationen die verschiedenen Bereiche der Oberfläche zeigen und wie sich Veränderungen an der Kreuzung in der Wahrheitstabelle widerspiegeln.

!!! abstract "Auf einen Blick"

    **:stopwatch: Dauer:**  
    45–60 Minuten

    **:busts_in_silhouette: Sozialform:**  
    Klassenunterricht, Partnerarbeit und kurze Einzelphasen

    **:computer: Computer:**  
    Ein Computer oder Tablet pro Zweiergruppe

    **:brain: Vorwissen:**  
    Die Lernenden können sichere und unsichere Verkehrssituationen unterscheiden.  
    Idealerweise wurde zuvor Baustein 1 durchgeführt.

    **:package: Material:**  
    LogicTraffic, Beamer oder Präsentationsbildschirm, Notizpapier

!!! note "Downloads zu Baustein 2"

    - [:material-image-outline: Bild: Aufbau der Webseite und ihre Bereiche](https://github.com/salomegolden/logictraffic/releases/download/images-v1/logictraffic_anleitung.png)
    - [:material-image-outline: Bild: Teilbereiche der Webseite](https://github.com/salomegolden/logictraffic/releases/download/images-v1/losungBeschriftungProgramm.png)
    - [:material-image-outline: Tafelbild: Beispiel für die Ergebnissicherung](https://github.com/salomegolden/logictraffic/releases/download/images-v1/b2_tafelbild.png)
    - [:memo: AB2.1 – Ergebnissicherung zur Orientierung auf der Webseite](https://github.com/salomegolden/logictraffic/releases/download/material-v1/b2_einfuhrung_logictraffic_AB.pdf)
    - [:film_projector: Präsentation mit Bildern von Kreuzungen](https://github.com/salomegolden/logictraffic/releases/download/material-v1/b2_prasentation_kreuzungen.pdf)

## Lernziele

Die Lernenden können …

- die zentralen Bereiche von LogicTraffic benennen;
- die Variablen `A`, `B`, `C` den entsprechenden Fahrspuren zuordnen;
- erklären, wie Ampelzustände mit `0` und `1` dargestellt werden;
- zu einer Ampelkombination die passende Tabellenzeile finden;
- sichere und unsichere Ampelkombinationen unterscheiden;
- die Bedeutung der Spalte «sicher» erklären;
- beschreiben, wie Kreuzung, Wahrheitstabelle und Formel zusammenhängen;
- die Rückmeldungen der Statusanzeige in Grundzügen deuten.

## Vorbereitung

- LogicTraffic auf den Geräten öffnen und die Funktionsfähigkeit prüfen.
- Eine einfache Situation mit zwei Fahrspuren auswählen.
- Dieselbe Situation für die gemeinsame Einführung über den Beamer bereitstellen.
- Falls Baustein 1 durchgeführt wurde, möglichst eine vergleichbare Verkehrssituation verwenden.
- Entscheiden, ob der Formelbereich zu Beginn ausgeblendet oder zunächst nicht thematisiert wird.

!!! note "Material"

    Für die Durchführung werden benötigt:

    - :globe_with_meridians: [LogicTraffic](https://logictraffic.ch/)
    - :material-tablet: ein Computer oder Tablet pro Zweiergruppe
    - :film_projector: ein Beamer oder Präsentationsbildschirm
    - :ledger: Notizpapier oder das Heft der Lernenden

!!! tip "Vorbereitung der Lernumgebung"

    Wählen Sie zunächst eine Situation mit zwei Variablen (1 oder 2, 11 ist auch möglich, aber ein Spezialfall). Dadurch gibt es nur vier mögliche Ampelkombinationen. Der Zusammenhang zwischen Kreuzung und Wahrheitstabelle bleibt so überschaubar.

## Programmaufbau

![Aufbau der Webseite und ihre Bereiche](https://github.com/salomegolden/logictraffic/releases/download/images-v1/logictraffic_anleitung.png)

| Bereich | Bedeutung |
| --- | --- |
| Kreuzung | Zeigt die Verkehrssituation, die Fahrspuren und die Ampeln. |
| Variablen | Bezeichnen die Fahrspuren mit `A`, `B`, `C` usw. |
| Wahrheitstabelle | Zeigt alle möglichen Kombinationen der Ampelzustände. |
| Spalte «sicher» | Legt fest, welche Kombinationen durch die Steuerung erlaubt werden. |
| Statusanzeige | Gibt eine Rückmeldung zur eingestellten Lösung. |
| Formelbereich | Beschreibt die als sicher festgelegten Zustände formal. |

!!! info "Fachlicher Hintergrund"

    Jede Zeile der Wahrheitstabelle steht für genau eine mögliche Kombination von Ampelzuständen.

    Bei zwei Ampeln gibt es vier Kombinationen:

    | `A` | `B` |
    | --- | --- |
    | `0` | `0` |
    | `0` | `1` |
    | `1` | `0` |
    | `1` | `1` |

    Im Kontext von LogicTraffic gilt:

    - `0`: Die Ampel ist rot.
    - `1`: Die Ampel ist grün.

    Die Werte `0` und `1` beschreiben zunächst nur die Zustände der Ampeln. Ob eine gesamte Kombination sicher ist, wird separat in der Spalte «sicher» festgelegt.

## Unterrichtsablauf

| Phase | Inhalt | Sozialform | Dauer |
| --- | --- | --- | --- |
| 1 | An den enaktiven Einstieg anknüpfen | Klassenunterricht | ca. 5 Min. |
| 2 | Oberfläche gemeinsam erkunden | Klassenunterricht | ca. 10 Min. |
| 3 | Ampelzustände und Tabellenzeilen untersuchen | Partnerarbeit | ca. 15 Min. |
| 4 | Sichere Zustände festlegen | Partnerarbeit | ca. 10–15 Min. |
| 5 | Darstellungen verbinden und Ergebnisse sichern | Klassenunterricht | ca. 10 Min. |

## Durchführung

### Phase 1 – An den enaktiven Einstieg anknüpfen

Falls Baustein 1 durchgeführt wurde, greift die Lehrperson die dort untersuchte Kreuzung nochmals auf. Die Lernenden erinnern sich daran, wie sie mit den Fahrzeugen und den drehbaren Ampelhölzchen sichere und unsichere Zustände dargestellt haben.

!!! quote "Einstiegsauftrag"

    Erinnert euch an die Kreuzung aus dem letzten Baustein.

    Überlegt:

    - Welche Informationen müssten wir einem Computer geben, damit er die Kreuzung darstellen kann?
    - Wie könnte der Computer verschiedene Ampelstellungen speichern?
    - Wie könnte er erkennen, ob eine Ampelstellung sicher ist?

Falls Baustein 1 nicht durchgeführt wurde, kann direkt eine einfache Kreuzung in LogicTraffic gezeigt werden.

!!! tip "Durchführungshinweis"

    Sammeln Sie die Vermutungen zunächst, ohne die Begriffe Wahrheitstabelle oder boolesche Formel vollständig zu erklären. Die Lernenden sollen die Darstellungen anschliessend im Tool selbst entdecken.

!!! note "Alternative Kreuzungen"

    Für einen Einstieg mit Verbindung zur realen Welt, können auch Bilder aus der [Präsentation Kreuzungen](https://github.com/salomegolden/logictraffic/releases/download/material-v1/b2_prasentation_kreuzungen.pdf) gezeigt werden. Dazu gehört dann die Frage, was es braucht, damit die entsprechende Kreuzung sicher funktioniert.

### Phase 2 – Oberfläche gemeinsam erkunden

Die Lehrperson öffnet eine einfache Situation mit zwei Fahrspuren in [LogicTraffic](https://logictraffic.ch/) und zeigt die Oberfläche über den Beamer.

Zunächst werden nur vier Bereiche betrachtet:

1. Kreuzung
2. Variablen
3. Wahrheitstabelle
4. Spalte «sicher»

Der Formelbereich wird noch nicht vertieft.

![Teilbereiche von LogicTraffic mit Beschriftungen](https://github.com/salomegolden/logictraffic/releases/download/images-v1/losungBeschriftungProgramm.png)

Die Abbildung kann über den Beamer gezeigt oder den Lernenden als Orientierung bereitgestellt werden.

!!! quote "Beobachtungsauftrag"

    Beobachtet genau, was passiert, wenn eine Ampel angeklickt wird.

    Achtet dabei auf:

    - die Farbe der Ampel;
    - die Werte `0` und `1`;
    - die markierte Zeile in der Wahrheitstabelle.

Die Lehrperson stellt nacheinander verschiedene Ampelkombinationen ein.

!!! quote "Gemeinsam festhalten"

    Gemeinsam wird festgehalten:

    - Jede Fahrspur besitzt eine Variable.
    - Die Variable beschreibt den Zustand der zugehörigen Ampel.
    - Die aktuelle Ampelstellung gehört zu genau einer Tabellenzeile.
    - Die Wahrheitstabelle enthält alle möglichen Ampelstellungen.

!!! info "Warum gibt es vier Tabellenzeilen?"

    Jede der beiden Ampeln kann zwei Zustände annehmen:

    - rot
    - grün

    Daraus entstehen vier mögliche Kombinationen:

    - beide rot;
    - `A` rot und `B` grün;
    - `A` grün und `B` rot;
    - beide grün.

!!! warning "Typische Lernschwierigkeit: 0 und 1"

    Lernende interpretieren `0` möglicherweise als «falsch» oder «falsch eingestellt» und `1` als «richtig».

    Stellen Sie deshalb immer wieder den Bezug zur Kreuzung her:

    - `0` bedeutet hier: rot.
    - `1` bedeutet hier: grün.

### Phase 3 – Ampelzustände und Tabellenzeilen untersuchen

Die Lernenden arbeiten in Zweiergruppen. Eine Person bedient LogicTraffic, die andere beobachtet und notiert. Nach der Hälfte der Zeit werden die Rollen gewechselt.

!!! quote "Lernauftrag 1 – Oberfläche untersuchen"

    Öffnet eine Situation mit zwei Fahrzeugen (Situation 1, 2, 11).

    Untersucht gemeinsam:

    1. Welche Variable gehört zu welcher Fahrspur?
    2. Was verändert sich, wenn ihr eine Ampel anklickt?
    3. Welche Tabellenzeile gehört zur aktuellen Ampelstellung?
    4. Welche vier Ampelkombinationen sind möglich?
    5. Woran erkennt ihr, dass ihr alle Kombinationen ausprobiert habt?

!!! note "Mögliche Ergebnissicherung"

    Alternativ zur selbst gezeichneten Tabelle kann das Arbeitsblatt  
    [:memo: **AB2.1 – Orientierung auf der Webseite**](https://github.com/salomegolden/logictraffic/releases/download/material-v1/b2_einfuhrung_logictraffic_AB.pdf)  
    eingesetzt werden. Es unterstützt die Lernenden dabei, die Bereiche der Oberfläche und ihre Funktionen festzuhalten.

???+ quote "Einträge ins Heft oder Notizbuch"

    Die Lernenden können ihre Beobachtungen in einer selbst gezeichneten Tabelle festhalten:

    | Ampel `A` | Ampel `B` | Tabellenwerte |
    | --- | --- | --- |
    | rot | rot | |
    | rot | grün | |
    | grün | rot | |
    | grün | grün | |

!!! tip "Durchführungshinweis"

    Lassen Sie die Lernenden die Tabelle selbst zeichnen. Dadurch wird sichtbar, ob sie die vier Kombinationen systematisch erfassen können.

    Unterstützende Fragen:

    - Welche Kombination fehlt noch?
    - Worin unterscheidet sich diese Zeile von der vorherigen?
    - Welche Ampel gehört zur ersten Spalte?
    - Wie kannst du die Tabellenzeile an der Kreuzung überprüfen?

??? example "Mögliches Ergebnis"

    | Ampel `A` | Ampel `B` | Tabellenwerte |
    | --- | --- | --- |
    | rot | rot | `0`, `0` |
    | rot | grün | `0`, `1` |
    | grün | rot | `1`, `0` |
    | grün | grün | `1`, `1` |

!!! warning "Typische Lernschwierigkeit: nur den aktuellen Zustand betrachten"

    Einige Lernende konzentrieren sich ausschliesslich auf die aktuell sichtbare Kreuzung.

    Erinnern Sie daran, dass die Wahrheitstabelle nicht nur den aktuellen Zustand zeigt. Sie enthält alle möglichen Kombinationen, auch wenn an der Kreuzung jeweils nur eine davon dargestellt wird.

### Phase 4 – Sichere Zustände festlegen

Nun untersuchen die Lernenden, welche Ampelkombinationen bei der gewählten Kreuzung (hier nur Kreuzungen 1 oder 2 sinnvoll) sicher sind.

!!! quote "Lernauftrag 2 – Sichere Zustände untersuchen"

    Probiert alle vier Ampelkombinationen aus.

    Entscheidet für jede Kombination:

    1. Ist die Verkehrssituation sicher oder unsicher?
    2. Woran erkennt ihr das an der Kreuzung?
    3. Welcher Wert muss in der Spalte «sicher» stehen?
    4. Wie verändert sich die Statusanzeige?

Die Lernenden tragen ihre Entscheidungen in LogicTraffic ein und beobachten die Rückmeldungen.

!!! tip "Durchführungshinweis"

    Fordern Sie bei jeder Entscheidung eine Begründung ein.

    Statt:

    > Diese Zeile ist falsch.

    sollten die Lernenden genauer formulieren:

    > Diese Kombination ist unsicher, weil sich die Fahrwege von `A` und `B` kreuzen.

!!! info "Sicher und optimal"

    Eine sichere Steuerung erlaubt keine gefährlichen Ampelkombinationen.

    Sie ist jedoch nicht automatisch optimal. Eine Steuerung kann unnötig viele sichere Kombinationen verbieten.

    Wenn beispielsweise alle Ampeln immer rot bleiben, entstehen zwar keine Kollisionen, der Verkehr wird aber vollständig blockiert.

!!! warning "Typische Lernschwierigkeit: sicher und optimal"

    Lernende setzen «sicher» und «optimal» möglicherweise gleich.

    Verdeutlichen Sie den Unterschied:

    - **sicher:** Keine gefährliche Kombination wird erlaubt.
    - **optimal:** Alle sicheren und sinnvollen Kombinationen werden zugelassen, ohne eine gefährliche Kombination zu erlauben.

### Phase 5 – Kreuzung, Tabelle und Formel verbinden

Erst nachdem Kreuzung und Wahrheitstabelle verstanden wurden, wird der Formelbereich einbezogen.

Die Lehrperson zeigt, wie sich die Formel verändert, wenn in der Spalte «sicher» ein Wert geändert wird.

!!! quote "Lernauftrag 3 – Drei Darstellungen vergleichen"

    Betrachtet dieselbe Sicherheitsregel in drei Darstellungen:

    1. :frame_photo: als Verkehrssituation;
    2. :material-table: als Wahrheitstabelle;
    3. :symbols: als Formel (hier bitte "einfachste" einstellen).

    Besprecht:

    - Was zeigt die Kreuzung?
    - Was zeigt die Wahrheitstabelle?
    - Was beschreibt die Formel?
    - Welche Informationen sind in allen drei Darstellungen gleich?

    Gemeinsam kann auch das Tafelbild ausgefüllt werden: 
    ![Tafelbild B2, generiert mit ChatGPT, GPT5.6](https://github.com/salomegolden/logictraffic/releases/download/images-v1/b2_tafelbild.png)

!!! tip "Durchführungshinweis"

    Die Begriffe DNF und KNF müssen in diesem Baustein noch nicht eingeführt werden.

    Entscheidend ist zunächst nur die Erkenntnis, dass die Formel dieselben sicheren Zustände beschreibt wie die Wahrheitstabelle.

!!! warning "Typische Lernschwierigkeit: Formel zu früh formalisieren"

    Die Formelansicht kann überfordern, wenn der Zusammenhang zwischen Kreuzung und Wahrheitstabelle noch nicht verstanden ist.

    Lassen Sie die Lernenden die Formel zunächst nur als dritte Darstellung derselben Sicherheitsregel betrachten. Falls gar kein Vorwissen zu den logischen Operationen und die Darstellung der logischen Formeln vorhanden ist, kann diese Phase auch noch weggelassen werden. 

## Ergebnissicherung

Die Ergebnisse werden gemeinsam gesammelt und als Tafelbild oder digitale Notiz festgehalten.

??? example "Ergebnisse"

    ![Tafelbild B2, generiert mit ChatGPT, GPT5.6](https://github.com/salomegolden/logictraffic/releases/download/images-v1/b2_tafelbild.png)

    **LogicTraffic verbindet mehrere Darstellungen**

    | Darstellung | Bedeutung |
    | --- | --- |
    | Kreuzung | zeigt einen konkreten Ampelzustand |
    | Wahrheitstabelle | zeigt alle möglichen Ampelzustände |
    | Spalte «sicher» | legt fest, welche Zustände erlaubt sind |
    | Formel | beschreibt die Sicherheitsregel formal |

    **Merksätze**

    - Jede Fahrspur wird durch eine Variable bezeichnet.
    - `0` steht in LogicTraffic für Rot.
    - `1` steht in LogicTraffic für Grün.
    - Jede Zeile der Wahrheitstabelle beschreibt eine mögliche Ampelkombination.
    - Die Spalte «sicher» bewertet die gesamte Kombination.
    - Die Formel beschreibt dieselben sicheren Zustände wie die Wahrheitstabelle.

## Erwartete Ergebnisse

Die Lernenden sollten am Ende beispielsweise erklären können:

> Wenn `A = 1` und `B = 0` ist, dann ist die Ampel von `A` grün und die Ampel von `B` rot.

> Die Wahrheitstabelle enthält alle möglichen Kombinationen der Ampelzustände.

> In der Spalte «sicher» wird festgelegt, welche Kombinationen erlaubt werden.

> Die Formel beschreibt dieselbe Sicherheitsregel wie die Wahrheitstabelle.

??? example "Mögliche Erklärung einer Situation"

    Wenn sich die Fahrwege von `A` und `B` kreuzen, dürfen nicht beide Ampeln gleichzeitig grün sein.

    Die Tabellenzeile `A = 1` und `B = 1` muss deshalb als unsicher markiert werden.

## Typische Lernschwierigkeiten

??? warning "0 und 1 werden mit falsch und richtig verwechselt"

    Die Werte beschreiben zunächst nur den Zustand einer Ampel:

    - `0`: rot
    - `1`: grün

    Ob die gesamte Kombination sicher ist, wird erst in der Spalte «sicher» festgelegt.

??? warning "Aktuelle Kreuzung und Wahrheitstabelle werden gleichgesetzt"

    Die Kreuzung zeigt jeweils nur eine Kombination. Die Wahrheitstabelle enthält dagegen alle möglichen Kombinationen.

    Lassen Sie die Lernenden wiederholt zwischen einer konkreten Ampelstellung und der zugehörigen Tabellenzeile wechseln.

??? warning "Sicherheit wird nur anhand einzelner Ampeln beurteilt"

    Nicht eine einzelne Ampel ist sicher oder unsicher, sondern die Kombination mehrerer Ampelzustände im Zusammenhang mit den Fahrwegen.

??? warning "Die Statusanzeige ersetzt die eigene Begründung"

    Lernende können versuchen, Werte so lange zu verändern, bis «optimal» erscheint.

    Verlangen Sie deshalb zuerst eine fachliche Entscheidung und erst danach die Überprüfung mit der Statusanzeige.

## Differenzierung

### Unterstützung

- Eine Situation mit nur zwei Variablen verwenden.
- Die Variablen direkt an den Fahrspuren zeigen.
- `0` und `1` zusätzlich mit roten und grünen Punkten notieren.
- Die vier möglichen Kombinationen gemeinsam vorgeben.
- Satzanfänge bereitstellen:

    > Die Tabellenzeile passt zur Kreuzung, weil …

    > Die Situation ist sicher, weil …

    > Die Situation ist unsicher, weil …

!!! tip "Unterstützung in der Partnerarbeit"

    Achten Sie darauf, dass nicht nur die technisch erfahrenere Person das Tool bedient.

    Lassen Sie die Rollen bewusst wechseln:

    - Person 1 bedient LogicTraffic.
    - Person 2 beschreibt und begründet.
    - Danach werden die Rollen getauscht.

### Erweiterung

- Eine Situation mit drei Variablen auswählen.
- Vorhersagen, wie viele Tabellenzeilen benötigt werden.
- Eine sichere, aber nicht optimale Lösung herstellen.
- Zwei verschiedene sichere Lösungen vergleichen.
- Beobachten, wie sich die Formel bei einer Änderung der Tabelle verändert.
- Eine Sicherheitsregel zuerst in Alltagssprache formulieren und anschliessend im Tool umsetzen.

!!! question "Vertiefende Reflexion"

    Bei zwei Ampeln gibt es vier mögliche Kombinationen.

    - Wie viele Kombinationen gibt es bei drei Ampeln?
    - Wie könnt ihr diese Anzahl bestimmen, ohne alle Kombinationen aufzuschreiben?
    - Warum wird eine systematische Darstellung bei mehr Ampeln immer wichtiger?

## Übergang zum nächsten Baustein

Zum Abschluss wird der Blick auf die systematische Konstruktion von Wahrheitstabellen gelenkt.

!!! question "Übergang zur Wahrheitstabelle"

    LogicTraffic zeigt bereits alle möglichen Ampelkombinationen.

    Wie können wir eine solche Wahrheitstabelle selbstständig aufbauen, ohne eine Kombination zu vergessen?

Diese Frage führt zum nächsten Baustein, in dem Wahrheitstabellen systematisch erstellt, gelesen und interpretiert werden.

## Materialien

!!! note "Benötigtes Material"

    - LogicTraffic
    - Computer oder Tablets
    - Beamer oder Präsentationsbildschirm
    - Notizpapier oder Hefte

!!! note "Ergänzendes Material und Downloads"

    - [:material-image-outline: **Aufbau der Webseite und ihre Bereiche**](https://github.com/salomegolden/logictraffic/releases/download/images-v1/logictraffic_anleitung.png)
    - [:material-image-outline: **Teilbereiche der Webseite**](https://github.com/salomegolden/logictraffic/releases/download/images-v1/losungBeschriftungProgramm.png)
    - [:material-image-outline: **Tafelbild zur Ergebnissicherung**](https://github.com/salomegolden/logictraffic/releases/download/images-v1/b2_tafelbild.png)
    - [:memo: **AB2.1 – Orientierung auf der Webseite**](https://github.com/salomegolden/logictraffic/releases/download/material-v1/b2_einfuhrung_logictraffic_AB.pdf)
    - [:film_projector: **Präsentation mit Bildern von Kreuzungen**](https://github.com/salomegolden/logictraffic/releases/download/material-v1/b2_prasentation_kreuzungen.pdf)

!!! note "Mögliche spätere Ergänzungen"

    Ergänzend könnten später noch ein Beobachtungsbogen zur Partnerarbeit, eine Merkkarte zu Kreuzung, Wahrheitstabelle und Formel sowie eine kurze Aufgabe zur formativen Lernstandserhebung entwickelt werden.
