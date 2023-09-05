---
marp: true
theme: default
class: invert
# paginate: true

footer: "@gitstua - September 2023"
html: true
allowlocalfiles: true

backgroundImage: url(./assets/github-mark-white.svg);
backgroundPosition: bottom 15px right 15px;
backgroundSize: 40px;

# A hubber image alt text must contain the text hubber to get the style which makes it a circle from the avatar



style: |
  font-family: 'Hubot Sans';
  section {
    font-family: 'Hubot Sans';
    color: #fff;
    src : url('https://fonts.googleapis.com/css2?family=Roboto+Mono:wght@300&display=swap');

  }
  footer {
    height: 20px;
    font-family: 'Arial';
    width:90%;
    font-family: 'Roboto Mono';
  } 

  img[alt~="hubber"] {
    border-radius: 50%;
    margin-right: 20px;
    border: 1.5px solid #6e40c9;
  }

  .center-hubber > p {
    display: flex;
    align-items: center;
  }
  
  li {
    margin: 0;
    padding: 20px 0 20px 84px;
    list-style: none;
    background-image: url("./assets/circle2.png");
    background-repeat: no-repeat;
    background-position: left center;
    background-size: 50px;
  }


---

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

<!-- hide footer in marp -->
# Agenda
<!-- 
_class: none 
_footer: ""
-->

- Key Features of GitHub Advanced Security (GHAS)
- Sample roll-out plan
- Details of each step in the plan

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

## 1. **Align** on what success looks like
- Reduce secrets in code
- Identify high risk repos
- Meet compliance requirements
- Reduce vulnerabilities in code

---
## 2. **Prepare** to enable at scale


**Prepare teams for code scanning**
- Collect information on your repositories and the languages used

**Prepare teams for secret scanning**
- Consider how Secrets found will be mitigated
- Consider any custom patterns you may want for your enterprise, organization or repository

**Integrate**
- Determine which integrations you will use for code scanning
---
## 3a. **Pilot** - Secret Scanning
- Identify some high-impact projects which you will use to learn
- Workshop before enablement
- Pilot
- Wrap-up workshop to evaluate learnings

---

<!-- 
default setup https://github.blog/2023-01-09-default-setup-a-new-way-to-enable-github-code-scanning/ 
-->
## 3b. **Pilot** - Code Scanning (CodeQL)
- Identify some high-impact projects which you will use to learn
- Workshop before enablement
- Consider `Default setup`
- Configure sample SARIF upload
- Pilot
- Wrap-up workshop to evaluate learnings

---
## 4. **Document** internal processes and procedures
Based on the learnings define internal processes and procedures to:
- Enable Code and Secret scanning on new organizations
- Define remediation plans for secrets located in code
- Manage vulnerbilities found with CodeQL and other tools
- Define how you will educate your developers how to get the best out of GHAS

---
## 5.**Secret** scanning
- Enable push protection first to find newly committed secrets
- Verify remediation process
- Enable secret scanning on each organization 
- Remediate secrets starting with most critical using the security information in repository
- Review progress using `security overview` at enterprise and organization levels

---
## 6a. **Code** scanning
- Educate the teams on how to mitigate vulnerabilities; assign subject matter experts
- Enable code scanning for your organizations, consider enabling for TypeScript or JavaScript first
- Remediate vulnerabilities starting with most critical using the security information in repository
- Review progress using `security overview` at enterprise and organization levels

---
## 6b. Code scanning **integration**
- Update your CI pipelines to use marketplace actions to integrate your other security tools
- Verify the SARIF files are uploaded and you can view the alerts at repository level
- Verify `security overview` at enterprise and organization levels show the alerts
