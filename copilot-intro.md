---
marp: true
theme: default
class: invert
# paginate: true

footer: "May 2023"
html: true
allowlocalfiles: true

backgroundImage: url(./assets/github-mark-white.svg);
backgroundPosition: bottom 15px right 15px;
backgroundSize: 40px;

# A hubber image alt text must contain the text hubber to get the style which makes it a circle from the avatar

style: |
  section {
    font-family: 'Hubot Sans';
    color: #fff;
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

# Introduction to GitHub Copilot

![bg right](https://octodex.github.com/images/total-eclipse-of-the-octocat.jpg)

Copilot overview

<div class="center-hubber">

![hubber gitstua](https://avatars.githubusercontent.com/gitstua?size=60) <span>@gitstua</span>
</div>

<!-- 
PREP
1. vscode - remove copilot
2. vs code insiders - install copilot
3. ensure python3 is installed
4. ensure dotnet is installed
5. ensure terraform plugin is installed

 -->

---

## Basic
Compile it to try it
![bg right:70% 90%](./assets/basic.gif)

---

## Intellisense
Type and you get ideas from your code
![bg right:70% 90%](./assets/intellisense.gif)

---

## GitHub Copilot
AI synthesizes code from your code
![bg right:70% 90%](./assets/copilot.gif)

---

## What is GitHub Copilot?

- AI-powered paired programming assistant
- Developed by GitHub and OpenAI
- Uses machine learning models to suggest code snippets

---

## How GitHub Copilot works
![bg left:30% 90%](https://octodex.github.com/images/total-eclipse-of-the-octocat.jpg)

- Uses OpenAI Codex model
- Analyzes context and patterns in codebase
- Suggests relevant code snippets when you type

---

## Benefits of using GitHub Copilot
![bg right:50% 90%](https://github.blog/wp-content/uploads/2023/02/GitHub-Copilot-for-Business.png?resize=2400%2C1260)
- Faster coding
- Improved accuracy
- Learning tool
- Less time writing the simple stuff

---

## Potential limitations of GitHub Copilot
We are constantly evaluating and improving Copilot including our vision of where you can improve the whole development cycle with our vision Copilot X.

- Limited language support
- Code quality process still required
- May not compile

<!-- It doesn't replace
- Your unit tests
- Your security tooling
- Your code review process
- Your code quality tooling
- Functional tests
-->

---
## Copilot for Business
- Enterprise controls such as enforcing blocking suggestions matching public code		
- Proxy support
- Allocate licences to users

---
## Demo 1 
### C#
<!-- ```
dotnet new console -o copilot
``` 
// obtain public ip address into variable
// obtain public ip address into variable using httpclient
// print public ip address
//get the current date and time
//print the current date and time
//get the current temperaturein london using httpclient from bbc weather
//print the current temperature in london
//make a list of zoo animals
//print 2 random animals from the list
//get a list of the azure ip addresses for azure 
//get a list of australin states short codes 
//print a random australian state
//print type of credit card based on number
//validate email address

-->

---
## Demo 2 
### Terraform
<!-- 
- get a quickstart from the web
- add some new stuff

 -->
---
## Demo 3 
### Python
<!-- 
- download an image from the web and save it to disk
- create a tumbnail 
- save the image as black and white
- save the image as sepia

-->


---
## Demo 4 
### Markdown
<!-- markdown presentation teaching the basics of azure 

presentation about dogs

-->

---
## Future of GitHub Copilot

- More tuned language support
- Improving performance
- Becoming an essential tool for developers
- More than just code suggestions, but a full development assistant

---
## Demo GitHub Copilot X

This is the intent on where we are going in the next versions. We are figuring out how this will work and how to make it work for you. 

<!-- 
OPEN THE GITHUB COPILOT X Chat GPT Panel

1. create a terraform file
2. create a python file
3. highlight some code and explain
4. ask it to summarize with fewer words
5. create some unit tests
6. /debug

PR
DOCS - https://copilot4docs.githubnext.com/
Voice
CLI

https://github.com/features/preview/copilot-x

 -->
---

## Conclusion

- GitHub Copilot is your AI-paired programming assistant
- Designed specifically to help synthesise code 
- GitHub Copilot for Business has enterprise controls

---
# Focus today was learning about GitHub Copilot functionality

## We didn't cover any of the following:
- GitHub Copilot pricing
- Any legal considerations

For these topics I will refer you to the Copolit FAQ avalable at [gh.io/copilotfaq](https://gh.io/copilotfaq)

