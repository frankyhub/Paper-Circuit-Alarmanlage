# Paper-Circuit-Alarmanlage
Einfache Alarmanlage mit zwei Transistoren und einer LED

Nach ener Idee von [Alex Kutschera](https://github.com/AlexKutschera)

![Schaltplan](/pic/Schaltplan.png)

## Funktinon
Die in der Schaltung genutzten Transistoren sind "NPN" Transistortypen (Pfeil nach außen). Die Spannung an B muss +0,7V gegenüber E sein, damit der Transistor durchschaltet, wobei gilt K benötigt eine positivere Spannung als E.
Im Alarmfall wird die Alarmschleife unterbrochen. Ist die Alarmschleife nicht unterbrochen, bringt R3 über R1 und die LED eine Spannung von > 0,7V an die Basis von T2. 
T2 ist leitend undhat einen geringen Widerstand zwischen E (Emitter) und K (Kollektor). Damit hat B, die Basis von T1 eine Spannung von <0,7V, und sperrt. Die LED leuchtet nicht.
Im Alarmfall geht die Spannung an B von T2 auf etwa 0Volt damit sperrt T2. Wenn T2 sperrt ist sein Widerstand wesentlich größer als R2 (22kOhm), weshalb über R2 dann eine 
Spannung >0,7 Volt an die Basis von T1 gelangt, dieser schaltet durch, die LED leuchtet.
Auch ein erneutes verbinden der Unterbrechung in der Alarmschleife bringt kein abschalten, da T1 die Spannung am Kollektor, an R3 und D1 fast 0Volt beträgt. An der Basis von T2 liegt keine Spannung größer 0,7Volt an, T2 sperrt deshalb. 
Erst die Betätigung des Tasters nach dem wiederverbinden der Alarmschleife setzt die Schaltung wieder auf "bereit".

----
----

