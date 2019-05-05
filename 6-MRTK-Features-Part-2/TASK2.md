# Create a scene loader

MRTK docs: [Button](https://github.com/Microsoft/MixedRealityToolkit-Unity/blob/mrtk_release/Documentation/README_Button.md)

Now that we have two different scenes with MRTK we can add a SceneLoader to our application so we can access both when building to the HoloLens. 

## ✏️ Create a new scene and parent components
Create a new scene in the scenes folder called `0_Menu`.

Add an empty GameObject called `Playspace`. Add an empty child component to `Playspace` called `SceneLoader`

## ✏️ Create a new script
Create a new script in the Scripts folder called `SceneLoader`. Open it in Visual Studio by double clicking on it.

In the 

Create a function that takes in the Scene-name as a parameter that we can use on buttons to load the scene we want. 

ℹ️ Check out the Unity documentation if you need a hint: [Unity docs](https://docs.unity3d.com/2018.3/Documentation/ScriptReference/SceneManagement.SceneManager.LoadScene.html).

When the script is done, add it to the `SceneLoader` GameObject. 

## ✏️ Two buttons
Add two buttons to `Playspace` and add the function you created to them to load one scene each. 

Change the button text to reflect which scene is loaded (The text can be changed on the label child object of the button). 

## ✏️ Edit build settings
Now that we can load different scenes we need the scenes to be a part of the build.

Go to **Files -> Builds settings** and add the new `0_Menu` scene. Drag the scene to the top of the list. The Scene on top is the first scene to be loaded. 

Make sure the two other scenes are checked. 

## ✏️ Build and deploy to the HoloLens emulator

Ask us if you want to try it out on the HoloLens. 

[Move along ▶](TASK3.md)️