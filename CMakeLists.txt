cmake_minimum_required (VERSION 3.22.1)
project (myprogram C)
add_executable(myprogram main.c)
install(TARGETS myprogram DESTINATION bin)
install(FILES main.c DESTINATION src)

include(CTest)

add_test("test1" "${CMAKE_CURRENT_BINARY_DIR}/${PROJECT_NAME}")

