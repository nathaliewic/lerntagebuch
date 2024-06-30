---
title: "11 Linked Data"
date: 2024-05-29
---

# Liebes Tagebuch
in dieser (bereits) letzten Vorlesung haben wir uns mit Linked Data beschäftigt. Dazu haben wir die aktuellen Datenmodelle, Linked Open Usable Data (LOUD) besprochen. Zu LLM zu Bibliotheks- und Archivinformatik und der Metadatenanreicherung haben wir eine Übung gemacht. 

Auf die Datenmodelle BIBFRAME und RiC möchte ich an dieser Stelle nicht weiter eingehen. [Hier](https://nathaliewic.github.io/lerntagebuch/2024/02/27/Funktion-und-Aufbau-von-Bibliothekssystemen.html) kann nachgelesen werden, was darunter verstanden wird.  
# LOUD
Anhand der Präsentationsfolien von Adrian Pohl wurden wir mit LOUD vertraut gemacht [(Link Folien)](http://slides.lobid.org/2021-weimar/). Auf LOUD möchte ich nun detailliert eingehen. Hier eine weitere [Quelle, die die Design Principles von LOUD erläutert](https://linked.art/loud/). Untenstehendes Zitat stellt dar, welche Punkte an Linked Open Data kritisiert werden:
«But it comes exclusively from a publishing perspective, and does not make any recommendations about how to publish data in a way that is usable by potential consumers. In the intervening time, the web community has recognized that we need 5 more stars, or design principles, to promote data consumption. If our data isn't used, then no value is gained from the resources that were invested in its creation, publication, maintenance and improvement. If we want our data to be used, then it needs to be usable: Linked Open Usable Data.»

LOUD richtet sich an die Entwicklerinnen und Entwickler sowie an die Nutzerinnen und Nutzer. 
Usability bedeutet, dass die Benutzerfreundlichkeit von der Zielgruppe abhängt. Die Zielgruppe für Daten sind Entwickler, und die Benutzeroberfläche für Entwickler ist die API, über die sie Zugriff auf die Daten erhalten. Die API für LOD erfolgt über HTTP, was gut verstanden wird, aber auch von der Ontologie abhängig ist. Ontologien sind in erster Linie für semantische oder theoretische Korrektheit entworfen, was das am wenigsten praktische Anliegen ist. Nun müssen die Abwägungen zwischen Vollständigkeit und Präzision des Ausdrucks und der Benutzerfreundlichkeit der resultierenden Datenkonstrukte ausbalanciert werden.
Fünf Designprinzipien bilden die Grundlage für die Benutzerfreundlichkeit.

1.	Abstraktion

Die Abstraktion ist wichtig. In der Quelle wird beschrieben, dass ein Autofahrer nicht die gleichen Informationen benötigt wie ein Mechaniker. Für den Autofahrer genügt also eine abstraktere Version als es der Mechaniker benötigt. Die Entwickler zielen also nicht auf die ontological purity ab, sondern auf die Interobilität der Systeme. 

3.	Reduktion der Barrieren

Wenn die Daten einfach verständlich sind, wird es mehr Leute geben, die sich mit den Daten befassen. Deshalb ist es wichtig, die Barrieren einfach zu halten. 

5.	Verständnis

JSON-LD ermöglicht es die Entwickler in ‘Ihrer’ Sprache anzusprechen. Folglich müssen sie sich nicht eine neue Ontology oder ein Vokabular lernen, um die Daten zu verstehen.

7.	Dokumentation

Dokumentation hilft die Daten zu verstehen. Deswegen sollte eine Dokumentation angefertigt werden. 

9.	Muster – an Stelle von Ausnahmen

Jede Ausnahme bildet eine Regel. Aus diesem Grund ist es wichtig, nicht Einzelfalllösungen zu finden sondern dafür Muster zu implementieren. 

# Reflexion zum Beitrag
Mit diesem Blogbeitrag habe ich mich mit einem (für mich) relativ technischen Thema beschäftigt. Das Thema finde ich sehr interessant, aber es ist auch sehr technisch. Wie bereits bei (dem Beitrag zu den Schnittstellen II)[https://nathaliewic.github.io/lerntagebuch/2024/04/05/schnittstellenII.html] habe ich mich mit diesem Blogbeitrag einem weiteren technischen Thema gewidmet. Diese Annäherungen mit den technischen Themen haben meinen Horizont sicherlich erweitert, auch wenn dies mit Herausforderungen verbunden war. Eine Herausforderung war beispielsweise, überhaupt zu verstehen, was mit den erwähnten Dingen gemeint ist, denn um über sie zu berichten, muss ich sie in einem ersten Schritt verstehen. Nach einiger Zeit und dem Lesen einiger Quellen konnte ich diese persönliche Herausforderung meistern. 

# Quellen:
<https://slides.lobid.org/2022-05-06-lod-dipf/#/53>
<https://linked.art/loud/>
<http://slides.lobid.org/2021-weimar/>
