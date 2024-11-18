# Player-movement
Tutorial for the player movement in my game
In this tutorial I will teach you how to move your player on X axis (left and right) in a 3D Pong game. It is beginner friendly, so anyone who is new to coding is welcome to try it out

## Prerequisites
Although this tutorial is easy to understand, there are some prerequisites to complete this without getting confused mid way through. 
Firstly, you have to have these programmes installed and ready to use: 
- Unity
- Microsoft Visual Studio 2022

 This tutorial is made in Unity 2022.3.46f1 and Microsoft Visual Studio 2022, so I would suggest using the same  to avoid any confusion

 If there is any assistance needed on downloading these programs, visit this site:
 link

 Also, if you are not completely sure how to navigate in Unity, follow this tutorial as an introduction or a reminder:
 link

 ## Objective
 The objective of this tutorial is to set the scene (add the players, ball, platform and the walls), add rigid body, physics, trigger and components to the objects as well as the Player C# script

 ## Setting the project

 ## Setting up the scene
 This is how I would like the scene to look before adding any code
 ![setting_up_the_scene](https://github.com/user-attachments/assets/422b71d4-5c47-4094-8781-3327f1ea89ff)

 In this scene, we have 4 cubes (2 players and 2 walls), 1 sphere (ball) and 1 plane (platform where everything is going to be on)
After adjusting the objects, create an empty object and group them

![Empty_object](https://github.com/user-attachments/assets/fea401d3-4cc0-46dd-9264-cc55dffe99d3)

As you can see in the picture, I named it Pong, but it is really up to your preference
![naming_the_object](https://github.com/user-attachments/assets/c88cf460-8c7e-474b-a4d9-02ce3b08d460)

In order for our project to be clear and organised, I suggest putting all the assets that we have made to the project in the assets area so it is easier to select them
I will just the player and the ball since those are the only objects I will code for now

![Assets](https://github.com/user-attachments/assets/4668723e-9ca8-48ea-b36b-e3f657b00b13)

Then we will select the cube and in the Inspector we will add a box collider which will later enable the cube to detect the ball when it hits it. 

![Box_collider](https://github.com/user-attachments/assets/febc4cad-7f94-4262-96c0-1be3dcf2b5be)


For the sphere, we will add a sphere collider and rigid body.

![sphere_collider](https://github.com/user-attachments/assets/2e68f8a8-c8da-4015-b8ae-8539fef0cda6)


Keep and eye out for the 2D options for colliders and rigid body. It is easy to accidentally pick them, so be careful! We want to implement 3D physics in the game, not 2D!

![Screenshot_(1)](https://github.com/user-attachments/assets/5bef8b5b-7f0a-43e3-889d-50d676877d27)


Perfect, now that we have set the scene, it is time to do some coding for the player!

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









 

