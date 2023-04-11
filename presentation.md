---
marp: true
theme: default
class: invert
# paginate: true

footer: "17 Feb 2023"
html: true
allowlocalfiles: true

backgroundImage: url(./assets/github-mark-white.svg);
backgroundPosition: bottom 15px right 15px;
backgroundSize: 40px;

# A hubber image alt text must contain the text hubber to get the style which makes it a circle from the avatar

style: |
  section {
    font-family: 'Hubot Sans';
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
  }

  .center-hubber > p {
    display: flex;
    align-items: center;
  }

  div.special li {
    margin: 0;
    padding: 36px 0 36px 84px;
    list-style: none;
    background-image: url("https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png");
    background-repeat: no-repeat;
    background-position: left center;
    background-size: 50px;

  }

  div.special li:nth-child(2){
    background-image: url("assets/graph-circle.png");
    
    img {
      color: red;
      border-radius: 50%;
      border: 5px solid red;
    }
  }


---

## Example of fancy list with circular icons
![bg left](https://octodex.github.com/images/deckfailcat.png)
<div class='special'>

- aaa
- bbb

</div>

---

# Contoso
## Customer Success Business Review
![bg right:40% 70%](https://avatars.githubusercontent.com/u/46500265?v=4)

<div class="center-hubber">

![hubber Stuart Eggerton](https://avatars.githubusercontent.com/gitstua?size=60) Stuart Eggerton

![hubber Jacola](https://avatars.githubusercontent.com/jacola?size=60) Jacola

</div>

---
# Architecture
![bg left 80%](./architecture.drawio.png)
- GHEC EMU
- On premises
  - JIRA
  - GitHub Actions Runners

---
<!-- This next line removes the invert so we match the background of the image we are using -->
<!-- 
class: none 
footer: ""
-->

# Awesome objective 1
![bg left](https://octodex.github.com/images/hula_loop_octodex03.gif)

## Progress
 
- test
- test

## Next

---
<!-- class: invert -->
# Using this slide deck template 
1. Ensure you have the vscode plugins installed 
  - https://marketplace.visualstudio.com/items?itemName=marp-team.marp-vscode
  - https://marketplace.visualstudio.com/items?itemName=hediet.vscode-drawio
1. 

---
![bg](https://octodex.github.com/images/deckfailcat.png)