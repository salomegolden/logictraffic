# Lernen und Lehren von Logik im Infromatikunterricht 
Boolesche bzw. aussagenlogische Inhalte werden in mehreren empirischen Arbeiten als zentral für kritisches Denken, Mathematik/Informatik und Problemlösen beschrieben, gleichzeitig aber als nachweislich schwierig zu erlernen mit typischen, gut dokumentierten Fehlvorstellungen [^1] [^2]. 

## Begründung für die Bedeutung im Unterricht 
Abgesehen von den inhaltlichen Verknüpfungen zu den Lehrplänen von Gymnasium und der obligatorischen Schule [Lernziele und Lehrplan](goals.md) zeigt auch die Forschung, dass Logik eine wichtige und grundlegende Basis darstellt: Studien betonen, dass logisches Denken Sprache, Erfahrung und Fachwissen verknüpft und so Problemlöse‑ und Entscheidungsfähigkeit unterstützt [^1]. 
In einer Studie zur Wiedereinführung von Logik in der Sekundarstufe berichten Schüler, dass sie Logik als hilfreich für Mathematik, Alltag und weitere Ausbildung einschätzen, wenn sie mit alltagsnahen Beispielen unterrichtet wird [^3].

## typische Fehlvorstellungen 
Im Folgenden werden typische Fehlvorstellungen beschrieben. Die Beschreibung und Konzepte stammen aus einer Forschungsarbeit welche mit Studierenden durchgeführt worden ist [^2]: 

??? error "Fehlvorstellung 1: Implikation wird als AND interpretiert"
    Lernende glauben, dass eine Aussage der Form „Wenn A, dann B“ bedeutet: A UND B müssen gleichzeitig wahr sein.
    
    ??? meta "Warum ist das falsch?"
        Die Implikation A→B ist nur dann falsch, wenn A wahr und B falsch ist.
        In allen anderen Fällen ist sie wahr, auch wenn A gar nicht eintritt.
        
    ??? meta "Warum die Fehlvorstellung entsteht"
        Alltagssprache erzeugt ein kausales Verständnis: „Wenn A passiert, muss B passieren“.
        
    !!! student "Merksatz gegen die Fehlvorstellung"
        Implikation beschreibt keine Kausalität, sondern eine logische Bedingung.
        Nur der Fall A wahr, B falsch macht sie falsch.

??? error "Fehlvorstellung 2: OR als "genau eine Bedingung" oder als Bestätigung eine der Bedingungen, statt als inklusives Oder"
    Lernende glauben, dass das logische Oder $A \lor B$ nur dann wahr ist, wenn genau eine der beiden Bedingungen wahr ist. Sie interpretieren OR also wie ein exklusives Oder (XOR). Oder sie denken: OR bedeutet, dass B gilt oder A gilt – aber nicht, dass beide gleichzeitig wahr sein dürfen.

    ??? meta "Warum ist das falsch?" 
        Das ODER ($\lor$) der Aussagenlogik sagt:
        Die Aussage ist wahr, wenn mindestens eine der Bedingungen wahr ist. 
        Sie ist also auch wahr, wenn beide wahr sind.

    ??? meta "Warum die Fehlvorstellung entsteht" 
        Alltagssprache benutzt „oder“ meistens exklusiv („Pizza oder Pasta?“ → meist nur eins).
        In vielen Übungsbeispielen tauchen OR‑Fälle nicht gleichzeitig wahr auf – der Fall „1/1“ wird unbewusst vergessen.

    !!! student "Merksatz gegen die Fehlvorstellung:"
        OR bedeutet: Mindestens eine Bedingung ist erfüllt - auch beide. 
        XOR bedeutet: Genau eine der Bedingung ist erfüllt. (Wobei das in Logictraffic nicht behandelt wird) 
    
??? error "Fehlvorstellung 3: Komplexe Operatoren werden auf „einfache“ AND/OR‑Muster reduziert
    Lernende versuchen, komplexere logische Ausdrücke – besonders die Implikation („Wenn A, dann B“) – auf vermeintlich einfache Muster wie A ∧ B oder A ∨ B zu reduzieren. Die vollständigen Wahrheitsbedingungen werden dabei nicht berücksichtigt. Typisch ist folgende fehlerhafte Reduktion: $A \rightarrow B$ wird zu $A \land B$ (beide müssen wahr sein) oder zu $A \lor B$ (mindestens eine Bedingung wahr)
    ??? meta "Warum ist das falsch?" 
        die Implikation ist nur dann falsch, wenn A wahr und B falsch ist. Weder AND noch OR besitzen diese Struktur — eine intuitive Reduktion verändert also die gesamte logische Aussage.
        
    ??? meta "Warum die Fehlvorstellung entsteht:" 
        Lernende suchen „einfache Muster“, um sprachliche Formulierungen schnell zu übersetzen.
        Alltagssprache erzeugt eine kausale Logik („Wenn A passiert, muss B passieren“) → wirkt wie AND

    !!! student "Merksatz gegen die Fehlvorstellung" 
        Eine Implikation ist keine UND‑ oder ODER‑Aussage.  Sie ist nur im Fall A=1, B=0 falsch – sonst wahr.

??? error "Fehlvorstellung 4: Nichtbeachtung komplementierter Variablen"
    Lernende berücksichtigen beim Bilden oder Interpretieren von logischen Ausdrücken nicht alle möglichen Wahrheitsfälle, insbesondere jene, in denen Variablen falsch (¬A, ¬B, …) sind. 
    Dadurch entstehen unvollständige oder falsche Normalformen (DNF, KDNF, KNF, KKNF). Typische vergessene Fälle: A ist falsch || alle Variablen sind falsch (∅‑Fall) || Kombinationen, in denen mehrere Variablen negiert sind

    ??? meta "Warum die Fehlvorstellung entsteht:" 
    Alltagssprache führt zu einem „positiven Denkmuster“: Man nennt nur, was vorhanden ist, nicht was fehlt.
    Das mentale Modell ist oft visuell („dann steht da nur A“), nicht tabellarisch‑formal.
    Fehlen der Systematik: Lernende prüfen nicht alle Kombinationen, sondern nur „naheliegende“ Fälle.

    !!! student "Merksatz gegen die Fehlvorstellung"
    Ein Fall ist nur korrekt beschrieben, wenn alle relevanten Variablen ausdrücklich vorkommen – als A oder als ¬A. Weggelassene Negationen führen fast immer zu falschen Formeln.
    

[^1]: Fehér, Z., Jaruska, L., Szarka, K., & Tóthová Tarová, E. (2023). Students’ propositional logic thinking in higher education from the perspective of disciplines. Frontiers in Education, 8. https://doi.org/10.3389/feduc.2023.1247653
[^2]: Herman, G. L., Loui, M. C., Kaczmarczyk, L., & Zilles, C. (2012). Describing the What and Why of Students’ Difficulties in Boolean Logic. ACM Transactions on Computing Education, 12(1), 1–28. https://doi.org/10.1145/2133797.2133800
[^3]: Milbou, L., Deprez, J., & Laenens, E. (o. J.). A study on the Reintroduction of Logic in Secondary Schools.
