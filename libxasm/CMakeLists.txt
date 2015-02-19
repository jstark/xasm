project(libxasm)

include_directories("${CMAKE_SOURCE_DIR}/include")

set(HEADERS )

set(LIBXASM_SOURCES
    libxasm.cpp)
add_library(libxasm ${LIBXASM_HEADER} ${HEADERS} ${LIBXASM_SOURCES})

