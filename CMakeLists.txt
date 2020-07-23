cmake_minimum_required(VERSION 3.14.0 FATAL_ERROR)
project(flatbuffers-fetch-cmake)
include(FetchContent)
FetchContent_Declare(
  flatbuffers
  GIT_REPOSITORY https://github.com/google/flatbuffers
  GIT_TAG        master
)
FetchContent_MakeAvailable(flatbuffers)