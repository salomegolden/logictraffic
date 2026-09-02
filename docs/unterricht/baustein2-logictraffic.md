# Baustein 2 – LogicTraffic kennenlernen

In diesem Baustein lernen die Lernenden die digitale Lernumgebung LogicTraffic kennen. Sie untersuchen, wie eine Verkehrssituation in der Lernumgebung dargestellt wird und wie Fahrspuren, Ampelzustände und die Wahrheitstabelle miteinander verbunden sind.

Im Zentrum steht zunächst nicht das formale Arbeiten mit Wahrheitstabellen oder booleschen Formeln. Die Lernenden sollen sich in der Lernumgebung orientieren und verstehen, wie dieselbe Verkehrssituation in unterschiedlichen Darstellungen sichtbar wird. Die Wahrheitstabelle wird dabei zunächst als Bestandteil von LogicTraffic kennengelernt. Ihr systematischer Aufbau wird erst in Baustein 3 vertieft.

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
    LogicTraffic, Computer oder Tablets, Beamer oder Präsentationsbildschirm, Notizpapier bzw. Heft und Arbeitsblatt

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
- erklären, wie die Ampelzustände Rot und Grün mit `0` und `1` dargestellt werden;
- zu einer konkreten Ampelstellung die entsprechende Tabellenzeile finden;
- sichere und unsichere Ampelkombinationen unterscheiden und ihre Entscheidung begründen;
- erklären, dass die Kreuzung jeweils einen konkreten Zustand zeigt, während die Wahrheitstabelle verschiedene mögliche Zustände darstellt;
- beschreiben, dass Kreuzung, Wahrheitstabelle und Formel unterschiedliche Darstellungen derselben Verkehrssituation bzw. Sicherheitsregel sind.

## Vorbereitung

- LogicTraffic auf den Geräten öffnen und die Funktionsfähigkeit prüfen.
- Eine einfache Situation mit zwei Fahrspuren auswählen.
- Dieselbe Situation für die gemeinsame Einführung über den Beamer bereitstellen.
- Falls Baustein 1 durchgeführt wurde, möglichst eine vergleichbare Verkehrssituation verwenden.
- Den Formelbereich zu Beginn noch nicht vertiefen.
- Das Arbeitsblatt AB2.1 bzw. Notizmaterial bereitlegen.

??? tip "Vorbereitung der Lernumgebung"

    Wählen Sie zunächst eine Situation mit zwei Variablen. Besonders geeignet sind die Situationen 1 oder 2.

    Dadurch gibt es nur vier mögliche Ampelkombinationen und der Zusammenhang zwischen Kreuzung und Wahrheitstabelle bleibt überschaubar.

    Situation 11 kann ebenfalls verwendet werden, stellt jedoch einen Spezialfall dar und eignet sich weniger gut für die erste Einführung.

## Programmaufbau

![Aufbau der Webseite und ihre Bereiche](https://github.com/salomegolden/logictraffic/releases/download/images-v1/logictraffic_anleitung.png)

| Bereich | Bedeutung |
| --- | --- |
| Kreuzung | Zeigt die Verkehrssituation, die Fahrspuren und die Ampeln. |
| Variablen | Bezeichnen die Fahrspuren mit `A`, `B`, `C` usw. |
| Wahrheitstabelle | Stellt die möglichen Kombinationen der Ampelzustände dar. |
| Spalte «sicher» | Zeigt, welche Kombinationen durch die Steuerung erlaubt werden. |
| Statusanzeige | Gibt eine Rückmeldung zur eingestellten Lösung. |
| Formelbereich | Beschreibt die Sicherheitsregel in formaler Form. |

!!! info "Von der Kreuzung zur Tabelle"

    Die Kreuzung zeigt jeweils eine konkrete Ampelstellung.

    Die Werte in der Wahrheitstabelle beschreiben dieselbe Ampelstellung in symbolischer Form:

    - `0` bedeutet: Die Ampel ist rot.
    - `1` bedeutet: Die Ampel ist grün.

    Bei zwei Fahrspuren können beispielsweise folgende Zustände auftreten:

    | `A` | `B` |
    | --- | --- |
    | `0` | `0` |
    | `0` | `1` |
    | `1` | `0` |
    | `1` | `1` |

    Wie solche Tabellen systematisch aufgebaut werden und weshalb bei zwei Variablen genau vier Kombinationen entstehen, wird in **Baustein 3** vertieft.

## Unterrichtsablauf – Überblick

| Phase | Inhalt | Sozialform / Medien | Richtwert |
| --- | --- | --- | --- |
| [1. Anknüpfen](#phase-1--an-den-enaktiven-einstieg-anknüpfen) | Verkehrssituation aus Baustein 1 aufgreifen und Übertragung auf den Computer vorbereiten | Plenum, enaktives Material / Präsentation | ca. 5 Min. |
| [2. Orientierung](#phase-2--logictraffic-gemeinsam-erkunden) | Oberfläche kennenlernen und zentrale Bereiche identifizieren | Plenum, Beamer, LogicTraffic | ca. 10 Min. |
| [3. Darstellungen verbinden](#phase-3--ampelzustände-und-tabellenzeilen-verbinden) | Ampelstellungen verändern und Zusammenhang zwischen Kreuzung, Variablen und Tabellenzeile untersuchen | Partnerarbeit, LogicTraffic, AB2.1 | ca. 15 Min. |
| [4. Sicherheit untersuchen](#phase-4--sichere-und-unsichere-zustände-untersuchen) | Ampelkombinationen anhand der Fahrwege beurteilen | Partnerarbeit, LogicTraffic | ca. 10–15 Min. |
| [5. Darstellungswechsel sichern](#phase-5--die-darstellungen-zusammenführen) | Kreuzung, Wahrheitstabelle und Formel als unterschiedliche Darstellungen vergleichen | Plenum, Beamer, Tafelbild | ca. 10 Min. |

## Durchführung

### Phase 1 – An den enaktiven Einstieg anknüpfen

**Ziel der Phase:**  
Die Lernenden übertragen ihre bisherigen Vorstellungen von Fahrspuren, Ampeln und Sicherheit auf eine digitale Darstellung.

Falls Baustein 1 durchgeführt wurde, greift die Lehrperson die dort untersuchte Kreuzung nochmals auf. Die Lernenden erinnern sich daran, wie sie mit Fahrzeugen und Ampelplättchen verschiedene Zustände dargestellt und auf ihre Sicherheit überprüft haben.

!!! quote "Einstiegsauftrag"

    Erinnert euch an die Kreuzung aus dem letzten Baustein.

    Überlegt:

    - Welche Informationen müsste ein Computer über diese Kreuzung kennen?
    - Wie könnte ein Computer darstellen, ob eine Ampel rot oder grün ist?
    - Wie könnte er verschiedene Ampelstellungen festhalten?

Die Vermutungen werden gesammelt, ohne bereits die formalen Grundlagen der Wahrheitstabelle zu erklären.

??? note "Alternative mit realen Kreuzungen"

    Falls Baustein 1 nicht durchgeführt wurde, können Bilder aus der  
    [:film_projector: **Präsentation mit Kreuzungen**](https://github.com/salomegolden/logictraffic/releases/download/material-v1/b2_prasentation_kreuzungen.pdf)  
    verwendet werden.

    Mögliche Leitfrage:

    > Welche Informationen braucht eine Ampelsteuerung, damit eine Kreuzung sicher funktioniert?

### Phase 2 – LogicTraffic gemeinsam erkunden

**Ziel der Phase:**  
Die Lernenden orientieren sich in der Lernumgebung und ordnen die Elemente der digitalen Darstellung den bereits bekannten Elementen der Verkehrssituation zu.

Die Lehrperson öffnet eine einfache Situation mit zwei Fahrspuren in [LogicTraffic](https://logictraffic.ch/) und zeigt die Oberfläche über den Beamer.

Zunächst stehen insbesondere folgende Bereiche im Zentrum:

1. Kreuzung;
2. Fahrspuren und Variablen;
3. Ampeln;
4. Wahrheitstabelle;
5. Spalte «sicher».

Der Formelbereich wird zunächst lediglich als weiterer Bereich der Lernumgebung benannt.

![Teilbereiche von LogicTraffic mit Beschriftungen](https://github.com/salomegolden/logictraffic/releases/download/images-v1/losungBeschriftungProgramm.png)

!!! quote "Beobachtungsauftrag"

    Beobachtet genau, was passiert, wenn eine Ampel verändert wird.

    Achtet dabei auf:

    - die Farbe der Ampel;
    - die zugehörige Variable;
    - die Werte `0` und `1`;
    - die entsprechende Zeile in der Wahrheitstabelle.

Gemeinsam wird festgehalten:

- Jede Fahrspur wird mit einer Variable bezeichnet.
- Jede Ampel kann rot oder grün sein.
- In LogicTraffic werden diese beiden Zustände mit `0` und `1` dargestellt.
- Eine konkrete Ampelstellung lässt sich auch als Zeile in der Tabelle darstellen.

??? warning "Typische Lernschwierigkeit: 0 und 1"

    Lernende können `0` als «falsch» und `1` als «richtig» interpretieren.

    Stellen Sie deshalb konsequent den Bezug zur Verkehrssituation her:

    - `0` = Ampel rot
    - `1` = Ampel grün

    Ob die gesamte Ampelkombination sicher ist, ist eine andere Frage.

### Phase 3 – Ampelzustände und Tabellenzeilen verbinden

**Ziel der Phase:**  
Die Lernenden wechseln selbstständig zwischen konkreter Verkehrssituation und symbolischer Darstellung.

Die Lernenden arbeiten in Zweiergruppen mit LogicTraffic.

Eine Person bedient zunächst die Lernumgebung, während die andere beobachtet, beschreibt und notiert. Anschliessend werden die Rollen gewechselt.

!!! quote "Lernauftrag 1 – Darstellungen untersuchen"

    Öffnet eine Situation mit zwei Fahrspuren.

    Untersucht:

    1. Welche Variable gehört zu welcher Fahrspur?
    2. Was verändert sich, wenn ihr eine Ampel anklickt?
    3. Welcher Wert gehört zu einer roten Ampel?
    4. Welcher Wert gehört zu einer grünen Ampel?
    5. Welche Tabellenzeile beschreibt die aktuelle Ampelstellung?

Zur Ergebnissicherung kann AB2.1 eingesetzt werden.

???+ quote "Einträge ins Heft oder Notizbuch"

    | Ampel `A` | Ampel `B` | Darstellung mit `0` und `1` |
    | --- | --- | --- |
    | rot | rot | |
    | rot | grün | |
    | grün | rot | |
    | grün | grün | |

??? example "Mögliches Ergebnis"

    | Ampel `A` | Ampel `B` | Darstellung mit `0` und `1` |
    | --- | --- | --- |
    | rot | rot | `0`, `0` |
    | rot | grün | `0`, `1` |
    | grün | rot | `1`, `0` |
    | grün | grün | `1`, `1` |

!!! tip "Zentraler Darstellungswechsel"

    Lassen Sie die Lernenden möglichst häufig in beide Richtungen übersetzen:

    **Kreuzung → Tabellenzeile**

    und

    **Tabellenzeile → Kreuzung**

    So wird die Wahrheitstabelle zunächst als symbolische Darstellung einer bereits verstandenen Verkehrssituation kennengelernt.

??? warning "Typische Lernschwierigkeit: Kreuzung und Tabelle"

    Die Kreuzung zeigt immer nur **einen konkreten Zustand**.

    Die Wahrheitstabelle enthält dagegen **verschiedene mögliche Zustände**.

    Der systematische Aufbau der vollständigen Wahrheitstabelle wird erst in Baustein 3 thematisiert.

### Phase 4 – Sichere und unsichere Zustände untersuchen

**Ziel der Phase:**  
Die Lernenden verbinden die symbolisch dargestellten Ampelzustände wieder mit der Bedeutung der Verkehrssituation.

Nun untersuchen die Lernenden verschiedene Ampelkombinationen und beurteilen diese anhand der Fahrwege.

!!! quote "Lernauftrag 2 – Sicherheit untersuchen"

    Stellt verschiedene Ampelkombinationen ein.

    Entscheidet jeweils:

    1. Welche Ampeln sind rot und welche grün?
    2. Wie wird diese Ampelstellung in der Tabelle dargestellt?
    3. Ist die Verkehrssituation sicher oder unsicher?
    4. Warum?

    Haltet eure Begründung fest.

Die Lernenden markieren anschliessend die entsprechenden Werte in der Spalte «sicher».

Die Rückmeldung von LogicTraffic kann zur Kontrolle verwendet werden, steht jedoch nicht im Zentrum der Aufgabe.

!!! tip "Erst begründen, dann überprüfen"

    Die Lernenden sollten ihre Entscheidung zunächst anhand der Fahrwege begründen.

    Erst danach wird die Rückmeldung der Lernumgebung betrachtet.

    Statt:

    > LogicTraffic sagt, dass die Lösung falsch ist.

    sollte die Begründung beispielsweise lauten:

    > Diese Kombination ist unsicher, weil sich die Fahrwege von `A` und `B` kreuzen und beide Ampeln grün sind.

??? warning "Typische Lernschwierigkeit: Sicherheit einer einzelnen Ampel"

    Eine einzelne Ampel ist nicht «sicher» oder «unsicher».

    Beurteilt wird immer die **gesamte Kombination der Ampelzustände im Zusammenhang mit den Fahrwegen**.

### Phase 5 – Die Darstellungen zusammenführen

**Ziel der Phase:**  
Die Lernenden erkennen, dass dieselbe Verkehrssituation bzw. Sicherheitsregel in LogicTraffic unterschiedlich dargestellt werden kann.

Gemeinsam werden nun die verschiedenen Bereiche der Lernumgebung miteinander verglichen.

!!! quote "Lernauftrag 3 – Dieselbe Situation, verschiedene Darstellungen"

    Betrachtet dieselbe Sicherheitsregel in LogicTraffic.

    Was zeigt …

    1. die Kreuzung?
    2. die Wahrheitstabelle?
    3. die Spalte «sicher»?
    4. die Formel?

Die Formel wird dabei bewusst nur auf einer grundlegenden Ebene betrachtet.

![Tafelbild B2, generiert mit ChatGPT, GPT5.6](https://github.com/salomegolden/logictraffic/releases/download/images-v1/b2_tafelbild.png)

Gemeinsam wird festgehalten:

| Darstellung | Was zeigt sie? |
| --- | --- |
| Kreuzung | eine konkrete Verkehrssituation |
| Variablen und `0`/`1` | die Ampelzustände in symbolischer Form |
| Wahrheitstabelle | verschiedene mögliche Kombinationen der Ampelzustände |
| Spalte «sicher» | welche Kombinationen zugelassen werden |
| Formel | beschreibt die Sicherheitsregel in kompakter formaler Form |

!!! tip "Die Formel nur als Ausblick"

    Die Lernenden müssen die Formel an dieser Stelle noch nicht lesen oder selbst bilden können.

    Entscheidend ist lediglich die Erkenntnis:

    **Auch die Formel beschreibt dieselbe Sicherheitsregel – nur in einer anderen Darstellung.**

    Das eigentliche Arbeiten mit booleschen Formeln folgt in Baustein 4.

## Ergebnissicherung

Zur Ergebnissicherung kann das Arbeitsblatt **AB2.1** oder das vorbereitete Tafelbild verwendet werden.

Am Ende des Bausteins sollten insbesondere folgende Zusammenhänge gesichert sein:

??? example "Mögliche Ergebnissicherung"

    **LogicTraffic stellt dieselbe Situation auf unterschiedliche Arten dar.**

    | Darstellung | Bedeutung |
    | --- | --- |
    | Fahrspur `A`, `B`, `C` … | Die Fahrspuren werden mit Variablen bezeichnet. |
    | `0` | Die zugehörige Ampel ist rot. |
    | `1` | Die zugehörige Ampel ist grün. |
    | Kreuzung | Zeigt eine konkrete Ampelstellung und die Fahrwege. |
    | Wahrheitstabelle | Stellt verschiedene mögliche Ampelstellungen symbolisch dar. |
    | «sicher» | Bewertet eine Kombination hinsichtlich der Sicherheit. |
    | Formel | Ist eine weitere, formale Darstellung der Sicherheitsregel. |

    **Merksatz**

    > Kreuzung, Wahrheitstabelle und Formel beschreiben dieselbe Situation bzw. Sicherheitsregel auf unterschiedliche Weise.

## Erwartete Ergebnisse

Die Lernenden sollten am Ende beispielsweise erklären können:

> Die Fahrspur `A` gehört zur Variable `A`.

> Wenn `A = 1` ist, zeigt die Ampel der Spur `A` grün.

> Wenn `A = 0` ist, zeigt die Ampel der Spur `A` rot.

> Die Kreuzung zeigt jeweils eine konkrete Ampelstellung.

> Dieselbe Ampelstellung kann mit `0` und `1` in der Tabelle dargestellt werden.

> Ob eine Kombination sicher ist, hängt davon ab, welche Fahrwege sich kreuzen.

> Die Formel ist eine weitere Möglichkeit, dieselbe Sicherheitsregel darzustellen.

## Differenzierung

=== "Unterstützende Massnahmen"

    - zunächst ausschliesslich mit zwei Fahrspuren arbeiten;
    - Variablen direkt an den entsprechenden Fahrspuren zeigen;
    - `0` zusätzlich mit einem roten und `1` mit einem grünen Ampelsymbol verbinden;
    - konkrete Ampelstellungen vorgeben und die passende Tabellenzeile suchen lassen;
    - Tabellenzeilen vorgeben und die entsprechende Ampelstellung einstellen lassen;
    - Satzstarter verwenden:

        > `A = 1` bedeutet …

        > Diese Tabellenzeile gehört zur Kreuzung, weil …

        > Die Kombination ist unsicher, weil …

=== "Weiterführende Aufgaben"

    - eine Situation mit drei Variablen untersuchen;
    - zu einer vorgegebenen Tabellenzeile die entsprechende Kreuzung einstellen;
    - eine konkrete Ampelstellung zunächst ohne Computer mit `0` und `1` notieren;
    - verschiedene sichere und unsichere Kombinationen begründen;
    - beobachten, wie sich der Formelbereich verändert, wenn andere Kombinationen als sicher festgelegt werden.

!!! tip "Kooperative Durchführung"

    Achten Sie darauf, dass nicht dauerhaft dieselbe Person das Gerät bedient.

    Eine mögliche Rollenverteilung:

    - **Person 1:** bedient LogicTraffic;
    - **Person 2:** beobachtet, beschreibt und begründet.

    Anschliessend werden die Rollen gewechselt.

## Didaktische Hinweise

LogicTraffic wurde gezielt dafür entwickelt, abstrakte Konzepte der Aussagenlogik über eine anschauliche Verkehrssituation zugänglich zu machen. Die ursprüngliche Konzeption verbindet dabei unterschiedliche Repräsentationsformen und einen hohen Grad an Interaktivität.

Für diesen Baustein steht deshalb insbesondere der **Darstellungswechsel** im Zentrum. Die Lernenden gehen von der bekannten Verkehrssituation aus und begegnen schrittweise abstrakteren Darstellungen:

**Verkehrssituation → Variablen und `0`/`1` → Wahrheitstabelle → Formel**

Die formalen Darstellungen werden dabei noch nicht vollständig erklärt. Vielmehr sollen die Lernenden erkennen, dass unterschiedliche Darstellungen auf dieselbe zugrunde liegende Situation bzw. Sicherheitsregel verweisen. Dieser Zugang entspricht der ursprünglichen Idee von InfoTraffic, abstrakte Inhalte über konkrete Beispiele sowie symbolische, ikonische und virtuell-enaktive Repräsentationen zu erschliessen.

## Übergang zum nächsten Baustein

Die Lernenden kennen die Wahrheitstabelle nun als eine Möglichkeit, Ampelzustände symbolisch darzustellen. Sie können zwischen einer konkreten Ampelstellung und der entsprechenden Tabellenzeile wechseln.

Bisher wurde die Tabelle jedoch von LogicTraffic vorgegeben.

Damit entsteht die nächste Frage:

!!! question "Wie entsteht eine vollständige Wahrheitstabelle?"

    Wenn wir die Tabelle nicht von LogicTraffic bekommen würden:

    **Wie könnten wir selbst alle möglichen Ampelkombinationen systematisch aufschreiben, ohne eine zu vergessen?**

Diese Frage bildet den Ausgangspunkt für:

[Baustein 3 – Wahrheitstabellen](baustein3-wahrheitstabellen.md)

Dort wird untersucht, wie Wahrheitstabellen systematisch aufgebaut werden, weshalb ihre Anzahl an Zeilen von der Anzahl der Variablen abhängt und wie damit alle möglichen Zustände vollständig erfasst werden können.