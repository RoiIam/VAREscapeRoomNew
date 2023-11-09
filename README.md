# VAR Escape room modified to run on Unity 2022.3.9f(or newer than 2020) with newest XRIToolkit
- It's a complete project, clone and add it to the Unity hub

## Modifications:
- deleted MasterController.cs , AlignmentTrigger.cs and WitchHouseHook.cs they were causing problems
- they are saved in VrBeginner/deletedBackup.zip
- MasterController.cs , AlignmentTrigger.cs (in backup.zip) are modified to use XR Origin
- correct teleport
- added XRIToolkit samples + XR Device Simulator
- uses OpenXR as a backend

## More notes:
- uses newest(2.5.0)XRI Toolkit, so it has new XR Origin instead of deprecated XR Rig
- uses URP rendering pipeline
- there is a prefab called XR device simulator(KB+mouse to simulate device, keybinds show on screen)- remove it when a real HMD is pluged in



### extra:
here is *probably incomplete* setup, how I upgraded it to work on newer versions
1. import starter assets (Window-Package Manager- XR Interaction Toolkit-Samples) ,
2.  now replace old XRRig game object in the scene with the one provided in Starter Assets-Prefabs folder called XR Origin (XR Rig).prefab 
3.  delete MasterController.cs script, AlignmentTrigger.cs and WitchHouseHook.cs 
4. those scripts just did some setup work.
5. you need to as weel add Locomotion references and XR Interaction Setups Input Action Manager
6. change right/left Teleport Interactor's Raycast Mask to Teleporter only to be able to teleport with right joystick
7. optionally disable haptics at ray, direct and teleport interactors-annoying


