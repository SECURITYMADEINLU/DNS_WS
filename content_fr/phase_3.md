# Phase 3 

## Préparation
*Nombre de participants* : 15 enfants, répartis en n groupes (possiblement 15 groupes de 1) et 1 animateur (sans préjuger des lois et réglementations locales)
*Matériel*: 
* n canevas à compléter
* n sets de cartes (6 cartes par set) représentant chacune des ressources à assembler
* n sets de cartes (6 cartes par set) représentant les ressources corrompues
* 1 vidéo-projecteur

## Objectifs détaillés
Les objectifs pédagogiques sont les suivants:
* Appréhender le concept de choix éclairé de son résolveur DNS
* Appréhender le concept de résolveur DNS menteur
* Appréhender le concept de diffusion de contenu malveillant par réponse DNS corrompues/menteuses


## Concepts abordés
Les concepts abordés durant cette phase sont les suivants :
* DNS Menteur
* Choix de son résolveur DNS


Les mots clefs suivants permettront au formateur d'approfondir le sujet par lui-même sur Internet:
DNS, résolveur, ressources externes, adresse IP, nom de domaine, FQDN, blacklist

Les définitions suivantes peuvent être utiles
* DNS: Domain Name System, Système de nommage des domaines. Permettant d'associer le nom d'un serveur (ex: www.facebook.com) à  une adresse IP (ex: 251.26.54.5)
* Résolveur: serveur effectuant l'association entre nom de domaine et adresse IP
* Adresse IP : identifiant d'un ordinateuInternet Protocol), comme un numéro de téléphone
* FQDN: Fully Qualified Domain Name. Designation d'un hôte (ou machine) sur r sur le réseau Internet (IP signifie un domaine. Le schéma est alors hote.domaine.tld
* Domaine : ensemble d'ordinateurs liés 

## Contexte extérieur
Cet atelier est l'occasion d'introduire la problématique du choix de son résolveur DNS. Là où beaucoup d'utilisateurs n'accordent aucune importance à cet élément technique, et font le choix de résolveur dont la politique est discutable (Google DNS, OpenDNS, etc.), il est primordial de faire la balance entre fiabilité et efficacité.
Cet atelier est également l'occasion d'introduire les problématiques de diffusion de contenu malveillant, comme des charges virales en corrompant des sites légitimes.


## Déroulé
Les enfants disposent d'un canevas à compléter par groupe, et du modèle qu'ils auront choisi à la phase 2 projeté par vidéo-projecteur. Les groupes d'enfants sont répartis entre une équipe bleue (Blue-Team) et une rouge (Red-Team). La répartition peut être de l'ordre de 1 groupe pour la Red-Team pour 14 pour la Blue-Team. L'objectif, connu publiquement, de chaque groupe de la Blue-Team est de constituer le plus rapidement possible son puzzle. L'objectif, caché au public et connu uniquement de la Red-Team, de la Red-Team est de fausser la réalisation des puzzles de la Blue-Team en donnant des pièces corrompues.

Chaque groupe dispose devant lui d'un écriteau indiquant si il veut être servi par l'ancien ou le nouveau résolveur DNS. 
L'animateur représente l'ancien résolveur DNS. Il peut délivrer à chaque tour 1 pièce telle que demandée par le groupe de joueurs.
La Red-Team représente le nouveau résolveur DNS. Il peut délivrer à chaque tour 2 pièces telles que demandées par le groupe de joueurs.
Ces caractéristiques sont communiquées publiquement avant le début de la phase.

Ainsi, un groupe choisissant de n'utiliser que le résolveur nouveau complètera son puzzle 2 fois plus rapidement qu'un groupe ayant choisi de n'utiliser que l'ancien résolveur DNS. Le but de chaque groupe étant de constituer le plus rapidement son puzzle, il fera vraisemblablement le choix d'un nouveau résolveur DNS.

Lorsqu'un groupe termine son puzzle, il inscrit le numéro de tour lors duquel il a terminé son puzzle. C'est son score (temporaire), plus celui-ci est bas, plus le groupe aura terminé rapidement son puzzle et donc sera près de la première place.
Lorsque tous les groupes ont achevé leur puzzle, l'animateur révèle que les pièce données par la Red-Team ont pu être corrompues et qu'il faut révéler des motifs cachés. Ces motifs cachés peuvent être révélés à l'aide d'un filtre de couleur. Chaque pièce de puzzle dispose d'un certain nombre de demi-motifs qui en s'assemblant avec les pièces jointes peuvent rendre un motif complet. 
Chaque groupe compte alors le nombre de motifs complets. L'animateur indique alors qu'il s'agit du nombre d'infections réalisées. Ce nombre est un handicap et sera retranché du score temporaire. Ainsi: (score temporaire) - (nombre de motifs complets) = (score définitif)
Le groupe ayant le score définitif le plus faible gagne alors.

L'animateur peut alors faire un rappel sur l'importance de choisir son résolveur DNS correctement, ou du moins, de ne pas suivre les nombreux tutos sur Internet qui peuvent parfois promettre une plus grande rapidité au détriment de la sécurité.



## Liens utiles
* [Changer son résolveur DNS, Stephane Bortzmeyer](http://www.bortzmeyer.org/changer-dns.html)
