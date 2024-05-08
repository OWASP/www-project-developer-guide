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
using its ability to analyse a Software Bill of Materials (SBOM).

The [Dependency-Track][deptrack-project] is an OWASP Flagship project
and can be installed using a docker-compose file from the Dependency-Track [website][deptrack].

#### What is Dependency-Track?

The [Dependency-Track][deptrack] tool provides an organization with a dashboard to analyze, oversee
and control the components for all of its projects.
It tracks component usage across every application in an organizations portfolio by analyzing exports
from multiple projects within the organization, via CycloneDX SBOMs and Vulnerability Exploitability Exchange.

It provides full-stack support for all types of component, including hardware and services.
Dependency-Track identifies multiple forms of risk, including components with known vulnerabilities,
by integrating with multiple sources of vulnerability intelligence such as the
National Vulnerability Database (NVD), GitHub advisories and others.

It has built-in repository support for various repository types,
and will provide risk and compliance for security, risk and operations.
See the [Documentation][deptrack-docs] for more information on the features provided by Dependency-Track.

#### Why use it?

By leveraging the capabilities of Software Bill of Materials (SBOM), Dependency-Track provides capabilities
that traditional Software Composition Analysis (SCA) solutions are unlikely to achieve.

The Dependency-Track dashboard has the ability to analyze all software projects within an organization.
It integrates with numerous notification platforms, for example Slack and Microsoft Teams, and can feed results
to various vulnerability aggregator tools such as DefectDojo or Fortify.

Dependency-Track is feature rich, it provides integrations and features that most organizations will need;
see the [Documentation Introduction][deptrack-docs] for a full list of these features.

#### How to use it

The OWASP Spotlight series provides an overview of tracking dependencies and inspecting SBOMs using Dependency-Track:
'Project 15 - [OWASP Dependency-Track][spotlight15]'.

Follow the [getting started guide][deptrack-docs] to install the Dependency-Track tool,
using the recommended deployment of a Docker container.

Although Dependency-Track will run with its default configuration
it should should be configured for the organization's specific needs.
The Dependency-Track configuration file is important for optimally running the tool
but this is outside the scope of the Developer Guide - see the Dependency-Track [documentation][deptrack-docs]
for a step by step guide to this configuration process.

----

[deptrack]: https://dependencytrack.org/
[deptrack-docs]: https://docs.dependencytrack.org/
[deptrack-project]: https://owasp.org/www-project-dependency-track/
[spotlight15]: https://youtu.be/irnZuLq4MDM
