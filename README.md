# IKTarget
A custom two-bone IK class for Godot 4.1 that doesn't throw a tantrum when you flip it.

So this is a bit janky still since I don't fully understand the math behind it. It works perfectly for me, your mileage may vary.

In order to get this to work you need to:

- Set the 'Bone Angle' and rotation of both bones in the chain to ZERO.
- Edit the sprites for the arm segments so they point to the RIGHT.
- Set the position and rotation of the sprites to ZERO, adjust them using their offset and flip_h/flip_v properties.
- Cross your fingers and hope it works

This means that when setting up your rig, all arms/legs using IK should be pointing to the right until you activate the IK.
