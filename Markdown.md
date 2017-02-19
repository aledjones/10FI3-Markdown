###Markdown

####Gliederung

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

5. Quellen


---

### 1. Markdown, eine universelle Sprache

##### 1.1 Was ist Markdown?

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

---

### 2. Syntax

##### 2.1 Einfache Formatierung

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

Weiter geht es mit Links und Images:

Code:

    [Ein Beispiel](http://www.google.de/ "Titel, der beim Überfahren mit der Maus angezeigt wird")
    
    allgemeine Syntax:

    ![Alternativtext](Bild-URL "Bildtitel hier")

    konkretes Beispiel:
    ![nur ein Beispiel](https://i.ytimg.com/vi/Zwtqvi0SttE/maxresdefault.jpg "Wütend?")
    
    Here's our logo (hover to see the title text):

    Inline-style: 
    ![alt text](http://centreinfection.s3.amazonaws.com/wp/sites/2/2015/03/13121802/generic-logo.jpg "Logo Title Text 1")

    Reference-style: 
    ![alt text][logo]

    [logo]: http://centreinfection.s3.amazonaws.com/wp/sites/2/2015/03/13121802/generic-logo.jpg "Logo Title Text 2"
    
Darstellung:

[Ein Beispiel](http://www.google.de/ "Titel, der beim Überfahren mit der Maus angezeigt wird")

allgemeine Syntax:

![Alternativtext](Bild-URL "Bildtitel hier")

konkretes Beispiel:
![nur ein Beispiel](https://i.ytimg.com/vi/Zwtqvi0SttE/maxresdefault.jpg "FFFFFFFFFFFFFFUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUU")

Here's our logo (hover to see the title text):

Inline-style: 
![alt text](http://centreinfection.s3.amazonaws.com/wp/sites/2/2015/03/13121802/generic-logo.jpg "Generisches Logo, yo")

Reference-style: 
![alt text][logo]

[logo]: http://centreinfection.s3.amazonaws.com/wp/sites/2/2015/03/13121802/generic-logo.jpg "Nochmal der gleiche Rotz, yo"

Mithilfe von folgender Syntax `:EMOJICODE:` kann man Emojis in Markdown hinzufügen.

Code:

    :shit:
    
Darstellung:

:shit:

Für mehr Syntaxen [hier](http://www.webpagefx.com/tools/emoji-cheat-sheet/ "Emojis") klicken.

##### 2.2 Komplexe Formartierung 

Eine Möglichkeit der Verwendung von einfachen Codeblöcken haben wir ja schon kennengelernt. Markdown bietet aber auch die Möglichkeit, Syntax-Highlighting für (fast) alle gängigen Programmiersprachen in Codeblöcken zu verwenden.
Hierzu müssen wir den Codeblock zunächst mit der noch nicht behandelten Methode mit je drei führenden und folgenden Backticks schreiben:

    ```
    'Dies ist ein Kommentar
    dim example as string = "Dies ist Beispielcode"
    example = "Dies ebenfalls"
    
    if example = "Dies auch" then
      dim i as integer = 1
      return i
    else
      dim i as integer = 1337
      return i
    end if
    ```
Dies gibt uns folgenden Codeblock:
```
'Dies ist ein Kommentar
dim example as string = "Dies ist Beispielcode"
example = "Dies ebenfalls"

if example = "Dies auch" then
  dim i as integer = 1
  return i
else
  dim i as integer = 1337
  return i
end if
```
Um nun Syntax-highlighting hinzuzufügen müssen wir hinter die ersten drei Backticks noch das Kürzel der entsprechenden Sprache (in diesem Fall `vbnet` für **VisualBasic.NET**) schreiben:

    ```vbnet
    'Dies ist ein Kommentar
    dim example as string = "Dies ist Beispielcode"
    example = "Dies ebenfalls"
    
    if example = "Dies auch" then
      dim i as integer = 1
      return i
    else
      dim i as integer = 1337
      return i
    end if
    ```
Was in diesen Codeblock resultiert:
```vbnet
'Dies ist ein Kommentar
dim example as string = "Dies ist Beispielcode"
example = "Dies ebenfalls"

if example = "Dies auch" then
  dim i as integer = 1
  return i
else
  dim i as integer = 1337
  return i
end if
```
Eine Liste mit Kürzeln unterstützter Programmiersprachen findet man beispielsweise [hier](http://tinker.kotaweaver.com/blog/?p=152 "Dies ist eine Liste. Ist eh egal was ich hier reinschreibe weil man das auf der .pdf eh nicht mehr sieht, also fuck that shit")

Weiterhin ist es auch möglich, Code innerhalb einer Zeile anzeigen zu lassen, sogennanten **Inline-Code**.
Hierzu umfasst man den gewünschten Text einfach mit einfachen Backticks:

    Dies ist ein `Beispiel` welches die Verwendung verdeutlicht.
Resultiert in:

Dies ist ein `Beispiel` welches die Verwendung verdeutlicht.

Man kann in Markdown, zwar nicht so leicht wie in anderen Sprachen Tabellen einfügen, aber es ist möglich. Und zwar folgender Maßen:

    |   |   |   |   |   |
    |---|---|---|---|---|
    |   |   |   |   |   |
    |   |   |   |   |   |
    |   |   |   |   |   |

Die herauskommende Tabelle sieht folgendermaßen aus:

|   |   |   |   |   |
|---|---|---|---|---|
|   |   |   |   |   |
|   |   |   |   |   |
|   |   |   |   |   |


##### 2.3 Bitmap-Support

Der Bitmap-Support in Markdown ist sehr hoch. Die einzigste vorraussetzung ist, dass das Bild eine Internet Adresse hat. So wie dieses:

Code:

    ![Google logo](http://www.google.com/images/logo.gif "Das Google logo")

Darstellung: 

![Google logo](http://www.google.com/images/logo.gif "Das Google logo")

Anhand dieses Beispieles ist sehr gut zu zeigen, dass mithilfe von Markdown sehr gut Bilder darzustellen sind. 
Die Syntax ist außerdem in *2.1 Einfache Formatierung* zu sehen

##### 2.4 Unterschiede zu gängigen Textverarbeitungen  

**Markdown** vs *Word*

Wenn man ein Word Dokument ohne hineinzuschreiben, ist es trotz allem ca 25 kB groß, da es Dokumenteigenschaften, Änderungen am Dokument (Schnellspeicherung), Datenspuren bei der Nutzung erweiterter Funktionen, Überarbeitungen, Kommentare, E-Mail-Header (Betreff, Adressaten), E-Mail-Verteiler für die Überarbeitung des Dokuments ("Laufzettel", routing slip), verschiedene Dateiversionen, Text- und Bildinhalte, die der Benutzer selbst "versteckt“, nicht sichtbare Teile von eingefügten Objekten (Tabellen, Diagramme, Bilder), ausgeblendeter Text, versteckter Text (durch geeignete Text-/Hintergrundfarbe oder farbigen Balken), Netzwerk und Computer Details, den Speicherort des Dokuments (inkl. Netzwerkpfad – falls vorhanden), auf welchem Drucker das Dokument zuletzt ausgedruckt wurd usw.     
Bei Markdown hingegen ist alles aus Text bzw einigen simplen Formatierungsbefehlen, außerdem ist die Syntax sehr einfach und schnell zu lernen. Man kann den geschriebenen Text leicht in andere Sprachen umwandeln. 
Derzeit findet in den USA ein regelrechter Markdown-Boom statt. Immer mehr kleinere Textverarbeitungen nutzen Markdown. Der Erfolg ist vor allem der neuen Mobilität geschuldet: Statt großer Datenmengen werden kleine Textschnipsel in Sekundenschnelle für alle Systeme synchronisiert – so bleiben Dokumente immer und überall aktuell, sei es auf dem Smartphone oder im Büro.
Für Layouts, Serienbriefe oder Magazine ist diese Form der Textbearbeitung jedoch keinesfalls geeignet; dazu sind die Formatierungsmöglichkeiten viel zu schmalbrüstig. Mit Stylesheets lassen sich die Formatierungen jedoch noch erweitern. 

**Fazit**: Sollte das Textverarbeitungprogramm Ihrer Wahl Markdown beherrschen, lohnt sich ein Blick darauf. 

===

**Markdown** vs *LaTeX*

Da nicht jeder gleich weiß was LaTeX ist, [hier](https://www.dante.de/tex/WasIstLaTeX.html) eine kleine Einführung.

LaTeX hat einige Vorteile gegenüber Markdown. Hier sind einige:

* man kann Druckdaten in Postscript oder PDF in einer sehr guten Layout- und Satzqualität erzeugen
* feste Layoutvorgaben von der Universität, dem Lehrstuhl, der Konferenz oder dem Journal (in bestimmten Bereichen auch Vorlagen)
* Einbinden von Literaturverweisen ist dank Bibtex/biblatex sehr flexibel
* man kann alles an Struktur und Layout umsetzen

wie schon häufiger erwähnt ist Markdown eine gut und schnell lernbare Sprache mit vielen Vorzügen. Sie besteht eigentlich nicht aus mehr außer Text.
Man kann relativ leicht Markdown Dokumente in LaTeX verwandeln, andersherum ist es um einiges schwieriger.

**Fazit**: Man solte in Markdown anfangen, kann aber sehr leicht auf LaTeX umteigen.


An den obigen Beispielen sieht man, dass Markdown eine sehr einfache und gute Markup-Sprache ist. Sie ist leicht zu lernen und zu verstehen. Außerdem kann man über die Sprache gut auf andere umsteigen bzw ein Dokument in eine andere Sprache verwandeln.

---

### 3. Einsatzgebiete

##### 3.1 Dokumentation von Code

Die Dokumentation von Code ist in Markdown sehr simpel. Man nutzt den sogenannten Codeblock. Die Syntax haben wir schon einmal unter *2.2 Komplexe Formatierung* erwähnt, sowie der Inline-Code und das Syntax-Highlighting von verschiedestens Sprachen (z.B. vbnet).
Hier ist noch mal der Link zur [Liste](http://tinker.kotaweaver.com/blog/?p=152 "Dies ist eine Liste. Ist eh egal was ich hier reinschreibe weil man das auf der .pdf eh nicht mehr sieht, also fuck that shit"), welche die verschiedenen Sprachen aufzählt.


##### 3.2 Simple Textverarbeitung  

Dieses Thema werden wir anhand eines Texeditors, in diesem Fall **Write!** erklären. Write! ist dabei allerdings nicht nur ein klassischer Markdown-Editor, sondern kann mit einigen Funktionen punkten, die teilweise recht untypisch in diesem Gebiet sind ,hier sind einige Beispiele  Wortkorrektur, automatische Wortvervollständigung und Rich-Text-Formatierungen (mitsamt Textfarben). Neben Markdown unterstützt Write! dazu mit Textile auch ein Wiki-ähnliches Markup, insofern hat man im Bezug auf die Texterstellung also eine schöne Auswahl an Auszeichnungssprachen. 
Weiteres über Textverarbeitung kann man [hier](http://appspezis.de/tag/textverarbeitung/) herausfinden.


---

### 5. Quellen

1. [Markdown Wikipedia](https://de.wikipedia.org/wiki/Markdown "Quelle")
2. [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet "Quelle")  
5. [Markdown Tabellen](http://www.tablesgenerator.com/markdown_tables)
3. [Markdown vs Word](http://www.chip.de/artikel/Alternativen-zu-Microsoft-Word-6_62389509.html)  
4. [Markdown vs LaTeX](https://www.schlosser.info/markdown-latex/)  
5. [Markdown Textverarbeitung](http://appspezis.de/write-windows/)
6. 
