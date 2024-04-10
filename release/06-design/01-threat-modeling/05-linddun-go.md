---

title: LINDDUN GO
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 6150
permalink: /release/design/threat_modeling/linddun-go/

---

{% include breadcrumb.html %}

### 4.1.5 LINDDUN GO

LINNDUN GO is a card game used to help derive privacy requirements during the software development life cycle.
The LINNDUN GO card set can be [downloaded][linddun-go-cards] as a PDF and then printed out.

#### What is LINDDUN GO?

[LINDDUN GO][linddun-go] helps identify potential privacy threats based on the key LINDDUN threats to privacy:

* Linking
* Identifying
* Non-repudiation
* Detecting
* Data Disclosure
* Unawareness
* Non-compliance

LINNDUN GO is similar to OWASP [Cornucopia][cornucopia] in that it takes the form of a set of cards that
can be used to gamify the process of identifying application privacy / security requirements.
The deck of 33 cards are arranged in suits that match each category of threats to privacy,
and there is a [set of rules][linddun-go-rules] to structure the game sessions.
Each LINDDUN GO card illustrates a single common privacy threat and suggested remediations.

#### Why use it?

[LINDDUN][linddun] is an approach to threat modeling from a privacy perspective.
It is a methodology that is useful to structure and guide the identification of threats to privacy,
and also helps with suggestions for the mitigation of any threats.

[LINDDUN GO][linddun-go] gamifies this approach to privacy with a set of cards and rules
to guide the identification process for threats to the privacy provided by the application.
This is a change to other established processes and provides a different and useful perspective to the system.

#### How to use LINDDUN GO

The idea for a LINDDUN GO is that it is played in person by a diverse team with as varied a set of viewpoints as possible.
The advice from the LINDDUN GO 'getting started' instructions is that this team contains some or all of:

* domain experts
* system architects
* developers
* the Data Protection Officer (DPO)
* legal experts
* the Chief Information Security Officer (CISO)
* privacy champions

The application should have already been described by an architecture diagram or data flow diagram
so that the players have something to refer to during the game.
[Download][linddun-go-cards] and printout the deck of cards.

Follow the [set of rules][linddun-go-rules] to structure the game session, record the outcome and act on it.
The outcome of the game is to identify possible privacy threats and propose remediations;
as well as having a good time of course.

----

[cornucopia]: https://owasp.org/www-project-cornucopia/
[linddun]: https://linddun.org/
[linddun-go]: https://linddun.org/go/
[linddun-go-cards]: https://downloads.linddun.org/linddun-go/default/latest/go.pdf
[linddun-go-rules]: https://linddun.org/go-getting-started/
