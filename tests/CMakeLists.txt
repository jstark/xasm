project(tests)

find_package(GTest REQUIRED)

set(TEST_HEADERS )
set(TEST_SOURCES 
    test.cpp)

include_directories(${GTEST_INCLUDE_DIRS})
add_executable(tests ${TEST_HEADERS} ${TEST_SOURCES})
target_link_libraries(tests ${GTEST_BOTH_LIBRARIES})
add_test(AllTests tests)
