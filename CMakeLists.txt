cmake_minimum_required(VERSION 3.17)

project(SDL2_Test)

set (CMAKE_MODULE_PATH ${PROJECT_SOURCE_DIR}/cmake)

set (CMAKE_CXX_STANDARD 17)

set(CMAKE_BUILD_TYPE Debug)

find_package(SDL2 REQUIRED)

include_directories(${SDL2_INCLUDE_DIR})

add_executable(SDL2_Test main.cpp)

target_link_libraries(SDL2_Test ${SDL2_LIBRARY} )


