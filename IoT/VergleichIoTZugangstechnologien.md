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
    + Außenbereich: maximal 100 m
    + Innenbreich. maximal 30 m

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
ZigBee sieht zwei Geräteklassen vor:  
+ Full Function Device (FFD): Ein FFD beherrscht den kompletten Protokollstack und kann mit RFDs und anderen FFDs kommunizieren.
+ Reduced Function Device (RFD): Ein RFD ist einfacher implementiert und kann nur mit einem FFD kommunizieren.

+ Netzwerkarchitektur
    + Stern
    + Cluster-Tree
    + Mesh-Netz

+ Übertragungsreichweite
    + ca. 10 m

+ Datenrate
    + 250 kBits/s

+ Energieeffizienz
    + sehr sparsam

+ Skalierbarkeit

+ Sicherheitsfunktion
+ 1. Stufe: "keine Sicherheitsvorkehrung". 
+ 2. Stufe: einfache Zugangskontrolle
+ 3. Symmetrischen Verschlüsselung mit AES und einer Schlüssellänge von 128 Bit.


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

### LoRaWAN Long Range Wide Area Network
+ Netzwerkarchitektur
    + Sterntopologie

+ Übertragungsreichweite
    + bis zu 15 km
+ Datenrate
    + 0,3 kbps bis zu 50 kbps
    
+ Energieeffizienz
    + sehr energieeffizient
    + Batterielaufzeit bis zu 10 Jahren

+ Skalierbarkeit
+ sehr hohe skalierbarkeit

+ Sicherheitsfunktion
+ Sicherheit auf Netzwerkebene und eindeutiger Netzwerkschlüssel (EUI64)
+ Ein einzigartiger Application Key (EUI64) sorgt für die Sicherheit auf der    Applikationsebene
+ Gerätespezifischer Schlüssel (EUI128)

### NB-IoT NarrowBand IoT
Bei NarrowBand IoT handelt es sich um einen Funkstandard, der speziell für das Internet der Dinge (IoT, Internet of Things) vorgesehen ist. Er setzt auf vorhandene Mobilfunknetze auf und ermöglicht die Vernetzung von Geräten und Maschinen bei hoher Funkabdeckung und geringem Energiebedarf.

+ Netzwerkarchitektur

+ Übertragungsreichweite
    + Signalreichweite bis zu >10 km
+ Datenrate
    + Up- und Downloadrate liegt bei ca. 250 kbit/s

+ Energieeffizienz
    + sehr geringer Energieverbrauch
    + Versorgung durch Batterien

+ Skalierbarkeit
    + hohe skalierbarkeit

+ Sicherheitsfunktion
    + gegenseitiges Authentifizieren
    + weißt alle Sicherheits und Datenschutzmerkmale von Mobilfunknetzten auf