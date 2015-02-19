cmake_minimum_required(VERSION 2.8)

project(XtremeScriptAssembler)

set(LIBXASM_HEADER "${CMAKE_SOURCE_DIR}/include/xasm.h")

add_subdirectory(libxasm)
add_subdirectory(xasm)

enable_testing()

# needs GTEST_ROOT defined
add_subdirectory(tests)
