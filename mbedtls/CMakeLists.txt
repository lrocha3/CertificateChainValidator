#Include the Headers
include_directories(${CMAKE_CURRENT_SOURCE_DIR}/include)

#Include the Sources

FILE(GLOB SOURCES ${CMAKE_CURRENT_SOURCE_DIR}/library/*.c)

add_library(mbedtls STATIC ${SOURCES})

target_include_directories(mbedtls INTERFACE ${CMAKE_CURRENT_SOURCE_DIR}/include)
