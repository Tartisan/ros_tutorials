cmake_minimum_required(VERSION 2.8.3)
project(learning_tf2)

## Compile as C++11, supported in ROS Kinetic and newer
# add_compile_options(-std=c++11)

## Find catkin macros and libraries
## if COMPONENTS list like find_package(catkin REQUIRED COMPONENTS xyz)
## is used, also find other catkin packages
find_package(catkin REQUIRED COMPONENTS
  roscpp
  rospy
  tf2
  tf2_ros
  turtlesim
)

catkin_package(
#  INCLUDE_DIRS include
#  LIBRARIES learning_tf2
#  CATKIN_DEPENDS roscpp rospy tf2 tf2_ros turtlesim
#  DEPENDS system_lib
)

include_directories(
# include
  ${catkin_INCLUDE_DIRS}
)

add_executable(static_turtle_tf2_broadcaster src/static_turtle_tf2_broadcaster.cpp)
target_link_libraries(static_turtle_tf2_broadcaster  ${catkin_LIBRARIES})

add_executable(turtle_tf2_broadcaster src/turtle_tf2_broadcaster.cpp)
target_link_libraries(turtle_tf2_broadcaster ${catkin_LIBRARIES})

add_executable(message_filter src/message_filter.cpp)
target_link_libraries(message_filter ${catkin_LIBRARIES})