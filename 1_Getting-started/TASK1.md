# 1 - Getting started

:pencil2:  Open Unity, enter a name and a location for your new project. Make sure 3D is selected as template and click **Create project**.

![Unity setup](Screenshots/unity_setup.png)

If you are using the default Unity layout it would look something like this: 
![Unity layout](Screenshots/unity_overview_default.png)
Note the panel names. They will be used throughout the tasks. 

Go to **Assets -> Import package -> Custom package** in the toolbar. Import the Microsoft.MixedReality.Tookit.Unity.Foundation-v2.0.0-Beta2.unitypackage downloaded from https://github.com/Microsoft/MixedRealityToolkit-Unity/releases/tag/v2.0.0-RC1.

Make sure all assets are checked and click **Import**.

Click **Apply** when you are prompted. 

When the assets are done loading go to **File -> Build settings**, double click on Universal Windows Platform and click on Switch platform. 

The Mixed Reality Toolkit assets will give you a new option in the toolbar. Go to **Mixed Reality Toolkit -> Configure**. 

New entities will appear in your Hierarchy view: 

![Hierarchy](Screenshots/hierarchy1.jpg)

:information_source: The **Directional Light** is not needed for the HoloLens as it does not use lights. But you can keep it there if you want to. The **MixedRealityToolkit** is the configurations. The **MixedRealityPlayspace** contains the camera configurations, event system and Gaze provider.

Save the new Scene by going to **File -> Save scene as**. Give it a name and save it in the scenes folder. 

Click on the **MixedRealityToolkit** in the Hierarchy. The toolkit options will appear in the Inspector. Click on **Copy & customize**.

*Experience settings:*  
We’ll set this to world as we can take advantage of the spatial mapping capabilities of the HoloLens.

*Camera settings:*  
Double click on the DefaultMixedRealityCamera. You can check the Is Camera Persist if you want the camera to stay the same across scenes. 

As you can see the Opaque Display Settings is set to Skybox and Ultra quality. This setting is for VR headsets.

The Transparent display settings is set to solid color and black, that way the background will be transparent in the HoloLens. As for quality the hardware in the HoloLens limits the graphics settings so keep it on Very low.

As the HoloLens has a transparent display, we don’t have to worry about the *Boundary System settings* so leave that unchecked. 

The same goes for the *Teleport System Settings*. 

The *Spatial Awareness System Settings* enables the spatial mapping on the HoloLens which allows us to interact with the real world in our application. Check this box. 

*Diagnostics* might be useful when testing our application, so leave that checked. 

Next we need take care of some of the project settings in Unity. Go to **File -> Build settings** and click **Add open scenes**. This will make sure our scene is included when we build the application later. 

A couple of settings in the Unity settings is also needed. Go to **Edit -> Project settings -> Player**. 

Under **Publishing** settings change the package name. This is the unique name for your application that the HoloLens uses. If you don’t change it and load two different applications they will overwrite each other. 

![Publish settings](Screenshots/publish_settings.jpg)

Next we need to make sure that the Virtual Reality supported checkbox is checked under **XR Settings**. This makes the application run as a VR application in the HoloLens. 

![XR settings](Screenshots/xr_settings.jpg)

That's it for the project settings, we are ready to create an application: 

[Task 2 - Creating an application](TASK2.md) :arrow_forward:

