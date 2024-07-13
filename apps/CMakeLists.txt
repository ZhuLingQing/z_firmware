cmake_minimum_required(VERSION 3.13.1)

set(ENV{APP_BASE} $ENV{ZEPHYR_BASE}/../apps)

list(APPEND BOARD_ROOT ${CMAKE_CURRENT_SOURCE_DIR})

find_package(Zephyr)

project(app LANGUAGES C)

target_sources(app PRIVATE src/main.c)
