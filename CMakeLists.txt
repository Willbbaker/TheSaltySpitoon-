cmake_minimum_required(VERSION 3.22.2)

project(physics_engine)

find_package(glfw3 CONFIG REQUIRED)

add_executable(physics_engine main.cpp)

target_link_libraries(physics_engine PRIVATE glfw)

set(CMAKE_C_FLAGS_DEBUG "-g -DDEBUG")

set(CMAKE_CXX_FLAGS_DEBUG "-g -DDEBUG")