cmake_minimum_required(VERSION 2.8)

set(PROJECT test_resource_message_table)

include (${CMAKE_SOURCE_DIR}/config.cmake)

add_executable(${PROJECT} ${HEADERS} ${SOURCES})

target_include_directories(${PROJECT} PRIVATE ${pe_lib_SOURCE_DIR} ${CMAKE_SOURCE_DIR}/tests/)

target_link_libraries(${PROJECT} PUBLIC pe_lib)

