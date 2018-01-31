---
project: tgf
type: info
title: 'Gameplay Programming'
categories: 
    - tgf
    - lovberg
---

### Ease of Use

<br>

To let designers do their job I had to make simple prefabs and components to reduce complexity and development time. The main goal was to have one prefab to control the combat, UI and everything else a battle required.

<br>

I solved this by making a prefab that contained all the main components of a battle and creating a component made for the game board detection.

<br>

The world detection added the board cells to an array and added a status depending on if the cell was blocked or not. This was used by the pathfinding.

<br>

To make it easy to create new and unique characters for the game a "Character Sheet" data container was created. This contained properties like name, stats and equipment. | ![Image of Character Sheet](/img/placeholder.gif)
