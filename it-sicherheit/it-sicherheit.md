# IT-Sicherheit
- [Grundlagen IT-Sicherheit](##  'Grundlagen IT-Sicherheit')
	- [Was sind Informationen und Daten?](#thema1)
	- [Cybercrime](#thema2)
	- [Sicherheitspakete](#thema3)
    - [Bedrohungen](#thema1)
	- [Technische Schutzmaßnahmen](#thema2)
- [Angreifer und ihre Motivation](#hauptteil)
	- [Motivation für Angriffe](#thema1)
	- [Potenzielle Angreifer im Intenet](#thema2)
- [Häufigste Angriffe](#thema3)	
    - [DOS und DDOS-Attacken](#schluss)
    - [Malware, Virus Wurm und Trojaner](#test)
    - [Spoofing]()
    

## Grundlagen IT-Sicherheit
**Mehrere Daten sind Informationen. Mehrere Informationen sind Wissen.**

### Was sind Informationen und Daten?
Daten können in digitaler Form aus Buchstaben, Zahlen oder Symbolen bestehen und gespeichert werden.

Zu Daten zählen erstellte Dokumente, Datenbanken und Programmcode.

Darauf aufbauend werden aus Daten infolge der Verarbeitung, Ausführung oder Ausgabe Informationen die eine Bedeutung oder Ausgabe Informationen die eine Bedeutung für den Benutzer/Empfänger haben.

Unter Informationen kann auch der Inhalt einer Mitteilung oder Nachricht verstanden werden.


### Cybercrime
Cybercrime umfasst die Straftaten, die sich gegen das Internet, Datennetze, informationstechnische Systeme oder deren Daten richten(Cybercrime im engeren Sinne) oder die mittels dieser Informationstechnik begangen werden.


### Sicherheitsaspekte
|Sicherheitspaket|Kurzbeschreibung|
|---|---|
|Zugrifsschutz|**Kontrolle des Systemzugangs** und Zugriffsbeschränkungen aus Systemfunktionen und Datenbestände|
|Authentizität|**Nachweisen der Identität** des Urhebers/Autors und des Datenmaterials|
|Vertraulichkeit|**Verhindern, dass Unberechtigte auf Daten zugreifen können**|
|Integrität|Nachweisen, dass die **Daten unverändert** vorliegen|
|Nachweisbarkeit|Prüfen der Authentuzität und Integrität der Daten auch von berechtigten Dritten, so das die **Verbindlichkeit der Kommunikation gewährleistet** ist|

### Bedrohungen
+ Bedrohungen können Sicherheitszielen zugeordnet werden, beispielsweise:  
    + Abhören ist eine Bedrohung der VErtraulichkeit
    + Sabotage ist eine Bedrohung der Verfügbarkeit
+ Angriffe bilden meist Kombinationen von Realisierungen ausgeführter Bedrohungen
    + z.B. Abhören und Maskarade stellen eine häufige Kombination dar.

||Vertraulichkeitet|Datenintegrität|Zurechenbarkeit|Kontrollierter Zugang|Verfügbarkeit|
|---|---|---|---|---|---|
|Maskerade|X|X|X|X|X|
|Abhören|X|||||
|Autorisierungsverletzung|X|X|X|X|X|
|Verlust oder Modifikation von Informationen||X|X||X|
|Fälschen von Informationen||X||||
|Abstreiten von Ereignissen|||X|||
|Sabotage|||||X|
+ Tabelle fasst zusammen, welche Sicherheitsziele durch welche KAtegorie eines Angriffs **primär** gefährdet sind
+ Angriffe bilden meist Kombinationen von Realisierungen aufgeführter Bedrohungen
    + z.B. Abhören und Maskerade stellen eine häufige Kombination dar.

### Technische Schutzmaßnahmen
In der digitalen DAtenwelt:
+ Authentizität:  
Besitz von Geheimnissen (Passwort, Signaturschlüssel)
+ Vertraulichkeit:  
Verschlüsselung, Zugriffsschutz/Rechte
+ Integrität:  
Entdeckung von Veränderungen (Verschlüsselung, digitale Signatur) phys. Zugriffsschutz auf Speicher/leitung
+ Verfügbarkeit:  
Betriebsabsicherung, Redundanz
+ Verbindlichkeit:  
digitale Signatur, Protokolldaten

## Angreifer und ihre Motivation
### Motivation für Angriffe
Warum greift jemand Daten oder ein Informatiksystem an?
1. Persönliche Bereicherung (Kriminelle)
2. Wirtschaftsspionage, staatliche Spionage (Firmen, Geheimdienste)
3. Wirtschaftssabotage , staatliche Sabotage (dito) "Cyber-Krieg"
4. Neugierde (irgendjemand)
    + aud die Daten oder auf den Angriff
5. Jugendlicher Übermut (Script-Kiddies)
6. Böswilligkeit (z.B.s oben: Ex-Freund)
7. Gerechtigkeitssinn ("Robin Hood")
8. Auf Risiken hinweisen (z.B. Chaos Computer Club)
### Potenzielle Angreifer im Intenet:   
#### **Insiders** <br>
Firmeneigene Mitarbeiter können die Ressourcen des Unternehmens angreifen oder stehlen, z.B. vertrauliche Dokumente, oder Server, indem sie ihre Privilegien im Unternehmen missbrauchen<br>
**Motive:** Neugierde, Frustration, Rache, Gier, Neid, ...<br>
+ Insider-Angriffe sind besonders gefährlich, da sie von innerhalb des Firmennetzwerks kommen - Intranet (Firmeneigenes Netzwerk)
+ Naivität oder Unachtsamkeit --> **Social Hacking**
+ Erhöhtes Risiko durch (mangelhafte) Einbindung von Home Büros und **"Bring Your Own Device"** (BYOD) in das Unternehmensnetzwerk
+ Nichteinhaltung von internen Sicherheitsanweisungen öffnen Türen für Angreifer

#### **Skript-Kiddies**<br>
Angreifer ohne tiefgreifende Cybersicherheitskentnisse, die Cybernagriffe mit Hacker-Tools starten <br>
**Motive:** Neugierde, just for fun, Angeberei, ...<br>
+ Wahllos und meist ohne direkte Kriminelle Absicht
+ Vor allem junge Menschen (Schüler, Studenten) die Beginnen sich mit Cybersicherheit auseinanderzusetzen
+ Viele Hacking-Tools stehen im Internet zum Download bereit
+ Besonders gefährlich: Denial-of-Service-Attacken (DoS)

#### **Hacker**<br>
Der Begriff Hacker wird unterscheidlich interpretiert
+ Der Begriff "Hacker" wurde ursprünglich als Anerkennung für besonders kreative und talentierte Personen genutzt
+ Später wird der Begriff Hacker von den Medien negativ besetzt aufgrund der Folgen von Indiskretionen und Schäden durch ihre Cyberattacken
+ Bezieht sich auf Personen mit tiefgreifendem teschnischen Wissen
+ Der Begriff "Hacker" kann wie folgt kategorisiert werden:
    + white hat hacker
    + grey hat hacker
    + black hat hacker
    + hacktivists

##### **White Hat Hacker**<br>
Die "guten" Hacker/ethischen Hacker<br>
+ Professionelle Experten, die nach Sicherheitsschwachstellen in Computersystemen, Anwendungen, Diensten, NEtzwerken, ... , suchen um zu helfen, das System vor zukünftigen möglichen Angriffen zu schützen. <br>
**Motive:** guter Samariter, Bewusstsein für Cybersicherheit erhöhen
+ **Sicherheitsanalysen** und **Penetrationstests** durchführen, um Sicherheitslücken in den Systemen zu erkennen
+ Informieren den autorisierten Besitzer über entdeckte Sicherheitslücken zur Verbesserung der Sicherheit von Computersystemen und Netzwerken
+ Verhindern und zukünftige Angriffe auf die Systeme durch Cyber-Kriminelle


##### **Black Hat Hacker**<br>
Die "bösen" Hacker/Cyberkriminellen<br>
+ Meist sind es professionelle Computerexperten, die sich in die Computersysteme hacken, um kriminelle Aktivitäten aus Eigeninteresse und Profitgier durchzuführen <br>
**Motive:** Geld, Macht, Erpressung, Berühmtheit, ... <br>
+ Ausnutzung von entdeckten Sicherheitslücken, um autorisierten Zugriff auf Computersysteme zu bekommen
+ Ziel ist es, Straftaten wie Diebstahl, Identitätsdiebstahl, Zerstörung von Dienstan, ... Durchzuführen
+ Zum eigenen Nutzen oder im Auftrag anderer
+ In den meisten Fällen werden entdeckte Sicherheitslücken geheim gehalten und mit anderen Black-Hat-Hackern geteilt z.B. im Darknet
+ Black Hat Hacker können die gestohlenen Informationen an die Öffentlichkeit (meist im Darknet) verkaufen:
    + E-Mail-Konten: $0,70 - $2,30
    + Führerscheininformationen: $20
    + Kreditkartendaten: $8,00 - $22,00
    + Medizinische Daten: Bis zu $1000
+ Sie bieten auch Dienste und Werkzeuge für verschiedene illegale Aktivitäten an, wie zum Beispiel:
    + Tool zum Hacken von Facebook-Konten: $19.99 (3 Monate)
    + Bewertung bei Google und Co.: $3 - $350
    + Zugang zu speziellen Benutzerkonten: $90 - $350


##### **Grey Hat Hacker** <br>
Zwischengruppe aus gutartigen und bösartigen Hackern
+ Meistens profesionelle Computerexperten, die sowohl gutartig und bösartig/eigennützige Ziele
    + Gefundene Sicherheitslücken in Computersystemen ausnutzen
    + Möglicherweise kriminelle Aktivitäten zum eigenen Vorteil starten
    + Gefundene Sicherheitslücken veröffentlichen, um das Sicherheitsbewusstsein zu erhöhen


##### **Hacktivist**<br>
Hacker + activists
+ Einzelpersonen oder Gruppen, die Computersysteme aus ideologische, soziale, politische oder religiöse Gründe angreifen


**Motive:** Bewustseinsbildung, Selbstego, politische Zielen, ... <br>
+ Angriffe auf Computersysteme starten, um auf die Probleme hinzuweisen und der Öffentlichkeit zu zeigen
+ Glauben, dass sie zu einer höheren Sache beitragen
+ Schrecken vor kriminellen Aktivitäten nicht zurück
+ Beeinflussen die Medien und die öffentliche Meinung mit falschen Meldungen und verwirrenden ideologischen Phrasen

Bekannte Gruppe: z.B. Anonymus

##### **"Gewöhnliche" Kriminelle**
Kriminelle, die das Internet für ihre Aktivitäten nutzen.
+ Traditionelle Kriminelle und das organisierte Verbrechen haben das Potenzial des Internets als globalen Marktplatz für ihre kriminelle Aktivitäten erkannt
    + Nutzung des Internet für kriminelle Aktivitäten, z.B. Drogen und Waffenschmuggel, Erpressung, Computerbetrug, ...
    + Die Behörden haben mehr Schwierigkeiten, die Gesetze durchzusetzen und die kriminellen Aktivitäten im Internet zu untersuchen als in der physischen Welt
        + **daher:** Regierungen könnten daran interessiert sein "Hintertüren" in kryptographisch geschützten Systemen zu installieren

##### **Geheimdienste & Spionage**
Umfangreiche Möglichkeiten des Internets bieten hohe Potenziale für Spione und Geheimdienste
+ **Wirtschaftskriminalität:** Diebstahl vertraulicher Informationen und Ausspionieren von Konkurenten
+ **Spionage:** Ausspionieren von politisch interessanten Akteuren in anderen Ländern
+ **Politisch** oder **wirtschaftlich** motivierte Cyber-Angriffe auf Dienste und Computersysteme


## Häufigste Angriffe
### DOS und DDOS-Attacken
#### Denial-of-Service
+ Angriff mit dem Ziel, die Verfügbarkeit eines Dienstes im Internet zu stören
#### Distributed Denial-of-Service
+ Denial-of-Service-Angriff, der von vielen verschiedenen Stationen im Internet, z.B. über ein Botnetz ausgeführt wird

### Malware - Virus, Wurm, Trojaner
#### **Mal**icious Soft**ware**
+ Bösartige Software - Software, die absichtlich entwickelt wurde, um Schäden an Computern, Netzwerken, Anwendungen, Diensten, ... anzurichten
+ **Virus**  
zerstörerisches Miniprogramm, das von den "indifizierten" Anwendungen oder Daten übertragen wird

+ **Wurm**  
bösartige Software, die sich automatisch über offene Netzwerkverbindungen verbreitet.

##### **Ziele:**

+ Einschränkung der Arbeitskapazität des Systems
+ Zerstörung oder Manipulation von Daten
+ Diebstahl von Passwörtern
+ Spionage und Sabotage
+ Erpressung
+ Fernsteuerung
+ ...
##### Der weg zum Computer
Malware- als eine der zentralen Waffen von Cyber-Kriminellen. Jedes Gerät und jedes Computersystem kann ein potenzielles Ziel für Malware sein. Kann sowohl Endanwender als auch Dienstanbieter infizieren. Potenziell sind Heimcomputer verwundbarer für Malware-Angriffe über das Internet. Malware sind besonders leicht für Angriffe nutzen. 
+ Cyber-Kriminelle entwickeln zunächst die Malware, um die Computersysteme der Opfer zu infizieren
+ Dann injizieren Cyberkriminelle die Malware in ein Medium, wie z.B. eine Anwendung oder E-Mail und senden die an potenzielle Opfer.
+ Sobald das Opfer auf den Datenträger zugreift, wird die Malware auf dem Computersystemen des Benutzers installiert.



### Spoofing und Phising
#### Spoofing
Angreifer sendet Nachrichten mit einer gefälschten Absendeadresse, z.B. gefälschte IP-Adressen oder E-Mail-Adressen.
+ Zum Beispiel:
    + CEO Betrug
    + Der gefälschte CEO weist die Buchhaltung an, eine Zahlung an ein unbekanntes Bankkonto zu senden.
Spoofing wird oft verwendet in Verbindung mit:
#### Phishing
"Social Engineering"-Methode, bei der Benutzer aufgefordert werden, ihre sensiblen Informationen wie z.B. Passwörter preiszugeben  

Angreifer verwenden gefälschte E-Mails, Websites, Telefonanrufe,...

### Defacement
Angriffe auf eine Website oder einen Webserver mit der Absicht seine Inhalte zu verändern (De-face = das Gesicht verändern)
+ Verwendet für...
    + Eigenwerbung von Hackergruppen, Blamagen von seriösen Diensten, ...
    + Angriff auf die Verfügbarkeit von Diensten
    + **Phishing von Benutzerdaten:**
        + Benutzer erkennen nicht, dass es sich bei der Website um einen nichtz autorisierte Fälschung ist
        + Angreifer können sensible persönliche Daten erlangen, wie Passwörter, Kreditkartennummern, ...

### Sniffing and Eavesdropping
#### Sniffing
Sniffing ist eine Methode zur Netzwerkdiagnose durch "Abhören" des gesamten Netzwerkverkehrs. Administratoren können es nutzen, um Fehler im Netzwerkverkehr zu erkennen, z.B. mit Hilfe von Netzwerk-Sniffing-Software :**Wireshark**
#### Eavesdropping (Lauschen)
Unter Abhören versteht man das unbefugte Schnüffeln-"Abhören" von Datenpaketen auf ihrem Weg durch das Netzwerk.
+ Angreifer verbindet sich mit dem Netzwerk des Opfers um die IP-Pakete zu sammeln und zu analysieren, um persönliche Daten oder andere vertrauliche private Informationen zu erfassen.
+ Direktes Mitlesen von unverschlüsseltem Datenverkehr
+ Verschlüsselter Datenverkehr kann aufgezeichnet und später entschlüsselt werden

### Weitere Angriffe auf Computersysteme
+ Nicht autorisierter physischer Zugriff auf das Computersystem
    + Diebstahl von Laptops, Smartphones, ...
    + Einbruch in Serverräumen
+ Social Engineering-Angriffe
    + ... nicht nur um Passwörter wie in dem Beispiel von Phishing zu stehlen
+ Angriff zum Entschlüsseln persönlicher Daten
    + Passwort knacken
    + Passwort erraten


### ARP-Spoofing
**???**


### Cache-poisoning / DNS-Spoofing
DNS-Spoofing und Cache Poisoning sind IT-Sicherheitsangriffe auf das Domain Name System, um die Zuordnung zwischen einem Domainnamen und der zugehörigen IP-Adresse zu fälschen. Der Zweck ist es, Datenverkehr unbemerkt zu einem anderen Computer zu lenken, zum Beispiel um einen Phishing- oder Pharming-Angriff durchzuführen.
**???**

### DHCP Security Probleme
**???**
Falsche Netzwerkkonfigurationen werden verteilt.
Denial of Service

### Port-Scanning
### Social Engineering
### Ransomware
### KeyLogger
### Brute-Force

### Bot-Netz
