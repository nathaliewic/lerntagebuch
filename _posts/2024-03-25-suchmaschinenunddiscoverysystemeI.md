---
title: "9 Suchmaschinen & Discovery-Systeme I"
date: 2024-05-27
---

# Liebes Tagebuch
in dieser Vorlesung haben wir uns mit Suchmaschinen & Discovery-Systemen beschäftigt. Zunächst gab es einen Nachtrag zu den Metadaten & den Schnittstellen. In diesem Blogbeitrag soll es aber um das neue Thema gehen. Bei Bedarf kann der Nachtrag [hier](https://pad.gwdg.de/HW9D520ORJu79RoIEueNCw) nachgelesen werden.
Dann ging es an das eigentliche Thema: In einer Live-Demonstration hat uns der Dozent die Installation & Konfiguration von VuFind nähergebracht. In dem folgen Blogbeitrag soll nun vertieft auf Solr & VuFind eingegangen werden. 
# Solr
![image](https://github.com/nathaliewic/lerntagebuch/assets/160014832/c26813cd-ce48-4ead-bb0c-eec413ec0d74)

Solr ist ein plattformunabhängiger Such-Server. Die Plattform ist zusammen mit Elasticsearch als Industriestandard bekannt und wird in verschiedenen Anwendungen genutzt. Solr basiert auf Java und gilt als eine der besten Lösungen für die Indizierung und Abfrage von digitalen Informationen aller Art. Solr bietet unter anderem die folgenden Eigenschaften:
-	Facetten-Suche
-	Kategorisierte Suche
-	Volltextsuche
-	Gewichtung von Treffern
-	Synonymsuche
-	Mehrsprachigkeit
Bevor man Daten nach Solr importiert, wird in der Regel ein Schema definiert. Dieses Schema definiert welche Felder existieren und welche Datentypen diese beinhalten dürfen. Diese Einschränkung dient dazu die Datenstruktur zu organisieren und Suchanfragen effizienter zu gestalten.  
Solr besitzt eine integrierte Suchoberfläche, diese wird normalerweise jedoch nur zu Demonstrationszwecken verwendet. Üblicherweise wird in der Produktionsumgebung eigene Benutzeroberflächen entwickelt oder auf kommerzielle Lösungen eingesetzt. 

# VuFind
![image](https://github.com/nathaliewic/lerntagebuch/assets/160014832/a5f81d48-b219-4b15-8e17-a5800d719b36)

VuFind ist ein Disvery-System das für Bibliotheken entwickelt wurde. Vufind ist eine Open Source Software und eine Alternative zu kommerziellen Lösungen wie Ex Libris Primo. Ex Libris Primo ist insofern ein guter Vergleich, als dass Primo auch auf Solr basiert.

# Vergleich Solr & VuFind
In der Übung während der Vorlesung haben wir VuFind & Solr einander gegenübergestellt. Diese Ergebnisse möchte ich kurz aufgreifen:
-	Wenn man bei VuFind zu tippen beginnt, werden bereits mögliche Suchen vorgeschlagen. Dies verlang eine hohe Performance des Systems, da während des Tippens in kurzer Zeit Vorschläge gemacht werden müssen. Wenn diese Vorschläge zu langsam erscheinen, haben sie keinen Nutzen mehr. 
-	Mit VuFind werden einige Links klickbar. Diese Links können intern von VuFind verlinken oder auch nach ausserhalb führen. 
-	VuFind ermöglicht verschiedene Zusatzfunktionen im Vergleich mit Solr. Mit Vufind können beispielsweise Darstellungen der Datensätze gedruckt oder als E-Mail versendet werden (vergl. untenstehendes Bild).
-	Die Benutzeroberfläche (VuFind) ermöglicht die Darstellung der Daten in verschiedene Sprache. Mit der Einstellung der Sprache werden gewisse Daten (bspw. das Format) in die entsprechende Sprache übersetzt.
-	
Die Unterschiede lassen sich darin begründen, dass die beiden Software unterschiedliche Zielgruppen besitzen: Während dem Solr intern von Administratoren genutzt wird, ist VuFind als Benutzeroberfläche an die Endnutzende gerichtet. In untenstehenden Bildern ist dies nochmals ersichtlich. Es ist erkennbar, dass für Solr (erstes Bild) ein gewisses Know-How vorausgesetzt wird. VuFind hingegen setzt kein Vorwissen zum Retrieval voraus. Die einfache Suche gestaltet sich sehr leicht analog zu google. VuFind verfügt aber auch über eine erweiterte Suche und über die Suche in spezifischen Feldern. 

![image](https://github.com/nathaliewic/lerntagebuch/assets/160014832/067aa682-33cd-4eed-bae8-c93efdc1c82d)

![image](https://github.com/nathaliewic/lerntagebuch/assets/160014832/1c60efcd-7b7c-4b13-8fe1-96134a1752cc)
  

# Quellen:
<https://www.exigo.ch/produkte/extras/solr>

<https://pad.gwdg.de/HW9D520ORJu79RoIEueNCw#>

