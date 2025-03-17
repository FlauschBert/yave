cmake_minimum_required(VERSION 3.28)
project(yave-build)

add_subdirectory(gdextension)

set(GODOTCPP_USE_HOT_RELOAD ON)
add_subdirectory(godot-cpp)