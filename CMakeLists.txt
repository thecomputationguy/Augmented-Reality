cmake_minimum_required(VERSION 3.4)

set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} ${CMAKE_CURRENT_SOURCE_DIR}/cmake-modules)

find_package(OpenCV REQUIRED)

project(Exercise01)

include_directories( ${OpenCV_INCLUDE_DIRS} )

set(Exercise01_SOURCES
        Exercise-1.cpp)
add_executable(Exercise01 ${Exercise01_SOURCES})
target_link_libraries (Exercise01 ${OpenCV_LIBS})
