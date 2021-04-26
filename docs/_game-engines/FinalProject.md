---
project_name: Particle Game Maker
---

# A Game Engine that uses the PongChamp Scripting Language to enable the creation of your own particle game!

Click [here](/game-engines-docs/FinalProject_Docs/index.html) to access the documentation. I suggest opening in a new tab.

## Compiling

The documentation linked above covers specifics on the project, but to compile simply run `make all`

 - Download the binaries: [PongChamp][1], [C++ program][2]

[1]:{{ site.url }}/download/PongChamp
[2]:{{ site.url }}/download/run_cpp_test

## Post Mortem

Many hours of work went into designing and implementing new systems for our game engine. In particular, we used a recursive quad-tree to sort our particles into small areas and make checking for collisions between particles much more efficient. A major challenge we faced when implementing this system was figuring out when to move particles between tree nodes, and perform other tree operations, in relation to when we executed particle behaviour. A particle could disappear from the tree before another particle needed to operate on the now missing particle, and so we needed to wait to execute tree operations until after all particle behaviour had been executed. Much effort also went into getting the tree to both grow and shrink when necessary.

If we had more time to work on this engine, adding more features would be our focus. For example, we could develop a graphical editor for the layout of the particle buttons. This could include the ability to drag buttons to their locations, edit their labels, and more. Aside from this, we could also add more options for the customization of particle behaviours. The current configuration options provide lots of variety, but are still more of a demo of the engine. Adding more of these behaviour customizations, as well as making them more configurable by the user, can make our engine much more powerful. In general, the focus of most future improvements could go towards making the game more customizable by the player, allowing for a greater diversity of particle simulation games to be made.

Another interesting direction we could pursue is to combine this engine with one of the GameObject based engines we already implemented. It could be interesting to develop a game where a player navigates through a world of simulated particles.


## Other Deliverables

#### Demo Video:

<video width="960" height="540" controls>
  <source src="/assets/vid/particle_engine.mov" type="video/mp4">
Your browser does not support the video tag.
</video>

