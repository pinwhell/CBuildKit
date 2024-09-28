project(CBuildKit)

install(DIRECTORY ${CMAKE_SOURCE_DIR}/cmake/ DESTINATION lib/cmake/cbuildkit
        FILES_MATCHING PATTERN "*")