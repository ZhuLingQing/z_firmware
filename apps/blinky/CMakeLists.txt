# SPDX-License-Identifier: Apache-2.0

set(ENV{APP_BASE} $ENV{ZEPHYR_BASE}/../apps)
list(APPEND BOARD_ROOT $ENV{APP_BASE})

cmake_minimum_required(VERSION 3.20.0)
find_package(Zephyr REQUIRED HINTS $ENV{ZEPHYR_BASE})
project(blinky)

target_sources(app PRIVATE src/main.c)
