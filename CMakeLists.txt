cmake_minimum_required(VERSION 2.8.3)
project(dwl_msgs)

message("Dynamic Whole-Body Locomotion (DWL) ROS messages")
message("Copyright (C) 2014-2018 Carlos Mastalli, <carlos.mastalli@laas.fr>")
message("All rights reserved.")
message("Released under the BSD 3-Clause License.")

find_package(catkin REQUIRED COMPONENTS message_generation message_runtime std_msgs geometry_msgs sensor_msgs)

add_message_files(
   FILES
    Vector2.msg
    Region.msg
    Contact.msg
    ContactSequence.msg
    ContactRegion.msg
    BaseState.msg
    JointState.msg
    JointCommand.msg
    ContactState.msg
    ReducedBodyState.msg
    ReducedBodyTrajectory.msg
    WholeBodyState.msg
    WholeBodyTrajectory.msg
    WholeBodyController.msg)


generate_messages(
   DEPENDENCIES
   std_msgs
   geometry_msgs)
   

catkin_package(
  CATKIN_DEPENDS message_runtime geometry_msgs)

