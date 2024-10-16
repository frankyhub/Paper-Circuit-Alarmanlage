<a name="oben"></a>

<div align="center">

|[:skull:ISSUE](https://github.com/frankyhub/Paper-Circuit-Alarmanlage/issues?q=is%3Aissue)|[:speech_balloon: Forum /Discussion](https://github.com/frankyhub/Paper-Circuit-Alarmanlage/discussions)|[:grey_question:WiKi](https://github.com/frankyhub/Paper-Circuit-Alarmanlage/wiki)||
|--|--|--|--|
| | | | |
|![Static Badge](https://img.shields.io/badge/RepoNr.:-%2012-blue)|<a href="https://github.com/frankyhub/Paper-Circuit-Alarmanlage/issues">![GitHub issues](https://img.shields.io/github/issues/frankyhub/Paper-Circuit-Alarmanlage)![GitHub closed issues](https://img.shields.io/github/issues-closed/frankyhub/Paper-Circuit-Alarmanlage)|<a href="https://github.com/frankyhub/Paper-Circuit-Alarmanlage/discussions">![GitHub Discussions](https://img.shields.io/github/discussions/frankyhub/Paper-Circuit-Alarmanlage)|<a href="https://github.com/frankyhub/Paper-Circuit-Alarmanlage/releases">![GitHub release (with filter)](https://img.shields.io/github/v/release/frankyhub/Paper-Circuit-Alarmanlage)|
|![GitHub Created At](https://img.shields.io/github/created-at/frankyhub/Paper-Circuit-Alarmanlage)| <a href="https://github.com/frankyhub/Paper-Circuit-Alarmanlage/pulse" alt="Activity"><img src="https://img.shields.io/github/commit-activity/m/badges/shields" />| <a href="https://github.com/frankyhub/Paper-Circuit-Alarmanlage/graphs/traffic"><img alt="ViewCount" src="https://views.whatilearened.today/views/github/frankyhub/github-clone-count-badge.svg">  |<a href="https://github.com/frankyhub?tab=stars"> ![GitHub User's stars](https://img.shields.io/github/stars/frankyhub)|
</div>





# Paper-Circuit-Alarmanlage
Einfache Alarmanlage mit zwei Transistoren und einer LED

Nach einer Idee von [Alex Kutschera](https://github.com/vektorious)

## Schaltplan

![Schaltplan](/pic/Schaltplan.png)

---

## Funktion

Die in der Schaltung genutzten Transistoren sind "NPN" Transistortypen (Pfeil nach außen). Die Spannung bei NPN-Transistoren muss an B +0,7V größer gegenüber E sein, damit der NPN-Transistor durchschaltet, wobei gilt: K benötigt eine positivere Spannung als E.

Ist die Alarmschleife <b>nicht</b> unterbrochen, bringt R3 über R1 und die LED eine Spannung von >0,7V an die Basis von T2. 
T2 ist deshalb leitend und hat einen geringen Widerstand zwischen E (Emitter) und K (Kollektor). Damit hat B, die Basis von T1 eine Spannung von <0,7V und sperrt. Die LED leuchtet nicht.

Im Alarmfall ist die Alarmschleife unterbrochen und die Spannung an B von T2 geht auf etwa 0Volt, damit sperrt T2. Wenn T2 sperrt, ist sein Widerstand wesentlich größer als R2 (22kOhm), weshalb über R2 dann eine Spannung >0,7 Volt an die Basis von T1 gelangt, dieser schaltet durch und die LED leuchtet.

Auch ein erneutes verbinden der Unterbrechung in der Alarmschleife bringt kein abschalten der LED, da die Spannung am Kollektor von T1, an R3 und D1 fast 0Volt beträgt. An der Basis von T2 liegt keine Spannung >0,7Volt an, T2 sperrt deshalb. 
Erst die Betätigung des Tasters S1 nach dem wiederverbinden der Alarmschleife setzt die Schaltung wieder auf "bereit".

---

## Paper Circuit

Verwende beidseitig leitendes CU-Klebeband.

![PaperCircuit](/pic/Paper-Circuit.png)


Farbcode der Widerstände:

![R](/pic/22k.png)


![R](/pic/470k.png)


![R](/pic/1M.png)

---

## BOM

| Stück | Bezeichnung |
| -------- | -------- | 
| 1        | 9V Clipp       | 
| 1        | 9V Batterie        | 
| 1        | R 470k        | 
| 1        | R 22k       | 
| 1        | R 1M        |
| 1        | LED 5mm rot        |
|2         | BC548       |
| 1        | [Taster](https://www.amazon.de/dp/B00SPUPVGU/?coliid=IHH4IX8I4SJ2L&colid=4ZNEYUX0MP5W&psc=1&ref_=list_c_wl_lv_ov_lig_dp_it_im)      |
| 1        | Schaltdraht        |
| 1        | CU-Band       |

---

<div style="position:absolute; left:2cm; ">   
<ol class="breadcrumb" style="border-top: 2px solid black;border-bottom:2px solid black; height: 45px; width: 900px;"> <p align="center"><a href="#oben">nach oben</a></p></ol>
</div>

---

