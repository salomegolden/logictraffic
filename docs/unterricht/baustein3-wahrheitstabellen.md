# Wahrheitstabellen im Unterricht

Eine Wahrheitstabelle zeigt für alle möglichen Kombinationen von Eingangswerten den zugehörigen Ausgangswert. In LogicTraffic bedeutet das: Alle Ampelzustände werden systematisch gesammelt und auf Sicherheit geprüft.

!!! abstract "Auf einen Blick"
    noch to do 


!!! note "Downloads zum Baustein"
    noch to do 

## Lernziele: 
Im Themenbereich der Wahrheitstabellen steht der Übergang von der anschaulichen Verkehrssimulation zur systematischen, tabellarischen Modellierung im Fokus. Die Lernziele gliedern sich in fachliche, methodische und metakognitive Aspekte:  

- Systematische Zustandserfassung: Die Lernenden verstehen eine Wahrheitstabelle als Methode, um alle $2^n$ denkbaren Ampelkonfigurationen bei $n$ Fahrspuren (Variablen) vollständig und lückenlos abzubilden.
- Semantische Zuordnung (Sicherheitsbewertung): Die Lernenden können für jede Belegungskombination bestimmen und begründen, ob die Verkehrssituation kollisionsfrei (sicher = 1) oder kollisionsgefährdet (sicher = 0) ist.
- Binäre Repräsentation verstehen: Die Lernenden verknüpfen den Zustand der Signalanlage sicher mit den formalen Wahrheitswerten ($1 = \text{Grün / Fahrt frei}$, $0 = \text{Rot / Halt}$).
- Darstellungswechsel: Die Lernenden vollziehen den Transfer von der ikonisch-animierten Verkehrskreuzung zur symbolisch-tabellarischen Repräsentation.
- Erkennen von Limitationen (Kognitiver Konflikt): Die Lernenden erkennen, dass Wahrheitstabellen bei steigender Spurenanzahl exponentiell wachsen ($2^n$) und als Steuerungswerkzeug unhandlich werden, was die Notwendigkeit kompakterer aussagenlogischer Formeln motiviert.

## Vorbereitung 


## Unterrichtsablauf - Überblick

| Phase | Inhalt (Stichworte) | Sozialform / Medien | Richtwert |
| :--- | :--- | :--- | :--- |
| **1. Einstieg & Problemstellung** | • Reaktivierung Simulation & Vorwissen<br>• Demonstration Situation 2 (2 Spuren)<br>• Leitfrage: Lückenlose Sicherheit aller Kombinationen?<br>• Ziel: Einführung der Wahrheitstabelle | **Plenum**<br>• Beamer / Tafel<br>• *LogicTraffic* | **ca. 7 Min.** |
| **2. Erarbeitung I**<br>*(2 Spuren)* | • Belegung klären: $0 = \text{Rot}$, $1 = \text{Grün}$<br>• Systematisches Eintragen der 4 Zustände ($2^2$) <br>• Spalte `sicher` bestimmen ($0 = \text{Kollision}$, $1 = \text{sicher}$)<br>• Visuelle Überprüfung per Simulation | **Partnerarbeit**<br>• Schüler-Geräte<br>• *LogicTraffic*<br>• Arbeitsblatt | **ca. 10 Min.** |
| **3. Vertiefung**<br>*(3 Spuren)* | • Erweiterung: Situation 3 (3 Spuren)<br>• Zustandsraum: 8 Zeilen ($2^3$)<br>• Geordnetes Binärmuster ($000$ bis $111$)<br>• Ausfüllen der Tabelle in der Software | **Partnerarbeit**<br>• *LogicTraffic*<br>• Arbeitsblatt | **ca. 15 Min.** |
| **4. Kognitiver Konflikt** | • Skalierung: Situation 10 (5 Spuren)<br>• Exponentielles Wachstum: 32 Zeilen ($2^5$)<br>• Erkenntnis: Grenzen & Ineffizienz der Tabelle<br>• Leitfrage: Notwendigkeit kompakter Formeln | **Plenum**<br>• Beamerprojektion<br>• Unterrichtsgespräch | **ca. 8 Min.** |
| **5. Sicherung & Ausblick** | • Festhalten der Kernpunkte ($2^n$-Systematik, $0/1$-Logik)<br>• Verbale Formulierung erster Vorfahrtsregeln<br>• Ausblick: Baustein 4 (Boolesche Formeln) | **Plenum / Einzelarbeit**<br>• Tafel<br>• Arbeitsblatt / Portfolio | **ca. 5 Min.** |

## Durchführung

### Phase 1 - Einstieg & Problemstellung

Sozialform / Medien: Plenum / Lehrgespräch; Beamer/Whiteboard mit Demonstration von LogicTraffic (Situation 2).  

??? info "Didaktische Absicht"

    Reaktivierung der Vorarbeiten (Ampelsteuerung) und Erzeugung eines Problembewusstseins für die Notwendigkeit einer lückenlosen, systematischen Dokumentation aller Schaltzustände. Der Wechsel von der spielerisch-intuitiven Exploration zur systematischen Erfassung markiert den Schritt von der Stufe Darstellen zur Stufe Strukturieren. Das Ziel ist die Erkenntnis, dass blosses Ausprobieren bei sicherheitskritischen Systemen nicht ausreicht.  

??? quote "Ablauf und Arbeitsauftrag"

    1. Die Lehrperson (LP) projiziert die 2-Spuren-Kreuzung (Situation 2) an die Wand.  
    2. Ein/e Schüler/in (SuS) schaltet die Ampeln über die Benutzeroberfläche interaktiv um und löst probehalber eine Simulation aus.  
    3. Die LP stellt die zentrale Problemfrage in den Raum.  

    !!! question "Zentraler Impuls / Leitfrage der Lehrperson"

        „Beim Ausprobieren hatten wir das Gefühl, die Kreuzung sei sicher. Wie können wir aber mathematisch zweifelsfrei beweisen, dass wir nicht eine einzige gefährliche Ampelkombination übersehen haben?“

        „Wie viele verschiedene Schaltzustände gibt es bei zwei Ampeln überhaupt?“

### Phase 2 - Erarbeitung 1 - Grundstruktur am 2-Spuren-Beispiel

Sozialform / Medien: Partnerarbeit (Pair Learning); Schülergeräte mit LogicTraffic, Arbeitsblatt mit 2-Spuren-Raster. 

??? info "Didaktische Absicht"

    Klärung der binären Semantik ($0 = \text{Rot}$, $1 = \text{Grün}$) und Erstellung der ersten vollständigen Wahrheitstabelle ($2^2 = 4$ Zustände).
    Pair Learning: Das gemeinsame Diskutieren am Bildschirm zwingt die Lernenden, ihre intuitive Wahrnehmung sprachlich in Wahrheitswerte zu übersetzen.

??? quote "Ablauf und Arbeitsauftrag"

    1. Die Lernenden öffnen zu zweit Situation 2 in LogicTraffic. 
    2. Das Tabellenraster wird formal definiert: Die Spalten $A$ und $B$ repräsentieren die Spuren/Ampeln (Aussagenvariablen); die Spalte sicher bildet das Gesamtergebnis ab. 
    3. Die Paare testen sukzessive die vier Zeilen ($00, 01, 10, 11$) in der Software und tragen den entsprechenden Sicherheitswert ein:
        - $00$: Beide Rot $\rightarrow$ kein Verkehr $\rightarrow$ sicher = 1.
        - $01$ / $10$: Nur eine Spur fährt $\rightarrow$ kollisionsfrei $\rightarrow$ sicher = 1.
        - $11$: Beide Grün $\rightarrow$ Kollision $\rightarrow$ sicher = 0.
    4. Über die Schaltfläche Simulieren wird die Kollision bei Belegung $11$ in der Software visuell verifiziert.

??? warning "Stolpersteine"

    Manche SuS interpretieren den Zustand $00$ (beide Rot) fälschlicherweise als unsicher (sicher = 0), weil „der Verkehr blockiert wird“. Hier muss präzisiert werden: sicher = 1 bedeutet ausschliesslich Kollisionsfreiheit, nicht Verkehrsfluss-Effizienz.

### Phase 3 - Vertiefung und Systematik - Die 3-Spuren-Kreuzung

Sozialform / Medien: Partnerarbeit mit Plenumsreflexion; LogicTraffic (Situation 3), Arbeitsblatt.  

??? info "Didaktische Absicht"

    Erkennen des exponentiellen Wachstums ($2^3 = 8$ Zeilen) und Etablieren eines geordneten Binärmusters zur lückenlosen Erfassung aller Kombinationen.

??? quote "Ablauf und Arbeitsauftrag"

    1. Wechsel zu Situation 3 (drei Fahrspuren: $A, B, C$, wovon sich zwei Spuren schneiden).
    2. Die LP fragt: „Wie viele Zeilen benötigen wir jetzt in unserer Tabelle?“ $\rightarrow$ Erarbeitung von $2 \times 2 \times 2 = 2^3 = 8$ Zeilen.
    3. Systematische Zählweise: Um keine Zeile doppelt aufzuschreiben oder zu vergessen, erarbeiten die Lernenden ein strukturiertes Muster (Dualzählung: $000, 001, 010, \dots, 111$).
    4. Die Schülerpaare füllen die Tabelle in LogicTraffic aus und nutzen das integrierte Feedback (Polizisten-Status), um zu prüfen, ob alle Zeilen korrekt als sicher oder unsicher klassifiziert wurden.

??? tip "Differenzierungsidee" 

    Schnellere Schülerpaare erhalten eine ausgedruckte oder vorbereitete Wahrheitstabelle mit 2–3 eingebauten Fehlern (z. B. Kollision fälschlicherweise als $1$ markiert). Der Auftrag lautet: „Stellt die verdächtigen Zeilen in LogicTraffic ein, findet die Kollisionen und korrigiert die Tabelle mit rotem Stift.“  

??? tip ":woman_police_officer: in LogicTraffic"

    Der [Polizisten-Status](../anhang/glossar.md#polizisten-status) gibt den SuS formativ Rückmeldung:  

    --8<-- "code/includes/begriffe.md:polizisten_status"

### Phase 4 - Kognitiver Konflikt - Grenzen der Wahrheitstabellen

Sozialform / Medien: Lehrgespräch / Plenum; Beamerprojektion von Situation 10 (5 Fahrspuren).

??? info "Didaktische Absicht"

    Aufzeigen der Skalierungsgrenzen von Wahrheitstabellen; Wecken einer intrinsischen Motivation für kompakte aussagenlogische Formeln (Brücke zu Baustein 4).

    Dieser kognitive Konflikt ist der didaktische Dreh- und Angelpunkt der gesamten Reihe: Die Wahrheitstabelle wird als notwendiges Zwischenwerkzeug gewürdigt, gleichzeitig wird jedoch ihre Ineffizienz für komplexe Steuerungsaufgaben erfahrbar gemacht, was die Boolesche Algebra als Problemlöser motiviert.  

??? quote "Ablauf und Arbeitsauftrag"

    1. Die LP blendet eine komplexe Kreuzung mit 5 Spuren ein (Situation 10).  
    2. Gemeinsame Berechnung der Zeilenanzahl: $2^5 = 32$ Zeilen.
    3. Die LP fragt provokativ: „Was passiert bei einer Kreuzung mit 10 Fahrspuren?“ $\rightarrow 2^{10} = 1024$ Zeilen.
    4. Die Klasse reflektiert: Das manuelle Ausfüllen und Abspeichern solcher Tabellen ist unübersichtlich, zeitaufwendig und extrem fehleranfällig. 

    !!! question "Zentrale Leitfrage für den Übergang" 

        „Können wir dem Steuerungscomputer der Ampel nicht eine kurze, schlaue logische Regel übergeben, anstatt ihm eine endlose Tabelle mit 32 oder 1024 Zeilen einzuspeisen?“

### Phase 5 - Sicherung und Ausblick

Sozialform / Medien: Plenum / Einzelarbeit; Tafelbild, Merkheft / Begleitportfolio.

??? info "Didaktische Absicht"

    Synthese der formalen Grundlagen und sprachliche Vorbereitung der Junktoren (Baustein 4: Boolesche Algebra). 

??? quote "Ablauf und Arbeitsauftrag"

    1. Festhalten der Kernregeln an der Tafel:
        - Anzahl Konfigurationen bei $n$ Spuren: $2^n$.
        - Belegungslogik: $1 = \text{Grün}$, $0 = \text{Rot}$; sicher = 1 (keine Kollision).
    2. Erstes verbales Formulieren von Sicherheitsregeln für Situation 3 durch die SuS (z. B.: „Wenn Spur C grün hat, dann müssen A und B rot haben“).  
    3. Ausblick auf Baustein 4: Wie diese Alltagssätze in Formeln mit $\land, \lor, \neg, \rightarrow$ übersetzt werden.
