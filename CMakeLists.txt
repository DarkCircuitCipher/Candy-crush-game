cmake_minimum_required(VERSION 4.0)
project(PF_PROJECT)

set(CMAKE_CXX_STANDARD 20)
find_package(raylib CONFIG REQUIRED)

add_executable(PF_PROJECT main.cpp
        graphics_core.cpp
        graphics_core.hpp
        cursor_input.cpp
        cursor_input.hpp
        grid_manager.cpp
        CMakeLists.txt)
target_link_libraries(PF_PROJECT PRIVATE raylib)