cmake_minimum_required(VERSION 3.15)

project(libstb_image
    DESCRIPTION "Image loader"
    LANGUAGES CXX)

set(PROJECT_SOURCE_DIR "${CMAKE_CURRENT_SOURCE_DIR}/src")

add_library(stb_image "${PROJECT_SOURCE_DIR}/stb_image.cpp")

target_include_directories(stb_image PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}/include")