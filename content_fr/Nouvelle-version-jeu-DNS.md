Durée totale du jeu: 30 minutes

Nombre d'enfant total: 12 

Objectifs du jeu:

1. Appréhender le concept de sites dynamiques nécessitant l'assemblage de multiples ressources hébergées sur d'autre serveurs

2. Appréhender le concept de résolveur DNS

3. Expliciter les aspects positifs d'un système de filtrage DNS (blocage de malware) et les aspects plus controversés (blocage de sites spécifiques)

Matériel: 

- panneaux avec rôles des enfants
- enveloppes

Règles du jeu:

Chaque enfant joue reçoit un numéro et joue un rôle prédéfini respectant un déroulement précis qui permet de comprendre la façon dont fonctionne un site web.

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

Le jeu se déroule de cette façon: une page d'un site Internet est projetée et les enfants vont réussir à comprendre comment est constituée cette page grâce à une sorte de jeu de rôle.

1/ L'enfant numéro 1 (navigateur) souhaite charger la page www.smile.lu/.

2/ L'enfant numéro 1 (navigateur) demande à l'enfant numéro 2 (résolveur DNS) "où sont les ressources" pour "www.smile.lu/index.html".

3/ L'enfant numéro 2 (résolveur DNS) demande à l'enfant numéro 3 (root) qui détient ".lu". Ce dernier indique que c'est l'enfant numéro 4 qui détient la réponse. 

4/ L'enfant numéro 2 (résolveur DNS) demande à l'enfant numéro 4 "smile.lu" qui est "smile.lu". L'enfant numéro 4 indique que c'est l'enfant numéro 6 qui détient la réponse. 

5/ L'enfant numéro 2 (résolveur DNS) demande à l'enfant numéro 6 qui a "www.smile.lu".  L'enfant numéro 6 indique un numéro d'"enfant ressource", exemple l'enfant numéro 8 (à ce niveau là, on parle en adresses IP, exemple: 192.162.2.3)

6/ L'enfant numéro 2 (résolveur DNS) dit à l'enfant numéro 1 (navigateur) "renseigne-toi auprès de l'enfant numéro 8". 

7/ L'enfant numéro 1 (le navigateur) demande à un l'enfant ressource numéro 8 "/index.html".

8/ L'enfant ressource numéro 8 donne à l'enfant numéro 1 (le navigateur) le fichier "index.html"

9/ Le fichier "index.html" contient des ressources hébergées sur d'autres serveurs (exemple: images, vidéos...)


PHASE 3

Le résolveur menteur.

C'est le résolveur qui bloque et décide q'une ressource est interdite. C'est là où on introduit la notion de filtrage.
Dans cette deuxième phase, les enfants se familiarisent avec le côté positif d'un filtrage DNS et son aspect négatif.















