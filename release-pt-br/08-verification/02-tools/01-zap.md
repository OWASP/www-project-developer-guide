---

title: Zed Attack Proxy
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order: 28210
permalink: /release-pt-br/verification/tools/zed_attack_proxy/

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

![ZAP logo](../../../../assets/images/logos/zap.png "OWASP ZAP"){: .image-right }

### 6.2.1 Zed Attack Proxy

The Zed Attack Proxy ([ZAP][zap]) verification and testing project is a widely used
dynamic application security testing tool used for web applications and proxies.

ZAP was for a long time an OWASP Flagship project and is now a project within
the [Crash Override][crash].
Installers for various platforms can be [downloaded][zapdownload] from the ZAP website.

#### What is ZAP?

The [Zed Attack Proxy][zap] is a tool that dynamically scans web applications.
ZAP can be used manually to test applications or can be run within an automated [CI/CD pipeline][cscicd] environment.

It is commonly used for Dynamic Application Security Testing (DAST), both manual DAST and automated in pipelines.
ZAP is also widely used for:

* Vulnerability Assessment
* Penetration Testing
* Runtime Testing
* Code Review

#### Why use it?

ZAP is easily installed, intuitive to use and is regularly updated to meet the evolving threat landscape.

ZAP is an effective tool that is widely used by a large community of testers, application developers and security engineers.
This makes it a tool that many teams will already be familiar with and probably using already;
you can almost regard ZAP is a common language within the security community when it comes to web application testing.

#### How to use it

The OWASP Spotlight series provides an overview of using ZAP: 'Project 12 - [OWASP Zed Attack Proxy (ZAP)][spotlight12]'.

ZAP [installers][zapdownload] can be downloaded for Windows, Linux and MacOS.
Once installed the follow the [getting started guide][zapstart] for an introduction on how to use it manually via the UI
or automatically within a CI/CD environment - and definitely check out the [Heads Up Display][zaphud] mode.

#### References

* [ZAP home page][zap]
* [OWASP Spotlight][spotlight12] on ZAP

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue080201] or [edit on GitHub][edit080201].

[crash]: https://crashoverride.com/open-source
[cscicd]: https://cheatsheetseries.owasp.org/cheatsheets/CI_CD_Security_Cheat_Sheet
[edit080201]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/08-verification/02-tools/01-zap.md
[issue080201]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=content&template=request.md&title=Update:%2008-verification/02-tools/01-zap
[spotlight12]: https://youtu.be/usIlW8Q-hc4
[zap]: https://www.zaproxy.org/
[zapdownload]: https://www.zaproxy.org/download/
[zaphud]: https://www.zaproxy.org/getting-started/#the-heads-up-display
[zapstart]: https://www.zaproxy.org/getting-started/
