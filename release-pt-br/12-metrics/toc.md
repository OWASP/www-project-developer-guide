---

title: Metrics
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order: 32000
permalink: /release-pt-br/metrics/

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

![Developer Guide](../../assets/images/dg_alt.png "OWASP Developer Guide"){: .image-right }

## 10. Metrics

Metrics are important in an organization for various reasons, and in software security they can be used to:

* measure the effectiveness of security controls
* determine security posture
* provide justification for security programs
* and others

At present the OWASP [Integration Standards project Application Wayfinder][intstand] project
does not identify any OWASP projects that gather or process metrics; this may change in the future.

### Strategy and Metrics

The software security program is foundational to the strategic planning an organizations security posture.
Metrics keep track of the security activities within the plan and provide the information for gap analysis.

The [Software Assurance Maturity Model][samm] (SAMM) provides descriptions and definitions
for the [Strategy and Metrics][sammgsm] business practices within the [Governance][sammg] business function.
It provides two streams for achieving organizational maturity:

* [Create and Promote][sammgsma]
  which concerns the risks identified within an organization and what level of risk is acceptable
* [Measure and Improve][sammgsmb] which describes monitoring the security strategy through metrics

The categories of metrics suggested by SAMM are :

* Effort metrics: the effort spent on security
* Result metrics: the results of security efforts
* Environment metrics: the environment where security efforts take place

There are other metrics, sometimes specific to an individual organization, that can also be collected and acted on.

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue1200] or [edit on GitHub][edit1200].

[edit1200]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/12-metrics/toc.md
[issue1200]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2012-metrics/00-toc
[samm]: https://owaspsamm.org/about/
[sammg]: https://owaspsamm.org/model/governance/
[sammgsm]: https://owaspsamm.org/model/governance/strategy-and-metrics/
[sammgsma]: https://owaspsamm.org/model/governance/strategy-and-metrics/stream-a/
[sammgsmb]: https://owaspsamm.org/model/governance/strategy-and-metrics/stream-b/
[intstand]: https://owasp.org/www-project-integration-standards/

Sections:
