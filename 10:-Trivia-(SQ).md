## Quick Links
:floppy_disk: [Trivia Game Download](https://github.com/cs210/2022-Meta2/tree/main/Trivia%20Gameshow%20VR)

:film_strip: [Trivia Game Recording](https://drive.google.com/file/d/1CklpJGEGu0gneaio9GR7O-2t53I9Wiai/view?usp=sharing)

# Introduction
In brainstorming different drivers for the exploration of GHA, we arrived on the idea of Trivia. Informed by talks with Jay Borenstein and Adam Tobin, a producer for one of the most popular game shows in America, the idea of Trivia compelled us as a technique to gamify exploration and unintentional learning. At the end of the first quarter, these efforts culminated in a low-fi version integrated within our Mesa Verde Figma Prototype [Link Here].


However, moving towards the second quarter, we wanted to further explore Trivia through a playable Unity prototype. In creating this prototype, we took a step in our journey to answer these questions:
* How can we create a Trivia experience that utilizes the capabilities of virtual reality?
* What does a trivia experience unique to each site look like?
* To what extent can Trivia motivate exploration through GHA?

The following wiki page will guide you through the process we took to answer the preceding questions.

## Creating a VR Trivia Experience
At the end of the winter quarter, our initial trivia prototype in Figma was designed as an overlay within the user's HUD. Moving forward, we wanted to explore what interactions engaged the user in a form that utilized the potential of virtual reality. The following section addresses how these design decisions were informed.

### :star_struck: Core Component 1: Become the Star of the Show
Drawing inspiration from popular television game shows, we wanted to provide a chance for the user to be the star of their own game show.  The first component engages the user by teleporting them into a platform that then raises into the stage. The setting is revealed to them as they enter the stage. In front of them are bright lights, pyro, and smoke. To their left and right are their competitors.

### :red_circle: Core Component 2: Quiz Buzzer
Based on popular quiz and game show mechanics that utilize buzzers, we wanted to allow users to have that same mechanic when completing the trivia. Rather than just a single button, we opted to have four buttons color-coded to an answer option. This introduces a more dynamic way of answering questions and is paired with haptic feedback and a sound effect when pressed. Looking forward, the trivia game show could allow a variety of interactive mechanisms that are based on question-type such as prompting the user to draw something.
![Correct](https://user-images.githubusercontent.com/53293116/172774033-54d3a288-45a4-4366-8c4d-29829f9efd5d.png)


### :studio_microphone: Core Component 3: Host of the Show
In every game show, there is a host that guides the participants. To emulate this, we used an artificial intelligence text-to-speech generator that read out the question and answers, as well as provided introductory/conclusive remarks. This component offers additional accessibility support and contributes to the social atmosphere of the game. An additional component could be integration with the Meta Avatars SDK to add an animated host with a voice actor.

### :trophy: Core Component 4: Reward and Stakes
To implement a scoring system, we chose to represent the score as the number of questions answered correctly. In previous iterations, we had tested the possibility of using a time-multiplier score but ultimately strayed away from this option as it encouraged rapid execution of the quiz as opposed to the exploration of the site. In addition to the scoring system, we prototyped a passport system. After completing the gameshow, the user would receive a passport stamp based on the number of questions guessed correctly. This stamp would be placed within their passport on the specified site page and ranges from bronze, silver, gold, and historian.
![Frame 1](https://user-images.githubusercontent.com/53293116/172777744-fa76f93f-4f23-4642-aa1d-3a1cd8ecb6d9.png)

![Trivia Updated Passport](https://user-images.githubusercontent.com/53293116/172777991-7d8685e3-ae3a-43c0-886a-7590da3cd6bb.png)

### 🆚 Core Component 5: Compete Against Friends and Family
Every game show isn't complete without a collaborative aspect. To prototype this, we set up three additional player podiums for a multiplayer experience. After or before exploring a site, users can enter the trivia game show and compete to see who knows the most.

![Screenshot (114)](https://user-images.githubusercontent.com/53293116/172611006-955161df-22d8-4d08-ae9e-fed7ea055b1d.png)

## Set Design and Scalability
### Considerations
The set of the game show is designed around Mesa Verde within the current prototype. This choice to select the site was informed by the idea of having a game show environment that holds similar aesthetic qualities as the site; however, it must be noted that, in practice, subject matter experts and ethical considerations should be consulted before choosing or creating a site. 

### Scalability

![Screenshot (115)](https://user-images.githubusercontent.com/53293116/172611028-9d8d6cb6-bc0c-4042-aac8-fada6b249396.png)
[Screenshot of Quiz Show Layout]
[Screenshot of Quiz Show 1]
[Screenshot of Quiz Show 2]

## Trivia and GHA Exploration
To test the potential of this trivia experience to motivate GHA exploration, we integrated it with our previous prototype. Conducting A/B tests, we presented the prototype of Mesa Verde either with or without the option to conduct the trivia. While the users tested, we took metrics such as:
* Number of POI's Explored
* Session Time
* User Flow (Do they return to Mesa Verde, Replay, or Explore a New Site)

The following table summarizes our quantitative findings:

After their experience, we then conducted a survey to gauge the user's motivation for engaging with trivia as well as ...

[Research Results and Findings]

