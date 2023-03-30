cmake_minimum_required(VERSION 3.10)
project(the_greatest_audio_show LANGUAGES CXX)

set(CMAKE_CXX_COMPILER clang++)
set(CMAKE_CXX_STANDARD 20)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR})

set(WARNING_FLAGS "-Wall -Wextra -Wno-multichar -Wno-unused-result")

include_directories(
)

set(CMAKE_EXE_LINKER_FLAGS "-pthread")

set(CMAKE_CXX_FLAGS   "-O3 ${WARNING_FLAGS} -fdeclspec")

add_executable(thegas
    src/main.cpp
)
