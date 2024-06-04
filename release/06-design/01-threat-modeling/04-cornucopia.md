---

title: Cornucopia
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 6140
permalink: /release/design/threat_modeling/cornucopia/

---

{% include breadcrumb.html %}

### 4.1.4 Cornucopia

OWASP Cornucopia is a card game used to help derive application security requirements
during the software development life cycle.
[Cornucopia][cornucopia] is an OWASP Lab project, and can be [downloaded][cornucopia-cards] from its project page.

#### What is Cornucopia?

Cornucopia provides a [set of cards][cornucopia-cards] designed to gamify threat modeling activities.
This is designed so that agile development teams can identify weaknesses in web applications
and then record remediations or requirements.

Cornucopia comes with the cards in various suits that cover the various security domains:

* Data validation and encoding
* Authentication
* Session management
* Authorization
* Cryptography
* Cornucopia

There is no one 'right' way to play Cornucopia but there is a suggested [set of rules][cornucopia-play]
to start the game off.
Cornucopia provides a [score sheet][cornucopia-score] to help keep track of the game session and to record outcomes.

To provide context each card in the Cornucopia deck references other OWASP projects:

* Application Security Verification Standard ([ASVS][asvs])
* Secure Coding Practices ([SCP][scp-v21]]) Quick Reference Guide
* [AppSensor][appsensor]

The SCP reference guide has now been incorporated into part of the [Developer Guide](../02-web-app-checklist/toc.md) itself.

#### Why use it?

Cornucopia is useful for both requirements analysis and threat modeling,
providing gamification of these activities within the development lifecycle.
It is targeted towards agile development teams and provides a different perspective to these tasks.

The outcome of the game is to identify possible threats and propose remediations.

#### How to use Cornucopia

The OWASP Spotlight series provides an excellent overview of Cornucopia and how it can be used for gamification:
'Project 16 - [Cornucopia][spotlight16]'.

Ideally Cornucopia is played in person using physical cards,
with the development team and security architects in the same room.
The application should already have been described by an architecture diagram or data flow diagram
so that the players have something to refer to during the game.

The suggested order of play is:

1. Pre-sort: the deck, some cards may not be relevant for the web application
2. Deal: the cards equally to the players
3. Play: the players take turns to select a card
4. Describe: the player describes the possible attack using the card played
5. Convince: the other players have to be convinced that the attack is valid
6. Score: award points for a successful attack
7. Follow suit: the next player has to select a card from the same suit
8. Winner: the player with the most points
9. Follow up: each valid threat should be recorded and acted upon

Remember that the outcome of the game is to identify possible threats and propose remediations,
as well as having a good time.

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue060104] or [edit on GitHub][edit060104].

[appsensor]: https://owasp.org/www-project-appsensor/
[asvs]: https://owasp.org/www-project-application-security-verification-standard/
[cornucopia]: https://owasp.org/www-project-cornucopia/
[cornucopia-cards]: https://owasp.org/www-project-cornucopia#div-cards
[cornucopia-score]: https://owasp.org/www-project-cornucopia/assets/files/Cornucopia-scoresheet.pdf
[cornucopia-play]: https://owasp.org/www-project-cornucopia#div-play
[edit060104]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/06-design/01-threat-modeling/04-cornucopia.md
[issue060104]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=content&template=request.md&title=Update:%2006-design/01-threat-modeling/04-cornucopia
[scp-v21]: https://owasp.org/www-project-secure-coding-practices-quick-reference-guide/assets/docs/OWASP_SCP_Quick_Reference_Guide_v21.pdf
[spotlight16]: https://youtu.be/NesxjEGX58s
