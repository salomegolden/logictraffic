# Normalformen 
???+ meta "Definition von Normalformeln" 
    Normalformen sind standardisierte Darstellungsformen für boolesche Funktionen, die beliebige logische Ausdrücke in eine einheitliche Struktur aus Konjunktionen und Disjunktionen überführen [^1], [^4]. Sie ermöglichen eine systematische Analyse und Vergleichbarkeit von logischen Funktionen.

!!! teacher "Konjunktive und Disjunktive Normalformen erklären" 
    Für Schülerinnen und Schüler können die KDNF und KKNF als zwei unterschiedliche Startegien erklärt werden, wie aus einer vorgegebenen Wahrheitstabelle systematisch eine dazu passende aussagenlogische Formel erzeugt werden kann. Hinweis: Für Schülerinnen und Schüler kann dieses Thema sehr herausfordernd sein [^5]

## Kanonische Disjunktive Normalform (KDNF) 
???+ student "Disjunktive Normalform" 
    Eine **Disjunktive Normalform** (DNF) ist eine grosse ODER-Verknüpfung von UND-Bedingungen [^1]. Jede UND‑Bedingung beschreibt eine Zeile der Wahrheitstabelle, in der das Ergebnis wahr (1) ist. (Hinweis: Das stimmt nur für die KDNF!) Wenn wir für jede Zeile der Wahrheitstabelle, in der die Funktion „wahr“ (1) ist, eine UND-Bedingung bauen – und in jeder dieser Bedingungen alle Variablen genau einmal stehen (entweder normal oder mit „NICHT“) –, dann verknüpfen wir diese mit ODER. Das Ergebnis ist die **kanonische (vollständige) disjunktive Normalform** (KDNF) [^1], [^2]. Zusammenfassend kann man sagen: Die KDNF beschreibt alle Fälle, in denen die Funktion wahr ist. 
    
    ??? student "Merksatz für die SuS:"
        Jeder Wahre Zeile (1) aus der Tabelle wird zu einem vollen UND-Baustein, alle Bausteine kommen mit ODER zusammen 
    
<!-- Naja, es gibt durchaus SuS die das nicht ganz so schnell kapieren. Denen kann es helfen, einen Merksatz zur Unterscheidung zu haben. Auch wenn es für dich von Beginn weg und für mich mittlerweile logisch ist. -->

??? logictraffic "Beispiel aus Logic Traffic für die KDNF - Situation 3" 

    === "Situation 3:" 
        ![Situation 3](../images/Situation3){ width="150" }
        
    === "Wahrheitstabelle zur Situation 3:"
        Um eine KDNF herzuleiten, betrachten wir als Erstes die Wahrheitstabelle.
        ![WahrheitstabelleSituation3](../images/WahrheitstabelleSituation3){ align=right }
        
    === "Herleitung kanonische Disjunktive Normalform"
        Die Funktion ist in 5 verschiedenen Zeilen wahr. Aus jeder dieser Zeilen entsteht eine UND Kette. Die **kanonische disjunktive Normalform** (KDNF) ist dann: 
        
        $$(\neg A \wedge \neg B \wedge \neg C) \lor (\neg A \wedge \neg B \wedge C) \lor (\neg A \wedge B \wedge \neg C) \lor (A \wedge \neg B \wedge \neg C) \lor (A \wedge B \wedge \neg C)$$ 

        ???+ logictraffic "Darstellung in LogicTraffic" 
            Im Unterricht mit Logictraffic wird diese Formel automatisch erstellt. Für die Anleitung zur Bedienung: LINK 
        
        Durch Zusammenfassen gleicher Teilbedingungen ergibt sich die gekürzte DNF:
        
        $$(\neg A \land \neg B)\lor(\neg C)$$
        
        ??? student "Erklärung in natürlicher Sprache:"
            Diese Formel drückt aus: Die Bedingung gilt genau dann, wenn entweder beide A und B falsch sind oder C falsch ist. Die Formel ist wahr wenn mindestens eine der beiden Situationen eintritt: 1. A ist falsch **und** B ist falsch (egal was C ist) oder C ist falsch (egal was A oder B sind) 

## Konjunktive Normalform (KNF) 

???+ student "Konjunktive Normalform" 
    Die **Konjunktive Normalform** (KNF) ist eine grosse UND‑Verknüpfung von ODER‑Bedingungen. [^1] [^2]. Jede ODER‑Bedingung beschreibt eine Zeile der Wahrheitstabelle, in der das Ergebnis falsch (0) ist. (Das stimmt allg. wiederum )bloss für KKNFs). Du kannst dir die KNF vorstellen wie ein Sicherheitscheck: Alle Bedingungen (die ODER-Klammern) müssen erfüllt sein, damit die ganze Sache „wahr“ ist. Wenn auch nur eine ODER-Klammer „falsch“ ist, scheitert alles [^3]. Wenn wir für jede Zeile der Wahrheitstabelle, in der die Funktion „falsch“ (0) ist, eine ODER-Bedingung bauen – und in jeder dieser Bedingungen alle Variablen genau einmal stehen (entweder normal oder mit „NICHT“) –, dann verknüpfen wir diese mit UND. Das Ergebnis ist die **kanonische konjunktive Normalform** (KKNF) [^1]. 

    ??? student "Merksatz für die SuS" 
        Jeder unsichere Zeile aus der Tabelle (0) wird zu einem vollen ODER-Baustein, alle Bausteine kommen mit UND zusammen – nichts fehlt, nichts wird gekürzt.
    
Durch die Arbeit mit der gleichen Tabelle erkennen Schülerinnen und Schüler gut, wie sich DNF und KNF ergänzen.

??? logictraffic "Beispiel aus Logic Traffic für die DNF - Situation 3" 

    === "Situation 3: "
          ![Situation 3](../images/Situation3){ width="150" }
          
    === "Wahrheitstabelle zur Situation 3: "
        ![WahrheitstabelleSituation3](../images/WahrheitstabelleSituation3){ width 100 }
        
    === "Herleitung Konjunktive Normalform "
        Die Funktion ist in 3 verschiedenen Zeilen falsch ($0$). Aus diesen Zeilen erzeugt man jeweils eine ODER Klammer. Daraus ergibt sich die **kanonische (vollständige) konjunktive Normalform** (KKNF): 
       
        $$(A \lor \neg B \lor \neg C)\land(\neg A \lor B \lor \neg C) \land (\neg A \lor \neg B \lor \neg C)$$ 
        
        Gekürzt ergibt das die KNF: 
        
        $$ (\neg B \lor \neg C) \land (\neg A \lor \neg C) $$ 

        ??? student "Beschreibung in natürlicher Sprache" 
            Diese Formel gilt genau dann, wenn beide Bedingungen erfüllt sind: C ist falsch oder (falls C wahr ist) sowohl A als auch B falsch sein müssen.
            Sie ist wahr, wenn C falsch ist (egal was A und B sind), **oder** wenn C wahr ist, aber **beide** A und B falsch sind.

## Zusammenfassung 
Für Schülerinnen und Schüler kann folgende Tabelle ein Überblick bieten. Es lohnt sich diese gross auszudrucken und bei entsprechenden Unterrichtsinhalten aufzuhängen. 

!!! student "Merktabelle der unten folgenden Erklärungen" 
    | Form | Bausteine                                             | Blick auf Wahrheitstabelle                                         |
    | ---- | ----------------------------------------------------- | ------------------------------------------------------------------ |
    | DNF  | ODER von UND‑Klammern         | Verknüpft alle Zeilen mit Ergebnis 1.           |
    | KNF  | UND von ODER‑Klammern  | Verknüpft alle Zeilen mit Ergebnis 0.  |

## Fächerübergreifenden Unterricht: 
Boolesche Normalformen (DNF, KNF) bieten vielfältige fachübergreifende Anknüpfungspunkte im Gymnasialunterricht. Diese sollen hier einzeln kurz vorgestellt werden: 

### Mathematik 
??? meta "Mengenlehre" 
    DNF entspricht der Vereinigung von Durchschnitten (Summe von Produkten), KNF dem Durchschnitt von Vereinigungen (Produkt von Summen) – direkte Analogie zu Venn-Diagrammen [^1].

??? meta "Algebra" 
    Boolesche Algebra als distributiver komplementärer Verband mit Axiomen wie Kommutativ‑ und De-Morgan-Gesetzen.

### Physilk 
??? meta "Schaltkreise" 
    Schaltalgebra in digitaler Technik (z. B. Logikgatter)

[^1]: Boolesche Funktionen und ihre Normalformen. (2021, Juni 22). https://lehrerfortbildung-bw.de/u_matnatech/imp/gym/bp2016/fb2/m02_aug/1_hintergrund/4_grund/06_funktionen/
[^2]: Inf-schule | Schaltnetze » Fachkonzept disjunktive Normalform. (o. J.). Abgerufen 17. März 2026, von https://inf-schule.de/rechner/digitaltechnik/Schaltnetze/Fachkonzept_Normalform
[^3]: Konjunktive Normalform: Umwandlung & Beispiel. (o. J.). StudySmarter. Abgerufen 17. März 2026, von https://www.studysmarter.de/schule/informatik/theoretische-informatik/konjunktive-normalform/
[^4]: Arnold, R., & Hartmann, W. (2007). LogicTraffic – Logik in der Allgemeinbildung. Informatik-Spektrum, 30(1), 19–26. https://doi.org/10.1007/s00287-006-0123-7
[^5]: Herman, G. L., Loui, M. C., Kaczmarczyk, L., & Zilles, C. (2012). Describing the What and Why of Students’ Difficulties in Boolean Logic. ACM Transactions on Computing Education, 12(1), 1–28. https://doi.org/10.1145/2133797.2133800

