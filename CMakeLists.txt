cmake_minimum_required(VERSION 3.0.0)
project(main VERSION 0.1.0)

file(GLOB SOURCE_FILE "source_file/*.cpp")

add_executable(main main.cpp ${SOURCE_FILE})

target_link_libraries(main PUBLIC SDL2 SDL2_image)
target_include_directories(main PUBLIC header_file)
target_compile_options(main PUBLIC -Wall -Wextra -Werror)
