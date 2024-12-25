project(cmake)

add_library(simplecmake hello.cc)

target_include_directories(simplecmake
    PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}/../include)