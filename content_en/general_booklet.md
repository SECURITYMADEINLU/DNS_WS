# Workshop DNS Filtering

## Objectives
The objectives of this workshop are to:
* To make children understand the concept of interdependence of resources in the rendering of a website
* Make children understand the basics of the naming system
* Make children understand the concept of filtering, notably by blacklist
* Raise children's awareness of censorship issues
* Educate children about the technical choices of DNS resolvers

## Process
This workshop takes place in 4 phases of game. Each phase of the game aims at a pedagogical objective:
* The first phase aims to present the concept of game via the puzzle and to make apprehend the concept of resolution DNS via a collaborative game
* The second phase aims to introduce the concept of filtering and creation of multi-dependency sites via a collaborative game
* The third phase aims to introduce the concept of misappropriation of the naming system for malicious purposes via a competitive game
* The fourth phase aims at introducing the concept of denial of service attack using the naming system

The children are arranged in the following way:


<Img src = "Disposition.png">
Image source: m.farcot - securitymadein.lu


### First phase
In the first phase, children aim to assemble a defined puzzle, the whole of which represents a web site (eg wort.lu) and each of the pieces represents a third-party resource (eg Facebook, Twitter, Trackers analytics or advertising). An illustration with the Lightbeam plugin is possible.
A group of children has a canevas representing the parts to assemble to get a complete website. Three other groups of children represent the technical intermediaries needed to obtain these pieces. This is for two groups to be the authoritative servers and for the last group to be the servers serving the HTTP requests requested by the group finalizing the puzzle.

### Second Phase
Children are led to design their own website, assembling bricks of third-party services available. Each group pitches its idea to the others. The pitch with the most votes is selected. However, facilitators may moderate and decide to prohibit certain services for arbitrary reasons. For example, children may initially have bricks related to the sale of sweets but see these bricks prohibited by the animators. This phase illustrates filtering by a third-party authority.

### Third phase
The children are divided into a blue team, whose goal is to assemble the puzzle corresponding to the site they designed during stage 2. And a red team whose goal is to corrupt the realization of this puzzle. The goal of each group (within the blue team) is to get a score as low as possible, corresponding to a quick resolution of the puzzle. To this end, the red team will play the role of a new DNS resolver that will give corrupt answers. In order to be attractive, the red team has an advantage over the historical DNS resolver. This advantage is realized by a higher resolution (ie: at each turn, the red team resolver will answer twice as many responses as the historical resolver).
The animator makes a turn of the children and each group can then request n pieces (according to the capacity of the resolver). Each turn a counter is incremented. When a group completes his puzzle, he receives as a temporary score the number of the turn he ends his puzzle.
At the end of this phase, the children are led to reveal, using a colored filter, the patterns appearing on the pieces corrupted by the red team. Each complete pattern revealed proves to be a penalty. The penalty amount is then added to the temporary score. The animator then reveals the existence of the red team and the functioning of the penalties. He then proposes to remake a session, it is the fourth phase.

### Fourth Phase
The children, always separated in red teams and blue team are brought to reproduce the third phase. It is expected that players will choose to use the historical DNS resolver rather than the red-team resolver. The players of the red team can then, for each sequence, make a number of queries to the historical DNS server equivalent to the number of penalties of the player making his request. This number p of requests will lead the facilitator to pass the turn of the children following the child who made his request. This allows to illustrate a congestion of the DNS server allowing to introduce the concept of denial of service by infection of a botnet, and the penalization of the community.

## Material
Children are separated into 3 groups. Each group has:
* 1 physical canvas (in the form of a terminal like a smartphone), for example made of wood and equipped with Scratch-type grip

The set has 3 * s pieces representing the services (where 3 * s represents the number of rooms available for each of the services available: eg, if there are 5 types of services, 3 * 5 = 15 pieces)
* These parts can be printed in plastified paper (models can be found on the repo git)
* The back of each piece has a Scracth-type attachment system for attachment to the canvas

The whole set has 3 * s pieces representing services having the same characteristics as before but having reasons to reveal.
Patterns can be printed using colored glyphs and revealed by a monochrome filter. They can also be affixed to UV ink and revealed under black light.

The animator has a technical booklet with technical references.

** version 0.5 **
** contact: loic.peden@savety.lu**
