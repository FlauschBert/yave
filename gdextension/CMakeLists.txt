project(yave)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

add_library(yave SHARED
        src/example.cpp
        src/example.h
        src/register_types.cpp
        src/register_types.h
        src/tests.h
)
target_link_libraries(yave PRIVATE godot::cpp)
target_link_options(yave PRIVATE -fno-rtti)