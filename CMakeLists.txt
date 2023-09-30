cmake_minimum_required(VERSION 3.26)
project(test)

set(CMAKE_CXX_STANDARD 17)

find_package(SDL2 REQUIRED COMPONENTS SDL2)
add_executable(test main.cpp)
target_link_libraries(test PRIVATE SDL2::SDL2)
