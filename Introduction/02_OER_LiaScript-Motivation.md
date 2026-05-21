<!--
author: Richard Diebel, Britta Petersen
email: diebel@ub.uni-kiel.de, b.petersen@rz.uni-kiel.de
version: 0.2.0
date: 2026-05-20
link: https://raw.githubusercontent.com/RDM4CAU/Intro-to-RDM/refs/heads/main/cau-style.css
comment: Workshop Open Educational Resources mit LiaScript erstellen: Anforderungen an OER, Vision und Motivation von LiaScript.
language: de
narrator: Deutsch Female

mode:     Presentation

repository: https://github.com/RDM4CAU/LiaPlayground
icon: https://raw.githubusercontent.com/RDM4CAU/TtL-FDM/main/images/fdm_lehre.png

import:   https://raw.githubusercontent.com/LiaTemplates/LiveEdit-Embeddings/refs/tags/0.0.1/README.md
          https://raw.githubusercontent.com/liaTemplates/AVR8js/main/README.md

-->

# OER & LiaScript

<section class="flex-container">

<!-- class="flex-child" style="min-width: 250px;" -->
> <h4>Open Educational Resources und LiaScript</h4>

<!-- class="flex-child" style="min-width: 200px;" -->
![partner_map](https://raw.githubusercontent.com/LiaPlayground/LiaScript_Workshop_Lehrende_an_Schulen/main/pic/LiaScript_Meets_OER.png "OER-Logo - Quelle: Jonathas Mello, erweitert durch Sebastian Zug und André Dietrich, CC BY 3.0, [https://commons.wikimedia.org/w/index.php?curid=18460156](https://commons.wikimedia.org/w/index.php?curid=18460156) erweitert um LiaScript Logo")

</section>


## Ausgangspunkt

>  <!-- Style="color:green" -->__Lehrende möchten motivierende, interaktive, digitale Lehrmaterialien in ihren Unterricht einbetten.__

                  {{0-1}}
********************************************

---------------------

Beispiel Quizze:


- [[male (der)] (female [die]) [neuter (das)]]
- [    [X]           [ ]             [ ]     ]  Mann - German for man
- [    ( )           (X)             ( )     ]  Frau - German for woman

********************************************

                  {{1-2}}
********************************************

---------------------

Beispiel 3D-Modelle:

??[ear model](https://sketchfab.com/3d-models/familienschacht-freiberg-germany-7c7d30506c554385a4a4321366e2e601)


********************************************

                  {{2-3}}
********************************************

---------------------

Beispiel Simulationsumgebung:

<div>
  <wokwi-led color="red" pin="13" port="B" label="13"></wokwi-led>
  <span id="simulation-time"></span>
</div>
```cpp       arduino.cpp
// einmaliges Ausführen
void setup() {
  pinMode(13, OUTPUT);
}

// Endlosschleife
void loop() {
  digitalWrite(13, HIGH);
  delay(1000);
  digitalWrite(13, LOW);
  delay(1000);              
}
```
@AVR8js.sketch

********************************************

                  {{3-4}}
********************************************

__Aber ...__

+ Die individuelle Umsetzung ist aufwändig und zeitintensiv.
+ Für verschiedene Formate (z.B. Text, Video, Audio, 3D-Modelle) gibt es unterschiedliche Werkzeuge.
+ Bestehende Inhalte sind nicht auf die individuellen Bedürfnisse von Lehrenden und Lernenden zugeschnitten.
+ ...

> Welche weiteren Hemmnisse kennen Sie aus Ihrer Praxis?

********************************************

{{4}}
```ascii

      Wunsch nach                                             Wunsch nach
  einfacher Umsetzung  -----------> Konflikt <----------- spezifischen Elementen
                                                               im Material
                                                                                                   .
```

### OER als Lösungsansatz

           {{0-3}}
**************************************

<!--
style="width: 100%; max-width: 860px; display: block; margin-left: auto; margin-right: auto;"
-->
```ascii

      Wunsch nach                                             Wunsch nach
  einfacher Umsetzung  -----------> Konflikt <----------- spezifischen Elementen
                                       |                       im Material
                                       |
                                       v
                              OER als Lösungsansatz

```

> OER beschreibt die gemeinsame Entwicklung, Nutzung und Verbreitung von Lehr- und Lernmaterialien, die unter einer offenen Lizenz stehen.

************************************

           {{1-2}}
**************************************

>  **Open Courseware / Open Educational Resources** ... teaching, learning and
> research materials in any medium, digital or otherwise,that reside in the
> **public domain** or have been released under an open license that permits
> no-cost access, use, **adaptation** and **redistribution** by others with no or 4
> limited restrictions. Open licensing is built within the existing framework of
> intellectual property rights as defined by relevant international conventions
> and respects the authorship of the work
>
> -- UNESCO 2002 Forum on the Impact of Open Courseware for Higher Education in Developing Countries [(Link)](https://unesdoc.unesco.org/ark:/48223/pf0000128515)

**************************************

           {{2-3}}
**************************************

| Anforderung an OER Materialien | Bedeutung                                  |
| ------------------------------ | ------------------------------------------ |
| `verwahren/vervielfältigen `   | Download, Speicherung und Vervielfältigung |
| `verwenden`                    | Nutzung im Lernkontext                     |
| `verarbeiten`                  | Umgestaltung und Adaption                  |
| `vermischen`                   | Kombination und Extraktion                 |
| `verbreiten`                   | (digitale) Publikation                     |


*_5 V-Freiheiten für Offenheit_ von Jöran Muuß-Merholz und Jörg Lohrer für [open-educational-ressources](https://open-educational-resources.de) - Transferstelle für OER*

**************************************

### Kritik am OER-Ansatz


| Ebene                               | Kernaussage                                                                                  |
| ----------------------------------- | -------------------------------------------------------------------------------------------- |
| Emotionale Einordnung               | "_Da kann ja jeder meine Arbeit für sich nutzen!_"                                           |
|                                     | "_Da kann mich ja jeder kontrollieren!_"                                                     |
| Rechtliche Herausforderungen        | "_Ich verwende viele Grafiken, bei deren Urheberrecht ich mir im besten Fall unsicher bin!_" |
| Auffindbarkeit                      | "_Ich finde keine Inhalte, die ich in meiner Lehre gewinnbringend integrieren kann!_"        |
| <!-- Style="color:red" --> Aufwand  | <!-- Style="color:red" --> "_Da muss man ja Informatik studiert haben!_"                     |
| <!-- Style="color:red" -->Abdeckung | <!-- Style="color:red" -->"_Da fehlen mir aber die Schnittstellen für meine Tools XY!_"      |

### Idealer Prozess

<!--
style="width: 100%; max-width: 860px; display: block; margin-left: auto; margin-right: auto;"
-->
```ascii

Kurs.txt         Version 1.0          Kurs.txt          Version 1.1
+--------------------------+          +---------------------------+
| Kurs  Deutsche Literatur |          | Kurs  Deutsche Literatur  |
| Autor Peter Muster       | "Fehler" | Autoren Peter Muster      |
|                          |------>   |         Angelika Maier    |----->
|~~~~~~~~~~~~~~~~~~~~~~~~~~|          |~~~~~~~~~~~~~~~~~~~~~~~~~~~|
| Ab 1756 bereiste Goethe  |---.      | Ab 1786 bereiste Goethe   |--.
| Italien ...              |   |      | Italien ...               |  |
                               |                                     |    Course.txt       Version 1.1.2
                               |                                     |    +----------------------------+
                               |                                     |    | Kurs  German Literature    |
                               |                                     |    | Autoren Peter Muster       |
                               |                                     .--> |         Angelika Maier     |
                               |                                          |         Steve Gray         |
                               |                                          |~~~~~~~~~~~~~~~~~~~~~~~~~~~~|
                               |                                          | In 1786 Goethe traveled to |
                               |                                          | Italy ...                  |
                               |      Kurs.txt         Version 1.0
                               |      +---------------------------+
                               |      | Kurs  Goethes Welt        |
                               |      | Autoren Peter Muster      |
                               .-->   |         Angelika Maier    |----->
                                      |~~~~~~~~~~~~~~~~~~~~~~~~~~~|
                                      | Während der italienischen |
                                      | Reise ...                 |
```
*Versionen der Lehrinhalte eines Kurses und deren Wiederverwendung in anderen Veranstaltungen*

{{1}}
********************************************************************************

| Anforderung                  | txt | Begründung                                               |
| ---------------------------- | --- | -------------------------------------------------------- |
| `verwahren/vervielfältigen ` | ++  | vorteilhaft wegen geringer Größe                         |
| `verwenden`                  | +   | analoge / digitale Verteilung an Studieren unkompliziert |
| `verarbeiten`                | ++  | verarbeitbar ohne zusätzliche Software                   |
| `vermischen`                 | +   | einfache Kombination von Textfragmenten per Copy&Paste   |
| `verbreiten`                 | +   | gut exportierbar                                         |

> **Moment, ein reines Textdokument ist als OER Inhalt perfekt?**

********************************************************************************

## Bisherige Praxis

In der Praxis treffen wir oft auf statische, nicht-interaktive und schwer veränderbare Lehr- und Lernmaterialien:

![PDF](https://upload.wikimedia.org/wikipedia/commons/8/87/PDF_file_icon.svg "Adobe SystemsCMetalCore, Public domain, via Wikimedia Commons") ![Prezi](https://upload.wikimedia.org/wikipedia/commons/b/b4/Prezi_logo_transparent_2012.svg "Prezi Inc., CC BY-SA 3.0 <https://creativecommons.org/licenses/by-sa/3.0>, via Wikimedia Commons") ![Powerpoint](https://upload.wikimedia.org/wikipedia/commons/1/16/Microsoft_PowerPoint_2013-2019_logo.svg?utm_source=commons.wikimedia.org&utm_campaign=index&utm_content=original "Microsoft, Public domain, via Wikimedia Commons")

## LiaScript

{{0-1}}
**********************
>[LiaScript](https://liascript.github.io/) ist 
>
>- eine Open Source Erweiterung der Auszeichnungssprache [Markdown](https://de.wikipedia.org/wiki/Markdown) und
>
>- eine JavaScript-basierte Laufzeitumgebung zur Erstellung interaktiver, offener und interoperabler Bildungsinhalte.

- LiaScript erweitert Markdown um Funktionen, die einen erweiterten Einsatz von Multimedia sowie verschiedene Interaktionen mit Nutzenden ermöglichen.

- LiaScript möchte auch Nutzer:innen ohne oder mit nur geringen Programmierkenntnissen die Entwicklung von Online-Kursen und offenen Bildungsressourcen (OER) ermöglichen.

- LiaScripte lassen sich serverlos im Netz verbreiten.

- LiaScript-Dokumente sind reine Textdokumente, deren Inhalt auch von einfachsten Texteditoren gelesen werden können. :-)

**********************

{{1-2}}
**********************

LiaScript erfüllt die oben genannten Anforderungen an OER:

> 1. Materialien müssen transformierbar sein, um eine Wiederverwendung zu ermöglichen. (_Verarbeiten/Verwenden/Verbreiten_) --> LiaScript kann in andere Formate wie PDF, Docx, HTML, SCORM u.v.m konvertiert werden
> 2. Materialien brauchen Metadaten, um auffindbar zu sein. (_Verbreiten_) --> LiaScript kann einen Metadatenblock am Anfang jedes Dokuments enthalten, der es auffindbar macht
> 3. Materialien brauchen offenkundige Versionierungen (_Verwalten_) --> LiaScript ist als einfaches Textformat über Git lückenlos versionierbar LiaScript und erlaubt die Anwendung von Methoden der verteilten Softwareentwicklung

**********************

{{2}}
**********************
Und weitere:

> 1. Einfache Syntax (_Verarbeiten/Vermischen/Verbreiten_)
> 2. Serverloses Hosten (_Verbreiten_)
> 3. Multimedialität und Interaktivität durch Medien und interaktive Elemente  (_Education_)

**********************

## LiaScript Alternativen
LiaScript steht im Wettbewerb mit verschiedenen anderen Werkzeugen und Formaten zur Erstellung digitaler Lerninhalte:
[^1]
- H5P: H5P ist ein weit verbreitetes Open-Source-Framework für interaktive Inhalte mit breiter LMS-Integration und vielen vorgefertigten Inhaltstypen. LiaScript hingegen verfolgt einen stärker textbasierten und flexiblen Ansatz, der technisch versierteren Nutzerinnen und Nutzern mehr Freiheiten bei der Gestaltung interaktiver Lerninhalte bietet.

- Autorenwerkzeuge: Kommerzielle Autorenwerkzeuge wie Articulate Storyline bieten grafische Editoren und richten sich an professionelle E-Learning-Designer. LiaScript verfolgt einen textbasierten Ansatz, der vor allem technisch versierte Autoren anspricht und weniger visuelle Unterstützung bietet.

- andere Markdown-basierte Systeme: Es gibt verschiedene Markdown-basierte Alternativen, die (z. B. Jupyter Notebooks, Quarto), die ebenfalls interaktive Inhalte ermöglichen.

\
\
\
---

[^1] LiaScript. (o. D.). In Wikipedia. Abgerufen am 20. Mai 2026, von https://de.wikipedia.org/wiki/LiaScript


# Referenzen

Sebastian Zug, André Dietrich, Martin Lommatzsch, Matthias Saurbier, Thomas Schumann (n. d.): LiaScript Workshop Lehrende an Schulen. (n.d.). Motivation. LiaScript. https://liascript.github.io/course/?https://raw.githubusercontent.com/LiaPlayground/LiaScript_Workshop_Lehrende_an_Schulen/refs/heads/main/Motivation.md#1