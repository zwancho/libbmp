
add_library(libbmppp STATIC libbmp.cpp)

target_include_directories(libbmppp PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}
)