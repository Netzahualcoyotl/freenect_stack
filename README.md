freenect_stack
==============

sudo apt-get install ros-noetic-rgbd-launch

make -p ~/catkin_ws/src
cd ~/catkin_ws/src
put the package freenect_stack
in ~/catkin_ws$catkin_make
$source devel/setup.bash

roslaunch freenect_launch freenect launch depth_registration:=true

Then start rviz and configure with: ‘Global Options’: ‘Fixed Frame’ > ‘camera_link’. Add display ‘pointcloud2’ and set topic to ‘/camera/depth_registered/points’

Build status on Travis CI [![Build Status](https://travis-ci.org/ros-drivers/freenect_stack.svg?branch=master)](http://travis-ci.org/ros-drivers/freenect_stack)

libfreenect based ROS driver

sudo apt-get install ros-noetic-openni-launch
roslaunch openni_launch openni.launch
