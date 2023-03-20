# IT-Sicherheit
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


### Port-Scanning
### Social Engineering
Angreifer versuchen sich als andere Personen oder Systeme auszugeben (Website oder Anwendung), um Benutzer dazu zu bringen, **geheime persönliche Informationen** weiterzugeben.
+ Beispiel:
    + Benutzer erhält einen Anruf von einer unbekannten Nummer
    + Angreifer gibt an ein Mitarbeiter der Bank des Benutzers zu sein und Hilfe zu benötigen um potenziell betrügerische Banküberweisungen zu überprüfen
**erzeugt eine Stress-Situation für den Benutzer**  
+ Der Angreifer bittet dann den Benutzer seine privaten Bankdaten anzugeben um die gefälschen Überweisungen zu "verifizieren"
+ Angreifer kann dann die Daten des Benutzers nutzen um sich bei der Bank zu authentifizieren


### Brute-Force
### Bot-Netz


### Spear-Phishing
Traditionelles, weit verbreitetes Phishing ist nicht mehr effektiv, um persönliche oder vertrauliche Informationen des Opfers zu gelangen. Angreifer wenden sich daher dem personalisierten Phishing oder Spear-Phishing zu.
+ Angreifer sammeln sehr detallierte Informationen über ihre Opfer, um sie später dazu zu benutzen ihr Vertrauen zu gewinnen.
    + Sammeln die Referenzen einer Person (z.B. Freund, Familienmitglied, Kollege), die das Opfer kennt und denen es vertraut aus Sozialen Medien oder aus dem Internet.
    + Das Opfer glaubt das die E-Mail von vertrauten Person stammt, weil die Nachricht Informationen enthält die nur diese Person kennt.
+ Spear-Phishing-Angriffe haben viel höhere Erfolgswarscheinlichkeit, erfodern aber mehr Arbeit für den Angreifer.
+ Personalisiertes Phishing ist daher sehr gefährlich und wird auf das Ziel direkt angewendet.
    + wichtige Personen, z.B. CEOS, Politiker, ...
    + sensible Bereiche, z.B. Militär, Wirtschaft,...
+ **Hinwei:s** Viele andere Angriffe im Internet basieren auf frühere personalisierte Phishing Angriffe.

### Malware
+ **Malware** - bösartige Software
+ wird über das Internet von Hackern und Cyber-Kriminellen auf das Gerät eines ahnungslosen Benutzers eingeschleust, um im Interesse der Cyber-Kriminellen zu handeln.
+ Ziele:
    + Einschränkung der Arbeitskapazität des Systems
    + Zerstörung oder Manipulation von Daten
    + Diebstahl von Passwörtern
    + Spionage und Sabotage
    + Erpressung
    + Fernsteuerung
#### Malware-Arten
+ Es gibt viele verschiedene Arten von Malware mit sehr unterschiedlichen Angriffsvektoren
+ Meist werden mehrere Schadfunktionen innerhalb einer Malware kombiniert
    + Trojan
    + Virus
    + Worms
    + Adware

#### Der Weg zum Computer
+ Jedes Gerät und jeses Computersystem kann ein potenzielles Ziel für Malware sein.
+ Kann sowohl Endanwender als auch Dienstanbieter infizieren
    + Potenziell sind Heimcomputer verwundbarer für Malware-Angriffe über das Internet
+ Malware sind besonders leicht für Angriffe zu nutzen.
+ Cyber-Kriminelle entwickeln zunächst die Malware, um die Computersysteme der Opfer zu infizieren
+ Dann injizieren Cyberkriminelle die Malware in ein Medium, wie z.B. eine Anwendung oder E-Mail und senden sie an potenzielle Opfer
+ Sobald das Opfer auf den Datenträger zugreift, wird die Malware auf dem Computersystem des Benutzers installiert.

Im Allgemeinen kann Malware auf Computersystemen installiert werden durch verschiedene Angriffsvektoren:
+ Menschliche Faktoren
Oft reicht die Unachtsamkeit des Opfers aus, um Malware auf dem Computersystem des Opfers zu installieren.

Malware kann auch durch Social Engineering in das Computersystem injiziert werden.
+ Beispiele:
    + Öffnen einer E-MAil mit bösartigem Anhang
    + Herunterladen und Öffnen von infizierten Dateien aus dem Internet
    + Herunterladen und Installieren von "hilfreicher" Software
    + Anschließen eines fremden USB-Sticks
    + Nutzung eines öffentlichen WLANs

+ Technische Faktoren / Ausfälle

#### Der Mensch als Sicherheitsrisiko
Der Menschliche Faktor steht für alle menschlichen Aspekte, die Sicherheitsrisiken im System schaffen. Es können zwei Kategorien des menschlichen Faktors unterschieden werden:
+ **Aktiv:** Risiko wird verursacht durch unwissentliches oder wissentliches Ausführen einer bestimmten  Tätigkeit.
+ **Passiv:** Das Risiko wird duch das Unterlassen einer bestimmten Tätigkeit verursacht, die hätte durchgeführt werden müssen.

##### Passive Menschliche Faktoren
Selbst wenn ein Unternehmen gute Sicherheitsrichtlinien vorgibt, kann es Mitarbeiter geben, die sich einfach nicht um die Richtlinien kümmern und sie nicht befolgen.
+ Sie halten sich nicht an Richtlinien/Normen
+  Könnten Sicherheitsprobleme verursachen, weill die nicht tun, was sie tun sollen.
+ Eine Lösung für dieses Problem sind spezielle Informationsveranstaltungen oder Workshops
    + Sensibilisierung der Mitarbeiter für das Thema
    + Darstellung der Folgen von mangelnder Vorsicht

#### Virus
Ein Virus ist eine Schadsoftware, die sich an ein Programm oder Datei ("Host") anheftet und sich auf andere Programme/Dateien weiter verarbeitet
+ Wenn der identifizierte Host geöffnet oder ausgeführt wird, wird das Zielsystem infiziert.
+ Der Schweregrad reicht von der Verursachung lästiger Effekte bis hin zur Schädigung von Daten, Software oder sogar Hardware.
+ Oft keine klare Definition
    + umgangssprachlicher Begriff für Maleware
    + Oberbegriff für alle Schadprogramme in einem Wirtsprogramm

#### Wurm
Ein Wurm ist eine Malware, die ihre Kopien über das Netzwerk oder Internet selbstständig verbreiten kann.
+ Start der Infekrion durch Ausnutzung von Schwachstellen auf dem Zielsystem oder das Ziel dazu bringt, die Malware auszuführen.
+ Funktioniert eigenständig, braucht keinen Wirt oder einen Menschen um sich zu replizieren und zu verbreiten.
+ Oft verbreiten sich Würmer schneller als Viren, z.B. Code-Red 2001
+ **Beispiel:**  
    +   ILOVEYOU - Wurm, der Social-Engineering-Techniken verwendet um Benutzer über eine E-Mail zu infizieren.  
    + Betreff der E-Mail :"ILOVEYOU" (Ich liebe dich)  
    + Anhang eines angeblichen Liebesbriefes ("Love-Letter-For_You.txt.vbs")
    + Enthält ein Visual Basic Script (.vbs) das schädlichen Programmcode ausführt, wenn der Anhang geöffnet wird.
    + Dateierweiterungen wurden nicht angezeigt -> Ziel wird nicht vermuten, dass der Anhang bösartig ist.
+ E-Mail-Adressbuch des Opfers wird verwendet, um den Wurm per E-Mail zu verbreiten
#### Trojaner
Trojaner sind Malware, die sich als echte und nützliche Anwendung tarnt und das Ziel dazu bringt sie zu installieren.
+ Enthält versteckte, dem Ziel unbekannte schädliche Funktionen z.B. das Herunterladen von anderen Schadprogrammen.
+ Bösartige Funktion wird parallel zu erwartenden Funktionen ausgeführt.
+ Vervielfältigt sich nicht und identifiziert keine anderen Daten

Trojaner haben verschiedene Ziele wie die Installation eines
+ **Backdoor:** Öffnet eine Hintertür im System des Opfers, um den Angreifer Fernsteuerzugriff auf das System des Opfers
+ **Spyware:** Überwacht und sendet Informationen über das System des Opfers, indem Aufzeichnung von Tastatureingaben, Zugriff auf Mikrofon oder Webcam, etc.
+ **Botnet:** Fügt das System des Opfers in ein Netzwerk von gekaperten und ferngesteuerten System hinzu, umCyberangriffe zu starten.
+ **Downloader:** Installiert andere Malware auf dem identifizierten System, z.B. Ransomware oder Würmer

Schutzprozess

### Rootkits und Backdoors
+ System hat eine "Hintertür", die es den Angreifern ermöglicht unbemerkt auf den Computer zuzugreiufen
+ Angreifer mit Administrationsrechten können die Hintertür nutzen, um Ihren Computer fernzusteuern z.B. Malware zu installieren, persönliche Daten zu stehlen oder Tastatureingabe aufzuzeichnen.
+ Antiviren-Scanner können dies nicht erkennen.

#### Rootkit
+ **Rootkit** - Komposition aus "root" (Administrationsrechte) und "Kit" (Softwarekomponente zur Entwicklung beliebiger Tools)
+ Software, die einem Angreifer/unbefugten Benutzer Administrationsrechte für ein Zielsystem ermöglichen
+ Erfordert, dass das Ziel das Rootkit installiert um zu funktionieren.
+ Ist so konzipiert, dass es im System versteckt und unerkannt bleibt.
+ Können Tools enthalten, die es Cyberkriminellen ermöglichen
    + Aktionen als Administrator auszuführen
    + die Sicherheit zu deaktivieren
    + Hintertüren auf dem System zu installieren

#### Backdoor
+ **Backdoor** - beschreibt jede Methode, um sich heimlich Zugang zu den Systemen zu verschaffen.
+ Umgehung von Sicherheitsmaßnahmen im System, z.B. Virenscanner, Firewall, ...
+ Erlangung höherer Zugriffsrechte, z.B. Root-Rechte

Backdoors können durch verschiedene Methoden erstellt werden.
+ Ausnutzung von Programmierfehlern (Bugs) oder Sicherheitslücken im System
+ Absichtlich erstellte, z.B. zur Wartung und Fehlersuche im System
+ Installieren durch Schadsoftware (Malware) z.B. Trojaner oder Wurm

#### Rootkit und Backdoor Schutzmaßnahmen
+ Verwenden Sie den Computer nur mit einem Konto, das keine Adminstrationsrechte hat
+ Allgemeine Sicherheitsmaßnahmen
    + Original-Software sorgfältig prüfen und installieren
    + installieren Sie regelmäßig Sicherheits-und Software-Updates
    + ändern Sie alle Standard-Passwörter

### Adware und Spyware
#### Adware
**Adware**- Malware, die zusätzlich zu ihrer eigentlichen Funktionalität **Werbung (Ads)** anzeigt.
+ Wird meist in Webbrowsern installiert und tarnt sich als echtes oder legitimes Programm/Plug-in
+ Zeigt trügerische, blinkende Pop-up-Werbung auf jeder Website für die Benutzer
+ Kann Benutzer dazu verleiten:
    + Malware oder unerwünschte Software zu installieren
    + auf eine gefälschte Phishing-Website zu gelangen
+ In den meisten Fällen harmlos und leicht zu entfernen, aber es könnte sehr lästig für die Benutzer sein.
#### Spyware
**Spyware** - Malware, die vertrauliche Informationen der Opfer aufzeichnet und stiehlt.
+ Kann bei der Installation einer scheinbar legitimen Software oder durch Ausnutzung von Sicherheitslücken im System installiert werden.
+ Läuft unbemerkt im Hintergrund und sammelt Informationen über die Benutzer
    + Emails
    + Bankdaten
    + Benutzername und Kennwort
+ Gesammelte Daten über die Opfer können missbraucht oder ohne deren Zustimmung an Dritte verkauft werden, z.B. im Darknet oder an Datenverkäufer

### Scareware und Rogueware 
Scareware auch Rogueware genannt- Malware (Taktik), die Benutzer erschreckt, mit dem Ziel, dass die Malware installieren, um vorgetäuschte Probleme auf ihren System zu lösen
+ Verwendet Social-Engineering-Angriffsmethode, indem sie gefälschte Meldungen, z.B. "Virus entdeckt" oder "Fehlermeldungen" angezeigt. Benutzer laden dann Software herunter oder kaufen sie, um diese "Probleme" zu lösen.
+ Ist in Wirklichkeit eine Malware, die persönliche Benutzerdaten stehlen oder die Kontrolle über das System des Benutzers übernehmen kann.


### Ransomware
Ransomware - Malware, die den Opfern den Zugriff auf ihren Computer verweigert oder wichtige Daten auf den Systemen verschlüsselt. Der Name leutet sich von ransom (Erpressung) und ware (Software) ab.
+ Nach der Infektion fordern Erpresser ein Lösegeld um das System freizuschalten oder die Dateien zu entschlüsseln.
    + zahlen mit Kryptowährungen (Bitcoin, MoneyPak, ...) oder anderen Online-Zahlungsmethoden
    + Aber keine Garantie, dass die Opfer nach der Zahlung wieder voll auf ihre Systeme zugreifen können.
+ Wie wird Ransomware auf dem System des Opfers installiert?
    + Durch das Öffnen von bösartigen E-Mai-Anhängen
    + Durch die Installation von gefälschter Software mit Malware
    + Durch den Zugriff auf bösartige Webseiten
+ Wie sich Ransomware bemerkbar macht
    + Blockiert Bildschirm
    + Warnungen und Pop-up-Meldungen von Erpresserbriefen
    + System funktioniert nicht mehr
+ Einige Eansomeware-Varianten "schlafen" zunächst unbemerkt auf dem System und werden später von den Angreifern "angeschaltet"

### Keylogger
Keylogger - Werkzeug zum Aufzeichnen oder Erfassen der gedrückten Tasten auf einer Tastatur (tastenanschlag).
+ Ein legales Werkzeug, das für rechtliche Zwecke verwendet werden kann.
    + Untersuchung des Tippverhaltens
    + Überwachung der Fernarbeit von Mitarbeitern


## Schutzmaßnahmen
### Schutzmaßnahmen gegen Malware
#### Programm-Updates
Programm-Updates schließen Systemschwachstellen und beseitigen Sicherheitsrisiken
+ Verwendung älterer Software-Versionen = Sicherheitsrisiko
+ Gefahr des Missbrauchs von öffentlich bekannten Sicherheitslücken

Updates installieren, sobald sie verfügbar sind.
+ Hersteller finden nicht alle Fehler in der Testphase
+ Viele Sicherheitslücken in Programmen werden oft erst während der Nutzung entdeckt
    + Auch durch Angriffe oder Analyse durch externe Experten
+ Bekannte Sicherheitslücken können in der Regel geschlossen werden durch kleinere Update-Pakete
+ Derzeit stellen die meisten Programme automatisch Informationen über verfügbare Updates bereit.
+ Es gibt Hilfsprogramme, die automatisch nach Updates der installierten Software suchen.
+ Auch gute Antivirenprogramme prüfen, ob die installierte Software aktuell ist.

**Aber bei allen Updates:**  
+ Die Vertrauenswürdigkeit der Quelle von Updates muss immer geprüft werden, um sicherzusatellen, dass die Updates echt sind. Andernfalls können Updates zu einer Sicherheitslücke werden, die zur Installation von Malware oder über Cyber-Attacke ausgenutzt werden können.

#### Anti-Viren-Software
Anti-Viren-Software auch Anti-Malware-Software genant bietet Methoden zur Erkennung von im Computersystem installierte Malware.
+ Erkennt Viren, Würmer, Trojaner, Sypware, Scareware und andere Malware-Typen.
+ Es überwacht auch Internetverbindungen und warnt vor den Zugriff auf unsichere Webseiten.
+ Das Programm sollte ein obligatorischer Bestandteil eines jeden Systems sein, um die Sicherheit des Computersystems zu gewährleisten.

#### Backups
Viele Malware-Angriffe im Internet führen zu Datenverlust oder Beschädigung. 
+ Im Falle eines Datenverlustes durch Schadsoftware oder Beschädigung des Betriebssystems können die Daten mit zuvor erstellten Sicherungskopien wiederhergestellt werden.
+ Wichtige und persönliche Daten müssen regelmäßig gesichert werden.
+ Viele Systeme bieten eine automatische Datensicherung in vordefinierten Intervallen.
+ Speicherung der (verschlüsselten) Sicherung auf externen Medien oder in der Cloud.
+ Achtung! Wenn es einem Angreifer gelingt sich Zugang zum Computer zu verschaffen, könnte der Benutzer den Zugriff auf die Backups verlieren.

#### Firewalls
Firewalls überwachen Netzwerk-Verbindungen und den entsprechenden Datenverkehr.
+ Können unautorisierte Verbindungsversuche verhindern
+ Zusätzlicher Schutz vor Netzwerkangriffen, wie z.B. Angriffe von Backdoors und Botnets.
+ Lokale Firewall funktioniert nur auf dem Rechner, auf dem sie installiert ist.
+ Netzwerk-Firewall überprüft den gesamten Netzwerkverkehr und wird in der Regel auf Verbindungsknoten zwischen dem lokalen Netzwerk und dem Internet installiert.

#### "Gesunder" Verdacht - Immer vorsichtig sein.
Der Verdacht ist der effektivste Schutz, der von den Anwerndern gegen Malware-Infektionen angewendet werden kann.
+ Die besten Schutzmechanismen sind nicht mehr wirksam, wenn der Benutzer nicht vertrauenswürdige Inhalte öffnet.
+ Prüfen Sie bei der Installation neuer Software immer Hersteller und Herkunft der Software.
+ Überprüfen Sie die Signatur der zu installierenden Software / Updates (kann automatisch durchgeführt werden)
+ Wenn eine Warnung erscheint, ist eine manuelle Überprüfung notwendig.
+ Nur Software installieren, die wirklich benötigt wird.
    + Installieren Sie keine unnötigen Anwendungen, Zusatzfunktionen oder optionale Plugins. Sie bieten einen unnötigen Zugangspunkt für Angreifer.
+ Aktive Inhalte (Flash,Java,Active X) im Webbrowser standardmäßig deaktivieren, da sie eine Reihe von verschiedenen Angriffs- und Einbruchsmöglichkeiten bieten.
+ E-Mail Anhänge nur öffnen wenn:
    + der Absender bekannt ist und der Text dem Absender zugeordnet werden kann.
    + eine E-Mail mit Anhängen erwartet wird.
+ Ruhe Bewahren bei (oft gefälschten) Online-Abmahnungen und Aufforderungen zur Zahlung von Bußgeldern.
+ Überprüfung von Installierter Software und entfernen unbenutzter Programme.

#### Schutz von Mobilen Geräten
+ Anwendungen nur aus vertrauenswürdigen Quellen beziehen
    + vorzugsweise nur aus offiziellen App Stores
    + Vorsichtig sein bei (neuen) Apps mit keinen oder wenigen Bewertungen
+ Apps und Betriebssystem des mobilen Geräts immer auf dem neusten Stand halten.
    rechtzeitige Installation von Updates
+ Backups erstellen
    + System kann aus altem Backup wiederhergestellt werden im Falle einer Infektion.
+ Apps immer nur minimale Berechtigung gewähren
    + Kann beim ersten Start oder in den Einstellungen eingerichtet werden.
    + Berechtigungen entsprechend den Funktionen der App auswählen.
        + Beispiel: Die Taschenlampen-App benötigt keinen Zugriff auf die Kontaktliste

### Passwort
#### Das Sichere Passwort
+ Wie werden Passwörter geknackt?
    + Die wenigsten Passwörter werden wirklich geklaut.
    + Die meisten Passwörter werden einfach erraten.
+ Ein Computer kann mehrere tausend Vergleiche pro Sekunde durchführen, somit sind alle kurzen Passwörter, selbst wenn sie aus zufälligen Zeichen bestehen nicht sicher!

#### Passwortverfahren
+ Probleme für Anwender: regelmäßige Passwortänderung.
+ Passwörter: *Quadratur des Kreises*
    + Passwörter dürfen nicht zu leicht zu knacken sein.
    + Passwörter muss man sich leicht merken.

#### Häufige Probleme bei Passwörtern
+ schwache Passwortregeln
+ schlechte Passworterneuerungsverfahren
+ schlechter Schutz gegen Brut-Force-Angriffe
+ unveränderbare Passwörter
+ unsichere Speicherung der Passwörter
+ unsicherer Transport der Passwörter

#### Das sichere Passwort
Passwörter sollten aus folgenden Elementen bestehen:
+ Großbuchstaben (ABCDEF...)
+ Kleinbuchstaben (abcdef...)
+ Sonderzeichen (!"§$%&)
+ Zahlen (1234567...)
Passwörter, die nicht mindestens 3 Sorten von Zeichen enthalten und kürzer als 8 Zeichen sind, sind in wenigen Minuten, wenn nicht Sekunden geknackt.

+ **Unsicher** sind Passwörter besonders, wenn sie persönliche Informationen enthalten wie:
    + Name, Geburtsdaten, o Ä von Freunden, Familie oder Haustieren
+ Die Passwörter können dann mit sogenannten **Wörterbuchangriffen** herausgefunden werden. Dabei wird eine Liste von Wörtern, die der Hacker aus dem persönlichen Umfeld der Zielperson entnommen hat, in eine Liste gepackt und durcheinander oder zusammengesetzt ausprobiert. Dabei kann der Hacker sein Programm so schreiben, dass beliebige Manipulationen an den möglichen Passwörtern vorgenommen werden können.

