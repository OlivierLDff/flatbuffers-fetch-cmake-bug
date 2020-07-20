cmake_minimum_required(VERSION 3.14.0 FATAL_ERROR)
message(STATUS "CMake Version : ${CMAKE_VERSION}")
project(flatbuffers-fetch-cmake)
include(FetchContent)
FetchContent_Declare(
  flatbuffers
  GIT_REPOSITORY https://github.com/google/flatbuffers
  GIT_TAG        9ecd2e16c2adb6fe9e3cf2fa8f4e1e310d48a1c2
)
FetchContent_MakeAvailable(flatbuffers)