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
3.3 Spezielle Einsatzgebiete  

4. Trivia

5. Quellen


---

### 1. Markdown, eine universelle Sprache

##### 1.1 Was ist Markdown?

Markdown ist eine so genannte Markup-Language, eine Textsprache zur Notation von Textdokumenten in einem universell lesbarem Standard.
Markdown wurde mit dem Ziel entwickelt, selbst im blanken Code-Zustand eine lesbare Syntax zu repräsentieren. 



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

Weitere Emojis sind [hier](http://www.webpagefx.com/tools/emoji-cheat-sheet/ "Emojis") zu finden.

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


### 3. Einsatzgebiete

##### 3.1 Dokumentation von Code




### 5. Quellen

1. [Markdown Wikipedia](https://de.wikipedia.org/wiki/Markdown "Quelle")
2. [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet "Quelle")  
3.
