# Miniature Delta Input

### Background
This project contains CAD files for 3D printing a mini delta input that can be used to explore the kinematics of a parallel robot. The design is loosely based on the force dimension. This is an educational low-fidelity model. I decided to build this originally as a test of a new Bambu 3D printer we purchased for the lab. However, I decided this was a cool project to open-source as it can be cheaply fabricated and used to explore some robotics/haptics concepts (e.g., kinematics, singularities, transparency).

https://github.com/user-attachments/assets/d3390f8c-db7c-49d0-812c-b1f60f3768bf

### Building the Mini Delta
This project only requires a 3D printer and minimal hardware to put together. All of the STLs and original CAD drawings are provided. This project has been tested with the Bambu labs P1S printer (we also provide assembly 3mfs). There may be a need to update some part dimensions depending on the quality/resolution of your printer. Here are the pieces:

| File/Piece | Quantity |
| -------- | ------- |
| v2_base | 1 |
| v2_wrist_handle | 1 |
| v2_base_pins | 3 |
| v2_bicep | 3 |
| v2_bicep_forearm_shaft_clamp | 12 |
| v2_bicep_forearm_connector | 6 |
| v2_forearm | 6 |
| M2 x 8mm ([from Amazon](https://www.amazon.com/gp/product/B094NVN97P))| 12 |
| M2 locking ([from Amazon](https://www.amazon.com/gp/product/B07L2W3QX3)) | 12 |

Assembling the mini delta should take less than 20 minutes. You will want some tools (e.g., allen wreches and needle-nose pliers or a small wrench) to fasten the bolts. Here are the assembly steps:
1. Put the base_pins through one side of the biceps
2. Press fit the pins into the base
3. Put a forearm_connector through each of the three free sides of the bicep
4. Secure the forearm_connectors in place by pressing in a shaft_clamp on both sides of each connector
5. Attach two forearms to each of the connectors using the M2 bolts and lock nuts. You should tighten enough so it is not loose, but not so tight that the members cannot move.
6. Put a forearm_connector through each of the three slots on the wrist_handle
7. Secure the forearm_connectors in place by pressing in a shaft_clamp on both sides of each connector
8. Attach the six forearms to the forearm_connectors using M2 bolts and lock nuts.
9. All done. Hope you enojoy!


### Interested in Building on This Project?
There is much more runway for building on this project to explore more robotics and haptics concepts. What I like about this version 0.0 is that it is very inexpensive. However, I think there are a number of exciting and low-cost directions that this can be taken. Please reach out (hagenow@csail.mit.edu) if you are interested to build this concept out further. Here are some opportunities that I think could be cool!
- Adding a passive gimbal at the end of the device (instead of the current handle) to have a 6 DOF kinematic model
- Adding potentiometers, some careful friction sources -- the current model falls down when you are not holding it), and an arudino to turn this into a low-cost 3-DOF input device that can be used for robot control inputs (e.g., teleoperation)
- Adding some low-cost (reasonably backdriveable motors) with encoders that can be used to turn this into a haptic/input device. Clearly the design and thin plastic members would not be good for transmitting force, but it would be cool nonetheless to iterate and get a low-cost 3-DOF open source haptic input out there.
