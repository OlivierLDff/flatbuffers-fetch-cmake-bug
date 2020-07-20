cmake_minimum_required(VERSION 3.14.0 FATAL_ERROR)
message(STATUS "CMake Version : ${CMAKE_VERSION}")
project(flatbuffers-fetch-cmake)
include(FetchContent)
FetchContent_Declare(
  flatbuffers
  GIT_REPOSITORY https://github.com/google/flatbuffers
  GIT_TAG        36fbe6f13e7e3a370edae090ca2292fae45235a9
)
FetchContent_MakeAvailable(flatbuffers)