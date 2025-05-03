<a href="https://devguide.owasp.org/"><img src="assets/images/dg_alt.png" alt="DevGuide logo" height="180px"/></a>

### Contributing

The Developer Guide has been updated for the modern security landscape,
concentrating less on covering everything in one document and more on introducing a subject/project
and then suggesting where more in-depth information can be found.
The project has a team of leaders that oversee the project
and contributions from members of the security community are positively encouraged.

All contributions and suggestions are certainly welcome, and we ask that
you follow the [contributing Code of Conduct][conduct].
Contributors can [make suggestions][issues] and provide changes via a [pull request][request].

Feel free to discuss topics in the [project wiki][wiki] and create new discussions.

Note that the [draft][draft] version provides the content for the released version of Developer Guide,
in the ['release'][release] directory, promoted during the automated release process.
Therefore any manual changes under the release directory are likely to be over-written.

### Ground rules

* follow our [Code of Conduct](code_of_conduct.md)
* ensure that all contributions meet the [license](license.txt)
* the use of generative AI is not prohibited but must be declared in the pull request

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
Follow the style used in OWASP flagship projects [ASVS][asvs] and [WSTG][wstg],
which is speaking from first person plural and semi-formal in tone.

### Technical level

Generally the guide is aimed at the introductory to medium technical levels,
and should rarely deal with any subject at an advanced level.
This is a deliberate policy that makes the guide accessible and keeps the length reasonable.

The overview/introduction of the main sections should be aimed at the introductory level,
with more detail contained in the sub-sections at a medium technical level.
Note this guide should not replicate the many detailed sources on specific security topics;
instead provide links to these specialist security knowledge bases.

### Page structure

Each sub-section should deal with one specific subject, for example 'Threat modeling',
or a single project such as the OWASP 'Threat Dragon' Builder/Tool project.

Sub-sections that describe an individual project should follow the same structure:

1. Introduction, summarizing the project at a very high level:
  _supply a couple of sentences on the project including its status as an OWASP project and where to find it_
2. The 'What', explaining what the project is to a general level:
  _go into more detail about the project so that a developer can gain an overview of what this project can provide for them_
3. The 'Why', explaining why developers will want to use the project:
  _provide more context for project that allows developers to determine whether to use it in their team_
4. The 'How', describe how to get started with the project
  _give a brief outline of how the project provides value for a web application development team_
  _Do not repeat the project documentation itself; ideally provide a primer and a pointer to the project documentation_
5. Further reading or resources, if any, providing links on the project at an advanced/detailed level

Note that the page describing a project should not be the same as the project documentation on the OWASP site,
the Developer Guide should strive to be a ' TL;DR ' for the project running to one or maybe two pages.

### Media kit

The OWASP projects have [media kits][media] that contain biographies of the project leaders and other project media.
This can be used for images and marketing material.

### Pull requests

The pull requests have checks applied to them:

1. Link checker for any broken links; if there is an imperative for a broken link then add it to `.lycheeignore`
2. Markdown lint that ensures the markdown is consistent and valid
3. Spell checker; new words that are not recognized can be added to `/.wordlist.txt`

if all these checks pass then both the PDF and ePub versions of the guide are provided as github artifacts.

### Running checks locally

The pipeline will apply checks to all pull-requests, and will fail on any error.
To run these checks locally before pushing a commit, run these commands from the top directory:

1. Link checker: `lychee --max-retries 1 --exclude-path './_includes/*.html' './**/*.md'`
2. Markdown linter: `markdownlint-cli2  **/*.md`
3. Spell checker: `pyspelling --config .spellcheck-en.yaml` (for english)
4. commands to set up the environment for PDF export

```text
mkdir draft/temp
mkdir assets/images/logos/publish
export RESOURCE_PATH="draft/assets/images:draft/assets:draft:assets/images/logos:assets/images:assets/images/logos/publish"
```

and the commands to create PDF export:

```text
tail -n +14 -q $(find draft -name "*[0-9]*.md" | sort) > draft/temp/draft.markdown
sed -i "s/{: .image-right }/{height=180px}/g" draft/temp/draft.markdown
pandoc -f markdown -o draft.pdf --resource-path="$RESOURCE_PATH" \
-fmarkdown-implicit_figures draft/title.pdf.yaml draft/temp/draft.markdown
```

Follow instructions to install the command line [lychee][lychee-install] and [pandoc][pandoc-install].

To install `markdownlint-cli2` use npm: `npm install markdownlint-cli2 --global`,
and to install `pyspelling` use pip: `pip install pyspelling`

----

[asvs]: https://owasp.org/www-project-application-security-verification-standard/
[conduct]: code_of_conduct.md
[dashboard]: https://github.com/orgs/OWASP/projects/14/views/1
[draft]: draft
[issues]: https://github.com/OWASP/www-project-developer-guide/issues/new/choose
[lychee-install]: https://lychee.cli.rs/
[media]: https://drive.google.com/drive/folders/1Ft8Ll0cgw0TIoub6aXTIJDmy0sk1RarU
[pandoc-install]: https://pandoc.org/installing.html
[release]: release
[request]: https://github.com/OWASP/www-project-developer-guide/pulls
[wiki]: https://github.com/OWASP/www-project-developer-guide/wiki
[wstg]: https://owasp.org/www-project-web-security-testing-guide/
