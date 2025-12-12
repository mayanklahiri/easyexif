cmake_minimum_required(VERSION 3.13)

project(EasyExif LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_library(easyExif
    exif.cpp
    exif.h
)

add_executable(easyExifDemo
    demo.cpp
)

target_link_libraries(easyExifDemo
    PRIVATE easyExif
)
