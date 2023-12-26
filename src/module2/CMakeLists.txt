cmake_minimum_required(VERSION 3.0.0)
project(module2)

include_directories(${HEADPATH})
aux_source_directory(./ SRC)
set(LIBRARY_OUTPUT_PATH ${LIBPATH})
add_library(${MODULE2} STATIC ${SRC})