project(mini-caffe C CXX)
cmake_minimum_required(VERSION 2.8)

include(mini-caffe.cmake)
include(tests/tests.cmake)
include(tools/tools.cmake)

IF (NOT MSVC)
  SET(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11 -pthread")
ENDIF()