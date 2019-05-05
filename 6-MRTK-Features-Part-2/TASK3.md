# Solver


## ✏️ Create a new scene and parent components
Create a new scene in the scenes folder called `4_Solver`.

Add an empty GameObject called `Playspace`.

## ✏️ Create a menu
Create a new empty GameObject called `Menu`.

Try to recreate this:   
![Menu](Screenshots/menu.jpg)

Some pointers: cube, Text mesh pro and a MRTK material.

## ✏️ Add a solver
When creating a menu like this, we can make it turn toward the user as the user moves around, and stay inside the viewport. 

To do this we first add the `Solver Handler`-script to the `Menu`-GameObject. 

Next we add the `Radial view`-script. 

Test it in `Play mode` and tweak the settings until you think it works as it should. 

## ✏️ Create a couple of prefabs

Find some 3D-models here: [https://poly.google.com/](https://poly.google.com/) and import them to the `Assets`-folder. 

️️️️️❗️ Remember that the HoloLens has limited processing power, so don't take the most advanced 3D models. 

Add the 3D-model to the Hierarchy, give it the `Manipulation handler`-script and scale it to a sensible size. Create a prefab of the 3D-model. 

## ✏️ Create a script
Create a new script called `Prefab`-spawner and create a script that takes in a GameObject (prefab) and spawns an instance of it.

## ✏️ Spawn the prefabs

Add buttons or 3D objects to the `Menu` that runs the spawn prefab function.

⭐️ Add different prefabs, spawn the prefabs in different locations, build an AppX and try it on the HoloLens (remember to change the Template 3D).

[Move along ▶](TASK.md)️