# B1-reseau-tp4

# I.Mise en place du lab

## 1.Création des réseaux

On crée les deux cartes réseaux sur VirtualBox en faisant fichier, host network manager, on crée deux cartes réseaux et on met les IP des cartes réseau suivantes :
* `10.1.0.1`  
* `10.2.0.1`  

On ne met pas de DHCP.

## 2.Création des VMs

Pour crée les clones du patron on fait un clique droit sur le patron et on fait "cloner".
Les trois clones ont une carte réseau avec une adresse IP différentes :
* `client1.tp4` a une adresse IP de `10.1.0.10`, elle servira de client (dans `net1`).
* `server1.tp4` a une adresse IP de `10.2.0.10`, elle servira de serveur (dans `net2`).
* `router1.tp4` a une adresse IP de `10.1.0.254` dans `net1` et une adresse IP de `10.2.0.254` dans `net2`, cette machine sera notre routeur, ce sera la passerelle de `client1` et `server1`