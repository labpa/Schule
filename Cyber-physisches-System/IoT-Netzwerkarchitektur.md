# IoT Netzwerkarchitektur und -design

## ETSI M2M Standardisierte Architektur
Ziel des Modells ist es einen gemeinsamen Rahmen für das Verständnis der Plazierung verscheidener Standards und Protokolle in einem IoT-System zu schaffen.  
Das Modell umfasst drei Bereiche:
+ Anwendungsbereich  
Managementfunktionen wie Datenanalyse, Konnektivitätsmanagement, intelligentes Energiemanagement, Fuhrparkmanagement und andere können auftreten.

+ Netzwerkbereich  
hier verlassen die Daten das lokale Netzwerk und werden mit Hilfe von drahtgebundenen und drahtlosen Protokollen zum Anwendungsbereich transportiert.

+ M2M Device Domain  
hier werden Endgeräte wie Sensoren, Aktoren und Steuerungen über M2M-Gateways mit dem Netz verbunden

|Schicht|Name|Funktion|
|:---:|---|---|
|7|Collaboration & Processes (Involving people and business processes)||
|6|Application (Reporting, analytics, control)||
|5|Data Abstraction (Aggregation and access)||
|4|Data Accumulation (Storage)||
|3|Edge (Fog) Compiuting (Data element analysis and transformation)||
|2|Connectivity (Connection and processing units)||
|1|Physical Devices & Controllers||

1. Schicht beherbergt die Dinge in der Internetbewegung. Endgeräte, verscheidene Sensoren. Alle Dinge, die Informationen Senden und Empfangen können. Ein Ding wird es in dem Moment, in dem es seine Umgebung wahrnehmen kann.

Eine Entsprechende Schicht fehlt im OSI Modell (1. Schicht)

2. 

3. Edge. Umwandlung von Daten. Die Informationsverarbeitung so früh wie möglich am Rand des Netzwerkes

4. Datensammlung. Erfasste Daten werden gespeichert. Die Daten werden konvertiert. 

5. Gleicht mehrere Datenformate ab. Viele Quellen werden verglichen. Vollständigkeit würd geprüft. Datanabstraktion wird geboten. Datenvirtualisierung. Aggregiert

6. Interpretation von Daten mit Softwareanwendungen. Überwachen, Berichte erzeugen. Datenanalyse findet hier statt. 

7. Eigene Daten werden mir Vergleichswerten Verbunden. Verscheidene Buisseness intelegent Lösungen teilen Daten aus und fügen dieße Werte zusammen.