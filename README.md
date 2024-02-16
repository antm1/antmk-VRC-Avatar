# antmk-VRC-Avatar
Avatar made from scratch to learn Blender. Welcome to use. 
Will hopefully rewrite this again some time to make it a lot cleaner and easier to understand but for now ChilloutVR instructions will hopefully be good enough for newer users to be able to figure things out. If not I would appreciate some input as to where people get lost so I can improve the readme. 

twobytworobotpallet is the image for texture. (Added OtherTextureSizes folder for different size textures to be easier to customize.)

Merged FBX is ready to import into unity. 

!!Important!! when importing the twobytwo texture make sure to change filter mode on the png in Unity to "Point (no filter)"
otherwise it will make the colors mix instead of being crisp pixels. 

For ChilloutVR:
1. Make sure you have imported the CCK (Content creation kit) https://documentation.abinteractive.net/cck/setup/
2. Drag and drop the avatar fbx file into the assets of your Unity project.
3. Do the same with twobytworobotpallet.png and set Filter Mode: Point (no filter) on the png
4. Make a new material and name it whatever you want.
5. Have the material selected then drag and drop the tworobotpallet.png into the Albedo section in the menu on the right hand of the screen.
That should be everything you need to do for the material but you are welcome to play with other settings for it if you'd like.
6. Now click on the avatar fbx file in the assets folder in the bottom middle area of the window.
7. The menu on the right hand side should change and near the top of that menu there are 4 tiles [Model] [Rig] [Animation] [Materials].
Click on [Rig], there should be an option that says "Animation Type" change that to Humanoid.
7.a. Optional: You can then click configure right under the "Avatar Definition" and that will take you to a menu where you can assign bones to different parts
(I usually switch the bones on the hands on each of the fingers to shift them down by one, and in the muscles section I set lower arm to not rotate to try to prevent the elbow socket from leaving its pins)
8. After you have set the Animation type to Humanoid hit apply
9. Drag your avatar FBX from the asset folder in the bottom middle of the window, to the grid or scene in the middle of your window.
10. Drag your material that you made with the texture and drop it on the avatar in the scene, it should now be colored.
11. Click on the avatar in the scene, in the right hand menu set transform position to 0 0 0 it should now be in the middle of the scene.
12. Also in the right hand menu, when you scroll down to the bottom there should be an [add component] button, click that and find "CVR Avatar" and add it.
13. That make a Voice Position and View Position move the View Position to around 1.65 Y and .1 Z and move the Voice Position to the mouth area.
14. ##WIP finish this part

For VRChat:
Make sure you have imported the 
(You will have to add VRC avatar descriptor,
would recommend to set camera height to 1.65.
Need to use autofix the couple problems in the vrc sdk control panel.
For quest compatibility you will need to make a VRC/Mobile/Standard-Lite material.)
~~!!Warning!! first time you sit down in a world you will be sent to the sky, each world. After first seat in world works fine.~~
(thanks to GhostRobot from Chillout VR for figurint out that my armature wasn't scaled properly on the export settings from blender to FBX)

Merged is model ready to be exported into FBX to import into Unity

Unmerged, parts of the body are seperate objects to be easy to change out only specific parts, all object origins should be at world origin
in order to Join objects.
!!WARNIGN!! normals will flip on some objects when you join them all together. 
-would recommend making normals visible
-click on a single face on each object with flipped normals and Ctrl + L to select all linked faces
-go to mesh -> normals -> flip normals
When exporting to FBX make sure to set the Transform settings to FBX All in the window that pops up after
you hit export to FBX in the [file] drop down menu.
