<!-- docs/includes/begriffe.md -->

# Stichwortverzeichnis: Logik & Boolesche Algebra

## A

--8<-- [start:absorption]
??? note "Fachbegriff: Absorption" {: #absorption }
    * **Fachlich:** Rechenregel der Booleschen Algebra ($A \lor (A \land B) \equiv A$ bzw. $A \land (A \lor B) \equiv A$)[cite: 1]. Ein Teilausdruck fällt weg, wenn sein Wahrheitswert bereits vollständig durch einen einfacheren Teilausdruck bestimmt wird[cite: 1].
    * **In LogicTraffic:** Ermöglicht die formale Kürzung überflüssiger Sicherheitsbedingungen bei der Formelminimierung (z. B. $\neg A \land (\neg A \lor \neg B) \equiv \neg A$)[cite: 1, 4, 5].
--8<-- [end:absorption]

--8<-- [start:aequivalenz]
??? note "Fachbegriff: Äquivalenz ($\equiv$ bzw. $\sim$)" {: #aequivalenz }
    * **Fachlich:** Logische Gleichwertigkeit zweier Formeln ($\phi \sim \psi$); beide besitzen für jede denkbare Belegung identische Wahrheitswerte[cite: 1].
    * **In LogicTraffic:** Zwei unterschiedliche Schaltformeln steuern die Ampeln in jeder Situation exakt gleich sicher und erzeugen dieselbe Spalte `sicher` in der Wahrheitstabelle[cite: 1, 4, 5].
--8<-- [end:aequivalenz]

--8<-- [start:aussage]
??? note "Fachbegriff: Aussage (Proposition)" {: #aussage }
    * **Fachlich:** Ein sprachliches Gebilde bzw. eine formale Aussage, die eindeutig entweder wahr ($1$) oder falsch ($0$) ist (Prinzip der Zweiwertigkeit)[cite: 1].
    * **In LogicTraffic:** Bezieht sich immer auf den konkreten Zustand einer Signalanlage (z. B. «Spur $A$ hat Grün»)[cite: 3, 4, 5].
--8<-- [end:aussage]

--8<-- [start:aussagenvariable]
??? note "Fachbegriff: Aussagenvariablen ($A, B, C, \dots$)" {: #aussagenvariable }
    * **Fachlich:** Buchstaben oder Symbole als Platzhalter für einen Wahrheitswert ($0$ oder $1$)[cite: 1].
    * **In LogicTraffic:** Jede Fahrspur bzw. Ampel der Kreuzung wird durch genau eine Variable repräsentiert[cite: 2, 4, 5].
--8<-- [end:aussagenvariable]

## B

--8<-- [start:boolesche_algebra]
??? note "Fachbegriff: Boolesche Algebra" {: #boolesche-algebra }
    * **Fachlich:** Mathematische Struktur und Regelwerk für logische Verknüpfungen mit Wahrheitswerten ($0$ und $1$) basierend auf formalen Axiomen (Kommutativität, Assoziativität, Distributivität, Komplement etc.)[cite: 1].
    * **In LogicTraffic:** Bildet die mathematische Grundlage zur formalen Beschreibung, Prüfung und Vereinfachung von Kreuzungssteuerungen[cite: 3, 4, 5].
--8<-- [end:boolesche_algebra]

## D

--8<-- [start:de_morgan]
??? note "Fachbegriff: De Morgan'sche Gesetze" {: #de-morgan }
    * **Fachlich:** Regeln zur Negation von Konjunktionen und Disjunktionen: $\neg (A \land B) \equiv \neg A \lor \neg B$ sowie $\neg (A \lor B) \equiv \neg A \land \neg B$[cite: 1].
    * **In LogicTraffic:** Transformiert das Verbot des gleichzeitigen Grüns zweier Spuren ($\neg(A \land B)$) direkt in eine handlungsorientierte Schaltungsregel («Spur $A$ hat Rot oder Spur $B$ hat Rot»)[cite: 3, 4, 5].
--8<-- [end:de_morgan]

--8<-- [start:disjunktion]
??? note "Fachbegriff: Disjunktion ($\lor$ / ODER)" {: #disjunktion }
    * **Fachlich:** Logisches ODER (nicht-exklusiv). Genau dann wahr ($1$), sobald mindestens eine der Teilaussagen wahr ist[cite: 1].
    * **In LogicTraffic:** $\neg A \lor \neg B$ bedeutet: Mindestens eine der beiden Spuren $A$ oder $B$ muss Rot haben (kein gleichzeitiges Grün)[cite: 3, 4, 5].
--8<-- [end:disjunktion]

## I

--8<-- [start:implikation]
??? note "Fachbegriff: Implikation ($\rightarrow$ / WENN ... DANN)" {: #implikation }
    * **Fachlich:** Logische Konditionalaussage / Subjunktion ($A \rightarrow B \equiv \neg A \lor B$). Nur dann falsch ($0$), wenn die Prämisse wahr ($1$) und die Konklusion falsch ($0$) ist[cite: 1].
    * **In LogicTraffic:** $A \rightarrow \neg B$ formuliert eine Schaltungsregel: «Wenn Spur $A$ Grün hat, dann muss Spur $B$ zwingend Rot haben»[cite: 3, 4, 5].
--8<-- [end:implikation]

## K

--8<-- [start:kdnf]
??? note "Fachbegriff: Kanonische Disjunktive Normalform (KDNF / CDNF)" {: #kdnf }
    * **Fachlich:** Eine ODER-Verknüpfung aller Minterme (Vollkonjunktionen aller beteiligten Variablen für jede Zeile der Wahrheitstabelle mit dem Ausgangswert $1$)[cite: 1, 4].
    * **In LogicTraffic:** Beschreibt die Steuerung als Summe aller erlaubten, kollisionsfreien Gesamtzustände der Kreuzung[cite: 4, 5].
--8<-- [end:kdnf]

--8<-- [start:kknf]
??? note "Fachbegriff: Kanonische Konjunktive Normalform (KKNF / CCNF)" {: #kknf }
    * **Fachlich:** Eine UND-Verknüpfung aller Maxterme (Volldisjunktionen zur gezielten Sperrung aller Zeilen der Wahrheitstabelle mit dem Ausgangswert $0$)[cite: 1, 4].
    * **In LogicTraffic:** Beschreibt die Steuerung durch das explizite Verbot aller kollisionsgefährdeten Ampelkombinationen[cite: 3, 4, 5].
--8<-- [end:kknf]

--8<-- [start:konjunktion]
??? note "Fachbegriff: Konjunktion ($\land$ / UND)" {: #konjunktion }
    * **Fachlich:** Logisches UND. Genau dann wahr ($1$), wenn alle verknüpften Teilaussagen wahr ($1$) sind[cite: 1].
    * **In LogicTraffic:** $A \land B$ beschreibt das gleichzeitige Grün zweier Spuren, was bei sich schneidenden Fahrwegen zu einer Kollision führt[cite: 3, 4, 5].
--8<-- [end:konjunktion]

## N

--8<-- [start:negation]
??? note "Fachbegriff: Negation ($\neg$ / NICHT)" {: #negation }
    * **Fachlich:** Logische Verneinung und Umkehrung eines Wahrheitswertes ($\neg 1 = 0$, $\neg 0 = 1$)[cite: 1].
    * **In LogicTraffic:** $\neg A$ steht für «Spur $A$ hat kein Grün» (also Rot)[cite: 3, 4, 5].
--8<-- [end:negation]

--8<-- [start:normalform]
??? note "Fachbegriff: Normalform (KNF / DNF / Simplest)" {: #normalform }
    * **Fachlich:** Standardisierte Formelstrukturen (KNF als Konjunktion von Disjunktionen, DNF als Disjunktion von Konjunktionen); minimierte Formen werden meist über den Quine-McCluskey-Algorithmus ermittelt[cite: 1, 4].
    * **In LogicTraffic:** Kompakte Steuerungsausdrücke, die im Dropdown-Menü ausgewählt oder im Formeleditor schrittweise optimiert werden können[cite: 4, 5].
--8<-- [end:normalform]

## P

--8<-- [start:polizisten_status]
??? note "Fachbegriff: Polizisten-Status (Feedback in LogicTraffic)" {: #polizisten-status }
    * **Fachlich:** Semantische Korrektheitsprüfung des logischen Gesamtausdrucks gegenüber der modellierten Sicherheitsmatrix[cite: 4].
    * **In LogicTraffic:** Visuelle Rückmeldung über das Polizisten-Icon in drei Stufen[cite: 4]:
        * **Not safe (Stopp-Geste):** Die Formel erlaubt mindestens eine Kollision (eine unsichere Konfiguration ist als $1$ deklariert)[cite: 4].
        * **Safe (nachdenklich):** Keine Kollision möglich, aber gefahrlose Ampelkonstellationen werden unnötig blockiert (mindestens eine sichere Konfiguration hat den Wert $0$)[cite: 4].
        * **Optimal (salutierend):** Exakte Übereinstimmung; alle sicheren Zustände sind freigegeben ($1$) und alle unsicheren gesperrt ($0$)[cite: 4].
--8<-- [end:polizisten_status]

## W

--8<-- [start:wahrheitstabelle]
??? note "Fachbegriff: Wahrheitstabelle (Truth Table)" {: #wahrheitstabelle }
    * **Fachlich:** Vollständige tabellarische Übersicht aller $2^n$ Belegungsmöglichkeiten für $n$ Variablen und dem resultierenden Gesamtwahrheitswert[cite: 1, 4].
    * **In LogicTraffic:** Tabelle aller Ampelkombinationen mit der Zielspalte `sicher` ($1$ = kollisionsfrei, $0$ = Kollisionsgefahr)[cite: 2, 4, 5].
--8<-- [end:wahrheitstabelle]

--8<-- [start:wahrheitswert]
??? note "Fachbegriff: Wahrheitswert ($0$ und $1$)" {: #wahrheitswert }
    * **Fachlich:** Die beiden Werte der klassischen zweiwertigen Logik ($1 = \text{wahr}$, $0 = \text{falsch}$)[cite: 1].
    * **In LogicTraffic:** Repräsentiert die Ampelphasen: $1 = \text{Grün (Fahrt frei)}$, $0 = \text{Rot (Halt)}$[cite: 2, 4, 5].
--8<-- [end:wahrheitswert]