---

title: Nettacker
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 8240
permalink: /release/verification/tools/nettacker/

---

{% include breadcrumb.html %}

<style type="text/css">
.image-right {
  height: 180px;
  display: block;
  margin-left: auto;
  margin-right: auto;
  float: right;
}
</style>

![Nettacker logo](../../../../assets/images/logos/nettacker.png "OWASP Nettacker"){: .image-right }

### 6.2.4 Nettacker

OWASP Nettacker is a command line utility for automated network and vulnerability scanning.
It can be used during penetration testing for both internal and external security assessments of networks.

The Nettacker [breaker/tool project][nettacker-project] is an OWASP Incubator Project;
the latest version can be downloaded from the project's [github repository][nettacker-install].

#### What is Nettacker?

[Nettacker][nettacker-project] is an automated penetration testing tool.
It is used to scan a network to discover nodes and servers on the network including subdomains.
Nettacker can then identify servers, services and port numbers in use.

Nettacker is a modular python application that that can be extended with other scanning functions.
The many modules available are grouped into domains:

* [Scan][nettacker-scan] modules for reconnaissance
* [Vulnerability][nettacker-vuln] modules that attempt specific exploits
* [Brute force][nettacker-brute] modules

Nettacker runs on Windows, Linux and MacOS.

#### Why use it?

Nettacker is easy to use from the command line, making it easy to use in scripts,
and also comes with a web browser interface for easy navigation of the results.
This makes it a quick and reliable way to gain information from a network.

Nettacker can be used both for auditing purposes and also for penetration testing.

#### How to use it

The OWASP Spotlight series provides an overview of attack surface management using Nettacker:
'Project 11 - [Nettacker][spotlight11]'.

The documentation for Nettacker is provided in the repository wiki pages;
follow [these instructions][nettacker-install] to install it.

Nettacker is a flexible and modular scanning tool that can be used in many ways and with many options.
The best way to start using it is by following the [introduction video][nettacker-intro] and then taking it from there.

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue080204] or [edit on GitHub][edit080204].

[edit080204]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/08-verification/02-tools/04-nettacker.md
[issue080204]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=content&template=request.md&title=Update:%2008-verification/02-tools/04-nettacker
[nettacker-brute]: https://github.com/OWASP/Nettacker/wiki/Modules#brute-modules
[nettacker-install]: https://github.com/OWASP/Nettacker/wiki/Installation
[nettacker-intro]: https://github.com/OWASP/Nettacker/wiki#introduction
[nettacker-project]: https://owasp.org/www-project-nettacker/
[nettacker-scan]: https://github.com/OWASP/Nettacker/wiki/Modules#scan-modules
[nettacker-vuln]: https://github.com/OWASP/Nettacker/wiki/Modules#vuln-modules
[spotlight11]: https://www.youtube.com/watch?v=OGv7OtG127A
