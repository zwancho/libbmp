cmake_minimum_required(VERSION 3.0.0)
project(libbmp VERSION 0.1.0)

include(CTest)
enable_testing()

add_library(libbmp STATIC libbmp.c)

target_include_directories(libbmp PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}
)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)

add_subdirectory(cpp)