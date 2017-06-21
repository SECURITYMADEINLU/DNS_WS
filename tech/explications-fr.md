# DNS ça sert à quoi ?
Sur Internet, les ressources (sites web, répertoires FTP, etc.) sont localisés sur des serveurs (de gros ordinateurs, qui servent les données demandées comme un serveur de restaurant des plats commandés). Ces serveurs sont identifiés et joignables par une adresse IP (pour Internet Protocol). Il s'agit d'un identifiant unique permettant de localiser et de joindre un serveur dans un réseau. Par analogie, on peut dire qu'il s'agit du numéro de téléphone d'un abonné. 

Sur Internet cependant, le nombre de serveurs est extrèmement important et il est impossible pour un esprit humain de retenir les coordonnées de chaque serveur que l'on veut interroger. C'est pour cela qu'il existe un protocole permettant de lier un nom (par exemple www.smile.lu) à une adresse IP (par exemple: 80.92.65.144). Chaque partie de droite du nom d'un serveur (ici "facebook" et "com") est appelée domaine. Le nom du protocole et du système qui le supporte est ainsi logiquement Système de Noms de Domaines. Ou Domain Name System (DNS) en anglais. Ce système joue le rôle d'annuaire.

Utiliser le nom d'un serveur plutôt que son adresse IP n'est pas utile qu'aux utilisateurs humains. En effet, cela permet de ne pas avoir à changer tout le web quand un serveur change d'adresse IP. Il suffit juste de mettre à jour les serveurs DNS.

# Problématiques de DNS
## Censure
Lorsqu'une entité (un gouvernement ou une entreprise) souhaite censurer un site web, la solution la plus simple consiste à manipuler le système DNS pour qu'il réponde de manière erronée et ne renvoie pas la bonne association [Nom d'un serveur]=[Adresse IP] mais renvoie l'adresse IP d'un autre serveur. Cette manipulation est effectuée par le résolveur DNS, puisque les serveurs faisant autorité sont controlés par les propriétaires du serveur censuré.
## Disponibilité
DNS est un système critique permettant de joindre les serveurs sur Internet à partir de leurs noms. Il arrive parfois, suite à des attaques informatiques ou des pannes, que des bouts du système DNS soient inopérants. On constate alors une "panne" d'une partie d'Internet (par exemple Twitter et Facebook seront injoignables).

# Terminologie du système DNS
Le système DNS se comporte en plusieurs partie: 
- Un client (l'ordinateur de l'utilisateur), qui interroge son serveur résolveur DNS
- Le serveur résolveur DNS va tenter de résoudre l'enigme de la question posée ("Quelle est l'adresse IP de www.smile.lu ?") en interrogeant des serveurs faisant autorité sur les domaines
- Les serveurs faisant autorité sur les domaines. Ils indiquent soit :
-- la réponse finale voulue
-- l'identifiant du serveur faisant autorité du niveau suivant (ex: le serveur faisant autorité sur .com. pourra indiquer quel serveur fait autorité sur .facebook.com.)
- Le serveur faisant autorité sur les domaines de premier niveau (comme .com.) est appelé Racine. 

# Analogie de fonctionnement
On peut prendre comme analogie de fonctionnement pour la quête de résolution le chemin que suit une lettre. Si l'on prend l'adresse suivante:
M. Martin
3 rue de la Gare
L-2140 Luxembourg
Luxembourg

Cette lettre postée en France sera d'abord expédiée vers la poste centrale du Grand-Duché de Luxembourg. Cette poste centrale joue le rôle de serveur racine. Elle connait les identifiants de toutes les postes de Luxembourg. Cette poste va alors diriger la lettre vers la poste de la ville de Luxembourg. Cette poste de la ville de Luxembourg connaît toutes les rues de Luxembourg. Elle va alors renvoyer cette lettre vers la poste de la rue de la Gare. La poste de la rue de la gare connaît tous les batiments de la rue. Elle va donner la lettre à un facteur qui ira déposer la lettre au 3 rue de la Gare dans la boîte aux lettres de M. Martin.

Il s'agit d'une résolution récursive d'une adresse postale. Pour DNS, le fonctionnement est équivalent. Il existe des serveurs faisant autorité sur des domaines entiers (comme la poste centrale du Grand Duché qui sait où sont les villes dans le pays), mais qui ne connaissent pas les plus bas niveaux (cette poste centrale de ne connaitra pas la localisation de la boite aux lettres de M. Martin). Ces serveurs faisant autorité renvoie alors le serveur résolveur vers le serveur faisant autorité sur le domaine suivant (ex: le serveur faisant autorité sur .com. va renvoyer sur le serveur faisant autorité sur facebook.com). Au final, seul le dernier serveur faisant autorité sur la dernière zone pourra donner la correspondance souhaitée entre le serveur www de la zone .facebook.com. et son adresse IP.

## Phase du jeu de résolution DNS
Dans le jeu, lorsque l'enfant qui joue le résolveur essaie de joindre www.smile.lu, il va d'abord interroger le serveur racine qui lui indiquera quel est l'identifiant du serveur faisant autorité sur le domaine .lu. Puis l'enfant ira interroger ce serveur faisant autorité sur le domaine .lu. pour tenter d'obtenir l'identité du serveur faisant autorité sur le domaine .smile.lu. Une fois connue l'identité de ce serveur, l'enfant va pouvoir interroger ce serveur faisant autorité sur le domaine .smile.lu. pour obtenir l'identifiant du serveur www.smile.lu. Le serveur faisant autorité sur .smile.lu va alors donner l'adresse IP de ce serveur www.smile.lu à l'enfant jouant le résolveur qui pourra donner cette information à l'enfant jouant le navigateur.

## Phase du jeu d'interrogation HTTP
Une fois connue la correspondance Nom du serveur <=> Adresse IP, l'enfant jouant le navigateur va pouvoir aller interroger l'enfant jouant le serveur www.smile.lu pour lui demander de lui donner la ressource index.html. Cette ressource est un canevas contenant les adresses de plusieurs ressources. Ces adresses se constituent de la manière suivante:
[nom du serveur hebergeant la ressource]/[nom de la ressource]
Pour obtenir toutes les pièces du canevas, l'enfant jouant le navigateur va devoir obtenir les identifiants correspondant aux noms de serveurs dont il dispose. Pour cela, il va interroger l'enfant jouant le résolveur qui devra refaire toute la phase de résolution DNS pour chacun des serveurs.
