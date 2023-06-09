husky_ros2
[![husky_humble_build](https://github.com/adeeb10abbas/husky_ros2/actions/workflows/ci.yml/badge.svg?event=push)](https://github.com/adeeb10abbas/husky_ros2/actions/workflows/ci.yml)
=====
ROS2 Humble port of the packages for [Husky Rover](https://github.com/husky/husky/) which only supports ROS2 Foxy as of now. Primarily for use at Drexel Wireless Systems Lab and Zhou Robotics at Drexel. 

_______

## To start -
 - Clone this repo under `src` in an overlay workspace 
 - Install the deps - `rosdep install --from-paths src --ignore-src -y`
 - `colcon build` from the root of the workspace
 - Source the installation to add the right stuff to PATH - `source install/setup.bash` 

To visualize in `rviz2` - `ros2 launch husky_viz view_model_launch.py`

Common ROS packages for the Clearpath Husky, useable for both simulation and
real robot operation.

 - husky_control : Control configuration
 - husky_description : Robot description (URDF)
 - husky_msgs : Message definitions
 - husky_navigation : Navigation configurations and demos

For Husky instructions and tutorials, please see [Robots/Husky](http://wiki.ros.org/Robots/Husky).

To create a custom Husky description or simulation, please fork [husky_customization](https://github.com/husky/husky_customization).

husky_desktop
=============

Desktop ROS packages for the Clearpath Husky, which may pull in graphical dependencies.

 - husky_viz : Visualization (rviz) configuration and bringup

For Husky instructions and tutorials, please see http://wiki.ros.org/Robots/Husky

husky_robot
===========

Robot ROS packages for the Clearpath Husky, for operating robot hardware.

 - husky_bringup : Bringup launch files and scripts.
 - husky_base : Hardware driver for communicating with the onboard MCU.

For Husky instructions and tutorials, please see http://wiki.ros.org/Robots/Husky

husky_simulator
==============

Simulator ROS packages for the Clearpath Husky.

 - husky_gazebo : Gazebo plugin definitions and extensions to the robot URDF.

For Husky instructions and tutorials, please see http://wiki.ros.org/Robots/Husky
