cmake_minimum_required(VERSION 3.20.0)
find_package(Zephyr REQUIRED HINTS $ENV{ZEPHYR_BASE})

project(SP25_buckler_blinky)

target_sources(app PRIVATE src/main.c)
