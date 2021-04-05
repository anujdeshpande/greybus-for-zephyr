# SPDX-License-Identifier: BSD-3-Clause

cmake_minimum_required(VERSION 3.13.1)
include($ENV{ZEPHYR_BASE}/cmake/app/boilerplate.cmake NO_POLICY_SCOPE)
project(greybus-uart)

zephyr_include_directories(../../../../../include)

target_sources(app PRIVATE src/main.c)

# if(CONFIG_PINMUX_MCUX_LPC)
#   zephyr_library_sources(pinmux.c)
# endif()
