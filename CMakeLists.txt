cmake_minimum_required(VERSION 3.16)
project(matchcore-cpp)

set(CMAKE_CXX_COMPILER clang++)
set(CMAKE_CXX_STANDARD 17)

include_directories(include)

file(GLOB SOURCE "src/*.cpp")

add_executable(matchcore ${SOURCES})
