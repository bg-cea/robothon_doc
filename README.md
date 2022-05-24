# OSCAR Team Robothon documentation

## Equipment used list

### Overall setup

[ADD setup photo]
The following image gives an overview of the robotic setup. The main visible components are:

- Franka Emika robot + gripper
- Photoneo M 3D scanner
- HTC Vive motion-capture setup (lighthouses + remote control)

![image info](./static/robothon_setup_annotated.jpg)

### Robot

The current setup uses a 7 DOF Franka Emika collaborative robot.
Robot control is done using the low level _Franka Control Interface_, connected to our in-house CEA LIST CORTEX robot controller. 

![image info](./static/franka_emika.jpg)

### Gripper

We use the standard Franka Emika gripper, with custom 3D printed fingertips. 
Those fingertips provide 3 surfaces of interest for improved dexterity, as illustrated in the next figure:
- clamping surface: the main gripping area, approx. 30x30mm, covered with rubber for improved gripping capability. Used for general grasping tasks.
- pressing surface: the tip of each jaw is covered with rubber (approx. 10x30mm) to enable shear forces application. Used for battery lid removal.
- steel blade: each jaw is equipped with a small (non cutting) steel blade, to provide fine poking and clawing capability. Used for batteries removal.

![image info](./static/robothon_mors_custom.jpeg)

### Teaching

Our team is using a _HTC Vive_ Motion-capture setup to teach easily various geometric primitives, such as waypoints and motions. 
Teaching is done with the HTC remote control. The current setup includes four LightHouses, to limit visual occlusions. The VR helmet is not used in this setup. 

![image info](./static/htc_vive_setup.jpg)

The HTC remote control is equipped with a custom 3D printed extension that provides a pointing tip to the user. All geometric primitives are learned in the tip frame. 

![image info](./static/robothon_vive_rc_teach.jpeg)
### Localization

Localization of the board is done with a _Photoneo PhoXi M_ 3D scanner (https://www.photoneo.com/products/phoxi-scan-m/).
The Photoneo is placed on a fixed pole, calibration with relation to the robot is done once. 

![image info](./static/photoneo.png)


## Software dependency list

The main software modules needed to operate the system are:
- CEA LIST CORTEX robotic framework : 
- CEA LIST SPIRE skills framework :
- CEA LIST Phosphorus framework :
- ROS : used as a communication middleware between SPIRE and Phosphorus frameworks

[insert diagram]

Those modules use various third party C++ and Python libraries, all of them being open-source projects, such as :
- Eigen : for C++ matrix computations
- Numpy : for python mathematical computations
- Open-CV : for 2D/3D image computation

## Quick start guide
[TODO]
