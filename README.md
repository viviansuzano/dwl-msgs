==============================================
The DWL's ROS messages
==============================================

Table of Contents
==============================================
1. [Introduction](#introduction)
2. [Software Overview](#software-overview)


Introduction
==============================================
The Robot Operting System (ROS) provides libraries and tools to help software developers create robot applications. It provides hardware abstraction, device drivers, libraries, visualizers, message-passing, package management, and more. For more details see: http://wiki.ros.org/

The Dynamic Whole Body Locomotion library (DWL) describes a set of core functions targeted to developed, design, and deploy locomotion algorithms, i.e. planning, control, etc. DWL is core library used in many projects of the Dynamic Legged Systems Lab of Istituto Italiano di Tecnologia (for more details about the project see http://www.iit.it/en/advr-labs/dynamic-legged-systems.html). For more details about DWL software infrastructure please visit https://github.com/robot-locomotion/dwl.

The DWL's ROS messages are a set of message description which are compatible with DWL standards. This allows us to define the standarized messages of DWL in ROS.

[![ScreenShot](https://j.gifs.com/zJEDWD.gif)](https://www.youtube.com/watch?v=ENHvCGrnr2g)


Software Overview
==============================================
The algorithms are built primarily in C/C++. The library uses a number of the local dependencies, which some of them are optionals.

The dwl-lcmtypes is a ROS packages with the following required dependencies:
* [CMake](http://www.cmake.org) (version 2.8.3 or higher)
* [DWL](https://github.com/robot-locomotion/dwl)


