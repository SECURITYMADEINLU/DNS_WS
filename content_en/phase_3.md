# Phase 3

## Preparation
* Number of participants *: 16 children (max), divided into 3 groups and 1 animator (without prejudice to local laws and regulations)
*Equipment*:
* 3 canvas to complete
* 3 sets of cards (6 cards per set) representing each of the resources to be assembled
* 3 card sets (6 cards per set) representing corrupted resources
* 1 video projector

## Detailed Objectives
The educational objectives are as follows:
* Understand the concept of informed choice of its DNS resolver
* Understand the concept of DNS resolver liar
* Understand the concept of disseminating malicious content by corrupt / lying DNS response


## Concepts covered
The concepts addressed during this phase are as follows:
* DNS Liar
* Choice of DNS resolver


The following keywords will allow the trainer to deepen the subject by himself on the Internet:
DNS, resolver, external resources, IP address, domain name, FQDN, blacklist

The following definitions may be useful
* DNS: Domain Name System, Domain Naming System. Allows to associate the name of a server (ex: www.facebook.com) with an IP address (ex: 251.26.54.5)
* Resolver: server performing the association between domain name and IP address
* IP address: identifier of a computer-based Internet Protocol), such as a telephone number
* FQDN: Fully Qualified Domain Name. Designation of a host (or machine) on r on the Internet network (IP means a domain.) The schema is then hote.domaine.tld
* Domain: set of computers linked

## Outside Context
This workshop is an opportunity to introduce the problem of choosing its DNS resolver. Where many users do not care about this technical element, and make the choice of resolver whose policy is questionable (Google DNS, OpenDNS, etc.), it is essential to balance the reliability and efficiency.
This workshop is also an opportunity to introduce the problems of spreading malicious content, such as viral loads by corrupting legitimate sites.


## Processing
The children have a canvas to complete by group, and the model they have chosen in phase 2 projected by video projector. The groups of children are divided between two Blue-Team and one Red-Team. The objective, known publicly, of each group of the Blue-Team is to constitute as quickly as possible his puzzle. The goal, hidden from the public and known only to the Red-Team, of the Red-Team is to distort the realization of blue-team puzzles by giving corrupted pieces.

Each group has a sign in front of it indicating whether it wants to be served by the old or new DNS resolver.
The host represents the old DNS resolver. He can issue 1 coin each turn as requested by the group of players.
The Red-Team represents the new DNS resolver. He can issue 2 coins as requested by the group of players.
These characteristics are communicated publicly before the start of the phase.

So a group choosing to use only the new resolver will complete its puzzle 2 times faster than a group that has chosen to use only the old DNS resolver. The goal of each group is to build up its puzzle as quickly as possible, it will likely make the choice of a new DNS resolver.

When a group finishes their puzzle, they write the number of the turn they finished their puzzle. It's his (temporary) score, the lower it is, the more the group will have finished its puzzle and will be close to the first place.
When all the groups have completed their puzzle, the facilitator reveals that the pieces given by the Red-Team have been corrupted and that hidden motives have to be revealed. These hidden patterns can be revealed using a color filter. Each piece of puzzle has a number of half-patterns that assembled with attachments can make a pattern complete.
Each group then counts the number of complete patterns. The facilitator then indicates that this is the number of infections. This number is a handicap and will be subtracted from the temporary score. Thus: (temporary score) - (number of complete patterns) = (final score)
The group with the lowest final score wins.

The facilitator can then remind you of the importance of choosing your DNS resolver correctly, or at least not follow the many tutorials on the Internet that can sometimes promise greater speed at the expense of security.



## Useful links
* [Change DNS resolver, Stephane Bortzmeyer] (http://www.bortzmeyer.org/changer-dns.html)