cmake_minimum_required(VERSION 3.0.0)
project(demo)

add_subdirectory(module1)
add_subdirectory(module2)

include_directories(${HEADPATH})

set(EXECUTABLE_OUTPUT_PATH ${EXECPATH})

add_executable(${EXECNAME} main.cc)