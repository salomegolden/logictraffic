# Baustein 3 – Wahrheitstabellen

In diesem Baustein lernen die Lernenden, Wahrheitstabellen nicht nur in LogicTraffic zu lesen, sondern selbstständig und systematisch aufzubauen.

Ausgehend von einer einfachen Kreuzung mit zwei Fahrspuren untersuchen sie, wie alle möglichen Ampelzustände vollständig erfasst werden können. Anschliessend übertragen sie die Systematik auf drei und mehr Variablen und erkennen, dass sich die Anzahl möglicher Zustände mit jeder zusätzlichen Variable verdoppelt.

Am Ende des Bausteins wird deutlich, dass Wahrheitstabellen zwar eine vollständige Beschreibung ermöglichen, bei vielen Variablen jedoch schnell sehr umfangreich werden. Diese Erkenntnis bereitet den Übergang zu kompakten logischen Formeln in Baustein 4 vor.

!!! abstract "Auf einen Blick"

    **:stopwatch: Dauer:**  
    ca. 45–60 Minuten

    **:busts_in_silhouette: Sozialform:**  
    Plenum, Partnerarbeit und kurze Einzelphasen

    **:computer: Computer:**  
    Ein Computer oder Tablet mit LogicTraffic pro Zweiergruppe

    **:brain: Vorwissen:**  
    - Die Lernenden kennen LogicTraffic.
    - Die Lernenden kennen Variablen als Bezeichnungen für Fahrspuren.
    - `0 = Rot` und `1 = Grün` sind bekannt.
    - Die Lernenden können eine konkrete Ampelstellung einer Tabellenzeile zuordnen.
    - Die Bedeutung der Spalte `sicher` ist grundsätzlich bekannt.
    - Idealerweise wurde zuvor Baustein 2 durchgeführt.

    **:package: Material:**  
    LogicTraffic, Computer oder Tablets, Beamer oder Präsentationsbildschirm, Arbeitsblatt bzw. Heft oder Begleitportfolio

!!! note "Downloads zu Baustein 3"

    - [:memo: Arbeitsblatt zu Wahrheitstabellen](LINK_ERGÄNZEN)
    - [:material-image-outline: Tafelbild / Merkhilfe zu Wahrheitstabellen](LINK_ERGÄNZEN)

## Lernziele

Die Lernenden können …

- eine Wahrheitstabelle als vollständige Darstellung aller möglichen Kombinationen von Variablenwerten erklären;
- für zwei und drei Variablen alle möglichen Belegungen systematisch und lückenlos aufschreiben;
- erklären, warum bei $n$ Variablen $2^n$ mögliche Belegungen entstehen;
- für jede Ampelkombination begründet entscheiden, ob die Verkehrssituation sicher oder unsicher ist;
- zwischen den Werten der Fahrspuren (`0` und `1`) und dem Wert der Spalte `sicher` unterscheiden;
- von einer konkreten Verkehrssituation zur symbolischen Darstellung in einer Wahrheitstabelle wechseln;
- erkennen, dass Wahrheitstabellen bei zunehmender Anzahl von Variablen schnell sehr umfangreich werden;
- daraus die Notwendigkeit einer kompakteren Darstellung ableiten.

## Vorbereitung

- LogicTraffic auf den Geräten öffnen und die Funktionsfähigkeit prüfen.
- Für den Einstieg eine einfache Situation mit zwei Fahrspuren vorbereiten.
- Eine Situation mit drei Fahrspuren für die Vertiefung vorbereiten.
- Für den abschliessenden Skalierungsvergleich eine Situation mit fünf Fahrspuren bereitstellen.
- Arbeitsblatt oder Heft für das eigenständige Erstellen von Wahrheitstabellen bereitlegen.
- Falls möglich, die Tabellen zunächst ausserhalb von LogicTraffic erstellen lassen und die Lernumgebung erst anschliessend zur Überprüfung verwenden.

??? tip "Abgrenzung zu Baustein 2"

    In Baustein 2 haben die Lernenden die Wahrheitstabelle bereits als Darstellung kennengelernt.

    In diesem Baustein steht eine neue Frage im Zentrum:

    > **Wie können wir selbst eine vollständige Wahrheitstabelle erstellen, ohne eine Kombination zu vergessen?**

    Der Schwerpunkt liegt deshalb nicht mehr auf der Orientierung in LogicTraffic, sondern auf der **Systematik und Vollständigkeit einer Wahrheitstabelle**.

## Fachlicher Hintergrund

Eine Wahrheitstabelle enthält alle möglichen Belegungen der verwendeten Variablen.

Da jede Variable in LogicTraffic genau zwei Zustände annehmen kann,

- `0` = Rot
- `1` = Grün,

verdoppelt jede zusätzliche Variable die Anzahl der möglichen Kombinationen.

| Anzahl Variablen | Anzahl möglicher Zustände |
| ---: | ---: |
| 1 | $2^1 = 2$ |
| 2 | $2^2 = 4$ |
| 3 | $2^3 = 8$ |
| 4 | $2^4 = 16$ |
| 5 | $2^5 = 32$ |

Allgemein gilt:

$$
\text{Anzahl der möglichen Belegungen} = 2^n
$$

Dabei bezeichnet $n$ die Anzahl der Variablen.

!!! warning "Zwei verschiedene Bedeutungen von 0 und 1"

    In LogicTraffic werden `0` und `1` auf zwei verschiedenen Ebenen verwendet.

    **Bei den Fahrspuren:**

    - `0` = Die Ampel ist rot.
    - `1` = Die Ampel ist grün.

    **In der Spalte `sicher`:**

    - `0` = Die Kombination ist unsicher.
    - `1` = Die Kombination ist sicher.

    Diese beiden Bedeutungen sollten im Unterricht konsequent voneinander unterschieden werden.

## Unterrichtsablauf – Überblick

| Phase | Inhalt | Sozialform / Medien | Richtwert |
| --- | --- | --- | --- |
| **1. Problemstellung** | Vorwissen aktivieren und nach einer vollständigen Darstellung aller Zustände fragen | Plenum, LogicTraffic / Beamer | ca. 5–7 Min. |
| **2. Systematisierung** | Wahrheitstabelle mit zwei Variablen selbstständig erstellen | Partnerarbeit, Arbeitsblatt / Heft, LogicTraffic | ca. 10–12 Min. |
| **3. Verallgemeinerung** | Vorgehen auf drei Variablen übertragen und die Regel $2^n$ entwickeln | Partnerarbeit, Arbeitsblatt, LogicTraffic | ca. 15 Min. |
| **4. Skalierungsproblem** | Wachstum der Wahrheitstabelle bei mehr Variablen untersuchen | Plenum, Beamer | ca. 8–10 Min. |
| **5. Sicherung und Ausblick** | Kernregeln sichern und zur Darstellung mit Formeln überleiten | Plenum / Einzelarbeit | ca. 5–10 Min. |

## Durchführung

### Phase 1 – Wie finden wir wirklich alle Zustände?

**Ziel der Phase:**  
Die Lernenden erkennen, dass zufälliges Ausprobieren nicht genügt, wenn alle möglichen Zustände vollständig erfasst werden sollen.

Die Lehrperson greift eine einfache Situation mit zwei Fahrspuren auf.

Falls Baustein 2 durchgeführt wurde, ist die Wahrheitstabelle in LogicTraffic bereits bekannt. Nun wird die Tabelle jedoch zunächst nicht als fertige Lösung verwendet.

!!! quote "Einstiegsfrage"

    Wir wissen:

    Jede Ampel kann entweder rot oder grün sein.

    **Wie können wir alle möglichen Ampelstellungen aufschreiben und sicher sein, dass wir keine vergessen?**

Die Lernenden sammeln mögliche Vorgehensweisen.

Dabei können unterschiedliche Strategien entstehen:

- zufälliges Ausprobieren;
- Kombinationen notieren;
- immer nur eine Ampel verändern;
- bereits untersuchte Kombinationen markieren;
- nach einem festen Muster vorgehen.

Die Lehrperson greift insbesondere die Frage nach der **Vollständigkeit** auf.

!!! question "Zentrale Leitfrage"

    Woran können wir erkennen, dass unsere Liste wirklich vollständig ist?

??? note "Didaktische Absicht"

    Die Wahrheitstabelle soll an dieser Stelle nicht einfach als fertige Konvention präsentiert werden.

    Die Lernenden sollen zunächst selbst das Problem erleben, alle möglichen Zustände vollständig und ohne Wiederholungen zu erfassen.

    Dadurch wird die tabellarische Systematik als Lösung eines konkreten Problems verständlich.

### Phase 2 – Eine Wahrheitstabelle mit zwei Variablen erstellen

**Ziel der Phase:**  
Die Lernenden erstellen für zwei Variablen selbstständig eine vollständige Wahrheitstabelle und erkennen ein systematisches Ordnungsmuster.

Die Lernenden arbeiten zunächst ohne die bereits ausgefüllte Wahrheitstabelle von LogicTraffic.

!!! quote "Lernauftrag 1 – Alle Kombinationen finden"

    Die Kreuzung besitzt zwei Fahrspuren `A` und `B`.

    Beide Ampeln können entweder rot (`0`) oder grün (`1`) sein.

    1. Notiert alle möglichen Kombinationen.
    2. Ordnet sie so, dass ihr sicher sein könnt, keine Kombination vergessen zu haben.
    3. Überlegt, wie viele Kombinationen es insgesamt geben muss.
    4. Prüft anschliessend eure Tabelle mit LogicTraffic.

Ein mögliches Ergebnis ist:

| `A` | `B` |
| --- | --- |
| `0` | `0` |
| `0` | `1` |
| `1` | `0` |
| `1` | `1` |

Gemeinsam wird herausgearbeitet:

$$
2 \cdot 2 = 4 = 2^2
$$

Beide Variablen können jeweils zwei mögliche Zustände annehmen. Deshalb entstehen insgesamt vier Kombinationen.

Anschliessend wird die Tabelle um die Spalte `sicher` ergänzt.

| `A` | `B` | `sicher` |
| --- | --- | --- |
| `0` | `0` | |
| `0` | `1` | |
| `1` | `0` | |
| `1` | `1` | |

!!! quote "Lernauftrag 2 – Sicherheit beurteilen"

    Prüft jede Tabellenzeile an der Kreuzung.

    Entscheidet:

    - Welche Ampeln sind grün?
    - Welche Ampeln sind rot?
    - Schneiden sich die Fahrwege der grünen Spuren?
    - Ist die Kombination sicher oder unsicher?
    - Welchen Wert erhält die Spalte `sicher`?

Die Lernenden begründen ihre Entscheidung zunächst anhand der Verkehrssituation und überprüfen sie anschliessend mit LogicTraffic.

??? warning "Typischer Stolperstein: Alle Ampeln sind rot"

    Manche Lernende beurteilen die Kombination `00` als unsicher, weil kein Verkehr fliessen kann.

    Hier sollte zwischen **Sicherheit** und **Effizienz** unterschieden werden.

    `sicher = 1` bedeutet:

    > Es kann bei dieser Ampelstellung zu keiner Kollision kommen.

    Eine Ampelstellung kann deshalb sicher sein, obwohl kein Fahrzeug fahren darf.

### Phase 3 – Von zwei zu drei Variablen

**Ziel der Phase:**  
Die Lernenden übertragen das Vorgehen auf drei Variablen und entwickeln eine allgemeine Strategie zur vollständigen Erfassung aller Kombinationen.

Nun wird eine Situation mit drei Fahrspuren verwendet.

!!! quote "Lernauftrag 3 – Drei Fahrspuren"

    Die Kreuzung besitzt nun drei Variablen:

    `A`, `B` und `C`.

    Überlegt zuerst:

    1. Wie viele verschiedene Kombinationen erwartet ihr?
    2. Wie könnt ihr diese Anzahl berechnen?
    3. Wie könnt ihr die Kombinationen so ordnen, dass keine fehlt und keine doppelt vorkommt?

Gemeinsam wird hergeleitet:

$$
2 \cdot 2 \cdot 2 = 8 = 2^3
$$

Anschliessend erstellen die Lernenden eine vollständige Wahrheitstabelle.

| `A` | `B` | `C` | `sicher` |
| --- | --- | --- | --- |
| `0` | `0` | `0` | |
| `0` | `0` | `1` | |
| `0` | `1` | `0` | |
| `0` | `1` | `1` | |
| `1` | `0` | `0` | |
| `1` | `0` | `1` | |
| `1` | `1` | `0` | |
| `1` | `1` | `1` | |

Die Lernenden können dabei das geordnete Muster erkennen:

`000`, `001`, `010`, `011`, `100`, `101`, `110`, `111`

!!! info "Systematisches Muster"

    Die Kombinationen können ähnlich wie beim binären Zählen geordnet werden.

    Bei drei Variablen sieht das Muster beispielsweise so aus:

    **Variable `C`:**

    `0, 1, 0, 1, 0, 1, 0, 1`

    **Variable `B`:**

    `0, 0, 1, 1, 0, 0, 1, 1`

    **Variable `A`:**

    `0, 0, 0, 0, 1, 1, 1, 1`

    Dadurch kann jede mögliche Kombination genau einmal aufgeschrieben werden.

Anschliessend beurteilen die Lernenden auch bei dieser Kreuzung die einzelnen Kombinationen als sicher oder unsicher.

LogicTraffic dient dabei zur Überprüfung der selbst erstellten Tabelle.

!!! tip "LogicTraffic als Kontrollwerkzeug"

    Lassen Sie die Lernenden die Wahrheitstabelle möglichst zuerst selbst erstellen.

    Erst danach werden die Kombinationen in LogicTraffic überprüft.

    Dadurch bleibt die Lernumgebung ein Werkzeug zur Exploration und Rückmeldung, ohne den eigentlichen Denkprozess vorwegzunehmen.

??? tip "Aufgabe für schnellere Lernende"

    Geben Sie eine Wahrheitstabelle mit eingebauten Fehlern vor.

    Mögliche Fehler:

    - eine Kombination kommt doppelt vor;
    - eine Kombination fehlt;
    - eine sichere Kombination ist als `sicher = 0` markiert;
    - eine unsichere Kombination ist als `sicher = 1` markiert.

    Auftrag:

    > Findet die Fehler, begründet eure Entscheidung und überprüft die Korrektur mit LogicTraffic.

### Phase 4 – Grenzen von Wahrheitstabellen

**Ziel der Phase:**  
Die Lernenden erkennen das exponentielle Wachstum von Wahrheitstabellen und entwickeln ein Bedürfnis nach einer kompakteren Darstellung.

Die bisherigen Ergebnisse werden gemeinsam gesammelt.

| Anzahl Variablen | Anzahl Tabellenzeilen |
| ---: | ---: |
| 1 | $2^1 = 2$ |
| 2 | $2^2 = 4$ |
| 3 | $2^3 = 8$ |
| 4 | $2^4 = 16$ |
| 5 | $2^5 = 32$ |

Die Lernenden formulieren daraus die allgemeine Regel:

$$
\text{Bei } n \text{ Variablen gibt es } 2^n \text{ mögliche Belegungen.}
$$

Nun wird eine Kreuzung mit fünf Fahrspuren gezeigt.

!!! quote "Impuls"

    Stellt euch vor, wir müssten für diese Kreuzung jede einzelne Ampelkombination von Hand untersuchen.

    - Wie viele Tabellenzeilen benötigen wir?
    - Wie übersichtlich ist diese Tabelle noch?
    - Was würde bei zehn Ampeln passieren?

Bei fünf Variablen entstehen:

$$
2^5 = 32
$$

mögliche Kombinationen.

Bei zehn Variablen wären es bereits:

$$
2^{10} = 1024
$$

mögliche Kombinationen.

!!! question "Zentrale Leitfrage"

    Wahrheitstabellen können alle möglichen Fälle vollständig darstellen.

    **Können wir dieselbe Sicherheitsregel auch kürzer beschreiben, ohne jede einzelne Kombination aufzuschreiben?**

??? info "Stärke und Grenze von Wahrheitstabellen"

    Wahrheitstabellen besitzen einen wichtigen Vorteil:

    > Sie zeigen **vollständig und eindeutig alle möglichen Zustände**.

    Gleichzeitig zeigt sich eine Grenze:

    > Mit jeder zusätzlichen Variable verdoppelt sich die Anzahl der möglichen Belegungen.

    Dadurch werden Wahrheitstabellen bei vielen Variablen schnell sehr umfangreich.

    Diese Erkenntnis motiviert die Suche nach einer kompakteren symbolischen Darstellung.

### Phase 5 – Ergebnisse sichern und zur Formel überleiten

**Ziel der Phase:**  
Die Lernenden sichern die grundlegende Systematik von Wahrheitstabellen und formulieren erste Sicherheitsregeln in Alltagssprache.

Gemeinsam werden die wichtigsten Erkenntnisse festgehalten.

??? example "Mögliche Ergebnissicherung"

    **Wahrheitstabellen**

    - Jede Variable besitzt zwei mögliche Werte: `0` und `1`.
    - Bei $n$ Variablen gibt es $2^n$ mögliche Kombinationen.
    - Eine vollständige Wahrheitstabelle enthält jede mögliche Kombination genau einmal.
    - In LogicTraffic bedeutet:
        - `0` bei einer Fahrspur = Rot
        - `1` bei einer Fahrspur = Grün
    - Die Spalte `sicher` bewertet die gesamte Ampelkombination:
        - `0` = unsicher
        - `1` = sicher
    - Wahrheitstabellen sind vollständig und eindeutig, werden bei vielen Variablen aber sehr umfangreich.

Anschliessend formulieren die Lernenden für eine einfache Kreuzung eine Sicherheitsregel zunächst in Alltagssprache.

Beispiele:

> Wenn Spur `C` grün ist, müssen die kreuzenden Spuren rot sein.

> `A` und `C` dürfen nicht gleichzeitig grün sein.

> Wenn `A` grün ist, muss `B` rot sein.

Die Regeln werden an dieser Stelle noch nicht formalisiert.

!!! question "Ausblick"

    Wie könnten wir eine solche Regel so aufschreiben, dass sie eindeutig und gleichzeitig viel kürzer als eine vollständige Wahrheitstabelle ist?

Damit ist der Übergang zu Baustein 4 vorbereitet.

## Ergebnissicherung

Am Ende des Bausteins sollten die Lernenden eine einfache Wahrheitstabelle selbstständig aufbauen und die grundlegende Regel $2^n$ erklären können.

Eine mögliche Merkhilfe:

| Begriff | Bedeutung |
| --- | --- |
| Variable | bezeichnet eine Fahrspur |
| `0` | Ampel ist rot |
| `1` | Ampel ist grün |
| Belegung | eine bestimmte Kombination der Variablenwerte |
| Wahrheitstabelle | vollständige Sammlung aller möglichen Belegungen |
| `sicher = 1` | Kombination ist kollisionsfrei |
| `sicher = 0` | Kombination ist nicht kollisionsfrei |
| $2^n$ | Anzahl möglicher Belegungen bei $n$ Variablen |

!!! success "Ich kann …"

    - für zwei Variablen alle vier Kombinationen aufschreiben;
    - für drei Variablen alle acht Kombinationen aufschreiben;
    - erklären, warum die Anzahl der Kombinationen $2^n$ beträgt;
    - eine Tabellenzeile an der Kreuzung darstellen;
    - entscheiden und begründen, ob eine Kombination sicher ist;
    - erklären, warum Wahrheitstabellen bei vielen Variablen sehr umfangreich werden.

## Erwartete Ergebnisse

Die Lernenden sollten am Ende beispielsweise erklären können:

> Bei drei Variablen gibt es acht mögliche Kombinationen, weil jede Variable zwei Werte haben kann:

$$
2 \cdot 2 \cdot 2 = 8
$$

> Eine Wahrheitstabelle ist vollständig, wenn jede mögliche Kombination genau einmal vorkommt.

> `A = 1` bedeutet, dass die Ampel der Spur `A` grün ist. Das bedeutet aber noch nicht, dass die gesamte Verkehrssituation sicher ist.

> Ob eine Kombination sicher ist, hängt davon ab, welche Fahrspuren gleichzeitig grün sind und ob sich ihre Fahrwege kreuzen.

> Bei fünf Variablen benötigt eine vollständige Wahrheitstabelle bereits $32$ Zeilen.

## Typische Lernschwierigkeiten

??? warning "0 und 1 werden auf beiden Ebenen verwechselt"

    Wiederholen Sie die Unterscheidung:

    **Variablenspalten:**

    - `0` = Rot
    - `1` = Grün

    **Spalte `sicher`:**

    - `0` = unsicher
    - `1` = sicher

??? warning "Kombinationen werden zufällig aufgeschrieben"

    Lernende finden möglicherweise verschiedene Kombinationen, können aber nicht begründen, warum ihre Liste vollständig ist.

    Fordern Sie deshalb ein erkennbares Ordnungsmuster ein.

    Die entscheidende Frage lautet:

    > Woher weisst du, dass keine Kombination mehr fehlt?

??? warning "Kombinationen werden vergessen oder doppelt notiert"

    Lassen Sie die Lernenden ihre Tabelle anhand des systematischen Musters überprüfen.

    Bei drei Variablen kann zusätzlich kontrolliert werden:

    > Enthält die Tabelle genau acht unterschiedliche Zeilen?

??? warning "Alle Ampeln auf Rot wird als unsicher interpretiert"

    Wenn alle Ampeln rot sind, fliesst zwar kein Verkehr, es kann aber auch keine Kollision entstehen.

    Sicherheit und Effizienz müssen deshalb getrennt beurteilt werden.

??? warning "Die Formel $2^n$ wird nur auswendig gelernt"

    Entwickeln Sie die Regel möglichst aus konkreten Beispielen:

    - eine Variable: $2$
    - zwei Variablen: $2 \cdot 2 = 4$
    - drei Variablen: $2 \cdot 2 \cdot 2 = 8$
    - vier Variablen: $2 \cdot 2 \cdot 2 \cdot 2 = 16$

    Erst danach wird zu $2^n$ verallgemeinert.

## Differenzierung

=== "Unterstützende Massnahmen"

    - zunächst nur mit zwei Variablen arbeiten;
    - Ampelzustände zusätzlich mit roten und grünen Symbolen darstellen;
    - eine Wahrheitstabelle teilweise vorausfüllen;
    - Karten mit allen möglichen Kombinationen zum Sortieren bereitstellen;
    - das Wechselmuster der einzelnen Spalten visuell hervorheben;
    - die Anzahl der Zustände zunächst als Produkt berechnen, bevor $2^n$ eingeführt wird;
    - konkrete Ampelstellungen mit dem enaktiven Material aus Baustein 1 nachstellen;
    - Satzstarter anbieten:

        > Diese Kombination ist sicher, weil …

        > Diese Kombination ist unsicher, weil …

        > Die Tabelle ist vollständig, weil …

        > Bei drei Variablen gibt es … Kombinationen, weil …

=== "Weiterführende Aufgaben"

    - eine Wahrheitstabelle für vier Variablen erstellen;
    - eine fehlerhafte Wahrheitstabelle korrigieren;
    - eine allgemeine Regel für das Wechselmuster der einzelnen Spalten formulieren;
    - für eine unbekannte Anzahl Variablen die Anzahl der Tabellenzeilen vorhersagen;
    - untersuchen, ab welcher Anzahl Variablen eine Wahrheitstabelle mehr als 100 Zeilen besitzt;
    - untersuchen, ab welcher Anzahl Variablen eine Wahrheitstabelle mehr als 1000 Zeilen besitzt;
    - zu einer Wahrheitstabelle Sicherheitsregeln in Alltagssprache formulieren.

!!! tip "Kooperative Durchführung"

    Auch in diesem Baustein können Rollen innerhalb der Partnerarbeit bewusst gewechselt werden.

    Eine mögliche Rollenverteilung:

    - **Person 1:** erstellt bzw. ergänzt die Wahrheitstabelle;
    - **Person 2:** kontrolliert Vollständigkeit und Begründungen.

    Anschliessend werden die Rollen gewechselt.

## Didaktische Hinweise

Dieser Baustein bildet innerhalb der Unterrichtsreihe den Übergang von der Nutzung einer bereits vorhandenen Darstellung zur **eigenständigen systematischen Modellierung**.

In Baustein 2 haben die Lernenden die Wahrheitstabelle bereits als symbolische Darstellung einer Verkehrssituation kennengelernt. Nun steht die Frage im Zentrum, wie eine solche Darstellung vollständig und systematisch konstruiert werden kann.

Wichtig ist deshalb, die fertige Wahrheitstabelle in LogicTraffic nicht zu früh als Lösung vorzugeben. Die Lernenden sollen zunächst selbst eine Strategie entwickeln, mit der alle möglichen Belegungen vollständig und ohne Wiederholungen erfasst werden können.

Die Regel $2^n$ sollte ebenfalls möglichst nicht als fertige Formel präsentiert werden. Sie entsteht aus den konkreten Fällen mit zwei und drei Variablen und wird anschliessend verallgemeinert.

Der abschliessende Vergleich verschiedener Variablenzahlen erzeugt einen gezielten kognitiven Konflikt: Wahrheitstabellen ermöglichen eine vollständige Beschreibung aller möglichen Fälle, werden mit zunehmender Anzahl von Variablen jedoch schnell sehr umfangreich. Dadurch entsteht aus dem Problem heraus die Motivation für eine kompaktere formale Darstellung.

## Übergang zum nächsten Baustein

Wahrheitstabellen besitzen einen grossen Vorteil:

> Sie zeigen vollständig und eindeutig, was bei jeder möglichen Kombination passiert.

Bei vielen Variablen werden sie jedoch sehr umfangreich.

Eine Kreuzung mit fünf Fahrspuren benötigt bereits:

$$
2^5 = 32
$$

Tabellenzeilen.

Bei zehn Fahrspuren wären es sogar:

$$
2^{10} = 1024
$$

Tabellenzeilen.

Damit entsteht die zentrale Frage:

!!! question "Übergang zu Baustein 4"

    Müssen wir wirklich jede einzelne mögliche Ampelstellung aufschreiben?

    **Oder können wir die Sicherheitsregel mit einer kurzen und eindeutigen Formel beschreiben?**

Diese Frage bildet den Ausgangspunkt für:

[Baustein 4 – Boolesche Formeln](baustein4-boolesche-algebra.md)