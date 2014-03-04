Grand Wizard
============

Authors:
* Grace Kihumba
* Maria Luisa Carrion
* Mustafa Tasdemir

The Game
========

Grand Wizard is a puzzle game that consists in creating a path to get to the end of a maze.

The story of the game is the following:

A dragon comes to attack the Wizard�s village every 100 years. The Wizard needs to create a magic potion to kill the dragon. 
He needs to collect all the ingredients needed for the potion by finding paths in a puzzle maze. If he gets the correct path, he obtains the magic potion ingredients and kills the dragon. However, he must avoid �spoofed� paths that lead him to monsters that will kill him.
	
Software
========
In order to open the project and run the demo, Game Salad v0.10.4.1 is needed.
Once you have Game Salad installed, open the Game.gsproj file.

Actors & Behaviors
==================
In order to create the first demo, we created the following actors in Game Salad:

1. Wizard: This is the actor that holds the image of the wizard. It has the "animate" behavior in order to update the wizard sprite as the player moves around. The position of this actor is constrained to the position of the Wizard Body actor.
2. Wizard Body: This actor is smaller than the wizard itself. This actor determines the portion of the wizard that collides with the terrain or walls. The main behavior of this actor is "move to", which makes it move to a certain location tapped by the user.
3. Circular Platform: This actor "rotates" when the wizard steps on it.
4. Square Platform: This actor moves to the right or left when the wizard steps on it.
5. Wall: walls are everywhere around the path to prevent the wizard from walking out of the path. Walls don't have a behavior. They just delimit the path that the wizard can take.
