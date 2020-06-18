#Lerntagebucheintrag zum Block 4

Liebes Lerntagebuch, 

Die zwei Hauptthemen des Blocks vom 5. Juni 2020 waren MarcEdit und VuFind. Angefangen haben wir jedoch mit OpenRefine. 

OpenRefine ist XXX. Als Hausaufgabe sollten wir die Library Carpentry Lessons bearbeiten. [Mehr dazu]
OpenRefine untersützt Formate, die für die Darstellung tabellarischer Daten verwendet werden, wie CSV, TSV oder auch XLS und XLSX. Man kann damit auch einfache XML- und JSON-Formate gestalten (wenn man etwas Übung darin hatte). Komplexe XML-Formate mit Hierarchien sind auch möglich, jedoch braucht man dazu zusätzliche Tools. Ausserdem kann OpenRefine zusammen mit MarcEdit für MARC21 benutzt werden. 

Die Haupteinsatzmöglichkeiten von OpenRefine sind: Exploration von Datenlieferungen, Vereinheitlichung und Bereinigung undAbgleich mit Normdaten in Wikidata, GND und VIAF. 

Nun kommen wir zu MarcEdit, was xxx ist. Wir haben eine Gruppenarbeit dazu bekommen und zwar sollten wir XLS-Transformationen bzw. Crosswalks vornehmen. Crosswalks werden zur Konvertierung vone einem Metadatenbestand in einen anderen verwendet. So kann man beispielsweise MARC21 zu DublinCore umkonvertieren. Crosswalks beinhalten auch Regeln, z.B. wie Elemente zugeordnet werden müssen. Dabei ist meist eine 1:1-Konvertierung eigentlich unmöglich. 
Ausserdem ist ein XSLT eine Programmiersprache zur Transformation von XML-Dokumenten. 
Die Aufgabe ging wie folgend: 
1) Nach Start des Programms wählt man den Icon "MARC Tools" aus. 
2) Somit bekommt man ein Fenster, wo man eine Datei zum Öffnen auswählen kann und deren Speicherort angeben muss. Herr Lohmeier hat uns dabei eine spezielle Datei bereits zur Verfügung gestellt, sodass diese nun geöffnet werden konnte und ich habe sie auf dem Desktop abspeichern wollen. 
3) Oberhalb dieser beiden Felder befindet sich auch das Feld "Select Operation", in dem man auswählen kann, von welchem Format in welchen man die Datei konvertieren möchte. Ich wähle hier bspw. MARC zu JSON. 
4) Auch habe ich das Kästchen Translate to UTF-8 angekreuzt (obwohl ich mir nicht sicher bin, ob das etwas gebracht hat). 
5) Sobald man auf "Execute" (oben rechts) klickt, wird die Datei nun im neuen Format auf meinem Desktop gespeichert und dort konnte ich sie auch aufrufen. 
Bei der Übung selbst habe ich folgende Formate ausprobiert:
- MARC –> JSON
- MARC –> DublinCore
- MARC21 –> MARC21XML

Als nächstes haben wir uns weiter etwas Theorie angeschaut: Schnittstellen SRU, OAI-PMH und Z39.50
Im Bibliotheks- sowie Archivbereich gibt es viele Übertragungsrpotokolle, die verwendet werden. Die am besten verbreitet sind: SRU (Search/Retrieve via URL (von der Library of Congress)), OAI-PMH (Open Archives Initiative Protocol for Metadata Harvesting (von Open Archives Initiative)) und Z39.50 (von der Library of Congress). 
Z39.50 und SRU werden eher für Live-Abfragen oder gezielten Datenabruf mit vielen Parametern geeignet, wobei OAI-PMH bei grösseren Datenabzügen und regelmässigen Aktualisierungen zum Einsatz kommt. Bei SRU und OAI-PMH werden die Anfragen mittels URL genertiert und sind daher direkt im Browser abrufbar. 
Dazu haben wir ebenfalls eine Aufgabe bekommen. Wir sollten uns die Dokumentation zur SRU-Schnittstelle von der Swissbib durchlesen und eine Abfrage mit den Parametern "Katalog der Bibliothek der FH Graubünden", "Suche über alle Felder nach Suchbegriff: open" und "Format:MARC XML - swissbib" stellen. Das sah wie folgt aus:
1) Auf der Webseite https://sru.swissbib.ch/sru/form muss man im ersten Feld oben links "dc.possessinginstitution" anstatt "dc.id" auswählen. Als "value" (weiter rechts) gibt man den Code für die FH Graubünden ein, der E27 wäre.
2) Im nächsten Feld wählt man "dc.anywhere" anstatt "dc.id" aus und gibt unter "value" "open" ein. 
3) Der letzte Parameter "Format: MARC XML - swissbib" ist bereits eingestellt unter "RecordSchema". 
4) Wenn man auf SubmitQuery klickt bekommt man dann 1146 Treffer. 
Die zweite und dritte Aufgabe habe ich dann nicht mehr gemacht.. 

Danach befassten wir uns mit ein paar Tools zur Metadatentransformation (Catmandu (Perl), Metafacture (Java) und OAI harvester für die Kommandozeile) sowie mit der Nutzung von JSON-APIs (z.B. lobid-gnd oder dem Tool ScrAPIr). 

Ein nächster wichtiger Punkt was die Besprechung der Hausaufgabe zu "Solr". Solar ist ein Industriestandard und kann Formate wie .doc, .xml oder .ppt importieren. Vor dem Import sollte festgehalten werden, wie das Schema der Daten aussieht. Und für uns wichtig: VuFind basiert auf Solr. [Mehr zur Hausaufabe)

Nun zur nächsten Aufgabe: VuFind. 
Wir sollten während dem Unterricht das Program "VuFind" auf unserer virutellen Maschine installieren. Bisher waren solche Installationen nicht gross problematisch, jedoch war diese Installation mehr als kompliziert. Obowhl wir eine ziemlich genaue Anleitung mit allen Codes zur Eingabe im Terminal bekommen haben, war die Installation nur bei einigen Personen von Anfang an erfolgreich. Bei mir gab es das Problem, dass obwohl ich alle Codes der Reihe nach und geduldig eingegeben hab, wollte das System nicht alle Archive herunterladen, sodass die Installation nur teilweise erfolgreich war. Aufgrund der fehlenden Archive war auch der Start des Programms nicht möglich. Ich habe mehrmals versucht, die gleichen Codes neu einzugeben, jedoch brachte das keinen Erfolg (war ich vermutet habe, jedoch trotzdem ausprobieren wollte, ob etwas besser gehen würde). "Dank" der Probleme, die auch andere Studierenden hatten, haben sich einige Lösungsmöglichkeiten entwickelt, die ich ebenfalls zu anwenden versucht habe. Kein Erfolg. Da Herr Lohmeier auch sehr mit den Problemen anderer Personen beschäftigt war, konnte ich nicht direkt Hilfe holen (die Gruppenmitglieder wussten auch nicht weiter) und so endete auch schon das Abenteuer mit VuFind. Wir haben uns die Ergebnisse anderer Gruppen trotzdem noch angeschaut bzw. klärten Fragen auf, jedoch war das weniger hilfreich, als wenn ich die Möglichkeit gehabt hätte, das System selbst auszuprobieren. 

Nach einem kleinen Marktüberblick über die Discovery-Systeme beendeten wir auch schon den Block 4. 
