#

cmake_minimum_required(VERSION 2.8)
project (foo)

set(TARGET_NAME ${CMAKE_PROJECT_NAME})

set(PROJECT_MAJOR_VERSION 0)
set(PROJECT_MINOR_VERSION 1)
set(PROJECT_PATCH_LEVEL 0)
set(PROJECT_VERSION ${PROJECT_MAJOR_VERSION}.${PROJECT_MINOR_VERSION}.${PROJECT_PATCH_LEVEL})

include(GNUInstallDirs)

find_package(PkgConfig REQUIRED)
add_subdirectory(qmldev)
