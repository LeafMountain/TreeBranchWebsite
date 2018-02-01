---
project: ue
type: info
title: 'Component System'
contributors: lovberg
categories: 
    - ue
    - lovberg
---

## Building a Prefab

### Components

PlayerInput | Takes care of where to send the input from the controller | 
Animate | Sends information to the animator component | 
FieldOfView | Draws a mesh to show an area | 
Counter | A component to keep track of an integer | 
Mover | The components that makes the object move | 
Rotator | Used to rotate the object | 
Respawnable | Teleports the object to last checkpoint upon trigger | 
Taggable | Tagging system to be able to check what kind of object this is | 
Instantiator | Creates a new object | 
AIController | The AI logic | 

<br>


<table>
    <tr>
        <td>
            <h3> Player Prefab </h3> <br>
        
            <ul>
                <li>Taggable (to tag the character as a player controlled unit)</li>
                <li>PlayerInput (to move the character)</li>
                <li>Counter (to keep track of health points)</li>
                <li>FieldOfView (show the area the player can see)</li>
                <li>Mover (to be able to move the character)</li>
                <li>Respawnable (teleports the player to the last checkpoint upon death)</li>
            </ul>
        </td>
        <td>
            <img src="/img/ue/componentplayer.png" alt="Player" height="300">
        </td>
    </tr>
</table>



<br>

<table>
    <tr>
        <td>
            <h3> Enemy Prefab </h3> <br>

            <ul>
                <li>Taggable (to tag the character as a AI controlled unit)</li>
                <li>AIController</li>
                <li>Counter (to keep track of health points)</li>
                <li>FieldOfView (the area the enemy can see)</li>
                <li>Mover (to let the AIController move the unit)</li>
                <li>Instantiator (splatter gore when hit)</li>
            </ul>
        </td>
        <td>
            <img src="/img/ue/componentzombie.png" alt="Zombie" height="300">
        </td>
    </tr>
</table>

<br>

<table>
    <tr>
        <td>
            <h3> Gun Prefab </h3> <br>

            <ul>
                <li>PlayerInput (to fire the weapon or reload)</li>
                <li>Counter (to keep track of ammo)</li>
                <li>Animate (to animate the model)</li>
                <li>Instantiator (to create bullets)</li>
            </ul>
        </td>
        <td>
            <img src="/img/ue/componentgun.png" alt="gun" height="300">
        </td>
    </tr>
</table>

<br>


All of these components can be used to create different kinds of mechanics in a game. The idea is to make the designer free to try new ideas without having to ask a programmer for new scripts with and also gives the designer the creative freedom he / she needs.
