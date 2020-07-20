cmake_minimum_required(VERSION 3.14.0 FATAL_ERROR)
message(STATUS "CMake Version : ${CMAKE_VERSION}")
project(flatbuffers-fetch-cmake)
include(FetchContent)
FetchContent_Declare(
  flatbuffers
  GIT_REPOSITORY https://github.com/google/flatbuffers
  GIT_TAG        515a4052a750dfe6df8d143c8f23cd8aaf51f9d7
)
FetchContent_MakeAvailable(flatbuffers)