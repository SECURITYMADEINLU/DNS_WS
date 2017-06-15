Durée totale du jeu: 30 minutes

Nombre d'enfant total: 12 

Objectifs du jeu:

1. Appréhender le concept de sites dynamiques nécessitant l'assemblage de multiples ressources hébergées sur d'autre serveurs

2. Appréhender le concept de résolveur DNS

3. Expliciter les aspects positifs d'un système de filtrage DNS (blocage de malware) et les aspects plus controversés (censure de sites spécifiques)

Matériel: 

- panneaux avec rôles des enfants
- enveloppes
- tampons pour confirmer que les différentes étapes ont bien été respectées
- chronomètre 

Règles du jeu:

Chaque enfant joue un rôle prédéfini en respectant un déroulement précis qui permet dans un premier temps de comprendre la façon dont fonctionne un site web et le filtrage DNS dans un second temps.

Agencement salle:

La salle est divisée en 3 zones principales: 1 zone DNS (zone B), 1 zone serveurs (zone C), 1 zone navigateur (zone A) (voir schéma).

Le jeu est divisée en 3 étapes: 

- Etape 1: explications générales du jeu
- Etape 2: chargement dynamique
- Etape 3: résolveur DNS: censure

Les joueurs:

-	L’enfant numéro 1 joue le rôle du navigateur (ZONE A)
-	L’enfant numéro 2 joue le rôle du résolveur DNS (ZONE B)
-	L’enfant numéro 3 joue le rôle du root (ZONE B)
-	L’enfant numéro 4 représente « .lu » et « .fr »  (ZONE B)
-	L’enfant numéro 5 représente « .com » (ZONE B)
-	L’enfant numéro 6 représente « smile.lu » et « google.com » (ZONE B)
-	L’enfant numéro 7 représente « facebook.fr » et « youtube.com » (ZONE B)
-	Les enfants numéro 8 / 9 / 10 / 11 / 12 jouent le rôle des ressources (ZONE C)

PHASE 1 & 2

Le jeu se déroule de cette façon: une page d'un site Internet est projetée sur un écran. Les enfants ont pour objectif de recréer cette page grâce à une sorte de jeu de rôle.

1/ L'enfant numéro 1 (navigateur) souhaite charger la page www.smile.lu/.

2/ L'enfant numéro 1 (navigateur) demande à l'enfant numéro 2 (résolveur DNS) "où sont les ressources" pour "www.smile.lu/index.html".

3/ L'enfant numéro 2 (résolveur DNS) demande à l'enfant numéro 3 (root) qui détient ".lu". Ce dernier indique que c'est l'enfant numéro 4 qui détient la réponse. 

4/ L'enfant numéro 2 (résolveur DNS) demande à l'enfant numéro 4 qui est "smile.lu". L'enfant numéro 4 indique que c'est l'enfant numéro 6 qui détient la réponse. 

5/ L'enfant numéro 2 (résolveur DNS) demande à l'enfant numéro 6 qui a "www.smile.lu".  L'enfant numéro 6 indique un numéro d'"enfant ressource", exemple l'enfant numéro 8 (à ce niveau là, on parle en adresses IP, exemple: 192.162.2.3: cela permet de montrer que l'on peut également arriver sur une page web en tapant cet enchaînement de chiffres dans un navigateur).

6/ L'enfant numéro 2 (résolveur DNS) dit à l'enfant numéro 1 (navigateur) "renseigne-toi auprès de l'enfant numéro 8". 

7/ L'enfant numéro 1 (le navigateur) demande à un l'enfant ressource numéro 8 "/index.html".

8/ L'enfant ressource numéro 8 donne à l'enfant numéro 1 (le navigateur) le fichier "index.html"

9/ Le fichier "index.html" contient des ressources hébergées sur d'autres serveurs (exemple: images, vidéos...)

Et ainsi de suite, le tour reprend pour la consistution d'autres sites Internet.

PHASE 3: le résolveur menteur

Dans cette deuxième phase, les enfants se familiarisent avec les aspects controversés d'un système de filtrage (la censure) et les aspects positifs qui permettent de bloauer des malware.

Cette phase introduit la notion de filtrage DNS. Lorsqu'un des enfants demande une ressource, celle-ci est indiquée comme "fichier interdit" ou "ressource non autorisée" afin de l'aider à comprendre la censure. Cette étape amène les enfants à réfléchir sur la notion de liberté d'expression.  

Cependant, cette étape démontre qu'il est également nécessaire d'effectuer les mises à jour sur un navigateur pour qu'il ne soit pas vulnérable face aux malware. Afin de démontrer cette problématique, un enfant joue le rôle du navigateur mis à jour tandis qu'un autre enfant joue le rôle du navigateur non mis à jour: les enfants comprennent très vite l'importance des mises à jour.

Enfin, pour introduire les malware, il sera demandé à l'enfant numéro 5 de distribuer des malware en donnant des réponses erronnées.

















