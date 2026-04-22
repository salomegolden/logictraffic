# Einführung in das Online Tool LogicTraffic 

Die Grundidee der Online Lernumgebung LogicTraffic ist es, eine aussagelogische Formel zu finden, welche die vorgegebene Verkehrssituation sicher macht. 

!!! logictraffic "Programmaufbau:" 
    ![LogicTraffic](../images/Screenshot%202026-04-22%20at%2009-49-45%20logictraffic_anleitung%20-%20logictraffic_anleitung.pdf.png)
    In der graphischen Lernumgebung werden Verkehrssituationen an einer Kreuzung dargestellt. Dabei wird jede Fahrspur durch eine Variable (A, B, C…) identifiziert und jede Spur hat eine dazugehörige Ampel. Daneben werden in einer Wahrheitstabelle alle Spuren aufgelistet und es wird festgelegt, welche Konfigurationen sicher sind. Hier entspricht „0“ (logisch falsch) einer roten Ampel, also „Fahrspur nicht frei“ und entsprechend „1“ (logisch wahr) einer grünen Ampel, also „Spur befahrbar“. Eine Statusanzeige gibt an, ob die aktuelle Belegung der Tabelle (also die Einträge in der „sicher“-Spalte) nicht sicher, nicht optimal oder optimal ist. Ebenfalls wird zur aktuellen Belegung der Tabelle eine aussagenlogische Formel in gewünschter Form angegeben. Im Weiteren steht ein Formeleditor zur Verfügung, in welchem direkt Formeln erstellt und editiert werden können.

## Konfrontationsaufgaben

### Konfrontationsaufgabe 1 
??? teacher "Aufgabe weglassen" 
    Diese Konfrontationsaufgabe kann auch weggelassen werden, falls zuvor der Einstieg ins Thema enaktiv durchgeführt wurde [Einstieg](../lessons/einstiegenaktiv.md). Allerdings bietet sie auch eine gute Wiederholung der sprachlichen Beschreibung von Situationen. 

!!! logictraffic "KA1 - Einführung LogicTraffic" 
    Die Lehrperson zeigt ein Foto/kurzes Video einer stark befahrenen Kreuzung mit Ampeln (Beamer/Arbeitsblatt) [Beispiele](../material/LogicTraffic%20-%20Einführung%20Konfrontationsaufgabe%201%20Mögliche%20Bilder%20von%20Kreuzungen%20und%20Verkehrssituationen.pdf).

    !!! student "Auftrag an die Lernenden, 5 - 10 Minuten"
        Beschreibe, was an dieser Kreuzung alles gleichzeitig passieren muss, damit niemand verunfallt.
        Formuliere mindestens drei „Wenn‑dann“-Sätze zur Kreuzung, z.B.:
            Wenn die Fußgängerampel grün ist, dann …
            Wenn ein Bus kommt, dann …
        Überlege:
            Wer oder was „entscheidet“, wann welches Licht leuchtet?
            Glaubst du, dass dahinter ein Programm steckt? Begründe.

### Konfrontationsaufgabe 2
??? teacher "Ziel der Aufgabe" 
    
!!! logictraffic "KA2 - Die Schaltzentrale - Problemfrage zum Tool" 
    
    Tafelbild mit der Leitfrage: "Stell dir vor, du bist die Schaltzentrale dieser Kreuzung. Wie würdest du die Ampeln so steuern, dass es nie zu Unfällen kommt?" -> Als Material kann man die Bilder von [KA1](#konfrontationsaufgabe-1) verwenden. 

    !!! student "Auftrag - Einzel oder Gruppenarbeit, 5-10 Minuten" 
        
        1. Skizziere auf einem Blatt grob eine Kreuzung (nur mit Strichen/Pfeilen).
        2. Schreibe dazu, wann welche Ampel „Grün“, „Rot“ oder „Gelb“ sein soll.  Nutze wieder Wenn‑dann‑Sätze.
        3. Tauscht euch kurz mit einer anderen Person aus: Finden sich Widersprüche? Gibt es Situationen, die ihr noch nicht geregelt habt? 
    
    !!! teacher "Anschlussfrage im Plenum" 
        „Wie könnten wir so etwas mit einem Computer programmieren, ohne eine Programmiersprache lernen zu müssen?“

    !!! teacher "Übergang zu Erarbeitungsaufgaben" 
        Die Lehrperson präsentiert kurz die Startseite von https://logictraffic.ch und lässt es kurz von Schüler:innen beschreiben: 
         
        - Wofür könnte das gut sein? 
        - Was könnte man damit machen? 

## Erarbeitungsaufgaben

### Erarbeitungsaufgabe 1 - Finde die Bausteine 
??? teacher "Ziel der Aufgabe" 
    Hier geht es um das Erarbeiten der "Sprache" von logictraffic.ch: Oberflächen, Bausteine, Simulation. 
    
    
    
!!! logictraffic "EA1 - Bedienung und Grundkonzept des Tools aufbauen" 
    
