project(xasm)

include_directories(${CMAKE_SOURCE_DIR}/include)

set(HEADERS )
set(SOURCES 
    xasm.cpp)

add_executable(xasm ${LIBXASM_HEADER} ${HEADERS} ${SOURCES})
target_link_libraries(xasm libxasm)

