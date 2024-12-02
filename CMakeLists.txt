cmake_minimum_required(VERSION 3.10)

project(CalculatorProject VERSION 1.0)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_library(calculator STATIC calculator.cpp)

add_executable(calculator_exe main.cpp)
target_link_libraries(calculator_exe calculator)
