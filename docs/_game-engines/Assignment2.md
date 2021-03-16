---
project_name: Assignment 2 - Platformer
---

# Our first platformer using SDL: Spooky Epic Platformer Hour

Click [here](/game-engines-docs/Assignment2_Docs/index.html) to access the documentation. I suggest opening in a new tab.

## Compiling

The documentation linked above covers specifics on the project, but to compile simply run `make all`

 - Download the [binary][1]

[1]:{{ site.url }}/download/platformer

## Post Mortem

Given more time to refine our game and engine, there are a number of design changes we would have implemented. First of all, we would have added functionality to allow game objects to easily find each other during gameplay. This change would have improved our game's efficiency as well as simplified some of the more abstracted aspects of our engine. Given more time, our implemented component abstraction could have been used to greater lengths than we accomplished.  For example: we would have used inheritance such that we could create custom GameObjects, and more unique game mechanics and levels. Our current model does allow for creating complex connected systems, but we did not have the time to implement it in our game.

Once the prior were achieved, we would go into optimizing our tilemap editor. Currently, it is functional, but in no means is it convenient. Working through the tilemap editor requires much unwanted clicking to get accross from tile to tile and to cycle back if you accidentally skipped past a tile you wanted to use. It is not very flexible, and feels very cluncky to use. With further polishing, this editor would be a very comfortable and convenient tool to use for building game levels.


## Other Deliverables

#### Demo Video:

<video width="960" height="540" controls>
  <source src="/assets/vid/platformer_demo.mov" type="video/mp4">
Your browser does not support the video tag.
</video>

#### Game Screenshots:

<img src="/assets/images/platformer/play.png">
<img src="/assets/images/platformer/freeze.png">
<img src="/assets/images/platformer/loss.png">
<img src="/assets/images/platformer/victory.png">

