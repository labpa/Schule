# Essen im Netz

## Gegeben
MySQL-Server
c#-Programm

## Ausgabe einer Liste mit Essen vom Server

+ MySql-Server:
    + Datenbank:    Lieferdienst
    + Tabelle:      Essen 

1. Starten in der Shell: mysql -u root 

2. Erstellen der Datenbank: create database lieferdienst; use lieferdienst;

```SQL
MariaDB [lieferdienst]> create table essen (
    -> eid int auto_increment primary key,
    -> bezeichnung varchar(50),
    -> preis decimal(5,2));
```

Wir erstellen einen Nutzer, 