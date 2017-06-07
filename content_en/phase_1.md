# Phase 1

## Preparation
* Number of participants *: 16 children, divided into 4 groups and 1 animator (without prejudice to local laws and regulations)

*Equipment*:
* 1 known canvas of a site determined in advance (ex: www.wort.lu)
* 12 numbered envelopes (3 bearing the number 1, 3 the number 2, 3 the 3, 3 the 4) and each carrying the FQDN of a server to be interrogated
* 12 signs (easel papers) bearing numbers 1 to 12 (one number per easel)
* 8 correspondence lists between number of children and second level domains
* 8 correspondence lists between number of children and third level domains
The lists and the contents of the envelopes are detailed in the attached form.

## Detailed Objectives
The educational objectives are as follows:
* Understand the concept of dynamic sites requiring the assembly of multiple resources
* Understand the concept of DNS resolver
* Understand the playful concept of puzzle completion

## Concepts covered
The concepts addressed during this phase are as follows:
* Dependencies from websites to external resources
* DNS naming system

The following keywords will allow the trainer to deepen the subject by himself on the Internet:
DNS, resolver, external resources, IP address, domain name, FQDN, blacklist

The following definitions may be useful
* DNS: Domain Name System, Domain Naming System. Allows to associate the name of a server (ex: www.facebook.com) with an IP address (ex: 251.26.54.5)
* Resolver: server performing the association between domain name and IP address
* IP address: The identifier of a computer on the Internet (IP stands for Internet Protocol), such as a telephone number
* FQDN: Fully Qualified Domain Name. Designation of a host (or machine) on a domain. The schema is then hote.domaine.tld
* Domain: set of computers linked

## Outside Context
This workshop allows to show the concept of recursion of the DNS and to explain the resolution of a FQDN by a resolver.
This workshop raises the issues related to the heterogeneity of the resources required for assembling a complete website. These resources can be essential to the smooth running of the site (such as integrated video) or unnecessary for the Internet user and intrusive (such as advertising trackers).

## Processing
The children are arranged in 4 groups.
* Group 1 represents the top level domain (ex: .lu, .com, .net, .fr ...)
* Group 2 represents the second level domain (eg savety.lu, aware.lu, wort.lu, wikipedia.org, etc.)
* Group 3 represents the servers of the third level domain (eg security.savety.lu, www.wort.lu, fr.wikipedia.org, etc.)
* Group 4 represents customers

Groups 1 to 3 are arranged in a U-shape as in the general arrangement layout of the room.

The facilitator has to face each child a sign with a number (ex: 3).
The facilitator distributes in group 3 a set of envelopes (numbered) with the same number of the child as the number of the envelope.
The facilitator divides into group 2 a set of (numbered) cards with the same number of the child as the number of the cards.
The facilitator divides into group 1 a set of (numbered) cards with the same number of the child as the number of the cards.
The facilitator then projects a slide showing the correspondences between the children of Group 1 and the top-level domains. This slide represents the root.

The aim of the children of Group 4 is to form a puzzle from the pieces contained in the envelopes of Group 3. The list of the pieces to be obtained is fixed and represents all the resources of a site (eg www.wort .lu) whose dependence has been promoted by the use of Lightbeam. This list is projected on the slide next to the "root" list.

The list is as follows:
- www.wort.lu/home.html
- cdn.wort.lu/image.png
- analytics.google.com/cookie.js
- ads.google.lu/pub.php


In order to obtain these pieces, the children of Group 4 must then decompose the path of obtaining the pieces. For example, to have the piece "www.wort.lu/home.html", the child of Group 4 must:
- Identify the number of the Group 1 child representing the .lu domain on the projected slide
- Go see the child of Group 1 representative .lu and ask him the number of the child .wort.lu representative
- Go see the child of Group 2 representative .wort.lu and ask him the number of the child representing www.wort.lu
- Go to the child of Group 3 representing www.wort.lu and ask for the room home.html in the envelope "www.wort.lu"

When the canvas is completed, the facilitator then presents the second phase.


## Useful links
* [Il était une fois Internet: le DNS - French] (http://www.iletaitunefoisinternet.fr/dns-bortzmeyer/index.html)