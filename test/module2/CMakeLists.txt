cmake_minimum_required(VERSION 3.0.0)
project(test_module2)

aux_source_directory(./ SRC)

set(EXECUTABLE_OUTPUT_PATH ${EXECPATH}/test)

add_executable(test_module2 ${SRC})

add_test(
    NAME        test_module2
    COMMAND     test_module2
)

set_tests_properties(test_module2 PROPERTIES TIMEOUT 5)