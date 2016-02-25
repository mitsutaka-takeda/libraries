cmake_minimum_required(VERSION 3.3)

project(stlab-libraries)

add_library(stlab-libraries
  src/future.cpp
  stlab/channel.hpp
  stlab/config.hpp
  stlab/future.hpp
  )

target_compile_options(
  stlab-libraries
  PUBLIC
  -std=c++14
  )

target_include_directories(
  stlab-libraries
  PUBLIC
  ${CMAKE_CURRENT_LIST_DIR}
  )
