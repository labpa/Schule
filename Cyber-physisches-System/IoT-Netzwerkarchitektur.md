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

### Schicht 1: Dinge: Sensoren und Aktoren Schicht
Es gibt unzählige Möglichkeiten, intelligente Objekte zu klassifizieren. Eine architektonische Klassifizierung könnte sein:
+ Batteriebetrieb oder Netzbetrieb
+ Mobil oder stationär -> klärt mögliche Energiequelle
+ Niedrige oder hohe Meldefrequent -> Höhere Frequenzen bedingen einen höheren Energieverbrauch
+ Einfache oder umfangreiche Daten
+ Report-Reichweite
+ Objektdichte pro Zelle


Beispiele:
+ **Energiequelle:**  batteriebetriebe, netzbetrieben, Solar betrieben, kinetisch betrieben
+ **Mobilität:** stationär, mobil, tragbar
+ **Sensorik:** Temperatur, Luftfeuchtigkeit, Bewegung, Licht, Beschleunigung, Druck, Lautstärke, CO2-Gehalt, Luftqualität
+ **Datenkomplexität:** einfache Daten (z.B. Temperatur), komplexe Daten (z.B. maschinelles Lernen)
+ **Drahtlose Kommunikation:** WLAn, Bluetooth, NFC, Mobilfunk, LoRaWAN
+ **Verbindungstyp:** Punkt-zu-Punkt, Mesh, Stern
+ **Report-Reichweite:** kurz, mittel, lang
+ **Objektdichte pro Zelle:** gering, mittel, hoch
+ **Verwendungszweck:** Heimautomation, industrielle Automatisierung, Smart-City, Gesundheitswesen, Landwirtschaft
+ **Echtzeit-Anforderungen:** Echtzeit-Verarbeitung, zeitlich unempfindlich

### Schicht 2: Kommunikationsschicht
Anbinden von Dingen an das Netzwerk

+ **Kommunikationsnetzwerk-Schicht:** Schicht zwei wird in vier weitere Teilschichten aufgeteilt.
    + Zugangsnetzwerk-Sublayer
    + Gateways und Backhaul-Netzwerk-Teilschicht
    + Netzwerk-Transport-Teilschicht
    + Iot-Netzwerkmanagement-Teilschicht

#### Einteilung nach Reichweiten (Entfernungsklassen im IoT)
+ PAN (Personal Area Network)
+ HAN (Home Area Network)
+ NAN (neighborhood area network)
+ FAN (field area network)
+ LAN (Local Area Network)

### Schicht 3: Anwendungs und Analyseschicht

#### Analyse- versus Steuerungsanwendung
Mehrere Anwendungen können dazu beitragen, die Effizienz eines IoT-Netzwerks zu steigern. Jede Anwendung sammelt Daten und bietet eine Reihe von Funktionen, die auf der Analyse der gesammelten Daten basiert. Es kann schwierig sein, die angebotenen Funktionen zu vergleichen.
+ Analyse Anwendung:
    + sammelt Daten von meheren intelligenten Objekten, verarbeitet die gesammelten Daten und zeigt Informationen an, die sich aus den verarbeiteten Daten ergeben.

+ Steuerungsanwendung
    + Steuert das Verhalten des Smart-Objekts ider das Verhalten eines mit dem Smart-Objekt verbundenen Objekts. Zum Beispiel kann ein Drucksensor mit einer Pumpe verbunden sein.

#### Daten- versus Netzwerkanalyse
Analytik ist ein allgemeiner Begriff, der die Verarbeitung von Informationen beschreibt, um aus dem gesammelten Daten einen Sinn zu machen. In der Welt des IoT ist eine mögliche Klassifizierung der Analysefunktion wie folgt:

+ Datenanalytik

* Netzwerk-Analytik

#### Erklärung DAtenarten
