cmake_minimum_required(VERSION 3.0)
project(converter)

SET(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall -std=gnu++0x")

# the -I flag in gcc
include_directories(
  ${PROJECT_SOURCE_DIR}/src/
) 

# creates ./build/bin/runner
add_executable(${PROJECT_NAME} src/main.cpp)
