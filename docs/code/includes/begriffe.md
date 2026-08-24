<!-- docs/includes/begriffe.md -->

# Stichwortverzeichnis: Logik & Boolesche Algebra

## A

--8<-- [start:absorption]
<span id="absorption"></span>

??? info "Absorption"
    * **Fachlich:** Rechenregel der Booleschen Algebra ($A \lor (A \land B) \equiv A$ bzw. $A \land (A \lor B) \equiv A$). Ein Teilausdruck fällt weg, wenn sein Wahrheitswert bereits vollständig durch einen einfacheren Teilausdruck bestimmt wird.
    * **In LogicTraffic:** Ermöglicht die formale Kürzung überflüssiger Sicherheitsbedingungen bei der Formelminimierung (z. B. $\neg A \land (\neg A \lor \neg B) \equiv \neg A$).
--8<-- [end:absorption]

--8<-- [start:aequivalenz]
<span id="aequivalenz"></span>

??? info "Äquivalenz ($\equiv$ bzw. $\sim$)"
    * **Fachlich:** Logische Gleichwertigkeit zweier Formeln ($\phi \sim \psi$); beide besitzen für jede denkbare Belegung identische Wahrheitswerte.
    * **In LogicTraffic:** Zwei unterschiedliche Schaltformeln steuern die Ampeln in jeder Situation exakt gleich sicher und erzeugen dieselbe Spalte `sicher` in der Wahrheitstabelle.
--8<-- [end:aequivalenz]

--8<-- [start:aussage]
<span id="aussage"></span>

??? info "Aussage (Proposition)"
    * **Fachlich:** Ein sprachliches Gebilde bzw. eine formale Aussage, die eindeutig entweder wahr ($1$) oder falsch ($0$) ist (Prinzip der Zweiwertigkeit).
    * **In LogicTraffic:** Bezieht sich immer auf den konkreten Zustand einer Signalanlage (z. B. «Spur $A$ hat Grün»).
--8<-- [end:aussage]

--8<-- [start:aussagenvariable]
<span id="aussagenvariable"></span>

??? info "Aussagenvariablen ($A, B, C, \dots$)"
    * **Fachlich:** Buchstaben oder Symbole als Platzhalter für einen Wahrheitswert ($0$ oder $1$).
    * **In LogicTraffic:** Jede Fahrspur bzw. Ampel der Kreuzung wird durch genau eine Variable repräsentiert.
--8<-- [end:aussagenvariable]

## B

--8<-- [start:boolesche_algebra]
<span id="boolesche-algebra"></span>

??? info "Boolesche Algebra"
    * **Fachlich:** Mathematische Struktur und Regelwerk für logische Verknüpfungen mit Wahrheitswerten ($0$ und $1$) basierend auf formalen Axiomen (Kommutativität, Assoziativität, Distributivität, Komplement etc.).
    * **In LogicTraffic:** Bildet die mathematische Grundlage zur formalen Beschreibung, Prüfung und Vereinfachung von Kreuzungssteuerungen.
--8<-- [end:boolesche_algebra]

## C

--8<-- [start:computational_thinking]
<span id="computational-thinking"></span>

??? info "Informatisches Denken (Computational Thinking)"
    * **Didaktisch:** Menschlicher Problemlösungsprozess (nach Wing), der Kernkompetenzen wie Dekomposition, Mustererkennung, Abstraktion und Algorithmenentwurf umfasst.
    * **Im LogicTraffic-Unterricht:** Schülerinnen und Schüler zerlegen Verkehrssituationen in Einzelkonflikte, erkennen wiederkehrende Schaltungsmuster und formulieren algorithmische Regeln zur Ampelsicherung.
--8<-- [end:computational_thinking]

## D

--8<-- [start:darstellungswechsel]
<span id="darstellungswechsel"></span>

??? info "Darstellungswechsel (Mehrfachrepräsentationen)"
    * **Didaktisch:** Die kognitive Fähigkeit, zwischen verschiedenen Repräsentationsformen eines Konzepts (handelnd, bildhaft, tabellarisch, formal-symbolisch) hin- und herzuwechseln und Zusammenhänge zu erkennen.
    * **Im LogicTraffic-Unterricht:** Vollzieht sich entlang der 4-Stufen-Progression: Vom *Handeln* (Kreuzungsmatte) über das *Darstellen* (Simulation) und *Strukturieren* (Wahrheitstabelle) bis hin zum *Formalisieren* (Formeleditor).
--8<-- [end:darstellungswechsel]

--8<-- [start:de_morgan]
<span id="de-morgan"></span>

??? info "De Morgan'sche Gesetze"
    * **Fachlich:** Regeln zur Negation von Konjunktionen und Disjunktionen: $\neg (A \land B) \equiv \neg A \lor \neg B$ sowie $\neg (A \lor B) \equiv \neg A \land \neg B$[cite: 1].
    * **In LogicTraffic:** Transformiert das Verbot des gleichzeitigen Grüns zweier Spuren ($\neg(A \land B)$) direkt in eine handlungsorientierte Schaltungsregel («Spur $A$ hat Rot oder Spur $B$ hat Rot»).
--8<-- [end:de_morgan]

--8<-- [start:disjunktion]
<span id="disjunktion"></span>

??? info "Disjunktion ($\lor$ / ODER)"
    * **Fachlich:** Logisches ODER (nicht-exklusiv). Genau dann wahr ($1$), sobald mindestens eine der Teilaussagen wahr ist.
    * **In LogicTraffic:** $\neg A \lor \neg B$ bedeutet: Mindestens eine der beiden Spuren $A$ oder $B$ muss Rot haben (kein gleichzeitiges Grün).
--8<-- [end:disjunktion]

## E

--8<-- [start:eis_prinzip]
<span id="eis-prinzip"></span>

??? info "EIS-Prinzip & Virtuell-enaktive Repräsentation"
    * **Didaktisch:** Nach Jerome Bruner erfolgt Wissenserwerb über drei Ebenen: *enaktiv* (handelnd), *ikonisch* (bildhaft) und *symbolisch* (formalsprachlich). Für die Informatikdidaktik erweitern Hartmann & Arnold dies um den *virtuell-enaktiven Modus*.
    * **Im LogicTraffic-Unterricht:** Lernende erproben Kreuzungen zuerst haptisch mit Modellautos (*enaktiv*), schalten anschliessend virtuell Ampeln per Klick mit direkter Kollisionsüberprüfung (*virtuell-enaktiv*), analysieren statische Verkehrsbilder und Tabellen (*ikonisch*) und leiten Boolesche Formeln ab (*symbolisch*).
--8<-- [end:eis_prinzip]

--8<-- [start:enaktiv]
<span id="enaktiv"></span>

??? info "Enaktive Repräsentation (handelnd)"
    * **Didaktisch:** Wissenserwerb durch unmittelbares eigenes Tun, Ausprobieren und physisches Hantieren mit realen Gegenständen (nach Jerome Bruner). Diese Repräsentationsform eignet sich besonders für den Einstieg in ein abstraktes Thema, da Sachverhalte dadurch besser im Gedächtnis verankert werden
    * **Im LogicTraffic-Unterricht:** Lernende stellen Verkehrssituationen haptisch mit physischen Kreuzungsmatten, Modellautos und drehbaren Ampeln nach, um Vorfahrtsregeln und Kollisionsrisiken gegenständlich zu begreifen.
--8<-- [end:enaktiv]

## F 

--8<-- [start:fundamentale_ideen]
<span id="fundamentale-ideen"></span>

??? info "Fundamentale Ideen der Informatik"
    * **Didaktisch:** Zeitstabile, allgemeinbildende Kernkonzepte der Disziplin nach Schwill und Denning, die auf verschiedenen kognitiven Niveaus unterrichtet werden können (Horizontalkriterium, Vertikalkriterium, Sinnkriterium, Zeitkriterium).
    * **Im LogicTraffic-Unterricht:** Aussagenlogik, Modellierung und Systemdenken bilden fundamentale Basiskonzepte, die nicht nur für die Informatik, sondern für fundiertes Problemlösen im Alltag relevant sind.
--8<-- [end:fundamentale_ideen]

## I

--8<-- [start:ikonisch]
<span id="ikonisch"></span>

??? info "Ikonische Repräsentation (bildhaft)"
    * **Didaktisch:** Erfassen von Sachverhalten und Strukturen durch statische Visualisierungen, Bilder, Skizzen oder grafische Modelle (nach Jerome Bruner).
    * **Im LogicTraffic-Unterricht:** Statische Darstellungen von Kreuzungen, visualisierte Fahrspuren, Richtungspfeile und schematische Ampelgrafiken verdeutlichen die räumlichen Konfliktpunkte der Fahrwege.
--8<-- [end:ikonisch]

--8<-- [start:implikation]
<span id="implikation"></span>

??? info "Implikation ($\rightarrow$ / WENN ... DANN)"
    * **Fachlich:** Logische Konditionalaussage / Subjunktion ($A \rightarrow B \equiv \neg A \lor B$). Nur dann falsch ($0$), wenn die Prämisse wahr ($1$) und die Konklusion falsch ($0$) ist.
    * **In LogicTraffic:** $A \rightarrow \neg B$ formuliert eine Schaltungsregel: «Wenn Spur $A$ Grün hat, dann muss Spur $B$ zwingend Rot haben».
--8<-- [end:implikation]

--8<-- [start:informatische_modellierung]
<span id="informatische-modellierung"></span>

??? info "Informatische Modellierung & Abstraktion"
    * **Didaktisch:** Der Prozess, ein komplexes reales Problem auf seine wesentlichen Aspekte zu reduzieren und in eine formale, digital verarbeitbare Repräsentation zu überführen.
    * **Im LogicTraffic-Unterricht:** Eine reale Verkehrskreuzung wird vereinfacht als System binärer Fahrspuren modelliert (Grün = $1$, Rot = $0$, keine Gelbphase), um logische Abhängigkeiten und Kollisionsregeln formalisierbar zu machen.
--8<-- [end:informatische_modellierung]

## K

--8<-- [start:kdnf]
<span id="kdnf"></span>

??? info "Kanonische Disjunktive Normalform (KDNF / CDNF)"
    * **Fachlich:** Eine ODER-Verknüpfung aller Minterme (Vollkonjunktionen aller beteiligten Variablen für jede Zeile der Wahrheitstabelle mit dem Ausgangswert $1$).
    * **In LogicTraffic:** Beschreibt die Steuerung als Summe aller erlaubten, kollisionsfreien Gesamtzustände der Kreuzung.
--8<-- [end:kdnf]

--8<-- [start:kknf]
<span id="kknf"></span>

??? info "Kanonische Konjunktive Normalform (KKNF / CCNF)"
    * **Fachlich:** Eine UND-Verknüpfung aller Maxterme (Volldisjunktionen zur gezielten Sperrung aller Zeilen der Wahrheitstabelle mit dem Ausgangswert $0$).
    * **In LogicTraffic:** Beschreibt die Steuerung durch das explizite Verbot aller kollisionsgefährdeten Ampelkombinationen.
--8<-- [end:kknf]

--8<-- [start:konjunktion]
<span id="konjunktion"></span>

??? info "Konjunktion ($\land$ / UND)"
    * **Fachlich:** Logisches UND. Genau dann wahr ($1$), wenn alle verknüpften Teilaussagen wahr ($1$) sind.
    * **In LogicTraffic:** $A \land B$ beschreibt das gleichzeitige Grün zweier Spuren, was bei sich schneidenden Fahrwegen zu einer Kollision führt.
--8<-- [end:konjunktion]

--8<-- [start:kontextorientierung]
<span id="kontextorientierung"></span>

??? info "Kontextorientierung & Lebensweltbezug"
    * **Didaktisch:** Didaktisches Prinzip (u. a. «Informatik im Kontext» / IniK), bei dem Fachinhalte nicht abstrakt-systematisch, sondern eingebettet in bedeutungsvolle Problemstellungen aus der Lebenswelt der Lernenden eingeführt werden.
    * **Im LogicTraffic-Unterricht:** Der Straßenverkehr dient als vertraute Alltagsanalogie: Das intuitive Verständnis von Vorfahrt und Unfallgefahr motiviert direkt den formalen Bedarf nach Kollisionsfreiheit und Boolescher Logik.
--8<-- [end:kontextorientierung]

## N

--8<-- [start:negation]
<span id="negation"></span>

??? info "Negation ($\neg$ / NICHT)"
    * **Fachlich:** Logische Verneinung und Umkehrung eines Wahrheitswertes ($\neg 1 = 0$, $\neg 0 = 1$).
    * **In LogicTraffic:** $\neg A$ steht für «Spur $A$ hat kein Grün» (also Rot).
--8<-- [end:negation]

--8<-- [start:normalform]
<span id="normalform"></span>

??? info "Normalform (KNF / DNF / Simplest)"
    * **Fachlich:** Standardisierte Formelstrukturen (KNF als Konjunktion von Disjunktionen, DNF als Disjunktion von Konjunktionen); minimierte Formen werden meist über den Quine-McCluskey-Algorithmus ermittelt.
    * **In LogicTraffic:** Kompakte Steuerungsausdrücke, die im Dropdown-Menü ausgewählt oder im Formeleditor schrittweise optimiert werden können.
--8<-- [end:normalform]

## P

--8<-- [start:polizisten_status]
<span id="polizisten-status"></span>

??? info "Polizisten-Status (Feedback in LogicTraffic)"
    * **Fachlich:** Semantische Korrektheitsprüfung des logischen Gesamtausdrucks gegenüber der modellierten Sicherheitsmatrix.
    * **In LogicTraffic:** Visuelle Rückmeldung über das Polizisten-Icon in drei Stufen:
        * **Not safe (Stopp-Geste):** Die Formel erlaubt mindestens eine Kollision (eine unsichere Konfiguration ist als $1$ deklariert).
        * **Safe (nachdenklich):** Keine Kollision möglich, aber gefahrlose Ampelkonstellationen werden unnötig blockiert (mindestens eine sichere Konfiguration hat den Wert $0$).
        * **Optimal (salutierend):** Exakte Übereinstimmung; alle sicheren Zustände sind freigegeben ($1$) und alle unsicheren gesperrt ($0$).
--8<-- [end:polizisten_status]

## S

--8<-- [start:symbolisch]
<span id="symbolisch"></span>

??? info "Symbolische Repräsentation (formal-abstrakt)"
    * **Didaktisch:** Höchste Abstraktionsstufe zur Erfassung von Sachverhalten mittels formaler Zeichen, Text, mathematischer Notationen oder Codes (nach Jerome Bruner). Bietet den didaktischen Vorteil, komplexe Zusammenhänge äußerst kompakt und präzise zu beschreiben.
    * **Im LogicTraffic-Unterricht:** Beschreibung von Sicherheitsbedingungen durch formal-logische Notationen (z. B. Boolesche Formeln mit $\land, \lor, \neg, \rightarrow$, Normalformen KDNF/KKNF) sowie tabellarische Codierungen in der Wahrheitstabelle ($0$ und $1$).
--8<-- [end:symbolisch]

## V

--8<-- [start:virtuell_enaktiv]
<span id="virtuell-enaktiv"></span>

??? info "Virtuell-enaktive Repräsentation (simulativ-handelnd)"
    * **Didaktisch:** Informatikdidaktische Erweiterung der klassischen Bruner-Trias (nach Hartmann, Näf & Reichert sowie Arnold). Reale Handlungsprozesse werden durch interaktive Manipulation dynamischer Software-Objekte und Echtzeitsimulationen am Computer nachgebildet.
    * **Im LogicTraffic-Unterricht:** Durch Mausklicks auf Ampeln verändern Lernende Schaltzustände interaktiv und erhalten durch die animierte Verkehrssimulation unmittelbares Feedback (fließender Verkehr vs. Kollision).
--8<-- [end:virtuell_enaktiv]

## W

--8<-- [start:wahrheitstabelle]
<span id="wahrheitstabelle"></span>

??? info "Wahrheitstabelle (Truth Table)"
    * **Fachlich:** Vollständige tabellarische Übersicht aller $2^n$ Belegungsmöglichkeiten für $n$ Variablen und dem resultierenden Gesamtwahrheitswert.
    * **In LogicTraffic:** Tabelle aller Ampelkombinationen mit der Zielspalte `sicher` ($1$ = kollisionsfrei, $0$ = Kollisionsgefahr).
--8<-- [end:wahrheitstabelle]

--8<-- [start:wahrheitswert]
<span id="wahrheitswert"></span>

??? info "Wahrheitswert ($0$ und $1$)"
    * **Fachlich:** Die beiden Werte der klassischen zweiwertigen Logik ($1 = \text{wahr}$, $0 = \text{falsch}$).
    * **In LogicTraffic:** Repräsentiert die Ampelphasen: $1 = \text{Grün (Fahrt frei)}$, $0 = \text{Rot (Halt)}$.
--8<-- [end:wahrheitswert]
