---

title: Remediation
layout: col-document
tags: OWASP Developer Guide
author:
contributors:
document: OWASP Developer Guide
order: 504

---

{% include breadcrumb.html %}
### 5.4 Remediation

Risk management is the identification, assessment, and prioritization of risks to the application or system.
The objective of risk management is to ensure that uncertainty does not deflect the endeavor from the business goals,
and remediation is the strategy chosen in response to identifying this risk.

Risk management can be split in two parts. First, determine which risks exists and then secondly handling those risks in a way that is best for the business;
risk management should always be business driven.

There are four common ways to handling risk:

1. Acceptance: the business is aware of the risk but has decided that no action needs to be taken; the risk is deemed acceptable

2. Mitigation: the risk is considered serious enough to require implementation of security controls to remove the risk

3. Transferring: the risk is considered serious but can be transferred to another party

4. Elimination: the risk can be avoided or removed completely, often by removing the object with which the risk is associated

Examples:

1. Acceptance: sometimes risks are so low in priority or bearable that it is not worth mitigating,
    an example might be where the version of software is revealed but this is acceptable (or even desirable)

2. Mitigation: there are many examples of where risks are mitigated;
    for example input sanitization or output encoding may be used for information supplied by an untrusted source,
    or the use of encrypted communication channels for transferring high risk information

3. Transferring: a common example of transferring risk is the use of third party insurance in response to the risk of RansomWare.
    Insurance premiums are paid but losses to the business are covered by the insurance

4. Elimination: an example may be that an application implements legacy functionality that is no longer used,
    if there is a risk of it being exploited then the risk can be eliminated by removing this legacy functionality

\newpage
