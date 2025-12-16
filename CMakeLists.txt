cmake_minimum_required(VERSION 3.22.2)

project(TheSaltySpitoon-)

find_package(glfw3 CONFIG REQUIRED)
find_package(glad CONFIG REQUIRED)
find_package(OpenGL REQUIRED)

add_executable(TheSaltySpitoon- main.cpp)

target_link_libraries(TheSaltySpitoon- glfw)
target_link_libraries(TheSaltySpitoon- OpenGL::GL)
target_link_libraries(TheSaltySpitoon- glad::glad)

set(CMAKE_C_FLAGS_DEBUG "-g -DDEBUG")

set(CMAKE_CXX_FLAGS_DEBUG "-g -DDEBUG")