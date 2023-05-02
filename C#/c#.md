# Objektorientierte Programmierung mit C#

+ Prezedurale Programmierung: 
    + Variablen für die Speicherung


+ Objektorientierte Programmierung:
    + VAriablen und Prozeduren (Methoden) werden in Klassen zusammengefasst.
    |Bezeichnung|Preis|Menge|
    |---|---|---|
    ||||

Ausgangspunkt bei der Programmierung: Daten die gespeichert werden sollen.


1. Programmaufbau  
--> was gibt es im Programm

2. Programmablauf  
--> welche Artikel habe ich  
--> Auswahl Artikel für Verkauf  
--> Ausgabe ergebnis (Kann verkauft werden oder nicht)

## Erstellen eines Programms mit C#
--> Visual Studio 2022 --> Neues Projekt --> C# -->

Links: Programm  
Rechts: Bibliotheken / Verweise *.dll (dynamic link libraries)

Namensraum: jedes Projekt kann bestehen aus mehreren Klassen, die werden in Namensräumen / Paketen organisiert (Zusammengefasst)

ein Namensraum enthält eine Klasse

die Klasse enthält eine Methode, die bei Start des Programms ausgeführt wird

### Beispiel 1
Der Nutzer gibt eine ganze Zahl ein und das Programm gibt das Quadrat der Zahl aus.  
--> Wir orientieren und am EVA-Prinzip.  
Eingabe (eine ganze Zahl) Deklaration einer Variablen (1. Variablenname 2. Datentyp) --> Verarbeitung (quadrat = Zahl * Zahl) Wertzuweisung --> rechnen Zahl * Zahl und speichere in Variablen quadrat. Deklaration einer Variablen --> Ausgabe (das Quadrat)

Datentyp: int
--> was kann gespeichert werden
--> wie viel byte für die Speicherung

## Projekt Kontrollstrukturen
Kontrollstrukturen:  
Eingabe, Ausgabe, Deklaration von Variablen  
Verzweigung (if, switch)  
Wiederholungen (while, do...while, for)  
Array (foreach)

Aufrufen von Unterprogrammen
## Code Tag1

### Methoden.cs
```c#
using System;
using System.Collections;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Kontrollstrukturen
{
    internal class Methoden
    {
        /* Nach Eingabe eines Radius soll das Programm das Volumen einer Kugel ausgeben */
        public static void Beispiel1()
        {
            //Deklaration von Variablen (für Eingaben und Rechnung)
            double radius = 0, volumen = 0;

            //Eingabe von Radius
            Console.Write("Radius: ");

            double.TryParse(Console.ReadLine(), out radius);

            //Wertzuweisung
            //Literale 4 und 3 --> das sind ganze Zahlen (4/3 =>1) Also einen Punkt anhängen aus 4 wird 4.0 usw...
            volumen = 4.0 / 3.0 * Math.PI * Math.Pow(radius, 3);

            // Ausgabe
            Console.WriteLine("Volumen: " + volumen);
        }
    
        /* Wenn der Nutzer eine gerade Zahl eingibt öffnet sich das Tor zur Hölle*/
        public static void Beispiel2()
        {
            //Deklaration einer Variablen für die Eingabe
            int zahl;
            //Eingabe einer Zahl

            int.TryParse(Console.ReadLine(), out zahl);

            //WENN zahl gerade
            // im if() immer nur ein Vergleich
            //WANN ist eine zahl gerade: wenn der Rest bei Division durch 2 gleich 0 ist
            if(zahl%2 == 0)
            {
                Console.WriteLine("Welcome to hell");
            }
            else
            {
                Console.WriteLine("geh weg");
            }


        }
    
        /* Nach Eingabe von zwei Zahlen und Auswahl von + oder - wird das Ergebnis ausgegeben */
        public static void Beispiel3()
        {
            int zahl1, zahl2;
            char wahl; //Rechenoperation + oder - --> ein Zeichen
            Console.Write("Zahl1: ");
            int.TryParse(Console.ReadLine(), out zahl1);

            Console.Write("Zahl2: ");
            int.TryParse(Console.ReadLine(), out zahl2);

            Console.Write("Wähle: + oder - ");
            char.TryParse(Console.ReadLine(), out wahl);

            if (wahl == '+')
            {
                Console.WriteLine("Summe: " + (zahl1 + zahl2));
            }
            else if(wahl == '-')
            {
                Console.WriteLine("Differenz: " + (zahl1 - zahl2));
            }
            else
            {
                Console.WriteLine("Geh weg");
            }

            //Alternative: Fallunterscheidung (switch)
            switch (wahl)
            {
                case '+':
                    Console.WriteLine("Summe: " + (zahl1+zahl2));
                    break; //jeder Fall muss mit break beendet werden
                case '-':
                    Console.WriteLine("Differenz: " + (zahl1 - zahl2));
                    break;
                default:
                    Console.WriteLine("Geh Weg");
                    break;
            }



        }

        public static void Beispiel4()
        {
            decimal stunden = 0m;
            decimal lohn =  18.50m;
            decimal mehr = 0m;

            Console.Write("Gearbeitete Stunden: ");
            decimal.TryParse(Console.ReadLine(), out stunden);
            mehr = stunden - 170;

            if(stunden > 170)
            {
                Console.WriteLine((lohn*stunden)+((lohn*mehr)/100*20));
            } else
            {
                Console.WriteLine(stunden * lohn);
            }
        }


        public static void Beispiel5()
        {
            decimal rabatt = 0;
            decimal stueck = 0;

            Console.Write("Gewünschte Stückzahl: ");
            decimal.TryParse(Console.ReadLine(), out stueck);

            if(stueck < 100)
            {
                Console.WriteLine("Mengenrabatt von 2%");
            } else if (stueck >= 100 &&  stueck <= 200)
            {
                Console.WriteLine("Mengenrabatt von 10%");
            } else
            {
                Console.WriteLine("Mengenrabatt von 12%");
            }
        }


        public  static void Beispiel6()
        {
            decimal ticket = 2.00m;
            bool tag;
            bool woche;
            bool monat;

            Console.Write("Gewünschte Stückzahl: ");
            bool.TryParse(Console.ReadLine(), out tag);

            if (tag= true)
            {
                Console.WriteLine("Das Ticket kostet" + ticket + "€");
            } else if ( woche  = true )
            {
                Console.WriteLine("Das Ticket kostet" + ticket * 7 + "€");
            } else
            {
                Console.WriteLine("Das Ticket kostet" + ticket*30 + "€");
            }

        }


        /* 
         Der Nutzer gibt zwei Zahlen ein, die zweite Zahl darf aber nicht 0 sein.
         d.h. der Nutzer gibt die 2. Zahl so lange ein, bis diese nicht mehr 0 ist.
        */
        public static void Beispiel7()
        {
            double zahl1, zahl2;

            Console.Write("Zahl1: ");
            double.TryParse(Console.ReadLine(), out zahl1);

            //fußgesteuerte Schleife -- wird mindestens einmal gemacht.
            do 
            { 
                Console.Write("Zahl2: ");
                double.TryParse(Console.ReadLine(), out zahl2);
            }
            while (zahl2 ==0); //solange gilt... wiederhole ab do
            Console.WriteLine("Quotient: " + (zahl1 / zahl2));
        }

        /* Ein Nutzer gibt 10 Zahlen ein. Das Programm gibt die Summe der Zahlen aus*/
        public static void Beispiel8()
        {
            int zahl;
            int summe = 0;
            int anzahl = 1;



            while (anzahl < 11)
            {
                Console.Write("Geben Sie Zahl " + anzahl + " ein: ");
                int.TryParse(Console.ReadLine(), out zahl);
                summe = summe + zahl;
                anzahl++;
            }
            Console.WriteLine("Die Summe beträgt: " + summe);
            }

        public static void Beispiel9()
        {
            decimal zahl=  1;
            decimal summe = 0;
            decimal durchschnitt = 1;
            decimal anzahl = 0;
            while (zahl > 0)
            {
                Console.Write("Geben Sie eine Zahl ein: ");
                decimal.TryParse(Console.ReadLine(), out zahl);
                summe = summe + zahl;
                anzahl++;
                durchschnitt = summe / anzahl ;
            }
            Console.WriteLine("Die Summe beträgt:  " + summe + "  Der Durschnitt beträgt:" + durchschnitt);
        }

        //public static void Beispiel10()
        //{
        //    decimal kilometer;
        //    decimal mietkosten;

        //    Console.Write("Gefahrene Kilometer: ");
        //    decimal.TryParse(Console.ReadLine(), out kilometer);

        //    if (kilometer <= 200)
        //    {
        //        Console.WriteLine("");
        //    }




        //}











    }
}


```

### Programm.cs
```c#
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Kontrollstrukturen
{
    internal class Program
    {
        static void Main(string[] args)
        {
            //wir rufen das Beispiel auf
            //Methoden.Beispiel1();
            Methoden.Beispiel9();
        }
    }
}

```
