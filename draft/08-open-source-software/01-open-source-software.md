---

title: Open Source Software Introduction
layout: col-document
tags: OWASP Developer Guide
author: Shruti Kulkarni
contributors:
document: OWASP Developer Guide
order: 801

---

{% include breadcrumb.html %}

### 8.1 Introduction to Open Source software

The OWASP Development Guide is being rewritten by the OWASP community.
and the content of this section has yet to be filled in.

If you would like to contribute then follow the
[contributing guidelines](https://github.com/OWASP/www-project-developer-guide/blob/main/contributing.md)
and submit your content for review.

The following subsections are planned:
* Static Code Analysis (for licensing and dependencies)
* Third Party Software and Libraries (hive off to OWASP Dependency Tracker)
* Maintaining open source software/components: Binaries / pre-compiled code / packages – where source code sharing is not a part of the license
* Copying source code off public domain (internet)

* Static Code Analysis (for licensing and dependencies)
  * Consuming open source software has a heavy dependency on the license under which the open source software is available.
  * Following are some URLs to licensing details:

              https://choosealicense.com/licenses/

              https://tldrlegal.com/

              https://creativecommons.org/licenses/by/4.0/  

    It is important for the organisation to have a policy statement for consumption of open source software.
    From a licensing perspective and the implication of using a open source software incorrectly, maintain a procedure for approval of usage of selected open source software. 
    This could be in the form of a workflow or obtaining security approvals for the chosen open source software
    We realise it could be challenging, but if feasible, maintain a list of approved open source software
    
        * Address vulnerabilities with: Binaries / pre-compiled code / packages – where source code sharing is not a part of the license (Examples executables / nugets)
              - Where possible use version pinning 
              - Where possible use integrity verification
              - Check for vulnerabilities for the selected binies in vulnerability disclosure databases like
                         - CVE database (https://cve.mitre.org/cgi-bin/cvekey.cgi?keyword=bouncy+castle)
                         - VulnDB (https://vuldb.com/?id.173918)
              - If within the budget of your organisation, use an SCA tool to scan for vulnerabilities 
              - Always vet and perform due-diligence on third-party modules that you install in order to confirm their health and credibility.
              - Hold-off on upgrading immediately to new versions; allow new package versions some time to circulate before trying them out.
              - Before upgrading, make sure to review changelog and release notes for the upgraded version.
              - When installing packages make sure to add the --ignore-scripts suffix to disable the execution of any scripts by third-party packages.
              - Consider adding ignore-scripts to your .npmrc project file, or to your global npm configuration.
              - If you use npn, run npm outdated, to see which packages are out of date
              - Typosquatting is an attack that relies on mistakes made by users, such as typos. With typosquatting, bad actors could publish malicious modules to the npm registry with names that look much like existing popular modules.To address this vulnerability verify your packages before consuming them   

        * Address vulnerabilities with: where source code sharing is a part of the license 
              - [GitHub] CodeQL / third party tool
              - If within the budget of your organisation, use an SCA tool to scan for vulnerabilities
        
        * Security Testing: Binaries / pre-compiled code / packages – where source code sharing is not a part of the license (Examples executables / nugets)
              - Perform Dynamic application analysis
              - Perform Pen testing
              - Verify which tokens are created for your user or revoke tokens in cases of emergency - use npm token list or npm token revoke respectively.
              
        * Security Testing: where source code sharing is a part of the license 
              - Perform Static code analysis
              - Perform Dynamic application analysis
              - Perform Pen testing.
    
* Third Party Software and Libraries (hive off to OWASP Dependency Tracker)
    *  Address supply chain risk with: Binaries / pre-compiled code / packages – where source code sharing is not a part of the license (Examples executables / nugets)
            - Use  signed binaries / packages
            - Reference private feed in your code
            - Use controlled scopes
            - Lock files
            - Avoid publishing secrets to the npm registry (secrets may end up leaking into source control or even a published package on the public npm registry)

     *  Address supply chain risk with: where source code sharing is a part of the license
            - [GitHub]Check for dependency graph
            - [GitHub]Dependabot alerts
            - [GitHub]Commit and tag signatures

    * Monitor Dependencies: Binaries / pre-compiled code / packages – where source code sharing is not a part of the license (Examples executables / nugets)
           - Use dependency graphs
           - Enable repeatable package restores using lock files

    * Monitor Dependencies: where source code sharing is a part of the license
           - [GitHub]Check for dependency graph
           - [GitHub] Secret scanning
    
* Maintaining open source software/components: Binaries / pre-compiled code / packages – where source code sharing is not a part of the license 	
	         - Monitor for deprecated packages
	         - Use dependency graphs
           - Lock files
	         - Monitor vulnerabilities with:
                 - Check for vulnerabilities for the selected binies in vulnerability disclosure databases like
                         - CVE database (https://cve.mitre.org/cgi-bin/cvekey.cgi?keyword=bouncy+castle)
                         - VulnDB (https://vuldb.com/?id.173918)
           - If within the budget of your organisation, use an SCA tool to scan for vulnerabilities "

* Copying source code off public domain (internet) - For example source code that is on a blog or in discussion forums like stacktrace or snippets of example on writeups	
	        *******Don’t do it!!!*******


\newpage
