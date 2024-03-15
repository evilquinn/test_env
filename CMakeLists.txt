cmake_minimum_required(VERSION 3.20)

project(test_env C CXX)

add_executable(cpp32 main.cpp)
set_target_properties(cpp32 PROPERTIES COMPILE_FLAGS "-m32" LINK_FLAGS "-m32")

add_executable(cpp64 main.cpp)

add_executable(c32 main.c)
set_target_properties(c32 PROPERTIES COMPILE_FLAGS "-m32" LINK_FLAGS "-m32")

add_executable(c64 main.c)
