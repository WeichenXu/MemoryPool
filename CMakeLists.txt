cmake_minimum_required (VERSION 2.6)
project (MemoryPool)

# The version number
set (MemoryPool_VERSION_MAJOR 1)
set (MemoryPool_VERSION_MINOR 0)

# Compiler Options
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -g -std=c++11 -Wall -Wextra -Wno-unused-parameter -Werror$")

# Add the ./C-11 Memory Pool Directory into the search path for .h files
include_directories ("${PROJECT_SOURCE_DIR}/include")

add_executable (testStackAlloc test.cpp)
