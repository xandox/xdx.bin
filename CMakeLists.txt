cmake_minimum_required(VERSION 3.10)

project(xdx.bin CXX)

include($ENV{XDX_CMAKE_ROOT}/xdx.cmake)

include(deps.cmake)

xdx_project(
    NAME xdx
    TYPE exe
    SOURCES
        main.cpp
    PRIVATE_LINK
        xdx.cliopts
)
