---
title: "3. Vorlesung - Funktion und Aufbau von Bibliothekssystemen"
date: 2024-02-27
---

## Liebes Tagebuch
diese Vorlesungseinheit handelte von Metadatenstandards, Bibliotheksregelwerken, Datenformate und Bibliothekssystemen. 

## Metadatenstandards
### MARC21 
Zu Beginn haben wir uns mit dem Metadatenstandard MARC21 beschäftigt, welcher 1999 von der Library of Congress (LOC) entwickelt wurde. Das Dateiformat von MARC21 kann marc (.mrc) oder auch XML codiert sein (.xml ). Bei .mrc-Dateien gilt es zu beachten, dass diese nicht ohne weiteres d.h. ohne geeignete Software geöffnet werden können. Eine Möglichkeit diese Dateien auszulesen und abzuspeichern ist der Einsatz einer Bibliothekssoftware (siehe auch Abschnitt Bibliothekssoftware KOHA).  
MARC21 zeichnet sich durch die verschiedenen Felder aus. Diese Felder reichen von 001 bis 999. Die Felder werden im Bibliothekskontext dafür genutzt die Medien zu beschreiben. Jedes Feld hat seinen eigenen Verwendungszweck. Beispielsweise wird in Feld 100 die Haupteintragung der Person vermerkt, also beispielsweise die Autorin eines Buches. MARC21 wurde seit 1999 immer wieder überarbeitet (insgesamt 37 Updates). Jedoch wurde der Standard nicht grundlegend verändert, sondern eher ergänzt. Aufgrund des langen Bestehens beinhaltet der Standard folglich nicht mehr alle aktuellen Überlegungen. 
### Dublin Core
Dublin Core ist ein weiterer Metadatenstandard. Anders als MARC21 wird er aber auch weit über das Bibliothekswesen verwendet. Dublin Core ist simpler und verständlicher aufgebaut, da die Codierung sprechend ist und nicht wie bei MARC21 diverse Felder auswendig gelernt werden müssen. Untenstehend die Definition, die ChatGPT liefert:
<img width="454" alt="image" src="https://github.com/nathaliewic/lerntagebuch/assets/160014832/1a0bea8a-2ba9-49ae-a524-44cc7025960d">

## Regelwerke
### BIBFRAME
MARC21 ist sehr stark medienzentriert. Dies ist aufgrund der stärkeren digitalen Vernetzung der Informationswelt nicht mehr zeitgemäss. Aus diesem Grund hat die LOC im Jahr 2011 das Datenmodell Bibliographic Framework Initiative (BIBFRAME) begründet. So sollen Katalogisate auch in Zukunft austauschbar sein und bibliografische Daten sinnvoll erfasst werden können (Quelle).  
BIBFRAME lehnt an die Funcitional Requirements for Bibliographic Records (FRBR) an. Ähnlich wie FRBR unterscheidet BIBFRAME zwischen work, instance, item. Work ist eine Zusammenführung von Werk und Expression im FRBR-Modell. Instance entspricht der Manifestation und das item ist das Pendant zum Item (siehe auch Abbildung).
![image](https://github.com/nathaliewic/lerntagebuch/assets/160014832/8dfbecd7-49bf-40d2-a123-56efaedb83a6)

### Ressource Description and Access (RDA)
Ein weiteres bibliografisches Regelwerk ist RDA. Darin wird sehr konkret beschrieben, wie die einzelnen Angaben der Medien erfasst werden sollen. Die deutsche Nationalbibliothek hat die Implementierung des Regelwerks in den Jahren 2012 bis 2016 im DACH-Raum geleitet [https://www.dnb.de/DE/Professionell/Standardisierung/Standards/_content/rda.html]. 

## Bibliothekssoftware - KOHA 
Abschliessend haben wir uns mit der Open Source Bibliothekssoftware KOHA beschäftigt. KOHA ist eine umfassende Bibliothekssoftware, die von ca. 600 Personen mitgestaltet wird. Über OpenHub lässt sich erkennen wie ‘gesund’ das Projekt ist. Bei kommerziellen Anbietern ist ein Indikator für die Popularität die Verkaufszahlen, bei Open Source Projekten kann u.a. OpenHub Aufschluss darüber geben. Mit den Angaben aus Open Hub lässt sich schliessen, dass, wie erwähnt 600 Personen am Projekt beteiligt sind und die Year-over-Year-Commits (Y-O-Y) konstant bleiben. Das deutet daraufhin, dass immer noch aktiv am Code gearbeitet wird und das Projekt entsprechend 'gesund' ist. 

Die Software selbst gilt als Profisoftware. Sie richtet sich also an das Fachpersonal und ist auf eine schnelle Arbeitsweise ausgerichtet (Tastenkürzel, etc.). Wie bei kommerziellen Produkten sind alle notwendigen Funktionen für den bibliothekarischen Alltag vorhanden. Diese reichen vom Erstellen eines Nutzenden über die Erstellung von Mahnungen bis hin zur Erwerbung von Medien. 
 ![image](https://github.com/nathaliewic/lerntagebuch/assets/160014832/af972354-cbc5-4219-b42e-5d6501063e2d)

Aus persönlichem Interesse habe ich die Katalogisierungsoberfläche von ALMA und KOHA verglichen. Der kurze Vergleich mit ALMA zeigt, dass die Katalogisierungsoberflächen ähnlich aufgebaut sind. Im Vergleich zu ALMA ist KOHA insofern benutzendenfreundlicher, als dass darin die Felder kurz beschrieben werden. Bei ALMA erhält man lediglich eine aufsteigende Liste mit den Feldern. 
![image](https://github.com/nathaliewic/lerntagebuch/assets/160014832/271170a0-940e-40e1-9bba-16efdfd6e1a4)
![image](https://github.com/nathaliewic/lerntagebuch/assets/160014832/ad110d48-00f8-4e65-8b0e-a5ce01796951)

  
Abschliessend erhält man in der Demo von KOHA auch einen Einblick in die Softwarekonfiguration. Darin können diverse Systemparameter (bspw. Felder der Katalogisierungsvorlagen) angepasst werden. Dies ist sehr interessant, weil ich an meiner Arbeitsstelle in der wir mit ALMA arbeiten, keinen solchen Einblick ‘hinter die Kulissen habe’. 

