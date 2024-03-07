---

title: Dependency-Check
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 721
permalink: /draft/implementation/dependencies/dependency_check/

---

{% include breadcrumb.html %}

### 5.2.1 Dependency-Check

OWASP [Dependency-Check][depcheck] is a tool that provides Software Composition Analysis (SCA) from the command line.
It identifies the third party libraries in a web application project
and checks if these libraries are vulnerable using the [NVD database][nist-db].

Dependency-Check is an OWASP Flagship project and can be downloaded from the [github releases][depcheck-download] area.
Dependency-Check was started in September 2012 and since then has been continuously supported with regular releases.

#### What is Dependency-Check?

Dependency-Check is a Software Composition Analysis (SCA) tool that attempts to detect
publicly disclosed vulnerabilities contained within a project’s dependencies.
It does this by determining if there is a [Common Platform Enumeration][cpe] (CPE) identifier for a given dependency.

The core engine contains a series of analyzers that inspect the project dependencies
and identify the CPE for the given dependency.
If a CPE is identified then it is cross referenced to the [NIST CVE database][nist-db]
and any associated [Common Vulnerability and Exposure][cve] (CVE) entries are listed in the report.

Dependency-Check's core analysis engine can be used as:

* an Ant Task
* a Command Line Tool
* Gradle Plugin
* Jenkins Plugin
* Maven Plugin
* SBT Plugin

#### Why use it?

Checking for vulnerable components has been in the OWASP Top Ten '[A06 Vulnerable and Outdated Components][a06]'
and is one of the most straight-forward and effective security activities to implement.
The Dependency-Check tool provides this check for vulnerable components in CI/CD pipelines using the plugins.

In addition this is very useful for development teams;
the ability for vulnerable application components from the command line gives
immediate feedback to the developer without waiting for a pipeline to run.

#### How to use it

The OWASP Spotlight series provides an example of the risks involved in using out of date and vulnerable libraries,
and how to use Dependency-Check: 'Project 2 - [OWASP Dependency Check][spotlight02]'.

Refer to the Dependency-Check [documentation][depcheck-docs] to get started running from the command line.

* ensure Java is installed, for example from [Eclipse Adoptium][adoptium]
* download and unzip the latest Dependency-Check [release][depcheck-download]
* navigate to the Dependency-Check 'bin' directory and run, using threat Dragon as an example:
  `./dependency-check.sh --project "Threat Dragon" --scan ~/github/threat-dragon`
* open the html output file and act on the findings

The command line is useful for development and debugging, and a plugin can hen be installed
for a pipeline to generate the SCA reports depending on what automation environment is in place.

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue070201] or [edit on GitHub][edit070201].

[a06]: https://owasp.org/Top10/A06_2021-Vulnerable_and_Outdated_Components/
[adoptium]: https://adoptium.net/
[cpe]: https://nvd.nist.gov/products/cpe
[cve]: https://cve.mitre.org/
[depcheck]: https://owasp.org/www-project-dependency-check/
[depcheck-docs]: https://jeremylong.github.io/DependencyCheck/
[depcheck-download]: https://github.com/jeremylong/DependencyCheck/releases
[edit070201]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/07-implementation/02-dependencies/01-dependency-check.md
[issue070201]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=content&template=request.md&title=Update:%2007-implementation/02-dependencies/01-dependency-check
[nist-db]: https://nvd.nist.gov/
[spotlight02]: https://youtu.be/YAXf3TaAYeA

\newpage
