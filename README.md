# Ubuntu Samba
Om Linux als fileserver in een Windows netwerk te laten opereren, moet de Linux machine als Smba server worden geconfigureerd. Samba komt van SMB wat staat voor Service Message Block.

## Demo installatie en gebruik vagrant
Youtube: https://youtu.be/KABnIuaA8SM

## Voorwaarden software

De volgende software is nodig:
  * Virtualbox 5.0 of hoger
  * Git bash voor Windows
  * Vagrant 2.2.6 of hoger

## Installatie voor Windows
  * Installeer Virtualbox: https://www.virtualbox.org/wiki/Downloads
  * Installeer Git bash for Windows: https://gitforwindows.org/
  * Installeer Vagrant for Windows: https://www.vagrantup.com/downloads.html


## Het starten van vagrant
Open <b>Git Bash</b> in Windows en typ de volgende commandos:
  1. cd Documents;
  2. mkdir vagrant && cd vagrant *(tenzij de map vagrant al bestaat)*;
  3. git clone https://github.com/mbockstael/Ubuntu-samba.git;
  4. **cd Ubuntu-samba**;
  5. vagrant up;
  6. vagrant ssh;

## Opdracht
Je vind je opdracht op je virtuele omgeving in ***~/student/opdracht***

## Netwerk
De Vagrant VM zal 2 netwerk adapters hebben:
  * Nat : DHCP
  * Localhost : 192.168.10.101

## Vagrant commandos
Vagrant VM opstarten
```
vagrant up
```
Stoppen en afsluiten van de VM
```
vagrant halt
```
Verwijderen van een VM
```
vagrant destroy
```
ssh naar de VM
```
vagrant ssh
```
