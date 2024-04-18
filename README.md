# Robot_GUI Package

## Table of Contents

- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Result](#result)

## Introduction <a name="introduction"></a>
The robot_GUI package is the other part of the project aimed at creating a user-friendly graphical interface for robot teleoperation and monitoring. This package provides a GUI which is created using C++, ROS, and the CVUI library, which displays information about the robot. It enables users to interact and control robot's more efficiently.

## Prerequisites <a name="prerequisites"></a>

- ROS
- c++ compiler
- Linux
- OpenCV
- CVUI library

## Installation <a name="installation"></a>

1\. clone this repository inside your `catkin_ws/src` directory:
```bash
cd ~/catkin_ws/src
git clone https://github.com/Gokhulraj6200/robot_gui.git
```

2\. Compile the package:
```bash
cd ~/catkin_ws
catkin_make
```

3\. Source the ROS environment:
```bash
source devel/setup.bash
```

## Usage <a name="usage"></a>
1\. start the ROS core by using the following code:
```bash
roscore
```

2\. Launch the 'robot_info' node:
```bash
rosrun robot_info agv_robot_info_node
```

3\. Launch the 'distance_tracker_service' node:
```bash
rosrun distance_tracker_service distance_tracker_service
```

3\. lastly, launch the 'robot_gui_node' to control the robot using GUI:
```bash
rosrun robot_gui robot_gui_node
```

## Result <a name="result"></a>
A Teleoperation Control GUI is created which displays the following real time controls and information of the robot:

![GUI](https://github.com/Gokhulraj6200/robot_gui/assets/142083650/d7b6c27c-1ee9-4c54-8c55-40c6fba6c587)
