# Unity 2d Parallax Background

This repository contains a Unity 2D parallax script designed to create a parallax scrolling effect for layered backgrounds in your 2D game. The script allows you to adjust the parallax effect on both the X and Y axes for each layer, with specific behavior for near and far objects.

https://github.com/user-attachments/assets/b03b4ee8-f0ac-43c4-8454-cc1aa6a685c9

How to Use

Attach the Script to Each Layer:

Identify the GameObjects in your Unity scene that represent the background layers (e.g., sprites for sky, mountains, trees).
Attach the parallax script to each of these GameObjects by dragging the script onto them or using the "Add Component" button in the Inspector and searching for the script name.
Ensure each layer has the script attached to enable the parallax effect.


Adjust Parallax Settings:

In the Unity Inspector, locate the parallax script component on each GameObject.
Adjust the Parallax X and Parallax Y fields to control the intensity of the parallax effect:
Parallax X: Controls horizontal movement relative to the camera.
Parallax Y: Controls vertical movement relative to the camera.
Values close to 1 (e.g., 0.9): Used for farther objects to create slower movement, simulating greater distance.
Values close to 0 (e.g., 0.1): Used for nearer objects to create faster movement, simulating proximity to the camera.


Experiment with values between 0 and 1 for each layer to achieve the desired depth effect. Farther layers (e.g., sky) should have values closer to 1, while nearer layers (e.g., foreground trees) should have values closer to 0.


Test the Scene:

Ensure your main camera is set up to move (e.g., following the player).
Play the scene in Unity to observe the parallax effect.
Fine-tune the Parallax X and Y values as needed to perfect the scrolling effect.



Notes

The script assumes a 2D setup with a moving camera. Ensure your camera is configured to track the player or move as intended.
For best results, organize your layers in the scene hierarchy and use appropriate sorting layers or Z positions to handle rendering order.
If the script references the camera, ensure the main camera is tagged as "MainCamera" in Unity.

Example

Attach the script to three layers:
Sky (Parallax X: 0.95, Y: 0.9) – Farther, moves very slowly.
Mountains (Parallax X: 0.5, Y: 0.5) – Midground, moves at moderate speed.
Trees (Parallax X: 0.1, Y: 0.2) – Nearer, moves quickly.


When the camera moves, the Sky will appear distant with minimal movement, while Trees will move faster, creating a sense of depth.

Contributing
Feel free to fork this repository and submit pull requests with improvements or bug fixes. For issues, please open a GitHub issue with details.









