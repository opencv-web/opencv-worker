cmake_minimum_required(VERSION 3.5)
project(opencv_worker)

set(CMAKE_CXX_STANDARD 11)

# OpenCV
find_package(OpenCV REQUIRED)
include_directories(${OpenCV_INCLUDE_DIRS})

add_executable(opencv_worker main.cpp)
target_link_libraries(opencv_worker ${OpenCV_LIBS})
