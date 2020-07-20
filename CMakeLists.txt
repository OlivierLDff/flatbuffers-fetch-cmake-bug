cmake_minimum_required(VERSION 3.14.0 FATAL_ERROR)
message(STATUS "CMake Version : ${CMAKE_VERSION}")
execute_process(COMMAND git --version RESULT_VARIABLE GIT_VERSION)
message(STATUS "GIT_VERSION : ${GIT_VERSION}")
project(flatbuffers-fetch-cmake)
include(FetchContent)
FetchContent_Declare(
  uygautfzfgazeyfgezutfgejfzh
  GIT_REPOSITORY https://github.com/google/flatbuffers
  GIT_TAG        master
)
FetchContent_MakeAvailable(uygautfzfgazeyfgezutfgejfzh)