cmake_minimum_required(VERSION 3.14)

project(LibCronometro LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_library(LibCronometro SHARED
  LibCronometro_global.h
  cronometro.cpp
  cronometro.h
)

target_compile_definitions(LibCronometro PRIVATE LIBCRONOMETRO_LIBRARY)
