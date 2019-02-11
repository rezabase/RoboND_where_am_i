# RoboND_where_am_i
Udacity Robotics Nano Degree - Assigment 3

By: Reza Rahimi


Inline-style: 
![alt text](screenshots/rviz_amcl.png "Screenshot, Rviz on left, Gazebo on right")


## ROS and Gazebo

The project was developed on Ubuntu 16.04 LTS with ROS Kinetic, Gazebo. 

## Dependencies:

This is a ROS package demonstrating robot localisation, using AMCL. This is a one of the Udacity project assignment that is part of the Robotics Software Engineer Nanodegree program.  

The ROS project is utilising the following main nodes and packages: 

- Udacity pgm_map_creator: Creates pgm maps from Gazebo world files. The map is used for ROS localisation. Github link: https://github.com/udacity/pgm_map_creator

- ROS Navigation package can be downloaded from git: https://github.com/ros-planning/navigation
  The following nodes that are part of the navigation package are used: 
  
  1. amcl: Used for localisation of the Robot. More info: http://wiki.ros.org/amcl
  2. map_server: Offers map data as a ROS service. More ifo: http://wiki.ros.org/map_server
  3. move_base: Used to define a navigation goal position for the robot for testing. More info: http://wiki.ros.org/move_base
  

## Launch:

1. Go to the catkin_ws workspace
2. source devel/setup.bash
3. roslaunch RoboND_where_am_i world.launch
4. roslaunch RoboND_where_am_i amcl.launch
5. Use the "2D navigation Goal" in Arviz to set a target for the robot to move to. 
  



