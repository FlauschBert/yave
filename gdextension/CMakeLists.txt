project(yave)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

add_library(yave SHARED
        src/example.cpp
        src/example.h
        src/register_types.cpp
        src/register_types.h
        src/tests.h
)
target_compile_options(yave PRIVATE -Wl,--no-undefined -lm)
target_link_libraries(yave godot::cpp)