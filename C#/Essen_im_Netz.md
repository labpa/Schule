# Essen im Netz

## Gegeben
MySQL-Server
c#-Programm

## Ausgabe einer Liste mit Essen vom Server

## MySql

+ MySql-Server:
    + Datenbank:    Lieferdienst
    + Tabelle:      Essen 

### Datenbank erstellen
1. Starten in der Shell: mysql -u root 

2. 
+ Erstellen der Datenbank: create database 
+ Datenbank benutzen:         lieferdienst; use lieferdienst;

```SQL
MariaDB [lieferdienst]> create table essen (
    -> eid int auto_increment primary key,
    -> bezeichnung varchar(50),
    -> preis decimal(5,2));
```
Screenshoot 

![Alt text](./img/mysql.PNG)

### User erstellen
+ User Erstellen
```SQL
MariaDB [lieferdienst]> create user ronny@localhost identified by "1234";
Query OK, 0 rows affected (0.014 sec)
```
+ User rechte zuweisen
```SQL
MariaDB [lieferdienst]> grant select on lieferdienst.essen to ronny@localhost;
Query OK, 0 rows affected (0.006 sec)
```
+ kontrollieren 
    + root abmelden: ```SQL exit; ```
    + ronny anmelden: ```SQL mysql -u ronny -p ```

+ Ronny versucht etwas in die Tabelle einzufügen
```SQL
MariaDB [lieferdienst]> insert into essen (bezeichnung, preis) values ("Kartoffelbrei mit zwiebeln", 12.99);
ERROR 1142 (42000): INSERT command denied to user 'ronny'@'localhost' for table 'essen'
```

## Server
1. Apache starten
2. Ordner Prog in Verzeichnis: C:\xampp\htdocs erstellen 

## PHP
In Notepad++ wird ein neues PHP dokument mit folgendem Inhalt erstellt:

```php
<?php
	//Verbindung zur Datenbank
	$db = new mysqli("localhost", "ronny", "1234", "lieferdienst");
	
	//Erstellen SQL
	$sql = "select eid, bezeichnung, preis from essen";
	
	//wir senden die sql an den DB-Server
	//wir erhalten Zeiger an Anfang der Tabelle (vor der 1. Zeile)
	$tabelle = $db->query($sql);
	
	//wir holen die 1. Zeile in der Tabelle
	//fetch_assoc: assoziatives Array für eine Zeile
	//Zuordnung: feld->Wert
	$zeile = $tabelle->fetch_assoc();
	
	//solange noch eine zeile in der Tabelle
	while($zeile == true)
	{
		//Ausgabe der Zeile
		print_r($zeile);
		print("<br/>");
		
		//hohle die nächste Zeile
		$zeile = $tabelle -> fetch_assoc();
	}
	
	//Schließen Verbindung
	$db->close();
```

Zweite Variante:
```php
<?php
	//Verbindung zur Datenbank
	$db = new mysqli("localhost", "ronny", "1234", "lieferdienst");
	
	//Erstellen SQL
	$sql = "select eid, bezeichnung, preis from essen";
	
	//wir senden die sql an den DB-Server
	//wir erhalten Zeiger an Anfang der Tabelle (vor der 1. Zeile)
	$tabelle = $db->query($sql);
	
	//wir holen die 1. Zeile in der Tabelle
	//fetch_assoc: assoziatives Array für eine Zeile
	//Zuordnung: feld->Wert
	$zeile = $tabelle->fetch_assoc();
	
	//solange noch eine zeile in der Tabelle
	while($zeile == true)
	{
		//Ausgabe der Zeile
		print "$zeile[eid] <br/> $zeile[bezeichnung] <br/> $zeile[preis] <br/> <br/>";
		print("<br/>");
		
		//hohle die nächste Zeile
		$zeile = $tabelle -> fetch_assoc();
	}
	
	//Schließen Verbindung
	$db->close();
```




Das PHP Dokument wird als essen.php unter C:\xampp\htdocs\Prog abgespeichert.

## Ausgabe Browser
Zur Kontrolle im Browser folgenden link eingeben:
http://localhost/prog/essen.php

Ausgabe im Browser:
```PHP
Array ( [eid] => 1 [bezeichnung] => Pizza Funghi [preis] => 8.89 )
Array ( [eid] => 2 [bezeichnung] => Bulette [preis] => 4.99 )
Array ( [eid] => 3 [bezeichnung] => Gem?sepfanne [preis] => 6.99 )
Array ( [eid] => 4 [bezeichnung] => Creme brulee [preis] => 5.59 )
```

Seitenquelltext im Browser:
```html
Array
(
    [eid] => 1
    [bezeichnung] => Pizza Funghi
    [preis] => 8.89
)
<br/>Array
(
    [eid] => 2
    [bezeichnung] => Bulette
    [preis] => 4.99
)
<br/>Array
(
    [eid] => 3
    [bezeichnung] => Gem?sepfanne
    [preis] => 6.99
)
<br/>Array
(
    [eid] => 4
    [bezeichnung] => Creme brulee
    [preis] => 5.59
)
<br/>
```

## Hinzufügen von json_encode

```php
<?php
	//Verbindung zur Datenbank
	$db = new mysqli("localhost", "ronny", "1234", "lieferdienst");
	
	//Erstellen SQL
	$sql = "select eid, bezeichnung, preis from essen";
	
	//wir senden die sql an den DB-Server
	//wir erhalten Zeiger an Anfang der Tabelle (vor der 1. Zeile)
	$tabelle = $db->query($sql);
	
	//wir holen die 1. Zeile in der Tabelle
	//fetch_assoc: assoziatives Array für eine Zeile
	//Zuordnung: feld->Wert
	$zeile = $tabelle->fetch_assoc();
	
	//wir erstellen ein neues Array
	$daten = array();
	
	//solange noch eine zeile in der Tabelle
	while($zeile == true)
	{
		//wir fügen die Zeile dem Array hinzu
		array_push($daten, $zeile);
		
		//Ausgabe der Zeile
		//print_r($zeile);
		//print("<br/>");
		
		//print "$zeile[eid] <br/> $zeile[bezeichnung] <br/> $zeile[preis] <br/> <br/>";
		
		//hohle die nächste Zeile
		$zeile = $tabelle -> fetch_assoc();
	}
	
	//wir wandeln das Array in eine Zeichenkette - formatierung nach JSON - um
	$text = json_encode($daten);
	
	
	//wir lassen und den text ausgeben
	print $text;
    
	//Schließen Verbindung
	$db->close();
```
