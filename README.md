# Player-movement
Tutorial for the player movement
In this tutorial I will teach you how to move your player on X axis (left and right) with any type of input on the key.
This code is written in C# and it is suitable for a 3D game

## Prerequisites
Although this tutorial is beginner friendly, there are some prerequisites to complete this without getting confused mid way through.
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
   
 ## Setting the scene

 Firstly we have our Unity Project open. I have chosen a **3D project**, so the scene will be in 3D as well as the player. I have named my project TutorialPlayer Movement,but feel free to name it by your liking.
 After followoing these steps, this is what it should look like
 
 ![Opening_Unity (1)](https://github.com/user-attachments/assets/f69e46e2-e52b-43b6-ad16-f19f85cff36b)

 Great! So now we have our 3D project open and we can see all the information we have that will be useful for us. 
 On the left hand top corner you can see the name of the project, as well as the version of Unity I have used.
 Then we have a sample scene which will contain everything that is used in our scene. However we can always add and remove stuff from it. So far we have a Main camera and Directional Light
 Then we can see that we are in scene mode, which enables us to edit the scene and move through the scene when the game is not running. Game mode can be accessed when pressing the Game mode button with the joystick icon and pressing the play button.
 
![Game_mode](https://github.com/user-attachments/assets/02465de9-7935-4f34-8486-f18bde105f40)

Ofcourse, now when we press play, nothing will happen since the scene is empty and we have no scripts running. But we still hace the Diredtional Light working and are only able to see from the main camera point of view (whereas in the Scene mode, we can move our viewpoint).
Once we cleared this out, return back to the scene and let's add the player!

## Adding the player

We can go to **Hierarchy** and right click in the gray area.
Then a context menu will pop up which contains many objects that are useful for the game.

![Creating_a_3D_object](https://github.com/user-attachments/assets/d5f56e1e-1f66-4c8c-b42c-ed867d363a4b)


For example, use **Create Empty** (an empty object) can be used as a folder when making a game to organise a scene, to manage scripts in the scene or simply an invisible area that (with the help of code) will be able to recongnise a trigger and do something in the game. Shortly said, it is quite an adaptable object. Besides that, we have Effects, Light, Audio, UI... (which are all useful in making a game)
But for now, we want to create a **3D object**! When we drag over a 3D object, a sub menu will open which will show us a list of list of object we would like to add to the scene. It does not really matter which one would you like to use, since it will not affect the code, but I will be using a cube. 

![Creating_a_cube](https://github.com/user-attachments/assets/05e2409d-c24f-4e53-add6-ede1a6d04499)

Now that we have added a cube, this is what will be shown in the hierarchy.

![Cube_seen_in_the_hierarchy](https://github.com/user-attachments/assets/63ab4222-4d5f-4d90-9eca-3dcdc00adbcb)

Since we have it here, it is easy to access it anytime you need it.
To make it more clear what it is, we will rename it to **Player**.
Go to the Cube, right click on the object and a tab will show up. Left click on the Rename and simply type in Player.

![Screenshot_(7)](https://github.com/user-attachments/assets/c2962baf-c457-4b57-8263-5fdf31edb987)

This is what it should look like!
After typing it in, I suggest moving it to the assets so the Project can look more organised and we can access the **Player** more easily!
We can simply left click on the Player in the **Hierarchy**, hold the left click and drag it to **Assets**
The picture will show you what it looks like.

![Screenshot_(8)](https://github.com/user-attachments/assets/efe90b79-3263-4d81-a528-12f24eb620c8)

Perfect! Now we are able to access the Player by clicking it either in the Hierarchy, Assets, or in the Scenes!

![Cube_seen_in_the_scene](https://github.com/user-attachments/assets/a56ab2d3-3bf4-416e-b37c-ad678de9d3ce)

This is what the Player will look like in the scene.
We can see where it is, as well as the way it is facing us by an X, Y, Z arrows. X (according to the main camera) can move the Player left and right, Z back and forth, and Y axis up and down. 
The Sun above the player shows us where the Directional Light is.

Lastly, we can see the Player in the Inspector

![Player_in_inspector](https://github.com/user-attachments/assets/c77fc515-309d-4d3b-aee8-a5550f434423)

Inspector is used for modifying anything to the object, some of the exaples are:
- Adding tags (used for identifying the object in code)
- Transforming the object - positioning it on XYZ axis (shortcut on keyboard W), rotating in in different angles (shortcut E), scaling the object in either in width X axis, height Y axis and thickness in Z axis (shortcut R)
- Adding materials
- Adding components like colliders , physics and most importantly C# scripts

The first thing we will add is the RigidBody. This component adds physics to the player. It will enable our player to move.
You can add it by left clicking on the add component option and type in RigidBody.

![Capture5](https://github.com/user-attachments/assets/0126744c-3428-4f84-8c90-3275426d6ea9)

This is what the Rigidbody looks like! We will leave all the options as they are. 
If we press play now, the palyer will start falling down slowly, since we added some physics to it. To avoid this from happening, we are going to add a **plane** so our cube will have something to stand on!
To add a plane, go to **Hierarchy**, right click on the gray area, choose a 3D object and click on the plane!

![Screenshot (10)](https://github.com/user-attachments/assets/747890d6-7ca3-4403-aa91-ea1255f6f9d3)

There we have it. Just place it directly below the cube so they do not collide with each other.



After adding this, we will add another component called C# script.



## Making the script

This will be a simple code for moving the player left and right using A and D keys.
This script will enable us to move the player on an X axis . 

There are a few ways to add a script and assign it to a object. One way is to go is to drag your cursor to the assets (Scenes), right click to Create and press on C# script. You will see your script, named NewBehaviourScript, in the Assets.

It is useful to name a script before adding it to the object! If you add the script to the object and then opt to change the name of the script, you will need to change the name in the Microsoft Visual Studio as well. Avoiding this or forgetting this will lead to confusion. 
You can name the script however you like, (preferably associated to the object), but keep in mind that you cannot use space between the words (use the Camel Case). More explanation on the casing options visit this webpage on [Casing terminology](https://unity.com/how-to/naming-and-code-style-tips-c-scripting-unity) .

To sum it up, it is helpful to name a script in order to navigate through your project (especially helpful when you have more scripts in your project). Do it before adding it to the object and do not use spaces when naming it!

The other way is to go to the |Inspector, go to Add Component, left click on it, scroll all the way down or type in the search tab **New Script**. The naming process goes the same.

Both ways are correct!

![Screenshot (9)](https://github.com/user-attachments/assets/fb1345e6-1975-409f-8f36-b574f3df32b9)

I have named it PlayerMovement like shown in the picture.

If you have made the script, you are free to proceed with the tutorial!

## Coding the Player

- The next step will be openning the script! You just double left click on the script and Microsoft Visual Studio will open.
- The other way is to select the object, go to the inspector and add a component (new script). Either way, make sure to change the name of the scripts immediatelly because if you wish to alter it afterwards, you will also need to rename it in the Visual Studio. I will name the script Player , since we want to code 
Having made the script and assigned it to both cubes, open the script in Microsoft Visual Studio by pressing the script.

When we open a script, this is what is shown in the editor.

![basic editor view](https://github.com/user-attachments/assets/b05163fe-4e1b-4bab-b238-d769c5cc7303)

This is what the editor should look like without entering any code.
We have got a few things to explain before changing anything in the editor.

![basic_editor_view](https://github.com/user-attachments/assets/c68463b3-579d-48ab-bb8c-7eead5fdc29b)

Using directives - allows you to use types defined in a namespace without having to specify the full namespace needed of that type, it is a library of definitions that help us when writing the code without having to explain every single step. Sometimes they are not needed and it depends on the things we want to do in the game, either way, the editor will let you know by fading the unneccesary lines or underlining the codes missing the directive.
Class definition - this classifies the project and the project we are working on
Functions- The flow of our game depends on which of these areas we want to put our code in. Do we want a code to be updated in the first frame  (void Start) or do we want the program to refresh its code each frame (void Update). If the answer is neither, or if  we want it to be updated at a specific time, then we create a separate void for it, but later about that!

it is time to put a first line of code in the script.
![Capture2 (2)](https://github.com/user-attachments/assets/b230e7c7-c14c-4b4d-b459-08e6ffc46c71)
This will generate speed for the player. 
we can also delete the two upper lines because they will not be needed in the script. Then we add these two lines

![Capture3](https://github.com/user-attachments/assets/a91ece47-45d0-4f6c-b90e-cb358e9083b1)

Every line of code ends with the semicolon
public is all lower case, and KeyCode is with an uppercase K and C.
Save with control or command S to save and go back to Unity.

Now with the player selected, you will find some new fields in the scripts component that is attached to the player.

![Capture4](https://github.com/user-attachments/assets/4414e5f1-ea6d-47d0-a5c0-0f08b3e569eb)

They can be visible in the inspector because we set them to public. This makes it more simple for us because we can always adjust this and play with it!

![Capture5](https://github.com/user-attachments/assets/232e1357-716b-47f5-b074-473bbd2cf76a)

As I said, you can set everything to your liking, but I have set the speed to 5, D key for right button and A key for the left one.
Having changed that, the game is still not complete, and if you enter play mode, nothing will happen. 

If you have successfully adjusted the speed and the controlls it is time to proceed to the editor.
Now we need to do 2 things:
-reference to the **Rigidbody**
-detect player input (*if we press right, the player moves right, if we press left, the player goes to the left, and if we press nothing, the player stops moving*)

**Rigidbody**

Go back to our script and add private Rigidbody

![Capture6](https://github.com/user-attachments/assets/25d11bbe-cffd-49ce-b51d-649d522213bc)

And then in the start method we add the rigidbody. 

![Capture7](https://github.com/user-attachments/assets/55c46bf9-cd36-4b11-bab4-b2df922460a9)

GetComponent will get the RigidBody from the game object

**Player Input**

For this we will go to the Update method and create a bool for the input.
we will make two bools, one for the right and one for the left control.

![Capture8](https://github.com/user-attachments/assets/581368f0-4421-4424-9402-be9a52f686d3)

If we go back to Unity and want to move the player left and right, we can see that the cube is moving on the Z axis- it changes value in the bracket from - (left) to + (right)


![Capture1](https://github.com/user-attachments/assets/518b38db-5a3d-4880-91d6-54afec30a752)

Having this in mind, if we go back to Unity and we add an if statement

![Capture2](https://github.com/user-attachments/assets/834a030f-68bf-465f-8c43-9540319b76a1)
If the pressedRight parethensis is right or if we press the button for the right side movement (which we set to key D), we will set the velocity to move in the positive Z direction.
- Vector3 stands for a position in 3D space
- forward means that we are moving on the Z axis

We are going to dp the same thing for the left side movement

![Capture3](https://github.com/user-attachments/assets/7e03c68f-e1b1-4e33-9c80-4c34956dd33a)

The only difference is that we have put Vector3.back
We did this because when we press the A key, we want the cube to translate to a negative direction of the Z axis. 
Note that Vector3.forward and Vector3.back only work as a tandem. If you use one of them independetly, it is not going to work.

The next thing we want to add to this is an if statement if none of these buttons are held, what is the player going to do.
![Capture4](https://github.com/user-attachments/assets/63ad10e2-d0bb-4c16-b5d2-1e505bd53fe8)

We also put this in the update void below the previous if statement. This if statement means that if we do not hold the D and A key, the player will stop moving.
You might be wondering what the new characters do in this code.
- The exclamation mark before the pressedRight and pressedLeft is the negation. It means "not" as in !True = Wrong.
- The && stands Conditional logical AND operator. This operator checks if both conditions are true for the if statement to return true. So for instance, my script if we do not press either of the keys, the player is not going to move.

So now  our code is able to understand our mechanic: if we press the D key, our player is going to move to the right on the Z axis,if we press the A key, our player is going to move to the left. If we do not press any button, our player will stop its movement and remain where it is. 

This is all you need to do make your character move. You can save the script and go back to Unity.
























 

