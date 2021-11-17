cmake_minimum_required (VERSION 3.10.2)

project (Project)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} ${COVERAGE_FLAGS} -Wall")
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} ${COVERAGE_FLAGS} -Wall")

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

#Set the folder for the binary
set(EXECUTABLE_OUTPUT_PATH ${CMAKE_CURRENT_SOURCE_DIR}/binary)

#Main Application
add_subdirectory(application)

#Libraries
add_subdirectory(mbedtls)
