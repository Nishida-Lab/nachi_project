cmake_minimum_required(VERSION 2.8.3)
project(nachi_mz07_moveit_config)

find_package(catkin REQUIRED)

catkin_package()

find_package(roslaunch)
roslaunch_add_file_check(test/moveit_planning_execution_launch_test.xml)

install(DIRECTORY launch DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})
install(DIRECTORY config DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})

