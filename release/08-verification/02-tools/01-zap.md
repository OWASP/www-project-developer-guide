---

title: Zed Attack Proxy
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 8210
permalink: /release/verification/tools/zed_attack_proxy/

---

{% include breadcrumb.html %}

### 6.2.1 Zed Attack Proxy

The Zed Attack Proxy ([ZAP][zap]) verification and testing project is a widely used
dynamic application security testing tool used for web applications and proxies.

ZAP was for a long time an OWASP Flagship project and is now a project within
the Software Security Project ([SSP][ssp]) organization, which itself is part of the [Linux Foundation][lf].
Installers for various platforms can be [downloaded][zapdownload] from the ZAP website.

#### What is ZAP?

The [Zed Attack Proxy][zap] is a tool that dynamically scans web applications.
It is commonly used for Dynamic Application Security Testing (DAST) but also has multiple uses:

* Vulnerability Assessment
* Penetration Testing
* Runtime Testing
* Code Review

ZAP can be used manually to test applications or can be run within an automated CI/CD environment.

#### Why use it?

ZAP is easily installed, intuitive to use and is regularly updated to meet the evolving threat landscape.

ZAP is an effective tool that is widely used by a large community of testers, developers, security engineers etc.
This makes it a tool that many teams will already be familiar with and probably using it already;
you can almost regard ZAP is a common language within the security community when it comes to web application testing.

#### How to use it

The OWASP Spotlight series provides an overview of using ZAP: 'Project 12 - [OWASP Zed Attack Proxy (ZAP)][spotlight12]'.

ZAP [installers][zapdownload] can be downloaded for Windows, Linux and MacOS.
Once installed the follow the [getting started guide][zapstart] for an introduction on how to use it manually via the UI
or automatically within a CI/CD environment - and definitely check out the [Heads Up Display][zaphud] mode.

----

[lf]: https://www.linuxfoundation.org/
[spotlight12]: https://youtu.be/usIlW8Q-hc4
[ssp]: https://softwaresecurityproject.org/
[zap]: https://www.zaproxy.org/
[zapdownload]: https://www.zaproxy.org/download/
[zaphud]: https://www.zaproxy.org/getting-started/#the-heads-up-display
[zapstart]: https://www.zaproxy.org/getting-started/
