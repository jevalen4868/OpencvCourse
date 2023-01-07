cmake_minimum_required(VERSION 3.24)
project(OpencvCourse)

set(CMAKE_CXX_STANDARD 20)

find_package(OpenCV REQUIRED)

include_directories(${OpenCV_INCLUDE_DIRS})

add_executable(OpencvCourse main.cpp)

target_link_libraries( OpencvCourse ${OpenCV_LIBS} )