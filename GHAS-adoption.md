---
marp: true
theme: gh-theme-2023
class: invert
# paginate: true

footer: " " #adding a space as a footer ensures we show the footer line
html: true
allowlocalfiles: true


# A hubber image alt text must contain the text hubber to get the style which makes it a circle from the avatar

---
<!-- 
_footer: ""
-->

# DRAFT - GitHub Advanced Security 
Understand and simplify adoption 

![bg right](https://octodex.github.com/images/total-eclipse-of-the-octocat.jpg)

<div class="center-hubber">

![hubber gitstua](https://avatars.githubusercontent.com/gitstua?size=60) <span>@gitstua</span>
</div>

<!-- 
PREP
1. Create a new repo
2. Setup a few files

 -->


---
<div class='agenda'>
<div>

# Agenda

</div>

<div>

- Key Features of GitHub Advanced Security (GHAS)
- Sample roll-out plan
- Details of each step in the plan

</div>

</div>

---
# GitHub Advanced Security Key Features
- **Secret Scanning** to mitigate the risk of secrets
- **Code Scanning** to reduce vulnerabilities in code
- **Integrate** with and display results from other security tools (Veracode, Snyk, Fortify and any which export SARIF format)
- **Dependabot** to check for and automate keeping dependencies up to date

---

<!-- 
_class: none 
-->

<!--
mermaid source
gantt
    title GHAS Adoption
    dateFormat DDDD-MM-YY
    axisFormat %
    Align   : a, 2023-10-01, 5d
    Prepare   : p, 2023-10-04, 5d
    Pilot   : pilot, after p, 1w
    Document    :d, after pilot, 5d
    Secrets    : s, after d, 10d
    Code : c, after s, 10d

-->


![bg 90%](https://kroki.io/mermaid/svg/eNpNzLEOgjAQgOHdp7jFjSYt6sJGJOpCYsLE2NCTNIGWtGf08S0HqLdcc_-X9toR7SANWRoQrreygdL4iax3fDea8OLDqAmqNKKuRdty0W8b17LnQznY3qVdgM4gl_lBKCmkyuBkuN8DTjogi-lPHH_CDp6WPr8y0A_CMGP1YlD57jmimw0U5tsXvH7SYBeQIhOIm0lYyQWcvcGUui1FTh-8PkdN)


---
<div class='new-list'>

# 1. What does success look like

## Align
- Reduce secrets in code
- Identify high risk repos
- Meet compliance requirements
- Reduce vulnerabilities in code

</div>


---

<div class='new-list'>

# 2. **Prepare** to enable at scale

## Code scanning
- Collect information on your repositories and the languages used

## Secret scanning
- Consider how Secrets found will be mitigated
- Consider any custom patterns you may want for your enterprise, organization or repository

## Integrate
- Determine which integrations you will use for code scanning

</div>

---
<div class='new-list'>

# 3a. Secret Scanning

## Pilot Secret scanning
* Identify some high-impact projects which you will use to learn
* Workshop before enablement
* Piloting
* Wrap-up workshop to evaluate learnings

</div>

---
<div class='new-list'>

<!-- 
default setup https://github.blog/2023-01-09-default-setup-a-new-way-to-enable-github-code-scanning/ 
-->
# 3b. Code scanning (CodeQL)

## Pilot Code scanning
* Identify some high-impact projects which you will use to learn
* Workshop before enablement
* Consider `Default setup`
* Configure sample SARIF upload
* Run the pilot
* Wrap-up workshop to evaluate learnings
</div>

---
<div class='new-list'>

# Internal processes and procedures
Based on the learnings define internal processes and procedures

## Document

* Enable Code and Secret scanning on new organizations
* Define remediation plans for secrets located in code
* Manage vulnerbilities found with CodeQL and other tools
* Define how you will educate your developers how to get the best out of GHAS

</div>

---
<div class='new-list'>

# 5. Secrets 
## Secret scanning
* Enable push protection first to find newly committed secrets
* Verify remediation process
* Enable secret scanning on each organization 
* Remediate secrets starting with most critical using the security information in repository
* Review progress using `security overview` at enterprise and organization levels
</div>

--- 
<div class='new-list'>

# 6a. Code scanning

## Remediation
* Educate the teams on how to mitigate vulnerabilities; assign subject matter experts
* Enable code scanning for your organizations, consider enabling for TypeScript or JavaScript first
* Remediate vulnerabilities starting with most critical using the security information in repository
* Review progress using `security overview` at enterprise and organization levels

<div class='new-list'>

---
<div class='new-list'>

# 6b. Code scanning 
## Integration
* Update your CI pipelines to use marketplace actions to integrate your other security tools
* Verify the SARIF files are uploaded and you can view the alerts at repository level
* Verify `security overview` at enterprise and organization levels show the alerts

</div>