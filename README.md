# CovidDataAnalysis
 
Datenquelle: Robert Koch Institut 

Terms of Use: Robert Koch-Institut; Bundesamt für Kartographie und Geodäsie 

Credits (Attribution): Robert Koch-Institut; Bundesamt für Kartographie und Geodäsie



Die Daten sind die „Fallzahlen in Deutschland“ des Robert Koch-Institut (RKI) und stehen unter der Open Data Datenlizenz Deutschland – Namensnennung – Version 2.0 zur Verfügung. 

Quellenvermerk: Robert Koch-Institut (RKI), dl-de/by-2-0



Haftungsausschluss: „Die Inhalte, die über die Internetseiten des Robert Koch-Instituts zur Verfügung gestellt werden, dienen ausschließlich der allgemeinen Information der Öffentlichkeit, vorrangig der Fachöffentlichkeit“. Erfahren Sie mehr hier. 

Datenschutzerklärung: „Die Nutzung des Webangebotes des RKI ist grundsätzlich ohne Bekanntgabe personenbezogener Daten möglich“. Erfahren Sie mehr hier. 



Beschreibung der Daten des RKI Covid-19-Dashboards (https://corona.rki.de)

Dem Dashboard liegen aggregierte Daten der gemäß IfSG von den Gesundheitsämtern an das RKI übermittelten Covid-19-Fälle zu Grunde
Mit den Daten wird der tagesaktuelle Stand (00:00 Uhr) abgebildet und es werden die Veränderungen bei den Fällen und Todesfällen zum Vortag dargstellt
In der Datenquelle sind folgende Parameter enthalten:
IdBundesland: Id des Bundeslands des Falles mit 1=Schleswig-Holstein bis 16=Thüringen
Bundesland: Name des Bundeslanes
Landkreis ID: Id des Landkreises des Falles in der üblichen Kodierung 1001 bis 16077=LK Altenburger Land
Landkreis: Name des Landkreises
Altersgruppe: Altersgruppe des Falles aus den 6 Gruppe 0-4, 5-14, 15-34, 35-59, 60-79, 80+ sowie unbekannt
Altersgruppe2: Altersgruppe des Falles aus 5-Jahresgruppen 0-4, 5-9, 10-14, ..., 75-79, 80+ sowie unbekannt
Geschlecht: Geschlecht des Falles M0männlich, W=weiblich und unbekannt
AnzahlFall: Anzahl der Fälle in der entsprechenden Gruppe
AnzahlTodesfall: Anzahl der Todesfälle in der entsprechenden Gruppe
Meldedatum: Datum, wann der Fall dem Gesundheitsamt bekannt geworden ist
Datenstand: Datum, wann der Datensatz zuletzt aktualisiert worden ist
NeuerFall: 
0: Fall ist in der Publikation für den aktuellen Tag und in der für den Vortag enthalten
1: Fall ist nur in der aktuellen Publikation enthalten
-1: Fall ist nur in der Publikation des Vortags enthalten
damit ergibt sich: Anzahl Fälle der aktuellen Publikation als Summe(AnzahlFall), wenn NeuerFall in (0,1); Delta zum Vortag als Summe(AnzahlFall) wenn NeuerFall in (-1,1)
NeuerTodesfall:
0: Fall ist in der Publikation für den aktuellen Tag und in der für den Vortag jeweils ein Todesfall
1: Fall ist in der aktuellen Publikation ein Todesfall, nicht jedoch in der Publikation des Vortages
-1: Fall ist in der aktuellen Publikation kein Todesfall, jedoch war er in der Publikation des Vortags ein Todesfall
-9: Fall ist weder in der aktuellen Publikation noch in der des Vortages ein Todesfall
damit ergibt sich: Anzahl Todesfälle der aktuellen Publikation als Summe(AnzahlTodesfall) wenn NeuerTodesfall in (0,1); Delta zum Vortag als Summe(AnzahlTodesfall) wenn NeuerTodesfall in (-1,1)
Referenzdatum: Erkrankungsdatum bzw. wenn das nicht bekannt ist, das Meldedatum
AnzahlGenesen: Anzahl der Genesenen in der entsprechenden Gruppe
NeuGenesen:
0: Fall ist in der Publikation für den aktuellen Tag und in der für den Vortag jeweils Genesen
1: Fall ist in der aktuellen Publikation Genesen, nicht jedoch in der Publikation des Vortages
-1: Fall ist in der aktuellen Publikation nicht Genesen, jedoch war er in der Publikation des Vortags Genesen
-9: Fall ist weder in der aktuellen Publikation noch in der des Vortages Genesen 
damit ergibt sich: Anzahl Genesen der aktuellen Publikation als Summe(AnzahlGenesen) wenn NeuGenesen in (0,1); Delta zum Vortag als Summe(AnzahlGenesen) wenn NeuGenesen in (-1,1)
IstErkrankungsbeginn: 1, wenn das Refdatum der Erkrankungsbeginn ist, 0 sonst
In der Tabelle werden die bundesweit einheitlich erfassten und an das Robert Koch-Institut (RKI) übermittelten Daten zu bestätigten COVID-19-Fällen dargestellt. COVID-19-Verdachtsfälle und -Erkrankungen sowie Nachweise von SARS-CoV-2 werden gemäß Infektionsschutzgesetz an das zuständige Gesundheitsamt gemeldet. Die Gesundheitsämter ermitteln ggf. zusätzliche Informationen, bewerten den Fall und leiten die notwendigen Infektionsschutzmaßnahmen ein. Die Daten werden spätestens am nächsten Arbeitstag vom Gesundheitsamt elektronisch an die zuständige Landesbehörde und von dort an das RKI übermittelt. Am RKI werden sie mittels weitgehend automatisierter Algorithmen validiert.

Es werden nur Fälle veröffentlicht, bei denen eine labordiagnostische Bestätigung unabhängig vom klinischen Bild vorliegt. Die Daten werden am RKI einmal täglich jeweils um 00:00 Uhr prozessiert. Die Daten stehen dann in den frühen Morgenstunden aktualisiert im Layer zur Verfügung.

Die Fälle werden dem Bundesland bzw. Landkreis zugeordnet, aus dem der Fall übermittelt worden ist, das entspricht in der Regel dem Wohnort bzw. gewöhnlichen Aufenthaltsort der Fälle und nicht dem Ort, wo sich die Person wahrscheinlich angesteckt hat. Für den regionalen Vergleich der Häufigkeit einer Krankheit (z.B. zwischen Kreisen oder Bundesländern) sollte anstelle der absoluten Fallzahlen die Inzidenz (Anzahl der Fälle pro 100.000 Einwohner) betrachtet werden, um Unterschiede in den Bevölkerungszahlen zu berücksichtigen. Die zur Inzidenzberechnung herangezogenen Bevölkerungszahlen werden von den Statistischen Landesämtern bereitgestellt. Bei der Darstellung der Neuinfektionen pro Tag wird das Meldedatum verwendet, also das Datum, an dem das GA Kenntnis von dem Fall erlangt und ihn als solchen elektronisch erfasst.



Disclaimer zu Genesenen:

Anhand der dem RKI von den Gesundheitsämtern übermittelten Detailinformationen zu einem Erkrankungsfall wird für jeden Fall eine Dauer der Erkrankung geschätzt. Für Fälle, bei denen nur Symptome angegeben sind, die auf einen leichten Erkrankungsverlauf schließen lassen, wird eine Dauer der Erkrankung von 14 Tagen angenommen. Bei hospitalisierten Fällen oder Fällen mit Symptomen, die auf einen schweren Verlauf hindeuten (z.B. Pneumonie) wird eine Dauer der Erkrankung von 28 Tagen angenommen. Ausgehend vom Beginn der Erkrankung, bzw. wenn der nicht bekannt ist, vom Meldedatum ergibt sich ein geschätztes Datum der Genesung für jeden Fall. Da im Einzelfall auch deutlich längere Erkrankungsverläufe möglich sind, bzw. die hier genutzten Informationen nicht bei allen Fällen dem RKI übermittelt werden, sind die so berechneten Daten nur grobe Schätzungen für die Anzahl der Genesenen und sollten daher auch nur unter Berücksichtigung dieser Limitationen verwendet werden.
