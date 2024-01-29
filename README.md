# Paper-Circuit-Alarmanlage
Einfache Alarmanlage mit zwei Transistoren und einer LED

Nach einer Idee von [Alex Kutschera](https://github.com/vektorious)

![Schaltplan](/pic/Schaltplan.png)


## Funktion

Die in der Schaltung genutzten Transistoren sind "NPN" Transistortypen (Pfeil nach außen). Die Spannung bei NPN-Transistoren muss an B +0,7V größer gegenüber E sein, damit der NPN-Transistor durchschaltet, wobei gilt: K benötigt eine positivere Spannung als E.

Ist die Alarmschleife <b>nicht</b> unterbrochen, bringt R3 über R1 und die LED eine Spannung von >0,7V an die Basis von T2. 
T2 ist deshalb leitend und hat einen geringen Widerstand zwischen E (Emitter) und K (Kollektor). Damit hat B, die Basis von T1 eine Spannung von <0,7V und sperrt. Die LED leuchtet nicht.

Im Alarmfall ist die Alarmschleife unterbrochen und die Spannung an B von T2 geht auf etwa 0Volt, damit sperrt T2. Wenn T2 sperrt, ist sein Widerstand wesentlich größer als R2 (22kOhm), weshalb über R2 dann eine Spannung >0,7 Volt an die Basis von T1 gelangt, dieser schaltet durch und die LED leuchtet.

Auch ein erneutes verbinden der Unterbrechung in der Alarmschleife bringt kein abschalten der LED, da die Spannung am Kollektor von T1, an R3 und D1 fast 0Volt beträgt. An der Basis von T2 liegt keine Spannung >0,7Volt an, T2 sperrt deshalb. 
Erst die Betätigung des Tasters S1 nach dem wiederverbinden der Alarmschleife setzt die Schaltung wieder auf "bereit".


## Paper Circuit
![PaperCircuit](/pic/Paper-Circuit.png)

[Taster](https://www.amazon.de/dp/B00SPUPVGU/?coliid=IHH4IX8I4SJ2L&colid=4ZNEYUX0MP5W&psc=1&ref_=list_c_wl_lv_ov_lig_dp_it_im)

----
----

