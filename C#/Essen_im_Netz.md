# Essen im Netz

## Gegeben
MySQL-Server
c#-Programm

## Ausgabe einer Liste mit Essen vom Server

+ MySql-Server:
    + Datenbank:    Lieferdienst
    + Tabelle:      Essen 

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


## Server
1. Apache starten
2. Ordner Prog in Verzeichnis: C:\xampp\htdocs erstellen 



Wir erstellen einen Nutzer, 