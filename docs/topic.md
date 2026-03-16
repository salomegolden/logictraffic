# Zur Sache 

## Grundlagen der Aussagelogik im Kontext von Logic Traffic 
In der Aussagelogik arbeiten wir mit Aussagen, denen eindeutig ein Wahrheitswert (_true_ oder _false_) zugeordnet werden kann. Für die informatische Umsetzung in Logic Traffic abstrahieren wir die Zustände der Ampelanlage (rot oder grün) auf binäre Werte. Wir arbeiten damit mit Aussagen wie "die Ampel ist grün". Dieser Satz kann nur **wahr** oder **falsch** sein – nichts dazwischen. Durch logische Operatoren wie UND, ODER oder NICHT lassen sich solche Aussagen kombinieren. 

??? logictraffic "Aussagelogik und Logictraffic"
    LogicTraffic nutzt Aussagenlogik, um Ampelzustände an Kreuzungen formal darzustellen. Jede Ampel wird durch eine Variable (A, B, C, …) repräsentiert, und jede Formel beschreibt, wann eine Ampel Grün ist. Durch Aussagenlogik lassen sich sichere oder unsichere Kreuzungssituationen beschreiben.

### Variablen und Zustände 
Eine boolsche Variable ist in der Informatik die kleinste Informationseinheit. Sie trägt genau eine Information, die entweder zutrifft oder eben nicht.

!!! logictraffic "Variable in LogicTraffic"
    In LogicTraffic steht jede Variable für den Zustand einer Ampel (rot $0$  / grün $1$).

### Aussagen 
eine **Aussage** wird durch drei Eigenschaften beschrieben [^1]: (1) eine Aussage ist eine sprachliche Einheit, die einen Sachverhalt ausdrückt. (2) Eine Aussage ist entweder _wahr_ (Wahrheitswert $1$) oder _falsch_ (Wahrheitswert $0$). (3) Welche Sprache den Sachverhalt beschreibt ist unerheblich. 

??? logictraffic "Aussage in LogicTaffic"
    
    Im Kontext von LogicTraffic beschreibt eine Aussage einen Sachverhalt (Zustand der Ampeln) den man überprüfen kann: "Ampel A hat grün". Solche Sätze werden im Modell in logische Ausdrücke übersetzt, die man dann mit Operatoren verbinden kann. In LogicTraffic repräsentiert jede Variable eine Aussage über den Zustand einer Ampel.

??? student inline "Beispiele für Aussagen"
    
    Beispiele für Aussagen:
    - Die Ampel A ist grün.
    - Auto fährt von Norden.
    - Auto darf nach rechts abbiegen.

### Junktoren und Operatoren 
Junktor = Ein Junktor (von lat. iungere = verbinden) ist ein logisches Verknüpfungszeichen, das zwei Aussagen zu einer neuen Aussage verbindet. Es gibt 3 Junktoren die in dieser Unterrichtseinheit behandelt werden:
1. logisches UND $\land$
2. logisches ODER $\lor$
3. Negation / Verneinung $\neg$
Durch Verknüpfung resp. Verneinung von Aussagen entstehen wiederum neue Aussagen.

??? student "Erklärung für Junktoren" 
    Als Erklärung für die Schülerinnen und Schüler kann folgende Analogie dienen: "_Junktoren funktionieren wie grammatikalische Bindewörter („und“, „oder“, „nicht“). Wir können Sprache so in eine formale Formel umwandeln._" 

!!! student "Operatoren - Definition" 
    Operator: In der Aussagenlogik sind Operatoren die „Rechenzeichen“ — sie definieren, wie aus gegebenen Werten (z. B. Ampel grün/rot) ein neuer Wert entsteht.

Hier findet sich eine Tabelle aller Operatoren, welche in den Aufgaben dieser Unterrichtsreihe verwendet werden: 

    | Operator    | LaTeX       | Verbale Bedeutung | Logische Form                   |
    | ----------- | ----------- | ----------------- | ------------------------------- |
    | Negation    | `\lnot A`   | A nicht           | $\lnot A$                       |
    | Konjunktion | `A \land B` | A und B           | $A \land B$                     |
    | Disjunktion | `A \lor B`  | A oder B          | $A \lor B$                      |
    | Implikation | `A \to B`   | wenn A, dann B    | $A \to B \equiv \lnot A \lor B$ |

!!! error inline "Typische Fehlvorstellungen"
    Gerade zu den Operatoren sind Fehlvorstellungen weit verbreitet [^6]. Es lohnt sich, diese zu kennen und im Unterricht auf sie zu achten. Die üblichen Fehlvorstellungen können hier nachgelesen werden: [Fehlvorstellungen :material-alert-decagram:](learninglogic.md)

## Darstellung der Situationen in LogicTraffic 
Logische Funktionen kann man auf unterschiedliche Arten darstellen wie z.B. Wahrheitstabellen, Normalformen und Parsebäume. In diesem Grundlagenunterricht mit LogicTraffic wird eine ikonische (bildliche) und symbolische (Formel & Wahrheitstabelle) sowie eine verbale (Ausformulierung durch Sprache) genauer beschrieben. 

!!! teacher "Didaktik des Darstellungswechsel
    Auf folgender Seite finden sich weitere Informationen zum Darstellungswechsel von enaktiver Darstellung über die ikonische zur symbolischen Darstellungsform: [Darstellungswechsel :material-circle-link:](topic/darstellungswechsel.md)

### Symbolische Darstellungen in LogicTraffic 

#### Wahrheitstabellen 
??? meta "Wahrheitstabelle"
    Eine tabellarische Darstellung einer logischen Funktion, die für jede mögliche Kombination von Eingangswerten (0 oder 1) den resultierenden Ausgangswert zeigt. Bei $n$ Variablen hat die Tabelle $2^{n}$ Zeilen [^2]. 

!!! teacher "Wahrheitstabellen im Unterricht" 
    Auf folgender Seite finden sich weitere Informationen wie man Wahrheitstabellen als Zwischenschritt zwischen ikonischer und symbolischer Darstellungsform im Unterricht nutzen kann: 
    [Wahrheitstabellen:material-link-circle:](topic/wahrheitstabellen.md){ .md-button }

    
#### Formeln 

!!! teacher "Normalformeln"
    Auf der folgenden Seite werden behandelten Normalformeln, ihre Herleitung und Anwendung in LogicTraffic nochmals genau erklärt: [Normalformeln :material-link-circle:](topic/normalformeln.md)


[^1]: Hoffmann, A., Marx, B., & Vogt, W. (2005). _Mathematik für Ingenieure 1: Lineare Algebra, Analysis - Theorie und Numerik_. Pearson Deutschland.

[^2]:Junker, M. (2025). _Logik für die Informatik: Eine Einführung in die Aussagenlogik, Prädikatenlogik und Berechenbarkeitstheorie_. Springer Berlin Heidelberg. [https://doi.org/10.1007/978-3-662-70825-5](https://doi.org/10.1007/978-3-662-70825-5)

[^3]: Kreuzer, M., & Kühling, S. (2014). _Logik für Informatiker_. Pearson Deutschland. [https://elibrary.pearson.de/book/99.150005/9783863267391](https://elibrary.pearson.de/book/99.150005/9783863267391)

[^4]: Reichardt, J. (2025). _Digitaltechnik und Digitale Systeme: Von der Booleschen-Algebra über VHDL zur High-Level Synthese_. De Gruyter. [https://doi.org/10.1515/9783111698977](https://doi.org/10.1515/9783111698977)

[^5]: Staab, F. (2012). _Logik und Algebra: Eine praxisbezogene Einführung für Informatiker und Wirtschaftsinformatiker_ (2. Aufl). De Gruyter. [https://doi.org/10.1524/9783486717532](https://doi.org/10.1524/9783486717532)
