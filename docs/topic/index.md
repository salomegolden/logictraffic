# Zur Sache 

!!! teacher "LogicTraffic"
    LogicTraffic simuliert eine Strassenkreuzung mit Ampeln für verschiedene Fahrspuren. Ziel ist es, eine logische Formel zu finden, die sicherstellt, dass kreuzende Spuren nie gleichzeitig grün haben – so verhindert man Unfälle. Das Programm zeigt, wie Logik im Alltag (z. B. Ampelsteuerung) angewendet wird [^12].

## Grundlagen der Aussagelogik im Kontext von Logic Traffic 
In der **Aussagenlogik** arbeiten wir mit Aussagen, denen eindeutig ein Wahrheitswert (wahr/`true`/1 oder falsch/`false`/0) zugeordnet werden kann [^11].

???+ student "Boolesche Logik"
    **Boolesche Logik** ist die formale Logik mit genau zwei Wahrheitswerten (wahr/falsch bzw. 1/0), in der Aussagen mit Junktoren wie UND ($\land$), ODER ($\lor$) und Negation ($\neg$) verknüpft werden [^5].

???+ logictraffic "Aussagelogik und Logictraffic"
    **LogicTraffic** nutzt Aussagenlogik zur formalen Modellierung von Ampelzuständen an Kreuzungen. Jeder Spur bzw. Ampel ist eine Variable (A, B, C, …) zugewiesen und Formeln beschreiben bestimte Zustände (z.B. "$A$ grün $\lor B$ rot" bzw. "Spur A befahrbar, Spur B gesperrt") [^11], [^10]. 

### Variablen und Zustände 
Eine boolsche Variable ist in der Informatik die kleinste Informationseinheit. Sie trägt genau eine Information, die entweder zutrifft oder eben nicht.

??? logictraffic "Variable in LogicTraffic"
    In LogicTraffic steht jede Variable für den Zustand einer Ampel (rot $0$  / grün $1$) [^10], [^11].

### Aussagen 
???+ student "Beispiele für Aussagen"
    Beispiele für Aussagen:
    
    - "Die Ampel A ist grün."
    - "Auto fährt von Norden nach Süden."
    - „Abbiegen nach rechts ist auf dieser Strasse erlaubt.“  
    
eine **Aussage** wird durch drei Eigenschaften beschrieben [^1], [^7]: 
    
1. eine Aussage ist eine sprachliche Einheit, die einen Sachverhalt ausdrückt.
2. Eine Aussage ist entweder _wahr_ (Wahrheitswert $1$) oder _falsch_ (Wahrheitswert $0$).
3. Die Sprache ist beliebig (natürlich oder formal)

??? logictraffic "Aussage in LogicTaffic"
    Aussagen beschreiben überprüfbare Sachverhalte (z. B. „Ampel A grün bzw. Spur ist befahrbar.“ → Variable A=1). In LogicTraffic gelten Aussagen für Spuren und Ampeln: "Ampel B hat grün“ ist äquivalent zu "Spur B ist befahrbar" und werden in LogicTraffic kompakt als $B = 1$ wiedergegeben. Derartige Aussagen werden zu logischen Formeln verknüpft, um scihere Kruezungskonfigurationen zu modellieren [^10], [^11]. 
    ??? student "Beispiele für Aussagen aus LogicTraffic" 
        * Einfache Aussage: A = "Spur A hat grün" 
        * Zusdammengesetzte Aussage: $A \land \neg B$ => „Spur A hat grün UND Spur B hat rot.“ (verhindert Kollision).
        
    ??? teacher "Aussagen entdecken" 
       Schüler:innen experimentieren, indem sie Ampeln klicken und sehen, wie Aussagen in der Wahrheitstabelle wahr/falsch werden.
    
### Junktoren und Operatoren 
??? meta "Definition von Junktor" 
    **Junktor**: Ein Junktor (lat. *iungere* = verbinden) ist ein logisches Verknüpfungszeichen, das zwei oder mehr Aussagen zu einer neuen Aussage verbindet [^7]. 

    <!-- ich meine tatsächlich, dass eine Negation kein Junktor ist, schaue ich aber nochmals nach!-->



!!! teacher "Junktoren in der Unterrichtseinheit"
    In dieser UE werden drei grundlegende Junktoren behandelt:

    1. **Konjunktion** $\land$ (UND)
    2. **Disjunktion** $\lor$ (ODER, inkl. inklusiver Sinn)
    3. **Negation** $\neg$ (NICHT) – unärer Junktor

    Die Implikation $\rightarrow wird als abgeleiteter Operator eingeführt $\to \equiv \neg A \lor B$


???+ student "Junktoren für SuS"
    Junktoren sind wie **Bindewörter** in der Grammatik: ‚und‘, ‚oder‘, ‚nicht‘ verbinden Wörter zu Sätzen – hier verbinden sie Aussagen zu neuen Aussagen [^5].  

???+ student "Operatoren für SuS" 
    **Operatoren** in der Aussagenlogik sind die „Rechenzeichen“, die aus Eingabewerten (wahr/falsch) einen Ausgabewert erzeugen. Sie definieren boolesche Funktionen [^9] [^3]. 


    
**Operatoren-Tabelle** (für diese UE):

| Operator     | LaTeX       | Verbale Bedeutung | Logische Äquivalenz         |
|--------------|-------------|-------------------|-----------------------------|
| Negation     | `\(\neg A\)`| „nicht A“         | $\neg A$                  |
| Konjunktion  | `A \(\land\) B` | „A und B“     | $A \land B$               |
| Disjunktion  | `A \(\lor\) B` | „A oder B“    | $A \lor B$               |
| Implikation  | `A \(\to\) B`| „wenn A, dann B“ | $A \rightarrow B$           |

!!! error inline end "Typische Fehlvorstellungen"
    Gerade zu den Operatoren sind Fehlvorstellungen weit verbreitet [^6]. Es lohnt sich, diese zu kennen und im Unterricht auf sie zu achten. Die üblichen Fehlvorstellungen können hier nachgelesen werden: [Fehlvorstellungen :material-alert-decagram:](difficulties.md)

Die Wahrheitstabellen der Operatoren in dieser Unterrichtseinheit stellen sich folgendermassen dar: 

#### Negation NOT
In der boolschen Algebra ist NICHT eine Grundverknüpfung bei der der Ausdruck den Wahrheitswert umkehrt. Die Wahrheitstabelle fasst hier alle möglichen Kombinationen zusammen [^13]: 

| $A$ | $\neg A$ |
|----|----|
|1|0|
|0|1|

#### Konjunktion AND
Die Konjunktion ist die UND-Verknüpfung. Sie ist genau dann wahr, wenn beide Teilaussagen A und B wahr sind. Sie ist also falsch, wenn nur eine der beiden Aussagen falsch ist. Hier die Wahrheitstabelle dazu [^13]: 

| $A$ | $B$ | $A \land B$ | 
|------|------|-------|
|1|1|1|
|1|0|0|
|0|1|0|
|0|0|0|

#### Diskunktion OR 
Die Disjunktion ist die einschliessende ODER-Verknüpfung. Sie ist, anders als die Konjunktion, wahr sobald einer der Aussagen (A oder B) wahr ist. Sie ist nur falsch, wenn beide Aussagen falsch sind. Dies zeigt auch die zugehörige Wahrheitstabelle [^13]: 

| $A$ | $B$ | $A \lor B$ |
|-----|----|------|
|1|1|1|
|1|0|1|
|0|1|1|
|0|0|0|

#### Implikation 
!!! meta "Implikation und Umgangssprache"
     Die Implikation ist die Verknüpfung, die sich am weitesten von der umgangssprachlichen Logik entfernt. Deshalb ist die umgangssprachliche Übersetzung der Implikation in die Formulierung „Aus A folgt B“ mit Vorsicht anzuwenden da dies nicht immer korrekt ist und impliziert, dass die beiden Teilaussagen gleichberechtigt sind, was bei der Implikation nicht mehr der Fall ist [^13]. 
     Empfohlen wird zum Beispiel die Formulierung: "A impliziert B" oder "A ist hinreichend für B" sowie "B ist notwendig für A"

!!! student "Begrifflichkeiten" 
    Damit die Implikation von Schüler:innen einfacher verstanden werden kann, lohnt es sich, die Begrifflichkeiten der Voraussetzung und der Schlussfolgerung einzuführen. Dabei wird die links vom Junktor stehende Aussage Voraussetzung und die rechtsstehende Schlussfolgerung genannt. 

 Eine Aussage A ⇒ B ist nur dann falsch, wenn A wahr und B falsch ist. Wenn man von einer falschen Voraussetzung A ausgeht und eine wahre Schlussfolgerung B hervorbringt, gilt die Implikation immer noch als richtig. Übersichtlicher wird diese Logik in der zugehörigen Wahrheitstabelle: 

| $A$ | $B$ | $A \Rightarrow B$| 
|----|----|------|
|1|1|1|
|0|1|1|
|1|0|0|
|0|0|1|

## Darstellung der Situationen in LogicTraffic 
Logische Funktionen lassen sich ikonisch (bildlich), symbolisch (Formel, Wahrheitstabelle) und verbal (natürliche Sprache) darstellen. LogicTraffic nutzt alle Ebenen für einheitliche Verständnisentwicklung [^11].

!!! teacher "Didaktik des Darstellungswechsel
    **Darstellungswechsel** (enaktiv → ikonisch → symbolisch): Detaillierte Unterrichtstipps siehe [Darstellungswechsel](darstellungswechsel.md).

### Symbolische Darstellungen in LogicTraffic 

#### Wahrheitstabellen 
???+ student "Definition Wahrheitstabelle"
    Eine **Wahrheitstabelle** listet für alle $2^n$ Eingabekombinationen $n$ Variablen den Ausgabewert einer booleschen Funktion auf [^2], [^8]. 
    
!!! teacher "Wahrheitstabellen im Unterricht"
    Zwischenschritt ikonisch ↔ symbolisch: Anleitung und Übungen siehe [Wahrheitstabellen](wahrheitstabellen.md).

#### Formeln 
???+ student "Definition boolesche (Aussagen-)Funktion"
    Eine boolesche (Aussagen‑)Funktion ordnet jeder Kombination von Eingabewahrheitswerten (z.B. A, B) genau einen Ausgabewert (0 oder 1) zu [^7].

!!! teacher "Normalformeln"
    Auf der folgenden Seite werden behandelten Normalformeln, ihre Herleitung und Anwendung in LogicTraffic nochmals genau erklärt: [Normalformen :material-link-circle:](normalformen.md)

[^1]: Hoffmann, A., Marx, B., & Vogt, W. (2005). _Mathematik für Ingenieure 1: Lineare Algebra, Analysis - Theorie und Numerik_. Pearson Deutschland.
[^2]:Junker, M. (2025). _Logik für die Informatik: Eine Einführung in die Aussagenlogik, Prädikatenlogik und Berechenbarkeitstheorie_. Springer Berlin Heidelberg. [https://doi.org/10.1007/978-3-662-70825-5](https://doi.org/10.1007/978-3-662-70825-5)
[^3]: Kreuzer, M., & Kühling, S. (2014). _Logik für Informatiker_. Pearson Deutschland. [https://elibrary.pearson.de/book/99.150005/9783863267391](https://elibrary.pearson.de/book/99.150005/9783863267391)
[^5]: Staab, F. (2012). _Logik und Algebra: Eine praxisbezogene Einführung für Informatiker und Wirtschaftsinformatiker_ (2. Aufl). De Gruyter. [https://doi.org/10.1524/9783486717532](https://doi.org/10.1524/9783486717532)
[^6]: Herman, G. L., Loui, M. C., Kaczmarczyk, L., & Zilles, C. (2012). Describing the What and Why of Students’ Difficulties in Boolean Logic. ACM Transactions on Computing Education, 12(1), 1–28. https://doi.org/10.1145/2133797.2133800
[^7]: Boolesche Funktionen und ihre Normalformen. (2021, Juni 22). https://lehrerfortbildung-bw.de/u_matnatech/imp/gym/bp2016/fb2/m02_aug/1_hintergrund/4_grund/06_funktionen/
[^8]: Wahrheitstafeln—Theoretisches Material. Mathematik, 6. Schulstufe. (o. J.). Abgerufen 17. März 2026, von https://www.yaclass.at/p/mathematik/6-schulstufe/mengen-und-mengenoperationen-17080/aussagen-und-mengen-17463/re-519f4254-a9a1-457b-aa7e-38b6386d9b1c
[^9]: Hintergrund. (2021, Juni 22). https://lehrerfortbildung-bw.de/u_matnatech/imp/gym/bp2016/fb2/m02_aug/1_hintergrund/4_grund/
[^10]: Leitprogramm LogicTraffic [BZZ - Modulwiki]. (o. J.). Abgerufen 17. März 2026, von https://wiki.bzz.ch/modul/mathe/ma1/thema/lu04logik/aufgaben/leitprogramm/start
[^11]: Arnold, R., & Hartmann, W. (2007). LogicTraffic – Logik in der Allgemeinbildung. Informatik-Spektrum, 30(1), 19–26. https://doi.org/10.1007/s00287-006-0123-7
[^12]: Arnold, R., Amstalden, B., & Bader, J. (2022). Enhancing the Role of Computational Thinking in Primary and Secondary Education in Switzerland. Proceedings of the 17th Workshop in Primary and Secondary Computing Education, 1–2. https://doi.org/10.1145/3556787.3556874
[^13]: https://de.wikiversity.org/wiki/Aussagenlogik/Elementare_Einf%C3%BChrung/Textabschnitt 
