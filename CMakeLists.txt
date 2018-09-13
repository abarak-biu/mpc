cmake_minimum_required(VERSION 3.5)
project(mpc)

set(CMAKE_CXX_STANDARD 11)

include_directories(include)
include_directories(include/mpc)
include_directories(include/mpc/garbled)
include_directories(test)

add_executable(unit_test
        include/mpc/garbled/gate.h
         test/unit_test.cpp)
