---

title: Amass
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 8220
permalink: /release/verification/tools/amass/

---

{% include breadcrumb.html %}

### 6.2.2 Amass

The OWASP Amass is a tool that provides  attack surface management for an organization's web sites and applications.
It used during penetration testing for network mapping of attack surfaces
and external asset discovery by integrating various existing security tools.

The Amass [breaker/tool project][amass] is an OWASP Flagship Project and installers can be
downloaded from the project's github repository [release area][amass-download].

#### What is Amass?

Amass is a command line tool that provides information on an organization's web sites,
using various open source information gathering tools and active reconnaissance techniques.

It is run from the command line and has three [subcommands][amass-docs] :

1. 'amass intel' collects intelligence on the target organization
2. 'amass enum' performs DNS enumeration and network mapping to populate the results database
3. 'amass db'

Each command comes with a wide set of options that controls the tools used and the format of the findings.

#### Why use it?

Amass is an important tool for security test teams. Amass is included in the [Kali Linux][kali] distribution,
which is widely used by penetration testing teams, with Amass providing a straightforward way
of running a wide set of reconnaissance and enumeration tools.

In addition , Amass is an easily used tool that is available to both legitimate test teams and malicious actors.
It is very likely that any given organization has been scanned and enumerated by Amass at some point,
either maliciously or legitimately, so at the very least it is useful to run the tool and inspect the findings.

#### How to use it

If [Kali Linux][kali] is being used then Amass comes ready installed,
otherwise a wide set of [installers][amass-install] is provided for other platforms.

The extensive [Amass tutorial][amass-tutorial] provides the best way of learning about using Amass and its features.

----

[amass]: https://owasp.org/www-project-amass/
[amass-docs]: https://github.com/owasp-amass/amass/blob/master/doc/user_guide.md
[amass-download]: https://github.com/owasp-amass/amass/releases
[amass-install]: https://github.com/owasp-amass/amass/blob/master/doc/install.md
[amass-tutorial]: https://github.com/owasp-amass/amass/blob/master/doc/tutorial.md
[kali]: https://www.kali.org/
