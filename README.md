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

Press on the Cube to select and in the Inspector we will 









 
