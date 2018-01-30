---
project: ue
type: info
title: 'Component System'
contributors: lovberg
categories: 
    - ue
    - lovberg
---

### Components

To be able to experiment with different perspectives the camera component is heavy customizable. The ability to switch between different perspectives made it possible to try the game in different ways and explore the different experiences the designer could create.

<br>

![Image of Camera Component in 3rd Person](/img/3rdperspective.png) | ![Image of 3rd Person Perspective](/img/3rdpsettings.png)
![Image of Camera Component in 1st Person](/img/1stperspective.png) | ![Image of 1st Person Perspective](/img/1stpsettings.png)

<br>

### Building a Prefab

This is a player character. It had several components to make it work.

* Player input (takes care of where to send the input from the controller)
* Animate (sends animation information to the animator component)
* Field of View (draws a mesh to show what the character sees)
* Health (a component with a counter to keep track of health points)
* Mover (the components that makes the character move)
* Rotator (used to rotate the character)
* Respawnable (teleports the character to last checkpoint upon trigger)
* SwapWeapon (trigger a chain of components to swap out the weapon prefab and bind the input mapper to the new weapon)
* Taggable (tagging system to be able to check what kind of game object this is)

All of these components can be used to create different kind of mechanics in a game. The idea is to make the designer free to try new ideas without having to ask a programmer for new components with a single use and also gives the designer the creative freedom he / she needs.


![Image of Player Character in Undead End](/img/compplayer.png)