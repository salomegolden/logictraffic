# Wahrheitstabellen

Wahrheitstabellen (auch Wahrheitstafeln, engl. truth tables) bilden das zentrale semantische Instrument der klassischen zweiwertigen Aussagenlogik. Sie erfassen den Wahrheitswertverlauf einer aussagenlogischen Formel für sämtliche möglichen Kombinationen von Eingangsbelegungen vollständig und deterministisch [^1], [^2], [^3].  

Wahrheitstabellen bilden im Unterricht die Brücke zwischen der spielerischen Verkehrssimulation und der formalen Aussagenlogik. Sie verorten sich in der auf der Stufe Strukturieren: Lernende verlassen das rein intuitive Ausprobieren und erfassen alle möglichen Signalzustände einer Kreuzung systematisch und lückenlos [^5].  

## Semantik: Wie die Kreuzung in Nullen und Einsen übersetzt wird

In der klassischen Aussagenlogik ist jede Aussage entweder wahr ($1$) oder falsch ($0$). In LogicTraffic wird diese zweiwertige Logik direkt auf die Ampeln und Spuren übertragen [^1]:  

| Element in LogicTraffic | Logische Bedeutung | Verkehrsbedeutung im Unterricht |
| ---- | ---- | ---- |
| Spur $A, B, C, \dots$ | Aussagenvariable | Repräsentiert die jeweilige Fahrspur bzw. deren Signalgeber. |
| Wahrheitswert $1$ (true) | Aussage ist wahr | Grüne Ampel: Fahrzeuge dürfen fahren (Freie Fahrt). |
| Wahrheitswert $0$ (false) | Aussage ist falsch | Rote Ampel: Fahrzeuge müssen anhalten (Halt). |
| Tabellenzeile (Belegung) | Variablenbelegung | Ein konkreter Gesamtzustand aller Ampeln an der Kreuzung. |
| Spalte sicher | Gesamtwahrheitswert $f(\beta)$ | $1 =$ kollisionsfrei (sicher) $0 =$ Kollisionsgefahr (Crash). |

??? warning "Didaktische Modellreduktion"

    In realen Kreuzungen gibt es Gelbphasen und Übergangszeiten. Zur didaktischen Reduktion arbeitet LogicTraffic statisch: Eine Spur hat entweder strikt Grün ($1$) oder strikt Rot ($0$). Dies ermöglicht es Schülerinnen und Schülern, elementare Aussagenlogik ohne zeitliche Komplexität zu erlernen.  

## Systematik statt Zufall: Der Zustandsraum ($2^n$)

Für jede Fahrspur gibt es genau zwei Möglichkeiten: Rot ($0$) oder Grün ($1$). Bei $n$ Fahrspuren ergeben sich daher mathematisch genau $2^n$ verschiedene Ampelkombinationen [^1], [^6]:

* 2 Spuren ($n=2$): $2^2 = 4$ Kombinationen.
* 3 Spuren ($n=3$): $2^3 = 8$ Kombinationen.
* 5 Spuren ($n=5$): $2^5 = 32$ Kombinationen.

### Synchrone Repräsentation (Darstellungswechsel)

Mehr Informationen zum Konzept vom [Darstellungswechsel](../didaktik/darstellungswechsel.md). 

LogicTraffic verknüpft die visuelle Simulation und die symbolische Tabelle synchron miteinander:  

* Schaltet man eine Ampel an der Kreuzung per Mausklick um, springt in der Tabelle automatisch der Cursor auf die entsprechende Zeile. 
* Umgekehrt visualisiert die Kreuzung sofort die Belegung, wenn eine Zeile in der Tabelle ausgewählt wird.  
* Dieser synchrone Wechsel unterstützt den Übergang von der virtuell-enaktiven Ebene (Klicken/Fahren) zur symbolischen Ebene (Zahlenwerte $0$ und $1$). 

## Didaktischer Nutzen

| Funktion | Nutzen im Unterricht |
| --- | --- |
| Visualisierung | Lernende sehen Ampelzustände und Sicherheitsstatus nebeneinander. |
| Systematisierung | Keine Kombination wird vergessen. |
| Interaktion | Klicks auf Ampeln oder Tabellenwerte verändern die Situation. |
| Formelbrücke | Aus sicheren Zeilen kann eine boolesche Formel entstehen. |

## Typische Situationen & Sicherheitsbewertung

### Die 2-Spuren-Kreuzung (Situation 2, $n=2 \rightarrow 4$ Zeilen)

=== "Beschreibung der Situation"

    Zwei Spuren $A$ und $B$ kreuzen sich rechtwinklig. Haben beide gleichzeitig Grün, kommt es zum Unfall.  
    ![Situation 2 - Screenshot aus LogicTraffic](https://github.com/salomegolden/logictraffic/releases/download/images-v1/situation2screenshot.png){ align=right }

=== "Wahrheitstabelle" 

    | $A$ | $B$ | `sicher` | fachliche & didaktische Begründung |
    | --- | --- | --- | ------ |
    | $0$ | $0$ | $1$ | Beide haben Rot. Kein Fahrzeug fährt $\rightarrow$ Kollisionsfrei. |
    | $0$ | $1$ | $1$ | Nur Spur $B$ fährt, $A$ steht $\rightarrow$ Kollisionsfrei. |
    | $1$ | $0$ | $1$ | Nur Spur $A$ fährt, $B$ steht $\rightarrow$ Kollisionsfrei. |
    | $1$ | $1$ | $0$ | Kollision! Beide Spuren fahren gleichzeitig in die Kreuzung. |

??? warning "Häufiges Fehlkonzept bei Zustand $00$ (Alle Rot)"

    * Schüleraussage: „Wenn alle Rot haben ($00$), ist das unsicher ($0$), weil nichts vorangeht und Stau entsteht!“    
    * Klärung im Unterricht: Die Spalte sicher prüft ausschliesslich die Unfallfreiheit, nicht den Verkehrsfluss oder die Effizienz der Ampel. Wenn alle Fahrzeuge stehen, kann physikalisch keine Kollision geschehen.

### Die 3-Spuren-Kreuzung (Situation 3, $n=3 \rightarrow 8$ Zeilen)

Spur $A$ und Spur $B$ verlaufen parallel (vertragen sich), während Spur $C$ als Abbieger beide Fahrwege schneidet.

=== "Beschreibung der Situation"

    Spur $A$ und Spur $B$ verlaufen parallel (vertragen sich), während Spur $C$ als Abbieger beide Fahrwege schneidet.
    ![Situation 3 - Screenshot aus LogicTraffic](https://github.com/salomegolden/logictraffic/releases/download/images-v1/situation3_3spuren.png){ align=right }

=== "Wahrheitstabelle"

    | $A$ | $B$ | $C$ | `sicher` | Verkehrsbeurteilung |
    | :---: | :---: | :---: | :---: | :--- |
    | 0 | 0 | 0 | **1** | Alles steht $\rightarrow$ sicher. |
    | 0 | 0 | 1 | **1** | Nur $C$ fährt $\rightarrow$ sicher. |
    | 0 | 1 | 0 | **1** | Nur $B$ fährt $\rightarrow$ sicher. |
    | 0 | 1 | 1 | **0** | **Kollision:** $B$ und $C$ kreuzen sich! |
    | 1 | 0 | 0 | **1** | Nur $A$ fährt $\rightarrow$ sicher. |
    | 1 | 0 | 1 | **0** | **Kollision:** $A$ und $C$ kreuzen sich! |
    | 1 | 1 | 0 | **1** | **Sicher:** $A$ und $B$ fahren parallel (kein Konflikt). |
    | 1 | 1 | 1 | **0** | **Kollision:** $C$ kollidiert mit $A$ und $B$. |

## Das Polizisten-Feedback als formative Diagnose

Das Polizisten-Icon in LogicTraffic gibt unmittelbare Rückmeldung über die Vollständigkeit und Korrektheit der Sicherheitsbewertung in der Tabelle [^1]:

| Status / Feedback | Polizist | Fachliche Bedeutung | Verkehrssemantik in LogicTraffic |
| :--- | :---: | :--- | :--- |
| **Unsicher**<br>*(Kollision möglich)* | ![Polizist Unsicher](https://github.com/salomegolden/logictraffic/releases/download/images-v1/lt_polizist_unsicher.png){ width="50" } | **Kollisionsgefahr:** Mindestens eine gefährliche Ampelkombination wurde fälschlicherweise als sicher (`1`) markiert. | Autos kollidieren im Kreuzungsbereich (Crash-Gefahr). |
| **Nicht ideal**<br>*(Zu vorsichtig)* | ![Polizist Safe](https://github.com/salomegolden/logictraffic/releases/download/images-v1/lt_polizist_nicht_ideal.png){ width="50" } | **Kollisionsfrei, aber restriktiv:** Keine Unfälle möglich, aber gefahrlose Kombinationen wurden unnötig auf `0` gesperrt. | Sicher, aber ineffizient. |
| **Optimal**<br>*(Perfekt gelöst)* | ![Polizist Optimal](https://github.com/salomegolden/logictraffic/releases/download/images-v1/lt_polizist_sicher.png){ width="50" } | **Sicher & vollständig:** Exakte Übereinstimmung; alle sicheren Zustände sind `1`, alle gefährlichen `0`. | Maximaler Verkehrsfluss bei 100% Kollisionsfreiheit. |


[^1]: Arnold, R., & Hartmann, W. (2007). LogicTraffic - Logik in der Allgemeinbildung. Informatik-Spektrum, 30(1), 19-26. https://doi.org/10.1007/s00287-006-0123-7
[^2]: Junker, M. (2025). _Logik für die Informatik: Eine Einführung in die Aussagenlogik, Prädikatenlogik und Berechenbarkeitstheorie_. Springer Berlin Heidelberg. https://doi.org/10.1007/978-3-662-70825-5
[^3]: Habiballa, H., & Kmet, T. (2008). Mathematical Logic and Deduction in Computer Science Education. Informatics in Education, 7(1), 75–90. https://doi.org/10.15388/infedu.2008.05
[^4]: Turtur, C. W. (2014). Aussagelogik. In C. W. Turtur, Prüfungstrainer Mathematik (S. 73–84). Springer Fachmedien Wiesbaden. https://doi.org/10.1007/978-3-658-03199-2_3
[^5]: Hartmann, W., Jäckel, S., Näf, M., & Reichert, R. (2026). Informatikunterricht planen und durchführen. Springer. https://doi.org/10.1007/978-3-662-72786-7
[^6]: Modrow, E., & Strecker, K. (2016). Didaktik der Informatik. De Gruyter.
[^7]: Hauser, U., Komm, D., & Serafini, G. (2019). Wie Mathematik und Informatik im Unterricht voneinander profitieren können. Informatik Spektrum, 42(2), 118–123. https://doi.org/10.1007/s00287-019-01165-2
