Hier kommt ausführlichere Theorie und didaktische Aufarbeitung zu den Normalformeln mit Links zu Erklärungsvideos etc. 

!!! teacher "Konjunktive und Disjunktive Normalformen erklären" 
    Für Schülerinnen und Schüler können die DNF und KNF als zwei feste „Bauweisen“ für logische Bedingungen erklärt werden, die man direkt aus einer Wahrheitstabelle ablesen kann.



## Disjunktive Normalform (DNF) 
!!! student "Disjunktive Normalform" 
    Disjunktive Normalform (DNF): Eine Disjunktive Normalform ist eine grosse ODER-Verknüpfung von UND-Bedingungen [^1]. Jede UND‑Bedingung beschreibt eine Zeile der Wahrheitstabelle, in der das Ergebnis wahr (1) ist.

!!! logictraffic "Beispiel aus Logic Traffic für die DNF - Situation 3" 
    === Situation 3: 
          ![Situation 3](../images/Situation3){ width="150" }
    === Wahrheitstabelle zur Situation 3: 
        ![WahrheitstabelleSituation3](../images/WahrheitstabelleSituation3){ width 100 }
    === Herleitung Disjunktive Normalform
        Die Funktion ist in 5 verschiedenen Zeilen wahr. Die vollständige (kanonische) disjunktive Normalform ist dann: 
        $$(\neg A \wedge \neg B \wedge \neg C) \lor (\neg A \wedge \neg B \wedge C) \lor (\neg A \wedge B \wedge \neg C) \lor (A \wedge \neg B \wedge \neg C) \lor (A \wedge B \wedge \neg C)$$
        Wenn wir dies nun kürzen kommen wir auf folgende DNF: 
        $$(\neg A \land \neg B)\lor(\neg C)$$
        ??? student "Erklärung in natürlicher Sprache:"
            Diese Formel drückt aus: Die Bedingung gilt genau dann, wenn entweder beide A und B falsch sind oder C falsch ist. Die Formel ist wahr wenn mindestens eine der beiden Situationen eintritt: 1. A ist falsch **und** B ist falsch (egal was C ist) oder C ist falsch (egal was A oder B sind) 

## Konjunktive Normalform (KNF) 
!!! student "Konjunktive Normalform" 
    Eine KNF ist eine grosse UND‑Verknüpfung von ODER‑Bedingungen. [^1] [^2]. Jede ODER‑Bedingung beschreibt eine Zeile der Wahrheitstabelle, in der das Ergebnis falsch (0) ist. Du kannst dir die KNF vorstellen wie ein Sicherheitscheck: Alle Bedingungen (die ODER-Klammern) müssen erfüllt sein, damit die ganze Sache „wahr“ ist. Wenn auch nur eine ODER-Klammer „falsch“ ist, scheitert alles [^3].

!!! logictraffic "Beispiel aus Logic Traffic für die DNF - Situation 3" 
    === Situation 3: 
          ![Situation 3](../images/Situation3){ width="150" }
    === Wahrheitstabelle zur Situation 3: 
        ![WahrheitstabelleSituation3](../images/WahrheitstabelleSituation3){ width 100 }
    === Herleitung Konjunktive Normalform 
        Die Funktion ist in 3 verschiedenen Zeilen falsch ($0$). Daraus ergibt sich die vollständige (kanonische) konjunktive Normalform: 
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
    | DNF  | ODER von UND‑Ketten (Minterme). wikipedia+2           | Verknüpft alle Zeilen mit Ergebnis 1. inf-schule+2                 |
    | KNF  | UND von ODER‑Klammern (Maxterme). formal.kastel.kit+2 | Verknüpft alle Zeilen mit Ergebnis 0. image.informatik.htw-aalen+2 |


[^1]: Boolesche Funktionen und ihre Normalformen. (2021, Juni 22). https://lehrerfortbildung-bw.de/u_matnatech/imp/gym/bp2016/fb2/m02_aug/1_hintergrund/4_grund/06_funktionen/
[^2]: Inf-schule | Schaltnetze » Fachkonzept disjunktive Normalform. (o. J.). Abgerufen 17. März 2026, von https://inf-schule.de/rechner/digitaltechnik/Schaltnetze/Fachkonzept_Normalform
[^3]: Konjunktive Normalform: Umwandlung & Beispiel. (o. J.). StudySmarter. Abgerufen 17. März 2026, von https://www.studysmarter.de/schule/informatik/theoretische-informatik/konjunktive-normalform/

