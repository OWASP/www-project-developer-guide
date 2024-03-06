---
title: WrongSecrets
layout: col-document
tags: OWASP Developer Guide
contributors: Ben de Haan 
document: OWASP Developer Guide
order: 908
permalink: /draft/training_education/wrongsecrets/
---

{% include breadcrumb.html %}

### 7.8 WrongSecrets

[OWASP WrongSecrets][wrongsecrets-project] is a production status project
and provides challenges focused on secrets management using an intentionally vulnerable application and environment.
The project offers standalone and Capture-the-flag modes, with a demo on [Heroku][heroku].

The project goals are to:

- Educate on secret management and its pitfalls
- Help people reflect on their secrets management strategy
- Promote secrets management as an important facet of security

#### What is WrongSecrets?

[WrongSecrets][wrongsecrets] provides challenges around secrets management across several layers:

- A Spring Boot Java application
- Application configuration
- Docker
- Kubernetes
- Vault
- AWS, GCP, or Azure
- Binaries / Reverse engineering

Scenarios vary in difficulty, and you can solve some of them just by using the browser on your mobile phone.
For others, you would need knowledge of cloud security or reverse engineering tools and cryptography.

#### Why use it?

If you, your team or your organization want to learn about secrets management and potential pitfalls,
you can do so with WrongSecrets' challenges.

Alternatively, you can use WrongSecrets as a secret detector testbed/benchmark.

#### How to use it

You can set WrongSecrets up in standalone or capture the flag (CTF) mode on Docker, Kubernetes, AWS, GCP or Azure.

Set-up guides for the standalone version are available in the [project README][readme].

For the CTF, the project also provides [set-up guides][ctf] and a [Helm chart][helm].

---

The OWASP Developer Guide is a community effort; if there is something that needs changing
then [submit an issue][issue0908] or [edit on GitHub][edit0908].

[ctf]: https://github.com/OWASP/wrongsecrets/blob/master/ctf-instructions.md
[edit0908]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/09-training-education/08-wrongsecrets.md
[helm]: https://owasp.org/wrongsecrets-ctf-party/
[heroku]: https://wrongsecrets.herokuapp.com/
[issue0908]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=content&template=request.md&title=Update:%2009-training-education/08-wrongsecrets
[readme]: https://github.com/OWASP/wrongsecrets/blob/master/README.md
[wrongsecrets]: https://github.com/OWASP/wrongsecrets
[wrongsecrets-project]: https://owasp.org/www-project-wrongsecrets/

\newpage
