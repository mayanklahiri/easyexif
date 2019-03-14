cmake_minimum_required(VERSION 3.7)
project(easyexif)

if(VERBOSE)
    add_definitions(-DDEBUG_COUT)
endif()

set(CMAKE_CXX_STANDARD 14)

add_executable(demo demo.cpp exif.cpp exif.h)
