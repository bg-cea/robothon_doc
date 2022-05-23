# OSCAR Team Robothon documentation

## Equipment used list

### Overall setup

[ADD setup photo]

### Robot

The current setup uses a 7 DOF Franka Emika collaborative robot.
Robot control is done using the low level _Franka Control Interface_, connected to our in-house CEA LIST CORTEX robot controller. 

[ADD ROBOT Illustration]

### Gripper

We use the standard Franka Emika gripper, with custom 3D printed fingertips. 
Those fingertips provide 3 surfaces of interest for improved dexterity, as illustrated in the next figure:
- clamping surface: the main gripping area, approx. 30x30mm, covered with rubber for improved gripping capability. Used for general grasping tasks.
- pressing surface: the tip of each jaw is covered with rubber (approx. 10x30mm) to enable shear forces application. Used for battery lid removal.
- steel blade: each jaw is equipped with a small (non cutting) steel blade, to provide fine poking and clawing capability. Used for batteries removal.

[ADD 3D gripper]

### Teaching

Our team is using a _HTC Vive_ Motion-capture setup to teach easily various geometric primitives, such as waypoints and motions. 
Teaching is done with the HTC remote control. The current setup includes four LightHouses. The VR helmet is not used in this setup. 

[ADD HTC VIVE photos]

### Localization

Localization of the board is done with a _Photoneo PhoXi M_ 3D scanner (https://www.photoneo.com/products/phoxi-scan-m/).
The Photoneo is placed on a fixed pole, calibration with relation to the robot is done once. 



## Software dependency list

The main software modules needed to operate the system are:
- CEA LIST CORTEX robotic framework : 
- CEA LIST SPIRE skills framework :
- CEA LIST Phosphorus framework :
- ROS : for 

Those modules use various third party C++ and Python libraries, all of them being open-source projects, such as :
- Eigen : for C++ matrix computations
- Numpy : for python mathematical computations
- Open-CV : for 2D/3D image computation
- 

## Quick start guide
