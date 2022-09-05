cmake_minimum_required(VERSION 3.0.2)
project(dynamics_pinocchio)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -pthread -fopenmp -std=c++11 -Wfatal-errors -Wl,--no-as-needed")

find_package(Eigen3 REQUIRED)

include_directories("/usr/include/eigen3")
include_directories(${pinocchio_INCLUDE_DIRS})
link_directories(${pinocchio_LIBRARY_DIRS})

add_executable(geometry-model geometry-models.cpp ${pinocchio_LIBRARIES})
target_link_libraries(geometry-model )



