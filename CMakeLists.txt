cmake_minimum_required(VERSION 2.8.3)
project(doogie_welcome)

find_package(catkin REQUIRED COMPONENTS
  roscpp
  rospy
  std_msgs
)

catkin_package(
 CATKIN_DEPENDS roscpp rospy std_msgs
)

include_directories(
  ${catkin_INCLUDE_DIRS}
)

add_executable(cpp_talker_node src/cpp_talker.cpp)
target_link_libraries(cpp_talker_node ${catkin_LIBRARIES})

add_executable(cpp_listener_node src/cpp_listener.cpp)
target_link_libraries(cpp_listener_node ${catkin_LIBRARIES})