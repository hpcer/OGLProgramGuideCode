cmake_minimum_required(VERSION 3.13)
project(OGLProgramGuide)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

set(EXECUTABLE_OUTPUT_PATH Bin)
set(LIBRARY_OUTPUT_PATH lib)

set(INCLUDE_LIST ${CMAKE_CURRENT_SOURCE_DIR})
set(SRC_LIST)

file(GLOB_RECURSE tmp ${CMAKE_CURRENT_SOURCE_DIR}/src/*.cc)
list(APPEND SRC_LIST ${tmp})

include_directories(${INCLUDE_LIST})

add_executable()