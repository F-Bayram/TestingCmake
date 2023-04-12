cmake_minimum_required(VERSION 3.0)
project(TestProject)
set(CMAKE_CXX_STANDARD 11)

add_library(bib SHARED bib.cpp)
add_executable(TestProgram main.cpp)
target_link_libraries(TestProgram bib)
