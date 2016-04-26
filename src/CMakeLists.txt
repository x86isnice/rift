cmake_minimum_required(VERSION 2.8 FATAL_ERROR)

project(rift)

find_package(PCL 1.7 REQUIRED)

include_directories(${PCL_INCLUDE_DIRS})
link_directories(${PCL_LIBRARY_DIRS})
add_definitions(${PCL_DEFINITIONS})

add_executable (example_rift_estimation example_rift_estimation.cpp)
target_link_libraries (example_rift_estimation ${PCL_LIBRARIES})

