---
title: "4 Archivsysteme"
date: 2024-03-12
---


# Liebes Tagebuch 

verteilt auf zwei Termine haben wir die Funktion und den Aufbau von Archivsystemen genauer betrachtet, sowie das Datenformat EAD  unter die Lupe genommen und mit ArchivesSpace gearbeitet. 

# ISAD(G)
Bis zur Einführung von Archivsystemen wurden in Archiven Findbücher eingesetzt. Diese waren handgeschriebene Bücher bzw. Sammelordner. ISAD(G) wurde 1994 eingeführt und im Jahr 2000 leicht überarbeitet. Es handelt sich um einen Standard zur archivischen Erschliessung, welches auf einem hierarchischen Modell basiert. Ausserdem wird das Provenienzprinzip berücksichtigt, d.h. die Verzeichnungseinheiten werden nach den Aktenbildnern geordnet. Im Rahmen dieses Blogbeitrags wird nicht noch weiter auf ISAD(G) eingegangen, da der Standard von einem neuen Standard nämlich Records in Context (RiC) abgelöst wird. 
# EAD
Das Datenformat Encoded Archival Description (EAD) ist ein auf XML basierender Standard zur Beschreibung von archivischem Material. EAD ist ein Austauschformat zwischen Archiven. Unter dem [Link](https://eadiva.com/) ist eine inoffizielle EAD-Dokumentation einsehbar, die von einer Einzelperson geführt wird. Beachtet werden muss, dass es verschiedene Versionen von EAD (u.a. EAD2002 und EAD3) gibt.

# Aktuelle Entwicklungen 
Untenstehend sind aktuelle Entwicklungen, die im Archivbereich zu verzeichnen sind, aufgeführt:
-	Die Einführung von RiC wird viel Aufwand bedeuten, da die Archivsoftware upgedatet werden muss oder gar auf ein neues System umgestellt werden muss. 
-	Mit dem Einsatz von Technik können immer mehr Volltexte generiert werden. Diese können noch automatisch angereicht werden durch Named Entity Recognition.
-	In Wikidata sind unter ‘archives at’ Organisationen verlinkt, die Material zum jeweiligen Thema besitzen.


#  ArchivesSpace
ArchivesSpace ist eine Open-Source Software. Es handelt sich um ein Archivinformationssystem. Der Webseite kann man entnehmen, dass es von Archivar*innen für Archive entwickelt wurde. ArchivesSpace ist eher auf Amerika ausgerichtet und profitiert von vielen zahlenden Mitgliedern. Dies ist ein Unterschied zu Koha (vergl. Blogeintrag zu [Koha](https://nathaliewic.github.io/lerntagebuch/2024/02/27/Funktion-und-Aufbau-von-Bibliothekssystemen.html). ArchivesSpace basiert auf verschiedenen Standards: DACS, ISAD(G)und ISAAR(CPF). Ausserdem werden der Import und Export von EAD-Daten, MARCXML-Daten und METS-Daten unterstützt. Beim Import gilt es zu beachten, dass selten ein verlustfreier Import gelingt. Es bedarf folglich einer Kontrolle der importierten Daten. Nichtsdestotrotz kann der Import Zeit sparen, da Daten von Hilfsmitarbeitenden ins System integriert werden können. 

# Persönliche Erfahrungen und Vergleiche
In meiner Ausbildung beim Staatsarchiv Bern haben wir auch Daten nach scopeArchiv importiert. Konkret handelte es sich um Daten von den Aktenbildnern. Dabei handelte es sich meist um CSV-Dateien. Häufig waren es Listen in denen beschrieben war, welche Dokumente in den jeweiligen Ordnern/Schachteln zu finden sind. Dies hat die Erschliessungsarbeit enorm vereinfacht, da es oftmals schwierig ist, den genauen Kontext der Entstehung zu rekonstruieren.

Unterschiede zu scopeArchiv, welche mir aufgefallen sind:
-	‘Unprocessed material’: die Daten, welche noch nicht erschlossen wurden, haben wir nicht im Katalog sichtbar gemacht. Einerseits bietet es zwar für die Nutzenden einen Überblick ‘was hinter den Kulissen’ passiert, andererseits könnte ich mir vorstellen, dass es für Verwirrung sorgt, wenn man Unterlagen publiziert, welche noch nicht vollständig erschlossen wurden.
-	Die Funktion ‘Calculate’: diese gab es nicht bei scopeArchiv. Ich musste jeweils die Laufmeter der einzelnen Einheiten manuell addieren. Dies ist eine Fehlerquelle und insofern bei ArchivesSpace besser gelöst.
-	scopeArchiv hat meinem Empfinden nach, eine einfachere Struktur. Den Wechseln zwischen den Modulen in ArchivesSpace fand ich verwirrend.
