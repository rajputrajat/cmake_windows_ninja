cmake_minimum_required(VERSION 3.16)

project(simple)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -fno-rtti -O3 -std=c++17  -fno-omit-frame-pointer -fno-exceptions")

add_executable(${PROJECT_NAME} main.cpp)
