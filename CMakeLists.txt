cmake_minimum_required(VERSION 3.13)
project(test_simbody)

set(CMAKE_CXX_STANDARD 17)

find_package(Simbody REQUIRED)

include_directories(${Simbody_INCLUDE_DIR})

add_executable(test_simbody main.cpp)
target_link_libraries(test_simbody ${Simbody_LIBRARIES})