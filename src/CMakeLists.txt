
set(target hello-world)

find_package(SDL2 REQUIRED)

add_executable(${target} ${CMAKE_CURRENT_SOURCE_DIR}/main.cpp)
target_link_libraries(${target} SDL2::SDL2)

