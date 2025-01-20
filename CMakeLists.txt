cmake_minimum_required(VERSION 3.5)

project(CBuildKit)

include(cmake/CBuildKit.cmake)

install_cfgpkg(cbuildkit "
include(\${CMAKE_CURRENT_LIST_DIR}/CBuildKit.cmake) 
")

install(DIRECTORY ${CMAKE_SOURCE_DIR}/cmake/ DESTINATION lib/cmake/cbuildkit
        FILES_MATCHING PATTERN "*")