---
marp: true
theme: default
class: invert
# paginate: true



html: true
allowlocalfiles: true

# A hubber image alt text must contain the text hubber to get the style which makes it a circle from the avatar



style: |
  @import url('https://fonts.googleapis.com/css2?family=Roboto&family=Roboto+Mono:wght@100;400&display=swap');
  @import url('https://fonts.cdnfonts.com/css/inter');

  section {
    font-family: 'Inter', sans-serif;
    color: #fff;
    font-color: #fff;
  }

  zzzfooter {
    height: 20px;
    font-family: 'Arial';
    width:90%;
    font-family: 'Roboto Mono';

    border-top: 1px linear-gradient(to right, #FE7A73 0%, #EB7BC6 25%,#44ADD1 75%, #54D165 100%);;
  } 
  
  footer {
    background-color: 1px solid pink;
    background: rgb(67,67,67);
    background: linear-gradient(0deg, rgba(67,67,67,1) 0%, rgba(255,255,255,1) 55%);
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
  
  .center-hubber > p {
    margin-top: 30px;
  }

  .agenda{
    display: grid;
    grid-template-columns:  auto minmax(0, 1fr);
    gap: 1rem;
  }
  .agenda li {
    font-size: 0.9em;
    margin: 0;
    padding: 15px 0 10px 84px;
  }

  li {
    margin: 0;
    padding: 20px 0 20px 84px;
    list-style: none;
  }

  .gradient-pink-to-green {
    width: 100%;
    height: 2px;
    background: linear-gradient(to right, #FE7A73 0%, #EB7BC6 25%,#44ADD1 75%, #54D165 100%);
    border-radius: .8em;
  }

  .gradient-pink-to-green-short {
    margin-top: 3px;
    width: 45%;
    height: 0.5px;
    background: linear-gradient(to right, #FE7A73 0%, #EB7BC6 25%,#44ADD1 75%, #54D165 100%);
    opacity: 0.5;
  }

  h1, h2 {
   border-bottom: 3px solid pink;
   border-image: linear-gradient(to right, #FE7A73 0%, #EB7BC6 25%,#44ADD1 75%, #54D165 100%) 10;
  }

  .columns {
      display: grid;
      grid-template-columns: repeat(2, minmax(0, 1fr));
      gap: 1rem;
  }

  .agenda h1, .columns h1 {
    border: none;
  }

  .agenda h1{
    padding: 15px;
    border: 2px solid white;
    font-weight: 100;
    /* make corners rounded */
    border-radius: 10px;
    font-size: 1em;
    margin-top: 140px;
  }

  .agenda > div:first-child {
    border-right: 3px solid pink;
    border-image: linear-gradient(to bottom, #FE7A73 0%, #EB7BC6 25%,#44ADD1 75%, #54D165 100%) 10;
    padding-right: 4rem;
  }
  .agenda > div:first-child, .columns > div:first-child {
    border-right: 3px solid pink;
    border-image: linear-gradient(to bottom, #FE7A73 0%, #EB7BC6 25%,#44ADD1 75%, #54D165 100%) 10;
  }

  .new-list{
    align-items: center;

  }

  .new-list h2{
    padding: 8px;
    border: 2px solid white;
    font-family: 'Roboto mono', sans-serif;
    text-decoration: normal;
    font-weight: normal;
    border-radius: 10px;
    font-size: 1em;    
    float: left;
    margin-right: 1rem;
    margin-left: 20px;
    width: 8em;
    text-align: center;
    border-radius: 35px;

  }

  .new-list ul{
    padding: 0;
    padding-top: 0px;
    padding-bottom: 0px;
    list-style: none;
    margin: 0;
    max-width: 60%;
    float: left;
    margin-right: 20px;
    padding-right: 20px;
  }


---
<!-- hide footer in marp -->
<!-- _footer: "" -->

# Actions Runner Controller Demo

![bg](./2023-GitHub-PresentationTemplate.png)


<!-- ![bg right](https://octodex.github.com/images/total-eclipse-of-the-octocat.jpg) -->

<div class="center-hubber">

![hubber gitstua](https://avatars.githubusercontent.com/gitstua?size=60) <span>@gitstua</span>
</div>

---
<!-- hide footer in marp -->
<!-- _footer: "" -->


<div class='agenda'>

  <div>

  # AGENDA
  </div>

  <div>

- What is ARC?
- ARC as part of Actions in the demo of the long text line running over
- Demo - deploying ARC
- Runner groups

  </div>

---

<div class='new-list'>

# Example of new-list div wrapping h1 h2 

## testing123
- world hello world hello world hello world hello world hello world hello world h- hello
- world

## H2
- a 
- d
- s


</div>

---

<div class='columns'>

  <div>

  # What is ARC?
  </div>

  <div>

  - the dog and the cat
  - b 
  - c
  - actions ghas runners repos and options
  - actions runner controller

  </div>

</div>

---

# ARC as part of Actions
<!-- <div class="gradient-pink-to-green-"></div>
<div class="gradient-pink-to-green-short"></div> -->

- a
- b
- c

---

# Demo - deploying ARC
<!-- 
- Open codespace
- show scaleset controller deployment
- show scaleset
 -->


---

# Runner groups

---

## Recap - Actions runners can be:

- Standard GitHub runners
- Larger GitHub hosted runners
- Running on a VM
- Running in Docker
- Running in Kubernetes

---

## Recap 2 - Actions Runner Controller
- A community project adopted under GitHub.com/actions/
- Elastic - a way to have runners which are created when jobs need them
- Run on your own hardware or in a cloud provider


## Resources
Some helpful resources are located at [gh.io/ARC-Resources](https://gh.io/ARC-Resources)
