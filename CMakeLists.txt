cmake_minimum_required(VERSION 3.15)
project(cmake)

add_subdirectory(include)
add_subdirectory(src)

option(BUILD_EXAMPLES "Whether or not build exampless" ON)
if(BUILD_EXAMPLES)
    message(STATUS "Building examples")
    add_subdirectory(example)
endif()