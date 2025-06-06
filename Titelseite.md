# Erfragen von Metadaten: Ein Fallbeispiel aus dem Europäischen und Deutschen Metadatenportal  
Um mit Daten arbeiten zu können, müssen diese auffindbar sein. Dieses <a href="https://jupyterbook.org/en/stable/intro.html" class="external-link" target="_blank">JupyterBook</a> vermittelt grundlegende Kenntnisse zur Datenabfrage, indem es relevante Datenportale vorstellt, über die Daten akquiriert werden können und Sie mit Metadaten, Standards und Abfragesprachen vertraut macht. 


```{figure} Datenwissenschaftler_analysiert_Baumverteilungen.png
---
name: Datenwissenschaftler analysiert Baumverteilungen
alt: Eine grafische Darstellung eines Datenwissenschaftlers der die Baumverteilung analysiert.
---
Datenwissenschaftler analysiert Baumverteilungen (KI generiert).
```

## Baumbestand-Analyse: Erfassung und Visualisierung der Verteilung der Baumarten
Der Baumbestand in deutschen Städten und ländlichen Regionen ist für Klimaanpassung, Umweltforschung und Stadtplanung von zentraler Bedeutung. Eine wichtige Grundlage für diese Arbeiten sind detaillierte Baumkataster, die Informationen zu Baumarten, Standorten und Zustand liefern. Doch wie gut sind diese Daten öffentlich zugänglich?

Dr. Amir Weber, ein Experte mit Interesse an städtischen und ländlichen Baumbeständen, möchte ein Dashboard zur Visualisierung der Baumartenvielfalt erstellen, das auf offenen Datensätzen basiert. Dazu stellt sich Dr. Weber die folgende Frage:

**Welche offen verfügbaren Daten existieren, die dazu beitragen können, den Baumbestand in einer bestimmten Region zu ermitteln?** 

Die Hauptfrage lässt sich also in mehrere Teilfragen untergliedern, die eine detaillierte Analyse der offenen Baumkataster-Daten ermöglichen. Diese Unterfragen fokussieren sich auf verschiedene Aspekte der Datensätze: die Gesamtzahl der Datensätze bundesweit, die Verteilung der Daten auf die einzelnen Bundesländer sowie die Unterschiede in der Zahl der Datenbereitsteller und der Vielfalt der bereitgestellten Formate in den jeweiligen Regionen.

- Wie viele Datensätze beinhalten das Wort „Baumkataster“ im Titel?
- Wer stellt die meisten Daten bereit?
- Wie unterscheiden sich die Bereitsteller in ihrer Anzahl an Formaten?

Diese Fragen sind der Ausgangspunkt für eine tiefere Untersuchung der verfügbaren offenen Daten. Dr. Weber plant, die Datensätze nach Bundesländern und Bereitstellern zu filtern, um ein besseres Verständnis darüber zu gewinnen, welche Regionen besonders viele und vielfältige Baumkataster-Daten zur Verfügung stellen. Recherchieren Sie mit ihm zusammen, wie die entsprechende Datengrundlage ist.  

Um die Fragen zu beantworten, vermittelt dieses JupyterBook Kenntnisse zu wichtigen Konzepten wie Semantic Web und Linked Data sowie Metadatenstandards und -qualität. Darüber hinaus erwartet Sie eine Einführung in die Benutzung der Abfragesprache SPARQL.  

## Bedeutung dieses Lehrbuchs für die Verwaltungswissenschaft
Die Auffindbarkeit von Daten wird durch Metadaten wesentlich vereinfacht. Ein grundlegendes Verständnis von Metadaten ist daher von entscheidender Relevanz. Dies gilt insbesondere für <a href="https://www.dcat-ap.de/" class="external-link" target="_blank">DCAT-AP</a> als gemeinsamer Metadatenstandard für offene Verwaltungsdaten. Des Weiteren lassen sich durch Abfragesprachen wie SPARQL passgenaue Informationen herausfiltern, was die Suche nach Datensätzen erleichtern kann.

## Zielgruppe
**Für wen ist dieses JupyterBook gedacht?**

Grundsätzlich steht das JupyterBook allen Interessierten offen.

Die explizite Zielgruppe sind jedoch promovierende und promovierte Wissenschaftler:innen sowie Lehrende aus der Verwaltungswissenschaft, da die hier vermittelten Inhalte anhand des häufig untersuchten Datentyps *Tabelle* aufbereitet sind. Zudem orientieren sich die hier entwickelten Lerneinheiten an einem für diese Disziplin typischen Fallbeispiel.


## Struktur der Fallstudie
Die zentrale Forschungsfrage, die in dieser Fallstudie untersucht wird, lautet: 

**Welche offenen Daten gibt es, die dazu beitragen, den Bewässerungsbedarf von Bäumen in einer bestimmten Region zu ermitteln?**

Basierend auf den verfügbaren offenen Datenquellen werden Abfragen mithilfe der Abfragesprache SPARQL entwickelt, um relevante Informationen zu extrahieren. Dabei wird die Nachnutzbarkeit der Daten untersucht, ihre Qualität bewertet sowie der Entstehungskontext nachvollzogen. Die Abfragen ermöglichen eine strukturierte Analyse der Daten, um spezifische Antworten zum Baumbestand zu erhalten.

Die Nutzung und erste Schritte mit SPARQL werden in dieser Fallstudie anschaulich erläutert.  


```{figure} FS-Schritte.png
---
name: steps of casestudy
alt: Skizzenhafte Darstellung der 4 Schritte dieser Fallstudie.
---
Visualisierung der 4 Schritte dieser Fallstudie.
```


**1. Technologien verstehen** 

Wir greifen in dieser Fallstudie auf Metadaten aus dem europäischen Metadatenportal <a href="https://data.europa.eu/en" class="external-link" target="_blank">data.europa</a> zurück. Daher werden zuerst die grundlegenden Technologien erläutert, die gängige Metadatenschemata ausmachen, nämlich Semantic Web & Linked Data.

**2. Werkzeuge kennenlernen**

Wir machen Sie mit einem der zentralen Werkzeuge für die Operationalisierung von Metadatenrepositorien vertraut: dem DCAT-AP-Standard, der auch die politisch-administrativen Aspekte im Kontext von öffentlicher Verwaltung und Open Data einbezieht. In dieser Fallstudie werden außerdem die Nutzung der Abfragesprache SPARQL und erste praktische Schritte anschaulich erklärt.

**3. Datenqualität messen:** 

Sie lernen, wie Sie Metadaten anhand von Maßnahmen zur Qualitätsmessung überprüfen können, um sicherzustellen, dass diese den Qualitätsanforderungen entsprechen. Dazu stellen wir Ihnen die verschiedenen Qualitätskriterien des Metadata Quality Assessment (MQA) für Metadaten vor.

**4. Praxis anwenden**
Im letzten Schritt der Fallstudie widmen wir uns der praktischen Anwendung und erläutern, wie Metadaten mithilfe der SPARQL-Abfragesprache abgefragt werden können. Dabei vermitteln wir zunächst die grundlegenden Konzepte von SPARQL, einschließlich der Syntax und zentraler Befehle. Im Anschluss führen wir gezielte Abfragen durch, die auf unsere Fragestellung ausgerichtet sind und evaluieren kritisch, in welchem Maß die aktuellen Implementierungen erfolgreich sind oder Optimierungspotenzial aufweisen.  

---
  

Die Gliederung der Fallstudie in Kapitel und Abschnitte können Sie immer in der Menüleiste auf der linken Seite nachvollziehen. Die rechte Menüleiste zeigt Ihnen an, in welchem Abschnitt eines Kapitels Sie sich gerade befinden.
Die einzelnen Kapitel sind so gestaltet, dass Sie sie sowohl chronologisch als auch separat voneinander durchgehen können.

Das JupyterBook lässt sich in zwei Hauptblöcke gliedern:


|       Block              |     Inhalte                                               |    Bearbeitungszeit              |  
|---------------------|----------------------------------------------------|----------------------------------------------------|
| **Block 1**           | Kapitel 2, 3, 4: Grundlagen des Semantic Web, Metadatenstandards und Metadatenqualität | ca. 3 x 15 Min pro Kapitel  |  
| **Block 2**| Kapitel 5: Praktische Anwendung von SPARQL: Abfrage von Daten zur Beantwortung der Forschungsfrage                                                     | 45 Min|
