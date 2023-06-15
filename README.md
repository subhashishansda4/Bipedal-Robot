## Description
**Modeled and Simulated a Bipedal Robot** using tools like *Fusion 360*, *MATLAB* and a little bit of *Mathematics*

Indepth report can be found here:\
[Report](https://github.com/subhashishansda4/Bipedal-Robot/blob/main/Modelling%20and%20Simulation%20of%20Bipedal%20Robot.pdf)

## Introduction
Bipedal Robots are robots which are capable of doing tasks like walking, strafing and other leg movements much like humans

Some of the these types of robots are:
* Digit
* Atlas
* HUBO (KHR-3)

Associated Companies:
* Agility Robotics
* Boston Dynamics
* Houston Mechatronics
* KAIST (Korea Advanced Institute of Science and Technology)

## Objectives
* To collect data from various research projects based on their experimental results
* To simulate joints of our model in MATLAB along with necessary conditions like damping and stiffness coefficients
* To design suitable model and control system if necessary
* To design robot parts and assemblies with the help of data collected
* Yo stress simulate our parts and make sure everything is feasible

## Observations
When robot is walking on the ground according to that the leg is divided into two portions:
1. **Stable Leg**
2. **Swing Leg**

A single cycle of walking can be divided into two phase:
1. **Single support phase**
2. **Double support phase**

In order to remain stable, the centre of gravity must fall under its polygon of support\
The support polygon is the smallest polygon obtain by connecting all points of contact of robot wih the walking surface

**Trajectory Planning**
* Teach initial and final points, intermediate path is not critical and is computed by the controller
* Continuous path motion
* Points generaly taught by manual lead through with high speed automatic sampling

**Dynamics of Manipulator**
* Kinematics of a robot manipulator deals with the relation between position and orientation of the end effector and the joint variable of the manipulator without considering the mass of links or the forces/torque acting on the manipulator
* Dynamics of a robot deals with the relation between position, velocity and acceleration of the robot's joints along with the force/torque at each joint to cause the motion

## Mechanics of Robot
**Normal Robot containing solid blocks, rigid transformations and joint blocks**

![1](https://github.com/subhashishansda4/Bipedal-Robot/blob/main/work/1.png)

![2](https://github.com/subhashishansda4/Bipedal-Robot/blob/main/work/2.png)

1

**Setting conditions such as changing pitch value of hip join to half and decreasing damping to 1/10**\
**Initialising conditions such as stiffness, damping, length, width, height, etc.**

2

## LIPM
**Linear Inverted Pendulum Model** is a simple and powerful model assumptions:
* Robot has constant height while walking
* Angular momentum around CoM is very small

**Finding initial conditions and time to create symmetric piece of trajectory, will be sufficient because we are simulating our model to walk in a straight line**\
**Mirroring the same for the other leg**

![3](https://github.com/subhashishansda4/Bipedal-Robot/blob/main/work/3.png)

3

**Setting parameters like height, swing height, step length, velocity, etc.**

4

**Finding joint angles from feet trajectories using inverse kinematics**\
**Inverse rotations for joint angles are done through computing analytical solution**

5

## Simulation
**Joint angles of legs are feed as input in our model**

![4](https://github.com/subhashishansda4/Bipedal-Robot/blob/main/work/4.png)

![5](https://github.com/subhashishansda4/Bipedal-Robot/blob/main/work/5.png)

**Simulation through simplified motion actuation approach**

6

## Graphs
**We used motion actuation for acutating robot joints cause it is easier and faster to simulate and does not offer much difference from force/torque actuation approach**

![6](https://github.com/subhashishansda4/Bipedal-Robot/blob/main/work/6.png)

## Renders
![1](https://github.com/subhashishansda4/Bipedal-Robot/blob/main/renders/1.jpg)

![2](https://github.com/subhashishansda4/Bipedal-Robot/blob/main/renders/2.jpg)

![3](https://github.com/subhashishansda4/Bipedal-Robot/blob/main/renders/3.jpg)

![4](https://github.com/subhashishansda4/Bipedal-Robot/blob/main/renders/4.jpg)

![5](https://github.com/subhashishansda4/Bipedal-Robot/blob/main/renders/5.jpg)

![6](https://github.com/subhashishansda4/Bipedal-Robot/blob/main/renders/6.jpg)