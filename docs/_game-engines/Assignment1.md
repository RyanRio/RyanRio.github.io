---
project_name: Project1 - Breakout
---

# My first game engines project!

Quick note before we get into things: Click [here](/game-engines-docs/Assignment1_Docs/index.html) to access the docs (I suggest opening a new tab)

## Compiling

The docs go into specific details about the project, but I'll quickly note that to compile simply run `python3 build.py`

 - Download the [binary][1]

[1]:{{ site.url }}/download/breakout

## Post Mortem

If I had more time there is really only one direction I would want to take the project. As we discussed in class, the line between a game engine and a game blurs, and in my opinion the blur happens depending on where the game is coupled to the engine. In my engine, resources are handled independently to the concept of a "breakout" game however things like GameObject are about 80/20 in terms of how independent they are. I was going in the direction of making GameObject's an abstraction the engine provides, however I ended up only utilizing that abstraction halfheartedly, creating classes to represent the ball and brick yet still coding some functionaltiy for them into the engine classes.

If I could achieve this separation, then I would want to look into tooling. For instance, I am pretty happy with how the LevelManager turned out, but it would be nice to be able to add bricks to a screen and then save that layout. This idea is essentially just "placing textures on a screen" which the engine should be able to handle. I am excited to get into tooling like this and look forward to implementing some in my upcoming platformer.

The Localization engine was a very interesting challenge. There were hundreds of posts online about how to get unicode working, but almost none of them worked for me. I ended up throwing together a bunch of different ideas and sifting through documentation, and the program functions as expected but now for instance printing to the terminal does not work. I am happy it works with the sdl_ttf library though. Tangentially, it would be nice to be able to instantiate all types of resources on the fly, in order to build a level.

## Other Deliverables

#### Demo Video:

<video width="960" height="540" controls>
  <source src="/assets/vid/breakout_demo.mov" type="video/mp4">
Your browser does not support the video tag.
</video>

#### Game Screenshots:

<img src="/assets/images/breakout_photo1.png">
<img src="/assets/images/breakout_photo2.png">
<img src="/assets/images/breakout_photo3.png">
