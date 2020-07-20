cmake_minimum_required(VERSION 3.14.0 FATAL_ERROR)
message(STATUS "CMake Version : ${CMAKE_VERSION}")
project(flatbuffers-fetch-cmake)
include(FetchContent)
FetchContent_Declare(
  flatbuffers
  GIT_REPOSITORY https://github.com/google/flatbuffers
  GIT_TAG        969d0f7a6317d8f4a7cdac63e514236c632f6093
)
FetchContent_MakeAvailable(flatbuffers)