# IKTarget
A custom two-bone IK class for Godot 4.1 that doesn't throw a tantrum when you flip it.

So this is a bit janky still since I don't fully understand the math behind it. It works perfectly for me, your mileage may vary.

In order to get this to work you need to:

- Set the 'Bone Angle' and rotation of both bones in the chain to ZERO.
- Edit the sprites for the arm segments so they point to the RIGHT.
- Set the position and rotation of the sprites to ZERO, adjust them using their offset and flip_h/flip_v properties.
- Cross your fingers and hope it works

This means that when setting up your rig, all arms/legs using IK should be pointing to the right until you activate the IK.

Here's a look at a working setup, flipping the root Node2D should successfully mirror the skeleton:

![image](https://github.com/elliottTreinen/IKTarget/assets/11053393/26cd01e4-2b00-473e-a8df-558c812f2ad7)

![image](https://github.com/elliottTreinen/IKTarget/assets/11053393/d445ced1-832b-46d4-9598-206e8dbcc77e)

![image](https://github.com/elliottTreinen/IKTarget/assets/11053393/25055012-591e-419e-9149-6d638d260361)

![image](https://github.com/elliottTreinen/IKTarget/assets/11053393/c044ccb6-476a-467a-ae82-a3d5ec06c9b0)

![image](https://github.com/elliottTreinen/IKTarget/assets/11053393/c95014a6-3e73-4a73-bdfe-81ad9ffdfb04)


And the sprites used:

![leg_1](https://github.com/elliottTreinen/IKTarget/assets/11053393/7f114d71-fa32-4223-8084-3a805065a12a)

![leg_3](https://github.com/elliottTreinen/IKTarget/assets/11053393/93e14bce-5beb-4039-b4ea-d2b2dae9a004)
