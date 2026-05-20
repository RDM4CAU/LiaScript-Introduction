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
-->

# LiaScript Vision

## Vision

     {{0-3}}
******************

> Lehrende möchten motivierende, interaktive Lehrmaterialien mit einem überschaubaren Aufwand realisieren, die optimal auf die eigenen didaktischen Ziele abgestimmt sind.

******************

    {{1-3}}
******************

> Das kann er/sie natürlich alleine realisieren, aber ...

---------------------

******************

    {{2-3}}
******************

**1. Muss er/sie sich über alle Inhalte selbst Gedanken machen**

**2. Muss er/sie sich erheblichen technischen Herausforderungen stellen**

---------------------

******************

{{3-4}}
**********************

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

**********************


## OER

{{0-1}}
>  **Open Courseware / Open Educational Resources** ... teaching, learning and
> research materials in any medium, digital or otherwise,that reside in the
> **public domain** or have been released under an open license that permits
> no-cost access, use, **adaptation** and **redistribution** by others with no or 4
> limited restrictions. Open licensing is built within the existing framework of
> intellectual property rights as defined by relevant international conventions
> and respects the authorship of the work
>
> -- UNESCO 2002 Forum on the Impact of Open Courseware for Higher Education in Developing Countries [(Link)](https://unesdoc.unesco.org/ark:/48223/pf0000128515)


{{1-2}}
******************

| Anforderung                  | Bedeutung                                  |
| ---------------------------- | ------------------------------------------ |
| `verwahren/vervielfältigen` | Download, Speicherung und Vervielfältigung |
| `verwenden`                  | Nutzung im Lernkontext                     |
| `verarbeiten`                | Umgestaltung und Adaption                  |
| `vermischen`                 | Kombination und Extraktion                 |
| `verbreiten`                 | (digitale) Publikation                     |

*_5 V-Freiheiten für Offenheit_ von Jöran Muuß-Merholz und Jörg Lohrer für [open-educational-ressources](https://open-educational-resources.de) - Transferstelle für OER*

******************

{{2-4}}
*********************

__Kritik an der 5V Definiotion__

> _1. Die 5V Definition fokussiert das Open in OER lässt aber das Education beiseite._
>
> _2. Die Verwaltung und Auffindbarkeit von OER Inhalten ist dadurch nicht erfasst._

**********************
    
## Bisherige Praxis

In der Praxis treffen wir oft auf statische, nicht-interaktive und schwer veränderbare Lehr- und Lernmaterialien:

![PDF](https://upload.wikimedia.org/wikipedia/commons/8/87/PDF_file_icon.svg "Adobe SystemsCMetalCore, Public domain, via Wikimedia Commons") ![Prezi](https://upload.wikimedia.org/wikipedia/commons/b/b4/Prezi_logo_transparent_2012.svg "Prezi Inc., CC BY-SA 3.0 <https://creativecommons.org/licenses/by-sa/3.0>, via Wikimedia Commons") ![Powerpoint](https://upload.wikimedia.org/wikipedia/commons/1/16/Microsoft_PowerPoint_2013-2019_logo.svg?utm_source=commons.wikimedia.org&utm_campaign=index&utm_content=original "Microsoft, Public domain, via Wikimedia Commons")

## Anforderungen an OER-Materialien

{{1-3}}
*********************

Um die OER Anforderungen umzusetzen, werden folgende Anforderungen an Lehr- und Lernmaterialien gestellt.

> 1. Materialien müssen rechtssicher nutz- und transformierbar sein, um eine Wiederverwendung zu ermöglichen. (_Verarbeiten/Verwenden/Verbreiten_)
> 2. Materialien brauchen Metadaten, um auffindbar zu sein. (_Verbreiten_)
> 3. Materialien brauchen offenkundige Versionierungen (_Verwalten_)

*********************

{{2-3}}
__Offensichtlich brauchen wir Formate, die neben den positiven Aspekten von Textdarstellungen auch das erweiterte Set von Anforderungen abdecken.__

## LiaScript

{{1-2}}
**********************
LiaScript ist eine offene Erweiterung der Auszeichnungssprache [Markdown](https://de.wikipedia.org/wiki/Markdown) und eine JavaScript-basierte Laufzeitumgebung zur Erstellung interaktiver, offener und interoperabler Bildungsinhalte.

- GitHub Flavored Markdown, erweitert um Funktionen, die einen erweiterten Einsatz von Multimedia sowie verschiedene Interaktionen mit Nutzenden ermöglichen.

- LiaScript soll auch Nutzer:innen ohne oder mit nur geringen Programmierkenntnissen die Entwicklung von Online-Kursen und offenen Bildungsressourcen (OER) ermöglichen.

- LiaScripte lassen sich serverlos im Netz verbreiten.

- LiaScript-Dokumente sind reine Textdokumente, deren Inhalt auch von einfachsten Texteditoren gelesen werden können. :-)

**********************

{{2-4}}
**********************

LiaScript erfüllt die oben genannten Anforderungen:

> 1. Materialien müssen transformierbar sein, um eine Wiederverwendung zu ermöglichen. (_Verarbeiten/Verwenden/Verbreiten_) --> LiaScript kann in andere Formate wie PDF, Docx, HTML, SCORM u.v.m konvertiert werden
> 2. Materialien brauchen Metadaten, um auffindbar zu sein. (_Verbreiten_) --> LiaScript kann einen Metadatenblock am Anfang jedes Dokuments enthalten, der es auffindbar macht
> 3. Materialien brauchen offenkundige Versionierungen (_Verwalten_) --> LiaScript ist als einfaches Textformat über Git lückenlos versionierbar

**********************

{{3-4}}
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