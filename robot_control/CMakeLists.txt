cmake_minimum_required(VERSION 3.0.2)
project(robot_control)


find_package(catkin REQUIRED COMPONENTS
  ackermann_msgs
  diagnostic_msgs
  diagnostic_updater
  nav_msgs
  roscpp
  rospy
  sensor_msgs
  std_msgs
  tf
)

catkin_package(
 CATKIN_DEPENDS ackermann_msgs
)
include_directories(
  ${catkin_INCLUDE_DIRS}
)

add_executable(robot_control_node src/robot_control.cpp)

target_link_libraries(robot_control_node
   ${catkin_LIBRARIES}
)
