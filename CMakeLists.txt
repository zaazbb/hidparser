cmake_minimum_required(VERSION 3.10)
project(hid-report-parser)

SET(CMAKE_C_COMPILER  ${COMPILEPATH}/aarch64-linux-gnu-gcc)
SET(CMAKE_CXX_COMPILER ${COMPILEPATH}/aarch64-linux-gnu-g++)

add_library(${PROJECT_NAME} STATIC HIDParser.c)
