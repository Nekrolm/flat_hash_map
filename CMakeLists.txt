cmake_minimum_required(VERSION 3.5)
project(bytell-hash-map LANGUAGES CXX)

add_library(bytell_hash INTERFACE)

target_include_directories(bytell_hash INTERFACE
    $<BUILD_INTERFACE:${PROJECT_SOURCE_DIR}/include>
    $<INSTALL_INTERFACE:include>)
add_library(ska::bytell_hash ALIAS bytell_hash)