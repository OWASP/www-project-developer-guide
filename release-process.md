<img src="assets/images/dg_logo_di.png" alt="DevGuide logo" height="220px"/>

The release process is in two stages; pre-release and the release itself

### Pre-release process

The pre-release process is semi-automatic, and triggers when the repo is tagged with a version number.
To trigger the release this process from within a cloned repo use a tag with an `-RCx` suffix,
where the number is incremented with each release candidate:

1. tag the release, for example for the first release candidate: `git tag 4.1.6-RC1`
2. push to the repo, for example: `git push origin 4.1.6-RC1`

The github release workflow will then create the pull-request with the proposed modifications to the release area.

Publish the link to this pull-request and ask for reviews and inputs.

If there are changes requested then go through this process again, incrementing the release candidate number,
for example `-RC2`.
When there are no further changes required then move on to the release process.

### Release process

The release process is automatic, and triggers when the repo is tagged with a version number.
To trigger the release this process from within a cloned repo:

1. tag the release, for example: `git tag 4.1.6`
2. push to the repo, for example: `git push origin 4.1.6`

The github release workflow then creates the pull request
with modifications to the release area promoted from the draft area.
Review the changes and, if all are correct, merge the pull request.
This will also automatically update the public web document and PDF/e-book versions.

It is good practice to bundle the PDF and ePub files into the [release area][release],
using the wording from the previous releases as a guide to the release notes.

----

OWASP DevGuide: _accessible security for developers_

[release]: https://github.com/OWASP/www-project-developer-guide/releases
