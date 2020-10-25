ackermann_vehicle
=================

ROS packages for simulating a vehicle with Ackermann steering  

2020SEP22 Currently all setup is using noetic. 

## Install effort controllers
sudo apt install ros-noetic-effort-controllers

## test if you have ackermann messages installed
`cd ackermann_vehicle_gazebo/nodes/

## Try to run the following script, and if it cannot find messages, then install them
python ackermann_controller.py  
sudo apt install ros-noetic-ackermann-msgs   
sudo apt-get install ros-melodic-ros-control  
sudo apt-get install ros-melodic-effort-controllers  

## Run 
roslaunch ackermann_vehicle_gazebo ackermann_vehicle.launch 

## Ackerman steering interface

rosrun rqt_ez_publisher rqt_ez_publisher


## Add PS4
http://ros-developer.com/tag/joystick/  
http://ros-developer.com/2017/07/28/control-your-robot-with-a-joystick-in-ros/  

Add ps4 joystick  
http://wiki.ros.org/joy
https://github.com/solbach/ps4-ros


** Install ros joy
** install ps4
** don't forget to change teh ps4 launch file for /dev/input/jsX
** gotta run rosrun joy_teleop joy_teleop.py

axes: [-0.0, -0.0, 1.0, -0.0, -0.0, 1.0, -0.0, -0.0]
buttons: [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]

axes:
0:
1:
2:
3: Right Joystick (L/R)
4: Right Joystick (U/D)
5: Right Trigger
6:
7:

button:
