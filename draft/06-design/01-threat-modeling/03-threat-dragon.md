---

title: Threat Modeling with Threat Dragon
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 613
permalink: /draft/design/threat-modeling/threat-dragon/

---

{% include breadcrumb.html %}

### 4.1.3 Threat Dragon

The OWASP [Threat Dragon][tdtm] project provides a diagrammatic tool for threat modeling
applications, APIs and software systems.
It is an OWASP Lab Project with [several releases][tddownload] and is in active development.

#### What is Threat Dragon?

Threat Dragon is a tool that can help development teams with their threat modeling process.
It provides for creating and modifying data flow diagrams which provide the
context and direction for the threat modeling activities.
It also stores the details of threats identified during the threat modeling sessions,
and these are stored alongside the threat model diagram in a text-based file.
Threat Dragon can also output the threat model diagram and the associated threats as a PDF report.

#### Why use it?

Threat Dragon is a useful tool for small teams to create threat models quickly and easily.
Threat Dragon aims for:

* Simplicity - you can install and start using Threat Dragon very quickly
* Flexibility - the diagramming and threat generation allows all types of threat to be described
* Accessibility - different types of teams can benefit from Threat Dragon’s simplicity and flexibility

It supports various methodologies and threat categorizations used during the threat modeling activities:

* STRIDE
* LINDDUN
* CIA
* DIE

and it can be used by a wide range of developers and teams:

* Simplicity - installation is easy and teams can start using Threat Dragon quickly
* Flexibility - the diagramming and threat generation allows all types of threat to be described
* Accessibility - various different types of teams can all benefit from Threat Dragon ease of use

#### How to use it

Threat Dragon is distributed as a cross platform desktop application as well a web application.
It is straightforward to start using Threat Dragon; the latest version is [available to use online][tddemo]:

1. select Login to Local Session
2. select Explore a Sample Threat Model
3. select Version 2 Demo Model
4. you are presented with the threat model meta-data which can be edited
5. click on the diagram Main Request Data Flow to display the data flow diagram
6. the diagram components can be inspected, and their associated threats are displayed
7. components can be added and deleted, along with editing their properties

The [desktop application][tddownload] can be downloaded for Windows, Linux and MacOS.
The web application can be run using a [Docker container][tddocker] or from the [source code][tdcode].

An important feature of Threat Dragon is the PDF report output which can be used for documentation
and GRC compliance purposes; from the threat model meta-data window click on the Report button.

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue060103] or [edit on GitHub][edit060103].

[issue060103]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2006-design/01-threat-modeling/03-threat-dragon
[edit060103]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/06-design/01-threat-modeling/03-threat-dragon.md
[tddemo]: https://www.threatdragon.com/#/
[tdcode]: https://github.com/OWASP/threat-dragon
[tddocker]: https://hub.docker.com/r/owasp/threat-dragon/tags
[tddownload]: https://github.com/OWASP/threat-dragon/releases
[tdtm]: https://owasp.org/www-project-threat-dragon/

\newpage
