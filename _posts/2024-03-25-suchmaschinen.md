---
title: "9 Suchmaschinen und Discovery Systeme II"
date: 2024-05-28
---

9 Suchmaschinen und Discovery Systeme II 
# Liebes Tagebuch
In dieser Vorlesung haben wir uns mit der Datenintegration und der Konfiguration von VuFind beschäftigt. In diesem Blogbeitrag möchte ich auf die Übungen, die wir in der Vorlesung gemacht haben, eingehen. Mit der Dateintegration sind also verschiedene Dinge zusammengekommen: Die Daten aus Koha, ArchivesSpace und DSpace haben wir nach VuFind integriert. 
# Übung 1
Wie bereits angetönt sollten wir in der 1. Übung die Daten von Koha, ArchivesSpace und DSpace nach VUfind importieren. Der Import der Daten von Koha und OpenRefine hat ohne Probleme funktioniert. Die Umbenennung der Institution hat zuerst jedoch nicht funktioniert, da wir vergessen haben die Zeile auszukommentieren. Als wir das Problem erkannt haben und korrigieren konnten, hat es dann funktioniert. In der Besprechung in der Klasse kam heraus, dass dies oftmals ein Fehler ist, der gemacht wird.  
Wie in der Auftragsstellung angekündigt wurde bei DSpace eine Fehlermeldung angezeigt. Die Fehlermeldung ist untenstehend ersichtlich. Der Fehler liegt darin, dass das Pflichtfeld ‘ID’ fehlt. Vufind liest marc21 daten und interpretiert die, und schickt die an solr. Solr (Link zur vorherigem Blogbeitrag) löst diese Fehlermeldung aus, da das seitens von Solr, wie erwähnt, ein Pflichtfeld ist.
 ![image](https://github.com/nathaliewic/lerntagebuch/assets/160014832/cfdbf21d-f3e6-4d7d-8128-4bb745a5888c)

Untenstehend der kontrollierte Datensatz. Darin ist ersichtlich, dass das Feld 001 ein controlfield ist. Dies ist wichtig zu beachten, denn ansonsten entsteht eine Fehlermeldung. In der Vorlesung haben wir (bzw. der Dozent) das Problem manuell behoben. In der Praxis würde man entweder den Export anpassen oder das Feld automatisiert anpassen. 
 ![image](https://github.com/nathaliewic/lerntagebuch/assets/160014832/82c01125-b081-4760-882d-e39a64977306)

Das Ergebnis der 1. Übung konnte dann in den Institutionen gesehen werden. Wir haben für OpenRefine und Koha eine einzelne Institutionen gemacht, was in der Praxis vermutlich weniger praktikabel ist, weil in der Institution Koha nur ein Datensatz enthalten ist. Dadurch hätte es in diesem Fall vermutlich mehr Sinn gemacht nur eine Institution zu erstellen. 
 ![image](https://github.com/nathaliewic/lerntagebuch/assets/160014832/f624aa92-2254-45d4-aba1-241d093ceb5a)


# Übung 2
Die zweite Übung betraf die Konfiguration von VuFind. Durch die Übung wurden die unterschiedlichen Konfigurationsmöglichkeiten sichtbar. Unsere Gruppe hat diverse Anpassungen am Design vorgenommen. Beispielsweise haben wir das Bild des Mediums auf die linke Seite verschoben. Dies wird mit dem Befehl ‘sidebarOnLeft = true’ erreicht.
Des Weiteren haben wir das Theme auf bootstrap3 geändert.
 ![image](https://github.com/nathaliewic/lerntagebuch/assets/160014832/d68cd656-076b-4e0a-adaa-f0b91f1b8cec)

Ausserdem haben wir den Tab-Titel geändert. Selbsterklärend würde man in der Praxis einen sinnvolleren Titel wählen. Hinzukommend haben wir auch noch den separator angepasst. Zwischen ‘Suchergebnisse’ und ‘hallihallo :)’ wird neu ein ‘-‘ verwendet. Standard ist das Doppelzeichen.
 
![image](https://github.com/nathaliewic/lerntagebuch/assets/160014832/90b955f8-8af2-4f87-8328-729f1a52474a)

# Marktüberblick - Vergleich von Software
Im Rahmen dieses Blogbeitrags kann ich nicht umfassend auf den Markt eingehen. Dies würde nämlich den Rahmen sprengen. Was jedoch gesagt werden kann, ist das in den letzten Jahren eine starke Marktkonzentration stattgefunden hat. In Hinblick auf die Zukunft bringt dies diverse Herausforderungen mit sich. Beispielsweise wird von Seiten der Besitzer der Anbieterfirmen das User Tracking ein grosses Interesse sein. Für die Bibliotheken gilt es also in Hinblick auf die Zukunft die Interessen der Nutzenden zu vertreten und sich für den adäquaten Datenschutz einzusetzen. 

