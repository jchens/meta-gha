## Quick Links
:floppy_disk: [Trivia Game Download](https://github.com/cs210/2022-Meta2/tree/main/Trivia%20Gameshow%20VR)

:film_strip: [Trivia Game Recording](https://drive.google.com/file/d/1CklpJGEGu0gneaio9GR7O-2t53I9Wiai/view?usp=sharing)

# Introduction
In brainstorming different drivers for the exploration of GHA, we arrived on the idea of Trivia. Informed by talks with Jay Borenstein, Hassan Karaouni, Adam Tobin, a producer for one of the most popular game shows in America, the idea of Trivia compelled us as a technique to gamify exploration and unintentional learning. At the end of the first quarter, these efforts culminated in a low-fi version integrated within our Mesa Verde Figma Prototype.


However, moving towards the second quarter, we wanted to further explore Trivia through a playable Unity prototype. In creating this prototype, we took a step in our journey to answer these questions:
* To what extent can Trivia motivate exploration through GHA?
* How can we create a Trivia experience that utilizes the capabilities of virtual reality?
* What does a trivia experience unique to each site look like?

The following wiki page will guide you through the process we took to answer the preceding questions.

# Trivia's Role in GHA Exploration
To test the potential of this trivia experience to motivate GHA exploration, we integrated it with our previous prototype. Conducting A/B tests, we presented the prototype of Mesa Verde either with or without the option to conduct the trivia. While the users tested, we took metrics such as:
* Number of POI's Explored
* Session Time
* User Flow (Pictured Below)
<img width="500" alt="User Flow Sadfa App (Community)" src="https://user-images.githubusercontent.com/53293116/172793409-51be0a1f-c651-46dc-ae3c-aa390d5a3171.png">

## Testing Results
The following table summarizes our findings:

### Findings

![Screenshot (137)](https://user-images.githubusercontent.com/53293116/172813533-36cf6f6d-aba6-45a5-aaab-957ac5d28049.png)

Given these results are pulled from a small sample size, some key findings are:
* Session time increase w/ trivia
* POI exploration count increase w/ trivia
* Users tend to return to the site when disappointed by their score, but explore a new site when satisfied

### Why Trivia?
After their experience, we then conducted a survey to gauge the user's motivation for engaging with trivia.
Notable quotes included:
> “I’ve always wanted to be on a game show, so this experience made that possible AND let me travel somewhere I’ve never been before.”

>“When I visit a place, I love to learn new things about it such as the culture, architecture, and history. Being able to play against my friends only makes it more exciting.”

>“I journal and scrapbook! Being able to collect these travel stamps/trophies reminds me a lot of the joy I get from doing that.”

Through reviewing user quotes and data, we holistically came to the conclusion that users decided to participate in trivia to **(1) preview a site, (2) test their knowledge and compete against others, and (3) gain a sense of accomplishment.**

# Creating a VR Trivia Experience
At the end of the winter quarter, our initial trivia prototype in Figma was designed as an overlay within the user's HUD. Moving forward, we wanted to explore what interactions engaged the user in a form that utilized the potential of virtual reality. The following section addresses how these design decisions were informed.

## :star_struck: Core Component 1: Become the Star of the Show
Drawing inspiration from popular television game shows, we wanted to provide a chance for the user to be the star of their own game show.  The first component engages the user by teleporting them into a platform that then raises into the stage. The setting is revealed to them as they enter the stage. In front of them are bright lights, pyro, and smoke. To their left and right are their competitors.

![Screenshot (138)](https://user-images.githubusercontent.com/53293116/172818034-2089eb2d-4933-4eff-b263-48c11b57aead.png)

![Screenshot (139)](https://user-images.githubusercontent.com/53293116/172818054-e7338e8d-758b-48a1-9590-691b41b15b9d.png)

![Screenshot (122)](https://user-images.githubusercontent.com/53293116/172818081-3b6c04f4-e28b-45a6-bead-58b3577db3e7.png)

## :red_circle: Core Component 2: Quiz Buzzer
Based on popular quiz and game show mechanics that utilize buzzers, we wanted to allow users to have that same mechanic when completing the trivia. Rather than just a single button, we opted to have four buttons color-coded to an answer option. This introduces a more dynamic way of answering questions and is paired with haptic feedback and a sound effect when pressed. Looking forward, the trivia game show could allow a variety of interactive mechanisms that are based on question-type such as prompting the user to draw something.
![Correct](https://user-images.githubusercontent.com/53293116/172774033-54d3a288-45a4-4366-8c4d-29829f9efd5d.png)


## :studio_microphone: Core Component 3: Host of the Show
In every game show, there is a host that guides the participants. To emulate this, we used an artificial intelligence text-to-speech generator that read out the question and answers, as well as provided introductory/conclusive remarks. This component offers additional accessibility support and contributes to the social atmosphere of the game. An additional component could be integration with the Meta Avatars SDK to add an animated host with a voice actor.

## :trophy: Core Component 4: Reward and Stakes
To implement a scoring system, we chose to represent the score as the number of questions answered correctly. In previous iterations, we had tested the possibility of using a time-multiplier score but ultimately strayed away from this option as it encouraged rapid execution of the quiz as opposed to the exploration of the site. In addition to the scoring system, we prototyped a passport system. After completing the gameshow, the user would receive a passport stamp based on the number of questions guessed correctly. This stamp would be placed within their passport on the specified site page and ranges from bronze, silver, gold, and historian.
![Frame 1](https://user-images.githubusercontent.com/53293116/172777744-fa76f93f-4f23-4642-aa1d-3a1cd8ecb6d9.png)

![Trivia Updated Passport](https://user-images.githubusercontent.com/53293116/172777991-7d8685e3-ae3a-43c0-886a-7590da3cd6bb.png)

## 🆚 Core Component 5: Compete Against Friends and Family
Every game show isn't complete without a collaborative aspect. To prototype this, we set up three additional player podiums for a multiplayer experience. After or before exploring a site, users can enter the trivia game show and compete to put their knowledge to the test. By providing a structured experience for friends to collaborate, the trivia is able to promote social engagement.

![Screenshot (114)](https://user-images.githubusercontent.com/53293116/172611006-955161df-22d8-4d08-ae9e-fed7ea055b1d.png)

# Set Design and Scalability
## Considerations
The set of the game show is designed around Mesa Verde within the current prototype. This choice to select the site was informed by the idea of having a game show environment that holds similar aesthetic qualities as the site; however, it must be noted that, in practice, subject matter experts and ethical considerations should be consulted before choosing or creating a site. 

![Screenshot (115)](https://user-images.githubusercontent.com/53293116/172611028-9d8d6cb6-bc0c-4042-aac8-fada6b249396.png)

## Scalability
To account for scalability to other sites, we decided to standardize the game components used within a trivia set. Provided below is a general layout, as well as a chart for component selection. The site-specific components can be developed independently from Unity and allow for subject-matter experts to be consulted.

![Frame 2](https://user-images.githubusercontent.com/53293116/172787198-1aa3fbdf-5428-4f1b-b5ef-5cc09b955eb3.png) 

![Screenshot (133)](https://user-images.githubusercontent.com/53293116/172789550-ea13dc0e-d9e5-475e-82c6-47c96e885096.png)




# Ideation and Prior Versions
The following figures and screenshots depict initial mood boards, user journeys, and prototypes generated throughout the development process.
## Trivia Gameshow Mood Board
![Inspiration board](https://user-images.githubusercontent.com/53293116/172802759-3671aa8d-ae8f-4097-95a7-d5c23a1975cf.png)

## Preliminary User Journey
![Screenshot (134)](https://user-images.githubusercontent.com/53293116/172813160-82e023c3-2a75-4329-812c-fc6e8a17af12.png)

## First Prototypes
![Frame 3](https://user-images.githubusercontent.com/53293116/172812740-21d48c09-7b97-4537-9cf1-f0cce9308d54.png)


