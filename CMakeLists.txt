cmake_minimum_required(VERSION 3.10)
project(furgbol_io)

message("Compiling furgbol_io library!")

include_directories("include")

add_library(furgbol_math "src/calc.cpp")

add_executable(teste_math "src/teste.cpp")
target_link_libraries(teste_math furgbol_math)
