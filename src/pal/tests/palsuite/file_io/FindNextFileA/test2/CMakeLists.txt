cmake_minimum_required(VERSION 2.8.12.2)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(SOURCES
  findnextfilea.c
)

add_executable(paltest_findnextfilea_test2
  ${SOURCES}
)

add_dependencies(paltest_findnextfilea_test2 CoreClrPal)

target_link_libraries(paltest_findnextfilea_test2
  pthread
  rt
  m
  CoreClrPal
)
