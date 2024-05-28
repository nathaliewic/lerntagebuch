---
title: "8 Suchmaschinen und Discovery Systeme"
date: 2024-28-05
---

# Suchmaschinen und Discovery Systeme
# Liebes Tagebuch
In dieser Vorlesung haben wir uns mit Suchmaschinen und Discovery-Systemen beschäftigt. Zunächst gab es einen Nachtrag zu den Metadaten und den Schnittstellen. In diesem Blogbeitrag soll es, um das neue Thema gehen. Bei Bedarf kann der Nachtrag hier (BAIN FS24 Zürich 11 Suchmaschinen und Discovery-Systeme (Teil 1/2) - HedgeDoc (gwdg.de))nachgelesen werden.
Dann ging es an das eigentliche Thema: In einer Live-Demonstration hat uns der Dozent die Installation und Konfiguration von VuFind nähergebracht. Dieser Input war zwar interessant, aber für mich als nicht technik-begeisterte Person schon ein wenig zu technisch. 
In dem folgen Blogbeitrag soll nun vertieft auf Solr und VuFind eingegangen werden. 
## Solr
 
Solr ist ein plattformunabhängiger Such-Server. Die Plattform ist zusammen mit Elasticsearch als Industriestandard bekannt und wird in verschiedenen Anwendungen genutzt. Solr basiert auf Java und gilt als eine der besten Lösungen für die Indizierung und Abfrage von digitalen Informationen aller Art. Solr bietet unter anderem die folgenden Eigenschaften:
-	Facetten-Suche
-	Kategorisierte Suche
-	Volltextsuche
-	Gewichtung von Treffern
-	Synonymsuche
-	Mehrsprachigkeit
Bevor man Daten nach Solr importiert, wird in der Regel ein Schema definiert. Dieses Schema definiert welche Felder existieren und welche Datentype diese beinhalten dürfen. Diese Einschränkung dient dazu die Datenstruktur zu organisieren und Suchanfragen effizienter zu gestalten.  
Solr besitzt eine integrierte Suchoberfläche, diese wird normalerweise jedoch nur zu Demonstrationszwecken verwendet. Üblicherweise wird in der Produktionsumgebung eigene Benutzeroberflächen entwickelt oder auf kommerzielle Lösungen eingesetzt. 

## VuFind
 
Eine Benutzeroberfläche, welche Solr im Backend nutzt, ist VuFind. VuFind ist ein Disvery-System das für Bibliotheken entwickelt wurde. Vufind ist eine Open Source Software und eine Alternative zu kommerziellen Lösungen wie Ex Libris Primo. Ex Libris Primo ist insofern ein guter Vergleich, als dass Primo auch auf Solr basiert.
## Vergleich Solr und VuFind
In der Übung während der Vorlesung haben wir VuFind und Solr einander gegenübergestellt. Diese Ergebnisse möchte ich kurz aufgreifen:
-	Wenn man bei VuFind zu tippen beginnt, werden bereits mögliche Suchen vorgeschlagen. Dies verlang eine hohe Performance des Systems, da während des Tippens in kurzer Zeit Vorschläge gemacht werden müssen. Wenn diese Vorschläge zu langsam erscheinen, haben sie keinen Nutzen mehr. 
-	Mit VuFind werden einige Links klickbar. Diese Links können intern von VuFind verlinken oder auch nach ausserhalb führen. 
-	VuFind ermöglicht verschiedene Zusatzfunktionen im Vergleich mit Solr. Mit Vufind können beispielsweise Darstellungen der Datensätze gedruckt oder als E-Mail versendet werden (vergl. untenstehendes Bild).
-	Die Benutzeroberfläche (VuFind) ermöglicht die Darstellung der Daten in verschiedene Sprache. Mit der Einstellung der Sprache werden gewisse Daten (bspw. das Format) in die entsprechende Sprache übersetzt. 
Die Unterschiede lassen sich darin begründen, dass die beiden Software unterschiedliche Zielgruppen besitzen: Während dem Solr intern von Administratoren genutzt wird, ist VuFind als Benutzeroberfläche an die Endnutzende gerichtet. In untenstehenden Bildern ist dies nochmals ersichtlich. Es ist erkennbar, dass für Solr (erstes Bild) ein gewisses Know-How vorausgesetzt wird. VuFind hingegen setzt kein Vorwissen zum Retrieval voraus. Die einfache Suche gestaltet sich sehr leicht analog zu google. VuFind verfügt aber auch über eine erweiterte Suche und über die Suche in spezifischen Feldern. 


  

## Eigene Erfahrungen - Vergleich zu Exlibris Primo 
Abschliessend möchte ich noch einen kurzen Blick auf Ex Libris Primo werfen. Untenstehend ein Bild der Suchoberfläche des Aargauer Bibliotheksnetzes:  
Wie ersichtlich wird, ist die Suchoberfläche recht ähnlich zu VuFind. Auch die Möglichkeiten der beiden Software sind sehr ähnlich.  
Quellen:
https://www.exigo.ch/produkte/extras/solr
https://pad.gwdg.de/HW9D520ORJu79RoIEueNCw#

