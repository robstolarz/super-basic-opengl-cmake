cmake_minimum_required(VERSION 3.6)
project(Test)
set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} "${CMAKE_SOURCE_DIR}/cmake")

if( CMAKE_BINARY_DIR STREQUAL CMAKE_SOURCE_DIR )
  message( FATAL_ERROR "In-source builds aren't allowed.\nDo `rm -f CMakeCache.txt && cd build && cmake ..` instead." )
endif()

find_package(GLFW REQUIRED)
include_directories(${GLFW_INCLUDE_DIR})

set(SOURCE_FILES
        src/main.cpp
)

add_executable(testexec ${SOURCE_FILES})
target_link_libraries(testexec ${GLFW_LIBRARIES})
