cmake_minimum_required(VERSION 3.10)

project(nvapi VERSION 570)

add_library(nvapi STATIC IMPORTED GLOBAL)
target_include_directories(nvapi INTERFACE "${CMAKE_CURRENT_SOURCE_DIR}")
set_property(TARGET nvapi PROPERTY IMPORTED_LOCATION "${CMAKE_CURRENT_SOURCE_DIR}/amd64/nvapi64.lib")
