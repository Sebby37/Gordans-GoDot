# GoDot Tutorial

## Creating a project
Click new project. I really didnt know what you were expecting.

## Adding stuff
To add assets and images, add them to a folder and put them in the same folder as that of your GoDot project, so they can communicate.

## Selecting a mode
At the top of the screen use the 2D and 3D buttons to change the scene to the appropriate view.

## Adding stuff, in the engine
To add a new sprite, simply create a new node by going to the plus button on the left side under scene. Then add the appropriate node, for a 2D body add a kinematic 2D body. To add collision add a collision body. To add a sprit, drag and drop it from your assets, then use the snap tool and select tool to mould it to your liking.

## Adding scripts
To add a new script, select the node you want to script to and press the new script button located at the edge of the scene tab.

## Creating an inheritable script
To add a inheritable script, create a new script:
```
extends "Node"
class_name "name of file to be inherrited"
```
And in your other file
```
extends "name of inherritable file"
```

## Basic Character Movement
(Using the inherritable script)
```
extends KinematicBody2D
class_name Actor

func _physics_process(delta): #is called once per frame
	var velocity: = Vector2(300, 0) #at 300 pixes per second (x,y)
	move_and_slide(velocity) #moving the character at

```

## Playing the game
To play the game, simply make sure your objects are inside the view mode (pressing G to disable the graph helps) and press F6. Pressing F3 flips you back to the script of the current selected node

## Advanced character movement

## Making a tileset
Create a new scene, named accordingly. Search for a node named "tileset." Then, on the right selected "create a tile set" and click on that once again to open up the editor. Then import a texture you want to use for the tiles. Then click new single tile, 