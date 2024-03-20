---

title: Dependency-Track
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 7220
permalink: /release/implementation/dependencies/dependency_track/

---

{% include breadcrumb.html %}

### 5.2.2 Dependency-Track

OWASP Dependency-Track is an intelligent platform for Component Analysis including Third Party Software.
It allows organizations to identify and reduce risk in the software supply chain
via its ability to analyse a Software Bill of Materials (SBOM).

The [Dependency-Track][deptrack-project] is an OWASP Flagship project
and can be installed using a docker-compose file from the Dependency-Track [website][deptrack].

#### What is Dependency-Track?

The [Dependency-Track][deptrack] tool provides an organization with a dashboard to analyze, oversee
and control the components for all of its projects.
It tracks component usage across every application in an organizations portfolio by consuming SBOMS
from multiple projects within the organization, via CycloneDX SBOMs and Vulnerability Exploitability Exchange.

It provides full-stack support for all types of component, including hardware and services.
Dependency-Track identifies multiple forms of risk including
Components with known vulnerabilities by integrating with multiple sources of vulnerability intelligence including
National Vulnerability Database (NVD), GitHub advisories and others.

It has built-in repository support for various repository types,
and will provide risk and compliance for security, risk and operations.
See the [Documentation][deptrack-docs] for an appreciation of the feature provided by Dependency-Track.

#### Why use it?

By leveraging the capabilities of Software Bill of Materials (SBOM), Dependency-Track provides capabilities
that traditional Software Composition Analysis (SCA) solutions just cannot achieve.

The Dependency-Track dashboard that will analyze all the software projects within an organization.
It integrates with numerous notification platforms, for example Slack and Microsoft Teams, and can feed results
to various vulnerability aggregator tools such as DefectDojo or Fortify.

Dependency-Track is feature rich, it provides integrations and features that most organizations will need;
see the [Documentation Introduction][deptrack-docs] for a full list of the features.

#### How to use it

The OWASP Spotlight series provides an overview of tracking dependencies and inspecting SBOMs using Dependency-Track:
'Project 15 - [OWASP Dependency-Track][spotlight15]'.

Follow the [getting started guide][deptrack-docs] to install the Dependency-Track tool,
using the recommended deployment of a Docker container.

Dependency-Track then needs to be configured, it comes with a default configuration but this needs to be tailored for
the specific organization. The configuration file is crucial to running the tool successfully,
and this is outside the scope of the Developer Guide - see the Dependency-Track [documentation][deptrack-docs]
for a step by step guide to this configuration.

----

[deptrack]: https://dependencytrack.org/
[deptrack-docs]: https://docs.dependencytrack.org/
[deptrack-project]: https://owasp.org/www-project-dependency-track/
[spotlight15]: https://youtu.be/irnZuLq4MDM

\newpage
