---
title: "7 Metadaten und Schnittstellen I"
date: 2024-04-05
---

# Liebes Tagebuch
in dieser Lerneinheit bzw. Lerneinheiten haben wir uns, über zwei Vorlesungen hinweg, mit Metadaten & Schnittstellen beschäftigt. In erster Linie haben wir uns dafür mit OpenRefine beschäftigt. ChatGPT liefert untenstehend die Definition von OpenRefine: 
![image](https://github.com/nathaliewic/lerntagebuch/assets/160014832/95a98ba5-c92c-4426-a3fd-76ef079b217a)


Insbesondere die grafische Benutzerfläche ist ein grosser Vorteil von OpenRefine. Hinzukommend ist auch die Datenanalyse & die Datenanreicherung ein wichtiger Punkt, der in der Definition von ChatGPT keine oder zumindest zu wenig Beachtung findet. Hinzukommend wird der reconciliation von OpenRefine eine grosse Bedeutung zugesprochen. Dadurch können Daten mit externen Services, wie bspw. Wikidata, abgeglichen werden. Nützlich ist auch, dass viele Formate von OpenRefine unterstützt werden, dazu gehören CSV, TSV, XLS, XLSX, TXT, XML und JSON. Zusammen mit MarcEdit kann OpenRefine auch für die Analyse bzw. Transformation von MARC21 genutzt werden.

Nun ist geklärt, um was es sich bei OpenRefine handelt. In der Folge haben wir OpenRefine über das Codespace gestartet. Dies war dank der guten Anleitung & Vorbereitung des Dozenten (auch für nicht Informatikerinnen) recht einfach zu bewerkstelligen. Der Dozent hat uns dann einige Basisfunktionen gezeigt, dazu gehörten Split, Cluster and edit und join. 

# Anwendung

Folglich haben wir uns dann selbst ans Ausprobieren gewagt. Zunächst erhielten wir noch einen Input zum Abgleich von Daten mittels Wikidata. Es war sehr interessant zu sehen und mitzuverfolgen, wie dieser Abgleich funktioniert. Nämlich ist reconciliation, wie erwähnt eine wichtige Funktion der Software OpenRefine.   
Mittels ‘Reverse Engineering’ haben wir uns mit den Feldern & der Syntax vertraut gemacht. Nachfolgend eine Erklärung zu Feld 100. Das Feld 100 wird jeweils für die Hauptverantwortlichkeitsangabe genutzt und kann nur ein einziges Mal pro Katalogisat vergeben werden. Aus diesem Grund wird jeweils die erste Person in Feld 100 eingetragen und die weiteren Personen in Feld 700. Das Feld 700 darf mehrmals genutzt werden. Die genaue Bedeutung der einzelner Felder kann [hier](https://www.loc.gov/marc/bibliographic/) nachgeschaut werden.
![image](https://github.com/nathaliewic/lerntagebuch/assets/160014832/f7cc955a-8a32-4984-a024-7e481cb03020)

-	Mit ‘datafield’ wird das Feld ausgewiesen, das folglich befüllt wird. Nachher werden die beiden Indikatoren erwähnt. Der erste Indikator ‘1’ bedeutet, dass es sich um ein Nachname handelt.

-	In Unterfeld a wird die Zelle ‘Authors’ nach dem Zeichen "|" aufgeteilt. Der Erste Wert wird genommen und an dieser Stelle geschrieben. 
-	Der Befehl ‘escape.xml’ stellt sicher, dass auch nicht XML konforme Zeichen korrekt ausgegeben werden. Ein Beispiel für ein solche Zeichen sind die Umlaute (ä, ö, ü).
In untenstehendem Bild wird das Feld 700, für die weiteren Verantwortlichkeiten, dargestellt:
![image](https://github.com/nathaliewic/lerntagebuch/assets/160014832/5e338dae-d2a2-49cf-be78-30e2a3952a0e)

-	forEach führt dazu, dass jeweils der nächste Wert (also in diesem Fall die Personenangabe) genommen wird und in das Feld eingefügt wird. Nach dem ‘slice’ wird der Wert in die Variable ‘v’ eingefügt und untenstehend bei ‘v.escape’ referenziert. 
-	Dies wird für jeden weiteren Namen getan.
Abschliessend haben wir versucht, ausgehend von einer CSV-Datei, einige Felder nach MARC-XML zu transformieren. Nach anfänglichen Schwierigkeiten hat dies gut funktioniert. Hilfreich war hierfür, dass wir alle die Bedeutungen der Felder kannten.

Um den Bogen zum Anfang zu spannen, gehe ich noch auf einen Punkt ein, der ChatGPT bereits angesprochen hat. OpenRefine gehörte anfänglich zu google – google hatte jedoch keine Verwendung mehr für die Software und ‘übergab’ sie der OpenSource Community. 

