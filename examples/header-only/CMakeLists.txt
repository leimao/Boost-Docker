cmake_minimum_required(VERSION 3.30.0)

project(Triple VERSION 0.0.1 LANGUAGES CXX)
# https://cmake.org/cmake/help/latest/policy/CMP0167.html
find_package(Boost CONFIG)

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_BUILD_TYPE RelWithDebInfo)

include_directories(${Boost_INCLUDE_DIRS})
add_executable(${PROJECT_NAME} main.cpp)
