---

title: Mobile Application Security
layout: col-document
tags: OWASP Developer Guide
contributors:
document: OWASP Developer Guide
order: 30050
permalink: /release-pt-br/culture_building_and_process_maturing/mobile_application_security/

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

![MAS logo](../../../assets/images/logos/mas.png "OWASP MAS"){: .image-right }

### 8.5 Mobile Application Security

The [MAS Verification Standard][masvs] (MASVS) explains the processes, techniques
and tools used for security testing a mobile application.

The OWASP [MAS Crackmes][mascrack], also known as UnCrackable Apps,
is a collection of reverse engineering challenges for the OWASP [Mobile Application Security][masproject] (MAS).

#### What is MAS Crackmes?

OWASP [MAS Crackmes][mascrack] is a set of reverse engineering challenges for mobile applications.
These challenges are used as examples throughout the OWASP [Mobile Application Security Testing Guide][mastg] (MASTG)
and, of course, you can also solve them for fun.

There are challenges for [Android][masandroid] and also a couple for [Apple iOS][masios].

#### Why use MAS Crackmes?

Working through the challenges will improve understanding of [mobile application security][csmas]
and will also give an insight into the examples provided in the MASTG.

#### How to try the challenges

1. Select and download a challenge into your mobile application environment
2. Satisfy the individual challenge exercise
3. Have fun

Each challenge has various solutions provided by the community; these can be used to compare with your solution.

#### References

* OWASP [Mobile Application Security][masproject] (MAS) project
* OWASP [MAS Crackmes][mascrack] UnCrackable Apps
* OWASP [MAS Testing Guide][mastg] (MASTG)
* OWASP [MAS Verification Standard][masvs] (MASVS)
* OWASP [Mobile Application Security][csmas] cheat sheet

----

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue1005] or [edit on GitHub][edit1005].

[csmas]: https://cheatsheetseries.owasp.org/cheatsheets/Mobile_Application_Security_Cheat_Sheet
[edit1005]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/10-culture-process/05-mas.md
[issue1005]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2010-culture-process/05-mas
[masproject]: https://owasp.org/www-project-mobile-app-security/
[masandroid]: https://mas.owasp.org/crackmes/Android/
[mascrack]: https://mas.owasp.org/crackmes/
[masios]: https://mas.owasp.org/crackmes/iOS/
[mastg]: https://mas.owasp.org/MASTG/
[masvs]: https://mas.owasp.org/MASVS/