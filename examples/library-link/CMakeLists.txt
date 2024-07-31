cmake_minimum_required(VERSION 3.30.0)

project(SubjectExtraction VERSION 0.0.1 LANGUAGES CXX)
# https://cmake.org/cmake/help/latest/policy/CMP0167.html
find_package(Boost CONFIG COMPONENTS regex)

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_BUILD_TYPE RelWithDebInfo)

include_directories(${Boost_INCLUDE_DIRS})
add_executable(${PROJECT_NAME} main.cpp)
target_link_libraries(${PROJECT_NAME} PRIVATE ${Boost_LIBRARIES})
