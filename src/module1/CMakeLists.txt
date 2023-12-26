cmake_minimum_required(VERSION 3.0.0)
project(module1)

include_directories(${HEADPATH})
aux_source_directory(./ SRC)
set(LIBRARY_OUTPUT_PATH ${LIBPATH})
add_library(${MODULE1} STATIC ${SRC})