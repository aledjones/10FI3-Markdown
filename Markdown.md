##Markdown

###Gliederung

1. Markdown, eine universelle Sprache   
1.1 Was ist Markdown?  
1.2 Vor- und Nachteile  

2. Syntax  
2.1 Einfache Formatierung  
2.2 Komplexe Formartierung  
2.3 Bitmap-Support  
2.4 Unterschiede zu gängigen Textverarbeitungen  

3. Einsatzgebiete  
3.1 Dokumentation von Code  
3.2 Simple Textverarbeitung  
3.3 Spezielle Einsatzgebiete  

4. Trivia

5. Quellen


---

## 1. Markdown, eine universelle Sprache

1.1 Was ist Markdown?

Markdown ist eine so genannte Markup-Language, eine Textsprache zur Notation von Textdokumenten in einem universell lesbarem Standard.
Markdown wurde mit dem Ziel entwickelt, selbst im blanken Code-Zustand eine lesbare Syntax präsentieren zu können.
Die geschrieben Dateien können von Programmen in jede erdenkliche Form umgesetzt werden, sei es HTML, PDF oder ePub-Formate. Man kann also sagen, dass Markdown zur späteren Anzeige "kompiliert" werden kann.
Vornehmlich wird Markdown in einem Umfeld eingesetzt, in dem die Arbeitsumgebung zur Dokumentation der Arbeit nicht gewechselt werden möchte. (Programmierung)

1.2 Vor- und Nachteile

Für Markdown werden nahezu keinerlei Vorkenntnisse benötigt. Zum erstellen eines ersten Markdown-Textes kann man einfach drauf los schreiben. Die Umsetzung übernimmt ein Parser, den man in den meisten Fällen ganz nach seinen Wünschen anpassen kann.
Markdown setzt komplett auf Textzeichen auf, die in der ASCII-Zeichentabelle zu finden sind. Da heißt, dass auch auf Systemen, die nicht mit Umlauten zurecht kommen, Markdown zum einsatz kommen kann. Umlaute werden selbstverständlich auch unterstützt. Die Syntax der Formatierung in Markdown besteht zumeist aus Leerzeichen und Abständen, was für Anfänger leicht verständlich ist, jedoch bei komplexeren Dokumenten zu Problemen führen kann.
Die Formatierung der Elemente ist Kontext-abhängig. Somit ist es zum Beispiel nicht möglich, einen Codeblock in eine Tabelle zu integrieren, da die Meisten Programme zur Umsetzung nicht damit zurecht kommen und die Syntax dies nicht vorsieht.
Ein weitere Nachteil ist, dass die letzte Vollversion der Software aus dem Jahr 2004 stammt. Um Markdown trotz dessen in der modernen Zeit einsetzen zu können, sind zahlreiche Dialekte der Sprache entstanden, die alle unterschiedliche Syntax enthalten können und sich von Version zu Version in ihrer Umsetzung unterscheiden.
Markdown wurde mit dem Ziel entwickelt, selbst im blanken Code-Zustand eine lesbare Syntax zu repräsentieren. 



##2. Syntax

2.1 Einfache Formatierung

In diesem Abschnitt wird als erstes ein Code-Block gezeigt und danach wie es aussieht, wenn man ihn in einem Markdown-Parser ausführt.   
Ein Code-Block wird hinzugefügt, indem man vor die entsprechende Zeile 4 Leerzeichen setzt.    
Zeilenumbrüche macht man sehr ähnlich mit 2 Leerzeilen am Ende einer Zeile.  


Fangen wir mit ein paar Grundlagen an:

Code:  
  
    *Kursiv*, **Fett** und ***Fett kursiv*** bzw. 
    _Kursiv_, __Fett__ und ___Fett kursiv___
    ~~Scratch this.~~

Darstellung:  
*Kursiv*, **Fett** und ***Fett kursiv*** bzw. _Kursiv_, __Fett__ und ___Fett kursiv___  
~~Scratch this.~~

Hier werden Aufzählungen, Pragraphen und Stichpunkte gezeigt:  

Code:  

    * Ein Punkt in einer ungeordneten Liste
    + Ein weiterer Punkt in einer ungeordneten Liste
        * Ein Unterpunkt, um vier Leerzeichen eingerückt
    - Statt * funktionieren auch + oder -
    
    1. Ein Punkt in einer geordneten Liste
    2. Ein weiterer Punkt; bei der Eingabe muss nicht auf irgendeine Reihenfolge geachtet werden, sondern nur darauf, dass es beliebige Ziffern sind
    1. Noch ein Punkt, der zeigt, dass auch die mehrfache Angabe derselben Ziffer möglich ist
    
Darstellung:  

* Ein Punkt in einer ungeordneten Liste
+ Ein weiterer Punkt in einer ungeordneten Liste
    * Ein Unterpunkt, um vier Leerzeichen eingerückt
- Statt * funktionieren auch + oder -  

1. Ein Punkt in einer geordneten Liste
2. Ein weiterer Punkt; bei der Eingabe muss nicht auf irgendeine Reihenfolge geachtet werden, sondern nur darauf, dass es beliebige Ziffern sind
1. Noch ein Punkt, der zeigt, dass auch die mehrfache Angabe derselben Ziffer möglich ist

Machen wir mit Überschriften in den verschiedenen Ebenen weiter:

Code:  

    # Überschrift in Ebene 1
    ## Überschrift in Ebene 2
    ### Überschrift in Ebene 3 
    #### Überschrift in Ebene 4   
    ##### Überschrift in Ebene 5 ist die kleinste Ebene  
    
    Für die ersten 2 Ebenen gibt es alternative Schreibweisen:
    Überschrift in Ebene 1
    ======================
    Überschrift in Ebene 2
    ----------------------
Darstellung:

# Überschrift in Ebene 1
## Überschrift in Ebene 2
### Überschrift in Ebene 3 
#### Überschrift in Ebene 4
##### Überschrift in Ebene 5 ist die kleinste Ebene

Für die ersten 2 Ebenen gibt es alternative Schreibweisen:
Überschrift in Ebene 1
======================
Überschrift in Ebene 2
----------------------
