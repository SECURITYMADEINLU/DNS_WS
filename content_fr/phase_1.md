# Phase 1 

## Préparation
*Nombre de participants* : 16 enfants, répartis en 4 groupes et 1 animateur (sans préjuger des lois et réglementations locales)

*Matériel*: 
* 1 canevas connu d'un site déterminé à l'avance (ex: www.wort.lu)
* 12 enveloppes numérotées (3 portant le numéro 1, 3 le numéro 2, 3 le 3, 3 le 4) et portant chacun le FQDN d'un serveur à interroger 
* 12 écriteaux (chevalets papiers) portant les numéros 1 à 12 (un numéro par chevalet)
* 8 listes de correspondance entre numéro d'enfants et domaines de second niveau
* 8 listes de correspondance entre numéro d'enfants et domaines de troisième niveau
Les listes et le contenu des enveloppes sont détaillés dans la fiche jointe.

## Objectifs détaillés
Les objectifs pédagogiques sont les suivants:
* Appréhender le concept de sites dynamiques nécessitant l'assemblage de multiples ressources
* Appréhender le concept de résolveur DNS
* Appréhender le concept ludique de complétion du puzzle

## Concepts abordés
Les concepts abordés durant cette phase sont les suivants :
* Dépendances des sites web à des ressources externes
* Système de nommage DNS

Les mots clefs suivants permettront au formateur d'approfondir le sujet par lui-même sur Internet:
DNS, résolveur, ressources externes, adresse IP, nom de domaine, FQDN, blacklist

Les définitions suivantes peuvent être utiles
* DNS: Domain Name System, Système de nommage des domaines. Permettant d'associer le nom d'un serveur (ex: www.facebook.com) à  une adresse IP (ex: 251.26.54.5)
* Résolveur: serveur effectuant l'association entre nom de domaine et adresse IP
* Adresse IP : identifiant d'un ordinateur sur le réseau Internet (IP signifie Internet Protocol), comme un numéro de téléphone
* FQDN: Fully Qualified Domain Name. Designation d'un hôte (ou machine) sur un domaine. Le schéma est alors hote.domaine.tld
* Domaine : ensemble d'ordinateurs liés 

## Contexte extérieur
Cet atelier permet de montrer le concept de récursivité du DNS et d'expliciter la résolution d'un FQDN par un résolveur.
Cet atelier permet de soulever les problématiques liés à l'hétérogénéité des ressources requises pour l'assemblage d'un site web complet. Ces ressources peuvent être essentielles au bon fonctionnement du site (comme des vidéos intégrés) ou inutiles pour l'internaute et intrusives (comme les traqueurs de publicité).

## Déroulé
Les enfants sont disposés en 4 groupes. 
* Le groupe 1 représente le domaine de premier niveau (ex: .lu, .com, .net, .fr...)
* Le groupe 2 représente le domaine de second niveau (ex: savety.lu, aware.lu, wort.lu, wikipedia.org, etc...)
* Le groupe 3 représente les serveurs du domaine de troisième niveau (ex: security.savety.lu, www.wort.lu, fr.wikipedia.org, etc.)
* Le groupe 4 représente les clients

Les groupes 1 à 3 sont disposés en U comme sur le schéma de disposition général de la salle.

L'animateur dispose face à chaque enfant un écriteau avec un nombre (ex: 3).
L'animateur répartit dans le groupe 3 un ensemble d'enveloppe (numérotées) en ayant le même numéro de l'enfant que le numéro de l'enveloppe.
L'animateur répartit dans le groupe 2 un ensemble de fiches (numérotées) en ayant le même numéro de l'enfant que le numéro des fiches.
L'animateur répartit dans le groupe 1 un ensemble de fiches (numérotées) en ayant le même numéro de l'enfant que le numéro des fiches.
L'animateur projette ensuite une diapositive montrant les correspondances entre les enfants du Groupe 1 et les domaines de premier niveau. Cette diapositive représente la racine.

Le but des enfants du Groupe 4 est alors de constituer un puzzle à partir des pièces contenues dans les enveloppes du Groupe 3. La liste des pièces à obtenir est fixée et représente l'ensemble des ressources d'un site (ex: www.wort.lu) dont la dépendance a été mise en avant par l'utilisation de Lightbeam. Cette liste est projetée sur la diapositive à coté de la liste "racine".

La liste se présente de la manière suivante:
- www.wort.lu/home.html
- cdn.wort.lu/image.png
- analytics.google.com/cookie.js
- ads.google.lu/pub.php


Afin d'obtenir ces pièces, les enfants du Groupe 4 doivent alors décomposer le chemin d'obtention des pièces. Par exemple, pour avoir la pièce "www.wort.lu/home.html", l'enfant du Groupe 4 devra:
- Identifier sur la diapositive projetée le numéro de l'enfant du Groupe 1 représentant le domaine .lu
- Aller voir l'enfant du Groupe 1 représentant .lu et lui demander le numéro de l'enfant représentant .wort.lu
- Aller voir l'enfant du Groupe 2 représentant .wort.lu et lui demander le numéro de l'enfant représentant www.wort.lu
- Aller voir l'enfant du Groupe 3 représentant www.wort.lu et lui demander la pièce home.html dans l'enveloppe "www.wort.lu"

Lorsque le canevas est complété, l'animateur présente alors la seconde phase.


## Liens utiles
* [Il etait une fois Internet: le DNS](http://www.iletaitunefoisinternet.fr/dns-bortzmeyer/index.html)
