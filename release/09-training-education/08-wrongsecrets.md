---
title: WrongSecrets
layout: col-document
tags: OWASP Developer Guide
contributors: Ben de Haan 
document: OWASP Developer Guide
order: 9260
permalink: /release/training_education/wrongsecrets/
---

{% include breadcrumb.html %}

### 7.8 WrongSecrets

[OWASP WrongSecrets][wrongsecrets-project] is a production status project
and provides challenges focused on secrets management using an intentionally vulnerable application and environment.
The project offers standalone and Capture-the-flag modes, with a demo on [Heroku][heroku].

#### What is WrongSecrets?

[WrongSecrets][wrongsecrets] goals are to:

- Educate on secret management and its pitfalls
- Help people reflect on their secrets management strategy
- Promote secrets management as an important facet of security

The project provides challenges around secrets management across several layers:

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

You can set WrongSecrets up in standalone or in capture the flag (CTF) mode on Docker, Kubernetes, AWS, GCP or Azure.

Set-up guides for the standalone version are available in the [project README][readme].

For the CTF, the project also provides [set-up guides][ctf] and a [Helm chart][helm].

---

[ctf]: https://github.com/OWASP/wrongsecrets/blob/master/ctf-instructions.md
[helm]: https://owasp.org/wrongsecrets-ctf-party/
[heroku]: https://wrongsecrets.herokuapp.com/
[readme]: https://github.com/OWASP/wrongsecrets/blob/master/README.md
[wrongsecrets]: https://github.com/OWASP/wrongsecrets
[wrongsecrets-project]: https://owasp.org/www-project-wrongsecrets/
