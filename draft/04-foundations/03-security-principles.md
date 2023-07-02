---

title: Principles of Security
layout: col-document
tags: OWASP Developer Guide
document: OWASP Developer Guide
order: 403

---

{% include breadcrumb.html %}

### 4.3 Principles of security

This section is a very brief introduction to some concepts used within the software security domain,
and these may not be familiar to many application developers.
The OWASP [Cheat Sheet Series][cheat] provides more in depth explanations for these security principles,
see the further reading at the end of this section.

#### Overview

There are various concepts and terms used in the security domain that are fundamental
to the understanding and discussion of application security.
Security architects and security engineers will be familiar with these terms and development teams
will also need this understanding to implement secure applications.

#### No security guarantee

One of the most important principles of software security is that **no** application or system is totally
100% guaranteed to be secure from all attacks. This may seem an unusually pessimistic starting point
but it is merely acknowledging the real world; given enough time and enough resources any system can be compromised.
The goal of software security is not '100% secure' but to make it hard enough and the rewards small enough
that malicious actors look elsewhere for systems to exploit.

#### Defense in Depth

Also known as layered defense, [defense in depth][did] is a security principle where defense against attack
is provided by multiple security controls.
The aim is that single points of complete compromise are eliminated or mitigated
by the incorporation of a series or multiple layers of security safeguards and risk-mitigation countermeasures.

If one layer of defense turns out to be inadequate then, if diverse defensive strategies are in place,
another layer of defense may prevent a full breach and if that one is circumvented then
the next layer may block the exploit.

#### Fail Safe

This is a security principle that aims to maintain confidentiality, integrity and availability
when an error condition is detected.
These error conditions may be a result of an attack, or may be due to design or implementation failures,
in any case the system / applications should default to a secure state rather than an unsafe state.

For example unless a subject is given explicit access to an object,
it should be denied access to that object by default.
This is often described as 'Fail Safe Defaults' or 'Secure by Default'.

In the context of software security, fail secure is commonly used interchangeably with fail safe,
which comes from physical security terminology.
Failing safe also helps software resiliency, so that the system / application can rapidly recover
upon design or implementation flaws.

#### Least Privilege

A security principle in which a person or process is given only the minimum level of access rights (privileges)
that is necessary for that person or process to complete an assigned operation.
This right must be given only for a minimum amount of time that is necessary to complete the operation.

This helps to limits the damage when a system is compromised by minimising the ability of an attacker
to escalate privileges both horizontally or vertically.
In order to apply this [principle of least privilege][elp] proper granularity
of privileges and permissions should be established.

#### Separation of Duties

Also known as [separation of privilege][sop], separation of duties is a security principle which requires that
the successful completion of a single task
is dependent upon two or more conditions that are insufficient for completing the task by itself.

There are many applications for this principle,
for example limiting the damage an aggrieved or malicious insider can do, or by limiting privilege escalation.

#### Economy of Mechanism

Also known as 'keep it simple', if there are multiple implementations then the simplest
and most easily understood implementation should be chosen.

The likelihood of vulnerabilities increases with the complexity of the software architectural design and code,
and increases further if it is hard to follow or review the code.
The attack surface of the software is reduced by keeping the software design
and implementation details simple and understandable.

#### Complete Mediation

A security principle that ensures that authority is not circumvented in subsequent requests of an object by a subject,
by checking for authorization (rights and privileges) upon every request for the object.

In other words, the access requests by a subject for an object are completely mediated every time,
so that all accesses to objects must be checked to ensure that they are allowed.

#### Open Design

The open design security principle states that the implementation details of the design
should be independent of the design itself,
allowing the design to remain open while the implementation can be kept secret.
This is in contract to security by obscurity where the security of the software
is dependent upon the obscuring of the design itself.

When software is architected using the open design concept,
the review of the design itself will not result in the compromise of the safeguards in the software.

#### Least Common Mechanism

The security principle of least common mechanisms disallows the sharing of mechanisms that are common
to more than one user or process if the users and processes are at different levels of privilege.

#### Psychological acceptability

A security principle that aims at maximizing the usage and adoption of the security functionality in the software
by ensuring that the security functionality is easy to use and at the same time transparent to the user.
Ease of use and transparency are essential requirements for this security principle to be effective.

Security mechanisms should not make the resource significantly more difficult to access
than if the security mechanism were not present.
If the security mechanism provides too much friction for the users then they may look for ways
to defeat the mechanism and “prop the doors open”.

#### Weakest Link

This security principle states that the resiliency of your software against hacker attempts will depend heavily
on the protection of its weakest components, be it the code, service or an interface.

#### Leveraging Existing Components

This is a security principle that focuses on ensuring that the attack surface is not increased
and no new vulnerabilities are introduced by promoting the reuse of existing
software components, code and functionality.

Existing components are more likely to be tried and tested, and hence more secure,
and also should have security patches available.
In addition open source components have the benefit of 'many eyes' and are likely to be even more secure.

#### Further reading

* OWASP Cheat Sheet series
  * [Authentication Cheat Sheet][ancs]
  * [Authorization_Cheat_Sheet][azcs]
  * [Secure Product Design Cheat Sheet][spdcs]

----

The OWASP Developer Guide is a community effort; if you see something that needs changing
then [submit an issue][issue0403] or a [pull request][pr] .

[ancs]: https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html
[azcs]: https://cheatsheetseries.owasp.org/cheatsheets/Authorization_Cheat_Sheet.html
[cheat]: https://owasp.org/www-project-cheat-sheets/
[did]: https://cheatsheetseries.owasp.org/cheatsheets/Secure_Product_Design_Cheat_Sheet.html#2-the-principle-of-defense-in-depth
[issue0403]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2004-foundations/03-security-principles
[elp]: https://cheatsheetseries.owasp.org/cheatsheets/Authorization_Cheat_Sheet.html#enforce-least-privileges
[pr]: https://github.com/OWASP/www-project-developer-guide/pulls
[sop]: https://cheatsheetseries.owasp.org/cheatsheets/Secure_Product_Design_Cheat_Sheet.html#1-the-principle-of-least-privilege-and-separation-of-duties
[spdcs]: https://cheatsheetseries.owasp.org/cheatsheets/Secure_Product_Design_Cheat_Sheet.html

\newpage
