# Wahrheitstabellen 

## Wahrheitstabellen und LogicTraffic 
???+ logictraffic "Wahrheitstabellen" 
    Wahrheitstabellen sind ein zentrales Werkzeug in LogicTraffic, um systematisch alle möglichen Zustände einer Verkehrskreuzung festzuhalten und zu überprüfen, ob Formeln sicher sind, sprich ob diese keine Kollisionen zulassen [^1].
### Definition 
??? student "Wahrheitstabelle" 
    Eine Wahrheitstabelle listet systematisch alle Kombinationen der Wahrheitswerte (0 = falsch/rot, 1 = wahr/grün) aller Variablen (bei Logictraffic entsprechen diese Spuren bzw. Ampeln) auf. Eine Wahrheistabelle für $n$ Variablen hat entsprchend $2^n$ Zeilen [^2]. Pro Zeile wird in der Wahrheitstabelle in einer zusätzlichen Spalte der jeweilige Wahrheitswert einer betimmten Formel angegeben.

### Wahrheitstabellen in Logictraffic 
!!! logictraffic "Wahrheitstabelle"
    In LogicTraffic entspricht die „sicher“-Spalte der Ampelsicherheit. Entsprechend sind 0 und 1-Werte in dieser Spalte wie folgt zu interpretieren:

    * 1: bei dieser Belegung der Wahrheitstabelle (also bei diesen Ampel-Einstellungen) sind keine Kollision möglich
    * 0: bei dieser Belegung der Wahrheitstabelle (also bei diesen Ampel-Einstellungen) sind Kollision möglich

    Diese Werte können z.B. durch klicken auf den aktuellen Wert geändert werden. Und entsprechend passt sich die zur Wahrheitstabelle automatisch generierte Formel unterhalb an.


???+ teacher "Sinn der Wahrheitstabelle in der Simulation" 
    In der Simulation dient die Wahrheitstabelle unterschiedlichen didaktischen Zielsetzungen: 

    * Visualisierung: Parallel zur Simulation zeigt die Tabelle Ampelzustände und Sicherheitsstatus (nicht sicher, nicht optimal, optimal).
    * Interaktion: Klicks auf Ampeln oder Tabelle aktualisieren die Formel automatisch (z. B. zu DNF oder KNF).
    * Lernweg: Schüler:innen markieren erst manuell „sichere“ Zeilen, dann generiert das Programm Formeln – ideal für entdeckendes Lernen.

[^1]: Arnold, R., & Hartmann, W. (2007). LogicTraffic – Logik in der Allgemeinbildung. Informatik-Spektrum, 30(1), 19–26. https://doi.org/10.1007/s00287-006-0123-7
