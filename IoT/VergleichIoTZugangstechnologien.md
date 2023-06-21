# IoT-Zugangstechnologien

## Vergleich der Protokolle nach
+ Netzwerkarchitektur: Struktur und Organisation des Netzwerks, z. B. Topologie und Geräterollen.
+ Übertragungsreichweite: Maximale Entfernung für zuverlässige Signalübertragung. Informationen
zur physikalischen Schicht und den drahtgebundenen oder drahtlosen Verfahren
+ Datenrate: Geschwindigkeit der Datenübertragung zwischen Geräten und Informationen zur MACSchicht
+ Energieeffizienz: Fähigkeit, Energie zu sparen und Batterielaufzeit zu verlängern.
+ Skalierbarkeit: Fähigkeit, mit wachsender Geräteanzahl im Netzwerk umzugehen.
+ Sicherheitsfunktionen: Mechanismen zum Schutz von Daten und Geräten vor unbefugtem

### 802.15.4
+ Netzwerkarchitektur
    + Stern
    + Peer-to-Peer
    + Baumstruktur
+ Übertragungsreichweite
    + Außenbereich: maximal 100m
    + Innenbreich. maximal 30m
+ Datenrate (brutto)
    + Europa: 20 kBit/s
    + USA: 40 kBits/s
    + Weltweit: 250 kBits/s
+ Energieeffizienz
+ Skalierbarkeit
+ Sicherheitsfunktion
    + Sicherheitsmaßnahmen auf MAC-Ebene durch Message-Integrity-Check und symmetrische Verschlüsselung. 
    + Es kann zwischen mehreren Verfahren gewählt werden, die auf CCM und AES basieren. 
    + Die Schlüssel werden durch die darüberliegende Schicht festgelegt und anschließend durch den MAC-Layer verwaltet. Die Verschlüsselung wird für jeden Kommunikationspartner separat festgelegt und automatisch vom MAC-Layer angewendet. War ein empfangenes Paket verschlüsselt, zeigt dies ein Parameter in der Indication-Primitive an.

### Zigbee
+ Netzwerkarchitektur
    + PAN-Koordinator
    + Full Function Deviced (FFD)
    + Reduced Function Device (RFD)
+ Übertragungsreichweite
+ Datenrate
+ Energieeffizienz
+ Skalierbarkeit
+ Sicherheitsfunktion

### 1901.2a
+ Netzwerkarchitektur
+ Übertragungsreichweite
+ Datenrate
+ Energieeffizienz
+ Skalierbarkeit
+ Sicherheitsfunktion

### 802.11ah
+ Netzwerkarchitektur
+ Übertragungsreichweite
+ Datenrate
+ Energieeffizienz
+ Skalierbarkeit
+ Sicherheitsfunktion

### LoRaWAN
+ Netzwerkarchitektur
+ Übertragungsreichweite
+ Datenrate
+ Energieeffizienz
+ Skalierbarkeit
+ Sicherheitsfunktion

### NB-IoT
+ Netzwerkarchitektur
+ Übertragungsreichweite
+ Datenrate
+ Energieeffizienz
+ Skalierbarkeit
+ Sicherheitsfunktion