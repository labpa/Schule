# Firewall

## Sicherheitsrichtlinien
+ Sicherheitsrichtlinien und Firewall Regeln festlegen.
+ Administrative Schnittstellen schützen
+ Notfallzugriff muss da sein
Über ein bestimmtes Netzwerk muss der Zugriff für die Admins immer möglich sein.
+ Log / Überwachung

## Firewallarten
+ Packetfilternde Firewalls
+ Circut Level Gateway
+ Stateful Inspection Firewall
+ Next-Generation Firewall
+ Application Level Fierewall
+ Unified Threat management


Eine Firewall muss mehr als nur Port oder IP blocking können. HTTPS Port 443


## DMZ


## Proxy

### Forward

### Reverse

## IDS - Intrusion Detection System
+ passives System
+ Soll eine Ergänzung zur Firewall sein
+ Es soll Muster / Anomalien erkennen  
Bei Erkennung -> Meldung an Admin  
Host-basiert / Netzwerk-basiert / Hybrid
Daten werden ausschlieslich gesammelt und Analysiert. Es wird nichts verhindert. 

## IPS - Intrusion Prevention System
+ HAt die selben Unterscheidungsmöglichkeiten wir IDS
+ aktives System
+ Erkennen von Angriffen
+ Abwehrmaßnahmen werden automatisch ergriffen
+ Funktioniert ähnlich wie IDS hat aber einige Unterschiede
+ Beide nutzen KI + FW
+ mögliche Abwehrmaßnahmen
    + Verbindung Unterbrechen
    + Pakete verwerfen
    + Verbindungen von Ziel und Quelle grundsätzlich Blocken
    + Admin Informieren

