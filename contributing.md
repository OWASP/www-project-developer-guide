### Contributing

The Developer Guide needs to be updated for the modern security landscape,
and OWASP is reviving this project to do just that.
The project has a team of leaders that will oversee the project
and now we need as many members of the security community as possible to contribute.

All contributions and suggestions are certainly welcome, and we ask that
you follow the [contributing code of conduct][conduct].
Contributors can [make suggestions][issues] and provide changes via a [pull request][request].

Feel free to discuss topics in the [project wiki][wiki] and create new discussions.

### Philosophy

The Developer Guide does not seek to duplicate the information contained in the many OWASP documentation projects;
these projects address their subject fully and completely.
Instead the Developer Guide is a starting point on a wide range of subjects
which a developer would need to know at least the basics.
The Developer Guide should supply this basic knowledge only,
and then refer the developer to further reading for more in-depth treatment of the subject.
As a rule of thumb, if a section is more than two pages then it is probably too long;
split the section up or refer to another more detailed project.

### Etiquette

There is a [project board][dashboard] which helps to coordinate contributions
and keeps track of progress towards each milestone.

* select an issue from the project board for the section you want to work on
* if this issue is free ask for it to be assigned to you
* if the issue has already been assigned then coordinate with the existing owner
* if there is not an existing issue that describes your content then [suggest one][issues]
* provide your contributed content as a [pull request][request]

### Style Guide

The Developer Guide will have many contributors, and it is an aim to keep the style of writing similar throughout.
It would be good to keep to a style used in OWASP flagship projects [ASVS][asvs] and [WSTG][wstg],
which is speaking from first person plural and semi-formal in tone.

### Technical level

Generally the guide is aimed at the introductory to medium technical levels,
and should rarely deal with a subject at an advanced level.
This is a deliberate policy that makes the guide accessible and keeps the length reasonable.

The overview/introduction of the main sections should be aimed at the introductory level,
with more detail contained in the sub-sections at a medium technical level.
Note this guide should not replicate the many detailed sources on specific security topics;
instead provide links to these specialist security knowledge bases.

### Page structure

Each sub-section should deal with one specific subject, for example 'Threat modeling' or 'Digests'.
The sub-sections ideally follow the same structure:

1. Overview, summarising the subject at an introductory level
2. Main body, explaining the subject to a medium/general level
3. Further reading, providing links to the subject at an advanced/detailed level
4. Resources, providing links to tools and applications that may be used when working within this domain

### Pull requests

The pull requests have checks applied to them:

1. Link checker for any broken links; if there is an imperative for a broken link then add it to `.lycheeignore`
2. Markdown lint that ensures the markdown is consistent and valid
3. Spell checker; new words that are not recognised can be added to `/.wordlist.txt`

if all these checks pass then both the PDF and ePub versions of the guide are provided as github artifacts.

[asvs]: https://owasp.org/www-project-application-security-verification-standard/
[conduct]: code_of_conduct.md
[dashboard]: https://github.com/orgs/OWASP/projects/14/views/1
[issues]: https://github.com/OWASP/www-project-developer-guide/issues/new/choose
[request]: https://github.com/OWASP/www-project-developer-guide/pulls
[wiki]: https://github.com/OWASP/www-project-developer-guide/wiki
[wstg]: https://owasp.org/www-project-web-security-testing-guide/
