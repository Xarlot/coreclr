cmake_minimum_required(VERSION 2.8.12.2)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(SOURCES
  test5.cpp
)

add_executable(paltest_wfopen_test5
  ${SOURCES}
)

add_dependencies(paltest_wfopen_test5 coreclrpal)

target_link_libraries(paltest_wfopen_test5
  ${COMMON_TEST_LIBRARIES}
)
