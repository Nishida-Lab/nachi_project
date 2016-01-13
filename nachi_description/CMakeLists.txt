cmake_minimum_required(VERSION 2.8.3)
project(nachi_description)
find_package(catkin REQUIRED)

find_package(roslaunch)
roslaunch_add_file_check(test/mz07/mz07_launch_test.xml)
