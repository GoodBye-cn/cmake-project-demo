cmake_minimum_required(VERSION 3.0.0)
project(test_module1)

aux_source_directory(./ SRC)
set(EXECUTABLE_OUTPUT_PATH ${EXECPATH}/test)

add_executable(test_module1 ${SRC})

add_test(
    NAME        test_module1
    COMMAND     test_module1
)

set_tests_properties(test_module1 PROPERTIES TIMEOUT 5)