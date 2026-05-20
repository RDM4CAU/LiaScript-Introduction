<!--
author: Britta Petersen
email: b.petersen@rz.uni-kiel.de
version: 0.1.0
date: 2026-05-20
comment: Workshop Open Educational Resources mit LiaScript erstellen: Ein Liascript zum Ausprobieren.
language: de
narrator: Deutsch Female

mode:     Presentation

repository: https://github.com/RDM4CAU/LiaPlayground
icon: https://raw.githubusercontent.com/RDM4CAU/TtL-FDM/main/images/fdm_lehre.png
link: https://raw.githubusercontent.com/RDM4CAU/Intro-to-RDM/refs/heads/main/cau-style.css

import:   https://github.com/LiaTemplates/Pyodide
-->

# Ausprobierkurs

Dieses Dokument ist ein **erster Kontakt** mit einem kleinen LiaScript-Kurs.

Es enthält drei kurze Einheiten, in denen Sie einige LiaScript-Funktionen einmal aus der Sicht eines Lernenden ausprobieren sollen.

> **Aufgabe für die nächsten 15-20 Minuten**
>
> Gehen Sie die folgenden Seiten durch und probieren Sie alle interaktiven Elemente aus.
>
> Notieren Sie sich:
>
> - Was gefällt Ihnen gut? Was nicht so gut?
> - Welche(s) Element(e) würden Sie vielleicht selbst einsetzen?
> - Was hat Sie überrascht oder was hat vielleicht anders funktioniert als erwartet?

> [!TIP]
> Klicken Sie links unten auf den Pfeil nach rechts, um auf die nächste Seite zu blättern. Alternativ können Sie auch die Pfeiltasten Ihrer Tastatur verwenden oder in dem Inhaltsverzeichnis auf der linken Fensterseite durch einen Klick in das gewünsche Kapitel navigieren.

## Konzept

Die kurzen Abschnitte sollen nur einen Eindruck vermitteln, wie mit Hilfe von LiaScript Wissensvermittlung unterstützt werden kann und zeigen nur ausschnitthaft einige LiaScript Funktionen.

Jeder Abschnitt fokussiert dabei einen anderen Aspekt:

| Abschnitt          | Fokus                                                                                       |
| ------------------ | ------------------------------------------------------------------------------------------- |
| OER - Was ist das?       | *Einbindung verschiedener Medientypen* - Wissensvermittlung ohne Medienbrüche |
| Datenkompetenz     | *von Daten und Code* - Visualisierung und ausführbarer Code                                  |
| Recherchekompetenz | *von Visualisierungen zu Quizzen* - Interktive Wissensüberprüfung                           |

## 1. OER - Was ist das?

> [!NOTE]
> **Worauf Sie in diesem Abschnitt achten sollten:** LiaScript ermöglicht die Einbindung verschiedener Medientypen und versucht, *Wissensvermittlung ohne Medienbrüche* zu ermöglichen: keine Tab-Wechsel, keine Tool-Sprünge, kein Kontextverlust.
> Zum dem Thema OER werden Sie im Folgenden mit *verschiedenen Medientypen* konfrontiert, die alle innerhalb dieses LiaScriptes dargestellt werden.

### OER - Einstieg per Video

> [!NOTE]
>**Was ist OER? Schauen Sie zum Einstieg ins Thema OER ein kurzes Viedeo und lösen Sie die Mini-Aufgabe unter dem Video!**

!?[OER Einführungsvideo](https://www.youtube.com/watch?v=1WnZD7E8FKY)

> **Mini-Aufgabe:** Was ist entscheident dafür, dass ein Material als OER bezeichnet werden kann?

{{1}}
> **Auflösung:** Damit ein Material als OER bezeichnet werden kann, ist die Angabe einer offnen Lizenz entscheident.

### OER und Lizenzen

![OER Logo](..\Global_Open_Educational_Resources_Logo-275x183.png "Das „Global OER Logo“ von Jonathas Mello unter CC BY 3.0 (via UNESCO)")

>Offenbar ist eine Ressource, die ich online zur Verfügung stelle nicht automatisch OER. Und Materialien, die ich online finden kann, sind ebenfalls nicht automatisch OER.
>
>Erst, wenn die Materialien mit einer entsprechenden **Lizenz** versehen sind, können Materialien offen und rechtssicher genutzt werden und gelten als OER.
>
>>**So steht es auch in der [Definition der UNESCO](https://www.unesco.de/themen/bildung/bildungsqualitaet/weltbildungsempfehlung/global-citizenship-education/friedens-und-menschen/open-educational-resources/):**
>>
>> ***Open Educational Resources (OER) sind Bildungsmaterialien jeglicher Art und in jedem Medium, die unter einer offenen Lizenz stehen. Eine solche Lizenz ermöglicht den kostenlosen Zugang sowie die kostenlose Nutzung, Bearbeitung und Weiterverbreitung durch Dritte ohne oder mit geringfügigen Einschränkungen.*** (Quelle: [UNESCO](https://www.unesco.de/themen/bildung/bildungsqualitaet/weltbildungsempfehlung/global-citizenship-education/friedens-und-menschen/open-educational-resources/))

> [!NOTE]
> Die nachfolgende, eingebettete Seite erläutert, was cc Lizenzen sind und listet die derzeit zur Verfügung stehenden sechs Lizenzen auf:

<iframe src="https://de.creativecommons.net/was-ist-cc/" width="100%" height="500" style="border: 1px solid #ccc; border-radius: 4px;"></iframe>

> **Mini-Aufgabe:** Scrollen Sie durch die Seite und finden Sie heraus, unter welcher Lizenz die Seite selbst steht.

{{1}}
> **Auflösung:** Die Seite selbst steht unter der [CC BY 4.0 Lizenz](https://creativecommons.org/licenses/by/4.0/)
> 
> **Beachten Sie:** Nur CC BY und CC BY SA gelten als offene Lizenzen im Sinne von OER!

### OERs suchen

Eine Möglichkeit unter mehreren ist die Suche nach OER via eines Metasuchindexes. Ein Beispiel hierfür ist [OERSI](https://oersi.org/resources/pages/de/about/)

<iframe src="https://oersi.org/resources/pages/de/about/" width="100%" height="500" style="border: 1px solid #ccc; border-radius: 4px;"></iframe>

> **Mini-Aufgabe:** Suchen Sie nach LiaScript. Finden Sie Resourcen?

### OERs publizieren

Ihnen stehen viele verschiedene Möglichkeiten offen, eigene Materialien zu publizieren. Um eine gute Auffindbarkeit und eine gute Nachnutzbarkeit der Materialien zu gewähleisten, sind beschreibende **Metadaten** von großer Bedeutung!

Die Metadaten sollten dabei in einem **maschienenlesbaren Format** vorliegen. Beispiele für häufig verwendete, maschienenlesbare Formate für Metadaten sind XML, JSON und YAML.

Das folgende Beispiel eines YAML wurde mit dem OERSI Metadatenformular erstellt und ist in dieses LiaScript hier als ***Code-Block*** integriert:

```YAML
{
  "@context": "https://schema.org/",
  "creativeWorkStatus": "Draft",
  "type": "LearningResource",
  "name": "LiaScript Ausprobiermodul",
  "description": "Ein Liascript zum Ausprobieren mit Inhalten zum Thema Open Educational Resources (OER). Das Modul ist Teil des Workshops Open Educational Resources mit LiaScript erstellen. ",
  "license": "https://creativecommons.org/publicdomain/zero/1.0/deed.de",
  "creator": [
    {
      "givenName": "Britta",
      "familyName": "Petersen",
      "id": "https://orcid.org/0000-0002-0355-2594",
      "type": "Person",
      "affiliation": ""
    }
  ],
  "keywords": [
    "Open Educational Resources",
    "OER",
    "Liascript",
    ""
  ],
  "inLanguage": [
    "de"
  ],
  "about": [
    "https://w3id.org/kim/hochschulfaechersystematik/n0"
  ],
  "learningResourceType": [
    "https://w3id.org/kim/hcrt/course",
    "https://w3id.org/kim/hcrt/web_page"
  ],
  "educationalLevel": [
    "https://w3id.org/kim/educationalLevel/level_A"
  ]
}
```

> **Lesart:** Jedes `"name": [...]`""-Element ist eine maschinenlesbare Aussage über diesen Kurs. Wird er als seprate Datei einem Git-Repositorium beigefügt, ist er lesbar für Suchmaschinen, OER-Repositorien und Linked-Data-Werkzeuge. Genau diese Form von Metadaten macht ein Lernmaterial als *Open Educational Resource* im Web auffindbar, zitierbar und nachnutzbar.

> [!TIP]  
> In der oberen rechten Ecke befindet sich ein **i-Icon** (ℹ️). Klicken Sie auf das Icon. Sie finden Metadaten zu diesm Modul in einer übersichtlichen Darstellung.

## 2. Datenkompetenzen 

> [!TIP]  
> ... (engl. Data Literacy) ist die Fähigkeit, Daten auf kritische Art und Weise zu sammeln, zu verwalten, zu bewerten, zu analysieren und zu interpretieren. Sie umfasst zudem die Fähigkeit, mit Daten zu kommunizieren und sie zu nutzen, um fundierte Entscheidungen zu treffen.

> [!NOTE]
> **Worauf Sie in diesem Abschnitt achten sollten:** Der Abschnitt zeigt beispielhaft, wie LiaScript die Integration von Daten und Code in Lernmaterialien ermöglicht — und damit die Vermittlung von Datenkompetenz unterstützen kann.

### Daten interpretieren

Schauen wir uns ein einfaches fiktives Beispiel aus einer Bibliothek an.

Die Tabelle zeigt Anzahl der Ausleihen und Vormerkungen pro Monat. Nutzen Sie die Stapel am rechten Spaltenrand um die Daten zu sortieren und bestimmen Sie auf diese Weise, in welchem Monat es die meisten Ausleihen gab.

<!-- data-type="barchart" -->
| Monat | Ausleihen | Vormerkungen |
| ----- | ---------:| ------------:|
| Jan   |      1240 |           95 |
| Feb   |      1180 |          102 |
| Mär   |      1320 |          110 |
| Apr   |      1450 |          135 |
| Mai   |      1610 |          128 |
| Jun   |      1555 |          140 |

> [!TIP]  
> Noch einfacher geht es mit dem integrierten Diagrammgenerator: klicken Sie auf den Button Balkendiagramm über der Tabelle, um die Daten visuell zu erkunden. Finden Sie die in der Werkzeugleiste unter dem Diagramm die Möglichkeit, die Daten gleich zu bearbeiten?

### Darf es ein bisschen Code sein?

> [!TIP]
> Manchmal reicht es nicht, Daten zu visualisieren - wir wollen auch Kennzahlen berechnen, um die Daten zu interpretieren. In diesem Beispiel wollen wir die Vormerkungsquote berechnen - also den Anteil der Vormerkungen an den Ausleihen pro Monat.
>
> Wir haben Ihnen den Code schon vorgegeben, Sie müssen lediglich die Zeile zur Berechnung der Vormerkungsquote einkommentieren und das kleine Beispiel neu ausführen. Probieren Sie es aus!

**Klicken Sie auf den Play-Button** (▶) im Code-Block:

```python        python_example.py
import pandas as pd

# hier werden die Daten als DataFrame angelegt - eine tabellarische 
# Datenstruktur, # die in Python häufig verwendet wird
daten = pd.DataFrame({
    "Monat":        ["Jan", "Feb", "Mär", "Apr", "Mai", "Jun"],
    "Ausleihen":    [ 1240,  1180,  1320,  1450,  1610,  1555],
    "Vormerkungen": [   95,   102,   110,   135,   128,   140]
})

# Berechne die Vormerkungsquote als neue Spalte
# Löschen Sie das Kommentarzeichen (#) am Anfang der nachfolgenden Zeile, 
# um die Berechnung der neuen Spalte zu aktivieren
# daten["Vormerkungsquote"] = daten["Vormerkungen"] / daten["Ausleihen"]
print(daten)
```
@Pyodide.eval

## 3. Recherchekompetenz — Boole'sche Operatoren

> [!TIP]  
> Recherchekompetenz ist eines der klassischen Schulungsthemen in Bibliotheken — und eines der am schwersten greifbaren. Wir machen es hier konkret: Sie bekommen einen überschaubaren Datenbestand, und der Klick auf ein Venn-Diagramm zeigt, welche Treffer eine Boole'sche Anfrage tatsächlich liefert.

> [!NOTE]
> **Worauf Sie in diesem Abschnitt achten sollten:** Im abschließenden Themenfeld dokumentieren wir die Quizformate, die Liascript abbildet um Lernstandserfassungen zu ermöglichen.

### Ein Mini-Datenbestand

Stellen Sie sich vor, eine Fachdatenbank hätte nur die folgenden zehn Treffer zu Ihrer Schulungsrecherche. Jeder Titel ist mit keinem, einem oder beiden der Schlagworte **Informationskompetenz (IK)** bzw. **Berufsbildung (BB)** verknüpft.

| #   | Titel                                                                                             |  IK  |  BB  |
| ---:| ------------------------------------------------------------------------------------------------- |:----:|:----:|
|  1  | *Informationskompetenz in Universitätsbibliotheken*                                               |  ✓   |      |
|  2  | *Suchkompetenz und Recherche-Training*                                                            |  ✓   |      |
|  3  | *Open Access und wissenschaftliche Informationskompetenz*                                         |  ✓   |      |
|  4  | *Digitale Informationskompetenz an Schulen*                                                       |  ✓   |      |
|  5  | *Informationskompetenz für Auszubildende in technischen Berufen*                                  |  ✓   |  ✓   |
|  6  | *Recherchetraining im dualen Berufsausbildungssystem*                                             |  ✓   |  ✓   |
|  7  | *Digitale Kompetenzen in der beruflichen Weiterbildung — Schwerpunkt Informationskompetenz*       |  ✓   |  ✓   |
|  8  | *Curriculumentwicklung in der Berufsausbildung*                                                   |      |  ✓   |
|  9  | *Duale Berufsausbildung im Wandel*                                                                |      |  ✓   |
| 10  | *Qualitätsstandards in der beruflichen Bildung*                                                   |      |  ✓   |

> Recherchekompetenz bedeutet hier, die Schlagworte so zu kombinieren, dass spezifische Treffermengen bereitgstellt werden. Die drei wichtigsten Operatoren sind `AND`, `OR` und `NOT` — sie entsprechen den Schnitt-, Vereinigungs- und Differenzmengen in der Mengenlehre.

| Operator | Bedeutung                           | Wirkung auf Treffermenge | Im Datensatz oben       |
|:--------:| ----------------------------------- |:------------------------:|:------------------------|
|  `AND`   | **Beide** Begriffe müssen vorkommen | verkleinert              | 3 Treffer (5, 6, 7)     |
|  `OR`    | **Mindestens einer** muss vorkommen | vergrößert               | 10 Treffer (alle)       |
|  `NOT`   | Begriff **darf nicht** vorkommen    | verkleinert              | 4 bzw. 3 Treffer        |

> Kleiner Merksatz: **AND ist streng, OR ist großzügig, NOT ist wählerisch.**

### Venn-Diagramm zum Datensatz

Das Diagramm visualisiert, wie sich die zehn Titel auf die drei Schnittbereiche verteilen:

<svg class="boole-venn" viewBox="0 0 440 270" xmlns="http://www.w3.org/2000/svg" style="max-width: 620px; display: block; margin: 0 auto;">
  <defs>
    <mask id="notB">
      <rect width="100%" height="100%" fill="white"/>
      <circle cx="260" cy="140" r="85" fill="black"/>
    </mask>
    <mask id="notA">
      <rect width="100%" height="100%" fill="white"/>
      <circle cx="180" cy="140" r="85" fill="black"/>
    </mask>
    <clipPath id="inA">
      <circle cx="180" cy="140" r="85"/>
    </clipPath>
  </defs>

  <text x="110" y="35" text-anchor="middle" font-size="13" fill="#2c3e50" font-weight="bold">Informationskompetenz</text>
  <text x="330" y="35" text-anchor="middle" font-size="13" fill="#2c3e50" font-weight="bold">Berufsbildung</text>

  <circle cx="180" cy="140" r="85" fill="#3498db" fill-opacity="0.5" mask="url(#notB)"/>
  <circle cx="260" cy="140" r="85" fill="#9b59b6" fill-opacity="0.7" clip-path="url(#inA)"/>
  <circle cx="260" cy="140" r="85" fill="#e74c3c" fill-opacity="0.5" mask="url(#notA)"/>

  <circle cx="180" cy="140" r="85" fill="none" stroke="#2c3e50" stroke-width="2" pointer-events="none"/>
  <circle cx="260" cy="140" r="85" fill="none" stroke="#2c3e50" stroke-width="2" pointer-events="none"/>

  <text x="115" y="145" text-anchor="middle" font-size="13" font-weight="bold" fill="#1a5490" pointer-events="none">IK NOT BB</text>
  <text x="220" y="145" text-anchor="middle" font-size="13" font-weight="bold" fill="#5b2c6f" pointer-events="none">IK AND BB</text>
  <text x="325" y="145" text-anchor="middle" font-size="13" font-weight="bold" fill="#922b21" pointer-events="none">BB NOT IK</text>

  <text x="220" y="255" text-anchor="middle" font-size="12" fill="#7f8c8d" pointer-events="none">IK OR BB = alle drei Bereiche zusammen</text>
</svg>

<br>

> [!NOTE]
> Die folgenden Aufgaben prüfen Ihr Verständnis am gleichen Datensatz — und zeigen gleichzeitig drei verschiedene LiaScript-Quizformate: **Einfachauswahl**, **Zahleneingabe** und **Mehrfachauswahl**. Jede Aufgabe hat einen ausklappbaren Hinweis (`?`). Aufgabe 1 und zwei haben jeweils eine auf- und einklappbare Lösung. Aufgabe 3 hat eine erweiterte Rückmeldung bei richtiger Antwort.

<br>

**Aufgabe 1 — Welcher Bereich entspricht welcher Anfrage?** *(Einfachauswahl)*

Welcher Bereich des Venn-Diagramms zeigt Titel, die mit *beiden* Schlagworten verknüpft sind?

- [( )] Der blaue Bereich (links)
- [(X)] Der violette Schnittbereich (Mitte)
- [( )] Der rote Bereich (rechts)
- [( )] Alle drei Bereiche zusammen
- [[?]] Hinweis: "Mit beiden Schlagworten" entspricht der Anfrage `IK AND BB`. AND meint immer den *Schnitt* zweier Mengen.

<details>
<summary><strong>Lösung anzeigen</strong></summary>

Der violette Schnittbereich. Drei Titel haben in der Tabelle beide Häkchen gesetzt:

- 5 · *Informationskompetenz für Auszubildende in technischen Berufen*
- 6 · *Recherchetraining im dualen Berufsausbildungssystem*
- 7 · *Digitale Kompetenzen in der beruflichen Weiterbildung — Schwerpunkt Informationskompetenz*

</details>

<br>

---

**Aufgabe 2 — Treffer zählen.** *(Zahleneingabe)*

Wie viele Titel aus dem Datensatz liefert die Anfrage `IK OR BB`?

- [[10]]
- [[?]] Hinweis: OR ist großzügig — es reicht, wenn *eines* der beiden Schlagworte gesetzt ist. Schauen Sie in die Tabelle: gibt es überhaupt einen Titel, der *gar kein* Häkchen hat?

<details>
<summary><strong>Lösung anzeigen</strong></summary>

**Alle zehn.** In diesem konstruierten Datensatz hat jeder Titel mindestens eines der beiden Schlagworte gesetzt — es gibt keinen "leeren" Eintrag. Das `OR` umfasst hier also den gesamten Bestand.

</details>

<br>

---

**Aufgabe 3 — Eine Kollegin braucht Beratung.** *(Mehrfachauswahl)*

Eine Kollegin sucht Bücher zur *Berufsbildung*, die *keinen* Informationskompetenz-Bezug haben. Welche Aussagen treffen zu?

- [[X]] Die passende Anfrage lautet `BB NOT IK`.
- [[X]] Sie liefert 3 Treffer.
- [[ ]] Sie liefert mehr Treffer als `IK NOT BB`.
- [[ ]] `BB NOT IK` und `BB AND NOT IK` liefern unterschiedliche Treffermengen.
- [[X]] Sie entspricht im Diagramm dem roten Bereich, der nicht mit dem blauen überlappt.
- [[?]] Hinweis: Lesen Sie das Diagramm als "BB ohne den Schnitt mit IK" — der rote Teil ohne den violetten.
******************
>Toll! Richtig :-)

Richtig sind die erste, zweite und fünfte Aussage. Die drei Treffer:

- 8 · *Curriculumentwicklung in der Berufsausbildung*
- 9 · *Duale Berufsausbildung im Wandel*
- 10 · *Qualitätsstandards in der beruflichen Bildung*

Zu den Distraktoren:

- `IK NOT BB` liefert **4** Treffer — also *mehr*, nicht weniger als `BB NOT IK`.
- `BB NOT IK` und `BB AND NOT IK` sind logisch äquivalent — das explizite `AND NOT` ändert nichts am Ergebnis.
**************

# Referenzen

> [!NOTE]
> Abschnitte 2. Datenkompetenz und 3. Recherchekompetenz dieses Dokuments entstammen:
>
>Sebastian Zug, André Dietrich, Anja Hawlitschek und Anja Schulz: LiaScript im Bibliotheksalltag (2026) lizenziert unter [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)

