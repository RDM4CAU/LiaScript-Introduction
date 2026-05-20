<!--
author:   IHR NAME
email:    ihre.mail@einrichtung.de
version:  0.1.0
language: de
narrator: Deutsch Female

comment:  Kurzbeschreibung Ihres Kurses (1-2 Sätze).

icon:     Link zu Ihrem Logo

import:   https://github.com/LiaTemplates/Pyodide
-->

[![LiaScript](https://raw.githubusercontent.com/LiaScript/LiaScript/master/badges/course.svg)](https://liascript.github.io/course/?<URL-ZU-DIESER-DATEI>)

# Titel Ihres Kurses

         --{{0}}--
Kurze Einleitung, die beim Öffnen automatisch vorgelesen wird. Ein bis zwei Sätze.

> **Auf einen Blick**
>
> - Was lernen Sie?
> - Für wen ist das gedacht?
> - Wie viel Zeit sollten Sie einplanen?

## Worum geht es?

         --{{0}}--
Hintergrund und Motivation. Warum ist dieses Thema für Ihre Zielgruppe relevant?

{{1}}
Ein zweiter Gedanke, der erst nach einem Klick erscheint.

{{2}}
Ein dritter.

# Baustein 1 — Inhalt

         --{{0}}--
Ein inhaltliches Kapitel. Hier erklären Sie die Sache.

## Text und Medien

         --{{0}}--
Normaler Markdown-Text funktioniert direkt. **Fett**, *kursiv*, `Code`.

Ein Bild aus einer freien Quelle:

![Beschreibung](https://upload.wikimedia.org/wikipedia/commons/thumb/7/7a/Bibliothek_Staedelschule.jpg/640px-Bibliothek_Staedelschule.jpg)

Ein eingebettetes Video:

!?[YouTube-Video](https://www.youtube.com/watch?v=VIDEO_ID)

## Eine Tabelle

         --{{0}}--
| Spalte A | Spalte B |
|----------|----------|
| Wert 1   | Wert 2   |
| Wert 3   | Wert 4   |

## Interaktives Code-Beispiel

         --{{0}}--
Dank des `import:` im Header läuft Python direkt im Browser:

```python
zahlen = [1, 2, 3, 4, 5]
print("Summe:", sum(zahlen))
print("Mittelwert:", sum(zahlen) / len(zahlen))
```
@Pyodide.eval

# Baustein 2 — Übung

         --{{0}}--
Interaktion ist das Herz von LiaScript. Hier einige typische Muster zum Kopieren.

## Single-Choice-Frage

         --{{0}}--
Welche der folgenden Aussagen trifft zu?

- [( )] Eine falsche Antwort.
- [(X)] Die richtige Antwort.
- [( )] Eine weitere falsche Antwort.
- [[?]] Ein Hinweis, den die Lernenden bei Bedarf aufklappen können.

## Multiple-Choice-Frage

         --{{0}}--
Was gehört zu guter OER-Praxis? (Mehrfachauswahl möglich)

- [[X]] Klare Lizenzangabe
- [[X]] Offenes Dateiformat
- [[ ]] Nur für den eigenen Gebrauch behalten
- [[X]] Versionierung

## Freitext-Frage

         --{{0}}--
Nennen Sie eine Situation aus Ihrem Alltag, in der dieses Wissen hilfreich wäre:

[[_______________________________________________________]]

## Zuordnungs-Übung

         --{{0}}--
Ordnen Sie den Begriff dem passenden Konzept zu:

- [[Autor|(Titel)|Jahr|Schlagwort]] "Einführung in X"
- [[Autor|Titel|(Jahr)|Schlagwort]] "2023"
- [[(Autor)|Titel|Jahr|Schlagwort]] "Mustermann, M."

# Baustein 3 — Vertiefung

         --{{0}}--
Ein Bereich für fortgeschrittene Inhalte oder Weiterverweise.

## Animierte Erklärung

         --{{0}}--
Ein Gedanke pro Klick:

{{1}}
**Erstens:** ...

{{2}}
**Zweitens:** ...

{{3}}
**Drittens:** ...

## Reflexionsfrage

         --{{0}}--
> Was würden Sie nach diesem Kurs anders machen als vorher?

# Abschluss

         --{{0}}--
Zusammenfassung und Ausblick.

## Was Sie mitnehmen

- [x] Zentrale Erkenntnis 1
- [x] Zentrale Erkenntnis 2
- [x] Zentrale Erkenntnis 3

## Quellen & Lizenz

         --{{0}}--
**Quellen**

- [Titel der Quelle 1](https://example.org)
- [Titel der Quelle 2](https://example.org)

**Lizenz**

Dieses Material steht unter [CC-BY 4.0](https://creativecommons.org/licenses/by/4.0/legalcode.de).

**Zitation**

> IHR NAME (Jahr). *Titel des Kurses*. Version 0.1.0. URL. DOI.  

## Kontakt

- Autor:in: IHR NAME
- E-Mail:   ihre.mail@einrichtung.de
- Einrichtung: IHRE Einrichtung

# Danke!
Vielen Dank fürs Durcharbeiten. Rückmeldungen, Verbesserungsvorschläge und Remix-Ideen sind ausdrücklich willkommen.