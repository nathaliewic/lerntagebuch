---
title: "8 Metadaten und Schnittstellen II"
date: 2024-04-05
---

# Liebes Tagebuch
in dieser Lerneinheit haben wir uns mit dem 2. Teil von Metadaten und Schnittstellen beschäftigt. Nach dem wir uns in der letzten Einheit mit Open Refine beschäftigt haben ging es nun um die Schnittstellen.
Zu Beginn haben wir uns die ‘Semesteraufgabe’ nochmals angeschaut. Dieses Mal lag der Fokus auf (wer hätte es gedacht) den Schnittstellen. Die Grafik der Semesteraufgabe zeigt, dass am Ende des Semesters, Daten aus unterschiedlichen Quellen in dem bibliothekarischen Suchsystem (Bibliothekskatalog) Vufind dargestellt werden sollen. 
![image](https://github.com/nathaliewic/lerntagebuch/assets/160014832/38f0bdf2-3cc4-4c6d-ad95-b2515a2f664d)

Da für die Semesteraufgabe ein OAI Harvester bzw. das OAI-PMH Protokoll verwendet wird, gehe ich in der Folge vertieft auf die OAI (Open Archives Initiative) ein. Die Open Archives Initiative entwickelt und fördert Interoperabilitätsstandards, die darauf abzielen, die effiziente Verbreitung von Inhalten zu erleichtern. Die OAI-Schnittstelle wird u.a. dafür genutzt in regelmässigen Abständen grosse Datenbestände zu aktualisieren:

«Über diese neue Schnittstelle können Normdaten in MARC21-XML und RDFxml und Titeldaten im Format DNB Casual (eine Auswahl von DublinCore-Elementen) und RDFxml kostenlos bezogen werden»

Grundlage für die regelmässige Synchronisation ist dafür der initiale Datenimport eines aktuellen Grundbestandes in die eigene Datenbank. Die jeweiligen Grundbestände stellt die DNB auf ihrer Webseite zur Verfügung. Diese Grundbestände wie auch die Schnittstelle sind kostenfrei. 
Für den Austausch von Metadaten braucht es einen Datenlieferanten (bspw. Deutsche Nationalbibliothek) und einen Dienstanbieter. Der Bezug der Daten läuft dann automatisiert durch den OAI-Harvester (siehe Bild). Zur Kommunikation wird ein Protokoll verwendet: das OAI-PMH. Dieses Protokoll ist webbasiert. Die Anfragen, die der OAI-Harvester stellt, lauten in etwa so: HTTP-GET oder HTTP-Post. Vom Datenlieferant erhält man dann wiederum eine HTTP- Antwort. Eingebettet in die XML-Struktur enthält die Antwort die angeforderten Metadaten. 
# Funktionen des OAI_PMH:
Das Protokoll beinhaltet sechs Basinsfunktionen. Diese werden an die baseURL angefügt mittels dem Zusatz ‘?verb=’. Untenstehend wird auf drei der Basisfunktionen eingegangen:
-	Identify: Dabei werden allgemeine Informationen zum OAI-Repository angezeigt.
-	ListSets: Dabei werden Informationen zu allen im OAI-Repository zur Verfügung gestellten Datenensets dargestellt. 
-	ListMetadataFormats: Dabei werden die vorhandenen Datenformate bzw. Informationen für den Export angebotenen Formate aufgelistet. 
Mittels der OAI-Anfrage werden alle Datensätze geliefert, die im angefragten Zeitraum geändert oder auch neu erstellt wurden. Über OAI können nur Datensätze mit dem Kriterium ‘Änderungsdatum’ abgefragt werden. Für andere Kriterien sollte mit der SRU-Schnittstelle gearbeitet werden. 

Die DNB veröffentlichte auch die Syntax von OAI- Anfragen: 
![image](https://github.com/nathaliewic/lerntagebuch/assets/160014832/79e3a5b2-e85b-48ed-8557-585f010b0be7)
![image](https://github.com/nathaliewic/lerntagebuch/assets/160014832/847929b8-c6d5-4e2b-9a12-c7d7b543a11b)
![image](https://github.com/nathaliewic/lerntagebuch/assets/160014832/ef7cafb0-f3da-4a09-9a6b-8813abfa62fe)

# Reflexion des Beitrags
Die Ausführung dieses technischen Themas war herausfordernd. Nichtsdestotrotz war es umso lehrreicher, weil ich mich mit einer Thematik auseinandergesetzt habe, mit der ich mich üblicherweise nicht beschäftige. Beim Verfassen des Beitrags habe ich gemerkt, dass mir das Verständnis dieses Themas schwerer fiel als bei anderen. Dies liegt wie erwähnt daran, dass ich mich bei den technischeren Themen nicht 'zu Hause' fühle. Ich fand es jedoch wichtig mich auch Mal mit einem Thema ausserhalb meiner Comfort Zone zu bewegen und mich mit diesem Beitrag vertieft einem technischen Thema auseinanderzusetzen. 
# Quellen
<https://d-nb.info/1044619376/34>
<https://www.dnb.de/DE/Professionell/Metadatendienste/Datenbezug/OAI/oai_node.html>
