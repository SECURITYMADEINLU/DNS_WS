# Phase 4 

## Préparation
*Nombre de participants* : 15 enfants, répartis en n groupes (possiblement 15 groupes de 1) et 1 animateur (sans préjuger des lois et réglementations locales)
*Matériel*: 
* n canevas à compléter
* n sets de cartes (6 cartes par set) représentant chacune des ressources à assembler
* 1 vidéo-projecteur

## Objectifs détaillés
Les objectifs pédagogiques sont les suivants:
* Appréhender le concept de botnet
* Appréhender le concept de déni de service distribué
* Appréhender le concept de Single Point of Failure représenté par le DNS


## Concepts abordés
Les concepts abordés durant cette phase sont les suivants :
* Botnet
* Saturation


Les mots clefs suivants permettront au formateur d'approfondir le sujet par lui-même sur Internet:
DNS, botnet, malware, Déni de service, DDoS

Les définitions suivantes peuvent être utiles
* DNS: Domain Name System, Système de nommage des domaines. Permettant d'associer le nom d'un serveur (ex: www.facebook.com) à  une adresse IP (ex: 251.26.54.5)
* Botnet : réseau d'ordinateurs infectés devenus des bots, ou zombies, et utilisés par des criminels pour des actions comme des DDOS
* Déni de service: action malveillante visant à saturer un serveur de requêtes pour l'empêcher de répondre aux requêtes légitimes
* DDoS: Déni de service distribué. Des milliers, voire des millions de machines sont utilisés pour réaliser un Déni de service simultané sur une même cible. 

## Contexte extérieur
Cet atelier permet de présenter les réseaux d'ordinateurs infectés (Botnet) et leurs actions de dénis de service. Actuellement, les attaques DDoS permettent de neutraliser des services comme DNS (on peut penser à l'attaque du 22 octobre 2016 contre les DNS de l'entreprise DYN qui ont paralysé une partie des sites comme Twitter, PSN, etc.: http://www.numerama.com/tech/203154-panique-aux-usa-des-dizaines-de-sites-web-inaccessibles-apres-une-attaque-ddos.html). 


## Déroulé
Comme dans la phase 3, les enfants disposent d'un canevas à compléter par groupe, et du modèle qu'ils auront choisi à la phase 2 projeté par vidéo-projecteur. Les groupes d'enfants sont répartis entre une équipe bleue (Blue-Team) et une rouge (Red-Team). La répartition peut être de l'ordre de 1 groupe pour la Red-Team pour 14 pour la Blue-Team. L'objectif, connu publiquement, de chaque groupe de la Blue-Team est de constituer le plus rapidement possible son puzzle. 

Lors d'un passage, le groupe interrogé demande sa pièce au résolveur DNS joué par l'animateur. Celui-ci lui répond et donne la pièce. La Red-Team va alors effectuer un nombre de requêtes illégitimes correspondant au nombre X de motifs complets trouvés pour ce groupe à l'étape 3. L'animateur va alors passer le tour des X groupes suivants.

L'animateur peut alors présenter les problématiques de déni de service distribué et l'aspect crucial du serveur DNS sans lequel aucun service n'est accessible. 



## Liens utiles
* [Changer son résolveur DNS, Stephane Bortzmeyer](http://www.bortzmeyer.org/changer-dns.html)
* [Panne des résolveurs DNS d'Orange, Stéphane Bortzmeyer](http://www.bortzmeyer.org/resolveur-dns-en-panne.html)
* [Dyn: Point technique sur NextImpact](https://www.nextinpact.com/news/101871-dyn-on-fait-point-sur-attaque-ddos-qui-a-impactee-nombreux-sites.htm)
