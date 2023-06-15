# Sicherung und Wiederherstellung
## Was sind Daten / Unternehmensdaten?
Es gibt unterscheidliche Arten von Unternehmensdaten.

+ Kundendaten
+ Produktionsdaten
+ Finanzdaten
+ Mitarbeiter
+ Planungsdaten

Was ist der Wert der Daten und wie definiert sich der Wert.

+ Arten von Daten
+ Speicheranforderung
+ Analyse von Daten
Sicherstellung der Sicherheit
Integration von Daten
Allgemein Verwalten von Daten

## Backup
+ kurz - mittelfristig
+ Schnelle wiederherstellung von Daten (IT-Safety)
+ werden ständig erneuert
+ Speichermedium muss räumlich getrennt sein
+ Sicherungskopie
+ Durchführung mit geeignetem Speichermedium

## Archivierung

 
|**Backup**| **Archivierung**|
|---|---|


|kurz-mittelfristig| langfristige Sicherung|

|regelmäßige Sicherungskopie wichtiger Daten|Daten werden dauerhaft in Archiv verschoben|

|Sicherung im Fall von DAtenverlust, Festplattenausfall, Cyberangriff...| Erfüllung gesetzlicher/brachenspezifischer Vorgaben/Regelungen|

|Daten werden in regelmäßigen Abständen überschrieben| Daten werden archiviert und danach nicht verändert|

## Speichermedien
+ USB-Stick
+ CD
+ DVD
+ Blue-Ray
+ SSD
+ HDD
+ Diekstte
+ Magnetbänder
+ SD-Karte
+ NAS
+ Cloud

### Kriterien
+ Übertragungsrate
+ Zugriffszeit (Schreiben / Lesen)
+ Speichergröße / Datenmenge
+ Haltbarkeit der Datenträger
+ Datenträger wiederbeschreibbarkeit
+ Schnittstelle
+ Kosten
+ Benutzerfreundlichkeit


### Kategorien
- Optisch (Cd, DVD, BluRay)
- Magnetisch (HDD, Magnetband)
- Halbleiterbasiert (SSD, Usb-Stick, SD-Karte)
- Cloud-Speicher (Onedrive, Selfhosted, AWS-Bucket)
- Netzwerkbasiert (NAS)

## Vorteile Nachteile Speichermedien
### CD, DVD, Blu-Ray
##### CD
- Geeignet für inkrementelle und differentielle Datensicherung/Archivierung
- Kapazität 650MB - 900MB
- Kosten gering
- Lebensdauer bei optimaler Lagerung 80-100Jahre
    - stabile Raumtemperatur von 25C
    - Luftfeuchtigkeit bei 40-60%
    - kein Licht, keine Kratzer
#### DVD
- wie CD
- Kapazität 4,7GB-17GB
- Kosten relativ günstig
- Lebensdauer 30 Jahre
#### Blu-Ray
- wie CD
- Kapazität: 25GB
##### Vorteile und Nachteile
- Risiken: Wärme, Feuchtigkeit, Licht, Fingerabdrücke, Kratzer, Bruch
- Voraussetzungen: PC mit geeignetem Laufwerk
- Nicht für ein Voll-Backup geeignet
- Flexibel/transportabel

### Speicherkarte
- Zwischenspeicher für Transport oder für Digital-Kameras etc.
- Kapazität bis zu 2 TB
- Kosten je nach Speichergröße ab ca 20 Euro für 64GB
- Lebensdauer 10k bis 100k Schreibzyklen
##### Vorteile und Nachteile
- Risiken: Verschmutzung, Korrosion, Beschädigung der Kontakte
- Voraussetzungen: Passender USB-Anschluss am Gerät
- Nur begrenzt wiederbeschreibbar
- Flexibel/transportabel

### USB-Speicher
- Geeignet für Datentransport
- Kapazität: 32MB - 1TB
- Kosten: ab 5Euro aufwärts
- Lebensdauer: je nach Anzahl der Schreibzyklen bis zu 10 Jahre
##### Vorteile und Nachteile
- Risiken: Verschmutzung, Korrosion, Beschädigung der Kontakte
- Voraussetzungen: Passender USB-Anschluss am Gerät
- Nur begrenzt wiederbeschreibbar
- Flexibel/transportabel

### SSD
- Vor allem für Voll-Backup und dauerhafte Datensicherung
- Kapazität: bis zu 5 TB
- Kosten´: je nach Speichergröße ab ca 100Euro
- Lebensdauer: 10 Jahre / 5k bis 10k Schreibzyklen
##### Vorteile und Nachteile
- Risiken: Relativ unempfindlich, da ohne extern bewegliche Teile
- Voraussetzungen: Passender Anschluss am gerät.
- Nur begrenzt wiederbeschreibbar.
- eingeschränkt Flexibel/transportabel

### Externe Festplatte
- Geeignet für Voll-Backup und dauerhafte Datensicherung
- Kapazität: bis zu 15 TB
- Kosten: je nach Größe ab ca 70 Euro
- Lebensdauer: ca 10 Jahre
##### Vorteile und Nachteile
- Risiken: Feuchtigkeit, Stöße, magnetische Felder, Verschleiß beweglicher Teile
- Voraussetzungen: Passender Anschluss am Gerät
- eingeschränkt Flexibel/transportabel

### Magnetband
- Geeignet für Server-Backups, Archivierung.
- Kapazität: mehr als 6 TB
- Lebensdauer: 10 - 30 Jahre
- Kosten: hoch
##### Vorteile und Nachteile
- Risiken: Wärme, Feuchtigkeit, magnetische Felder
- Voraussetzungen: Spezielles Bandlaufwerk
- Verliert ihrgendwann die Magnetisierung. Ablösung der Schichten des Bandes (Haltbarkeit)
- nicht Flexibel/transportabel

### NAS
|Vorteile|Nachteile|
|---|---|
|Übertragungsgeschwindigkeit|Übertragungsgeschwindigkeit ist sehr anfällig|
|Speichergröße|Sicherheitsproblem|
|RAID möglichkeit||

### Cloud
|Vorteile|Nachteile|
|---|---|
|große Haltbarkeit|IT-Experte notwendig|
|Anbieter kümmert sich um die Sicherheit|Kosten können im Worst-Case Hoch sein |
|Speichergröße am besten|Sicherheitsprobleme, da Daten übermittelt werden|
|Übertragungsrate|Internetverbindung muss immer da sein|
|Einfache Backup-Regeln einzuhalten||

### Cloud - Hybrid - NAS -Storage 
- Risiken: Angreifbar während der Datenübertragung. Server Ausfall. Abhängig vom Anbieter.
- Voraussetzungen: Zugung zu Internet/Netzwerk
- Daten lagern auf fremden Server
- Kosten, Datensicherheit und mögliche Offline-Zugriffe sind abhängig vom Anbieter/Lösung
- Sehr flexiebel, da weder orts noch gerätgebunden.


### automatisches Backup

|automatisch|manuell|
|---|---|
|**Voreile**|**Vorteile**|
|Zuverlässigkeit|Bessere Kontrolle|
|Konsistenz|Flexibilität|
|Sicherheit|Unabhängigkeit|
|Zeitersparnis||
|**Nachteile**|**Nachteile**|
|Erhöhter Kontrollaufwand|Unzuverlässigkeit|
|Abhängigkeit der Technik|Menschliches Versagen|
|Ressourcenverbrauch||

### NAS-Backup SAN-Backup Cloud-Services-Backup

|**NAS-Backup**|**SAN-Backup**|**Cloud-Services-Backup**|
|---|---|---|
|**Vorteile**|**Vorteile**|**Vorteile**|
|Einfache Integration|hohe Performance|Unbegrenzte Skalierbarkeit|
|geringe Kosten|gute Redundanz|Sehr gute Redundanz|
|schneller Zugriff|Zentralisiert Verwaltbar|einfachere Automatisierung|
||Zentralisiert Skalierbar||
|**Nachteile**|**Nachteile**|**Nachteile**|
|Abhängigkeit von Infrastruktur|hohe Kosten|Benötigt Internetzugang|
|Einzelner Speicherort|Komplexität|Datenschutz und Sicherheit|
|Sicherheitsrisiko|Potenziell Single point of failure|Langzeitkosten|
|||Eingeschränkte Kontrolle|
|**geeignet für**|**geeignet für**|**geeignet für**|
|kleine Struckturen|Große Infrastrukturen. Sehr hohe Leistungsanforderungen|Theoretisch Alle|


## Vollsicherung / Voll Backup
+ Sicherung aller Daten 

|Vorteile|Nachteile|
|---|---|
|alle Daten in der neusten Version|Zeitlich - Es dauert sehr lange|
|einfache Wiederherstellung|großer Ressourcenaufwand|
|Unabhängigkeit von anderen Sicherungen||
|einfacher Redundanzen zu bilden||

## Inkrementelles Backup
|Vorteile|Nachteile|
|---|---|
|reduzierter Speicherbedarf|aufwendig und komplexer bei Wiederherstellung|
|schnelles Backup|Abhängigkeit des Vorherigen Backup|
|effizientere Speichernutzung||

Eine Vollsicherung wird erstellt.
|Backup 01||
|---|---|
|Backup 01||
## Differentielles Backup

|Vorteile|Nachteile|
|---|---|
|einfache Widerherstellung|Potentieller Speicherzuwachs|


## Backupstrategien
+ Großvater - Vater - Sohn 
+ Turm von Hanoi
+ 3-2-1 Backup-Regel



