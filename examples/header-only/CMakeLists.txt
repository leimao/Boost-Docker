cmake_minimum_required(VERSION 3.0.0)

project(Triple VERSION 0.0.1 LANGUAGES CXX)
# https://cmake.org/cmake/help/v3.25/module/FindBoost.html
find_package( Boost REQUIRED)

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_BUILD_TYPE RelWithDebInfo)

include_directories(${Boost_INCLUDE_DIRS})
add_executable(${PROJECT_NAME} main.cpp)
