# UAS
task:
This program will be using a Forward Kinematics Controller for a 3DOF Robotic Arm
The homogeneous transformation matrix H0_3 for a 3-link robot arm is calculated using this code utilising the Denavit-Hartenberg (DH) technique.

The NumPy library is first imported into the code as np. Large, multi-dimensional arrays and matrices are supported by the Python programming language's NumPy module, which also offers a wide range of mathematical operations for use on these arrays.
Following that, the code reads values from four separate text files: a1.txt, a2.txt, a3.txt, and theta1.txt, theta2.txt, and theta3.txt. For the purpose of calculating the DH parameters for the robot arm, each of these files provides numerical values.
The DH parameters for each of the three links are then calculated using the following equations:

where i is the link's number, and ai, di, and thetai are values taken from the appropriate text files. 

Finally, the homogeneous transformation matrices for each link are printed to the console using the NumPy function matrix(). The transformation matrices H0_1, H1_2, and H2_3 are then multiplied together using the dot() function to calculate the overall transformation matrix H0_3, which is also printed to the console using the matrix() function.
