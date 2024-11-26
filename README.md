# Player-movement
Tutorial for the player movement
In this tutorial I will teach you how to move your player on X axis (left and right) with any type of input on the key.
This code is written in C# and it is suitable for both 2D and 3D game

## Prerequisites
Although this tutorial is beginner friendly, there are some prerequisites to complete this without getting confused mid way through
Firstly, you have to have these programmes installed and ready to use: 
- Unity
- Microsoft Visual Studio 2022

 This tutorial is made in Unity 2022.3.46f1 and Microsoft Visual Studio 2022, so I would suggest using the same  to avoid any confusion

 If there is any assistance needed on downloading these programs, visit this site:
 link

 Also, if you are not completely sure how to navigate in Unity, follow this tutorial as an introduction or a reminder:
 link

 ## Objective
 The objective of this tutorial is to make an object, add the needed components, write the script and attach it to the object.

 ## Setting the project

 - Open Unity
 - Select a project (whether you want it to be 2D or 3D)
 - Name it
 - 
 ## Setting the scene

 Firstly we have our Unity Project open. I have chosen a 3D project, so the scene will be in 3D as well as the player. I have named my project TutorialPlayer Movement,but feel free to name it by your liking.
 After followoing these steps, this is what it should look like
 
 ![Opening_Unity (1)](https://github.com/user-attachments/assets/f69e46e2-e52b-43b6-ad16-f19f85cff36b)

 Great! So now we have our 3D project open and we can see all the information we have that will be useful for us. 
 On the left hand top corner you can see the name of the project, as well as the version of Unity I have used.
 Then we have a sample scene which will contain everything that is used in our scene. However we can always add and remove stuff from it. So far we have a Main camera and Directional Light
 Then we can see that we are in scene mode, which enables us to edit the scene and move through the scene when the game is not running. Game mode can be accessed when pressing the Game mode button with the joystick icon and pressing the play button.
 
![Game_mode](https://github.com/user-attachments/assets/02465de9-7935-4f34-8486-f18bde105f40)

Ofcfourse, now when we press play, nothing will happen since the scene is empty and we have no scripts running. But we still hace the Diredtional Light working and are only able to see from the main camera point of view (whereas in the Scene mode, we can move our viewpoint).
Once we cleared this out, return back to the scene and let's add the player!

## Adding the player

We can go to hierarchy and right click in the gray area.
Then a context menu will pop up which contains many objects that are useful for the game.

![Creating a 3D object](https://github.com/user-attachments/assets/717af635-10b9-4cbd-bbf6-4dfc1ef2116e)

For example, use Create Empty (an empty object) can be used as a folder when making a game to organise a scene, to manage scripts in the scene or simply an invisible area that (with the help of code) will be able to recongnise a trigger and do something in the game. Shortly said, it is quite an adaptable object. Besides that, we have Effects, Light, Audio, UI... (which are all useful in making a game)
But for now, we want to create a 3D object! When we drag over a 3D object, a sub menu will open which will show us a list of list of object we would like to add to the scene. It does not really matter which one would you like to use, since it will not affect the code, but I will be using a cube. 



## Coding the player

This will be a simple code for moving the player left and right using A and D keys.
This script is not only going to move our player but also the computer as well. 

There are a few ways to add a script and assign it to a object. One way is to go to the assets (scripts), right click to Create and press on C# script. Afterwards drag it to the object you want to assign to in this case to both of the cubes.
The other way is to select the object, go to the inspector and add a component (new script). Either way, make sure to change the name of the scripts immediatelly because if you wish to alter it afterwards, you will also need to rename it in the Visual Studio. I will name the script Player , since we want to code 
Having made the script and assigned it to both cubes, open the script in Microsoft Visual Studio by pressing the script.

When we open a script, this is what is shown in the editor.

![basic editor view](https://github.com/user-attachments/assets/b05163fe-4e1b-4bab-b238-d769c5cc7303)
Since our code is simple, we will not need these two lines. How do we know that? When we see the lines are not showing their bold colour (the opacity is lower than the rest of the lines in the script), and if we hower with the mouse a yellow light will pop up saying that it is not neccessary for the script.

![Deleting unneccesary bs](https://github.com/user-attachments/assets/f32d982d-513f-4440-a9a0-a6f29b2417df)

![Screenshot (2)](https://github.com/user-attachments/assets/78ca6014-de3c-4310-84b1-97689f016318)

This is what will be shown, when the line is not needed for the code to run











 

