# Wahrheitstabellen 

## Wahrheitstabellen und LogicTraffic 
???+ logictraffic "Wahrheitstabellen" 
    Wahrheitstabellen sind ein zentrales Werkzeug in LogicTraffic, um alle möglichen Zustände einer Verkehrskreuzung zu überprüfen und logische Regeln zu validieren [^1].

### Definition 
??? student "Wahrheitstabelle" 
    Eine Wahrheitstabelle listet systematisch alle Kombinationen der Wahrheitswerte (0 = falsch/rot, 1 = wahr/grün) der beteiligten Aussagen auf und zeigt den Wert der Gesamtformel pro Zeile.
    Für $n$ Variablen hat eine Wahrheistabelle $2^n$ Zeilen [^2]. 

### Wahrheitstabellen in Logictraffic 
!!! teacher "Wahrheitstabelle"
    In LogicTraffic entspricht die „sicher“-Spalte der Ampelsicherheit: 1 = keine Kollision, 0 = Unfallgefahr.
    In der Simulation dient die Wahrheitstabelle unterschiedlichen didaktischen Zielsetzungen: 

    * Visualisierung: Parallel zur Simulation zeigt die Tabelle Ampelzustände und Sicherheitsstatus (nicht sicher, nicht optimal, optimal).
    * Interaktion: Klicks auf Ampeln oder Tabelle aktualisieren die Formel automatisch (z. B. zu DNF oder KNF).
    * Lernweg: Schüler:innen markieren erst manuell „sichere“ Zeilen, dann generiert das Programm Formeln – ideal für Entdeckendes Lernen.


[^1]: Arnold, R., & Hartmann, W. (2007). LogicTraffic – Logik in der Allgemeinbildung. Informatik-Spektrum, 30(1), 19–26. https://doi.org/10.1007/s00287-006-0123-7
