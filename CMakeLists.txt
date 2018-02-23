cmake_minimum_required(VERSION 3.0.2)
cmake_policy(SET CMP0048 NEW)

project(pasted VERSION 1.7)

set(CMAKE_AUTOMOC ON)

include(GNUInstallDirs)
include(CheckIncludeFile)
include(CheckFunctionExists)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11 -Wall -Wextra -pedantic")

find_package(PkgConfig REQUIRED)
find_package(Qt5Core      REQUIRED)
find_package(Qt5Widgets REQUIRED)
find_package(X11 REQUIRED)

add_subdirectory(pasted)
