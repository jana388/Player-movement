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
 ## Making the player

 Firstly we have our Unity Project open. I have chosen a 3D project, so the scene will be in 3D as well as the player. I have named my project TutorialPlayer Movement,but feel free to name it by your liking.
 After followoing these steps, this is what it should look like
 
 ![Opening_Unity](https://github.com/user-attachments/assets/5913fa76-6129-4fe2-acf3-f0772ea6e09c)






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











 

