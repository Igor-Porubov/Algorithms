add_executable(Lab2C lab2.c)
target_include_directories(Lab2C PUBLIC ../LibraryC)
target_link_libraries(Lab2C LibraryC)

add_test(NAME TestLab2C COMMAND Lab2C ${CMAKE_CURRENT_SOURCE_DIR}/input.txt)
