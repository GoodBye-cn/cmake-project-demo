cmake_minimum_required(VERSION 3.0.0)
project(demo VERSION 0.1.0)

include(CTest)
enable_testing()

# 设置静态库生成的路径
set(LIBPATH ${PROJECT_SOURCE_DIR}/lib)

# 设置头文件路径
set(HEADPATH ${PROJECT_SOURCE_DIR}/include)

# 设置可执行路径生成的路径
set(EXECPATH ${PROJECT_SOURCE_DIR}/bin)

set(MODULE1 module1)
set(MODULE2 module2)
set(EXECNAME demo)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)


add_subdirectory(src)
add_subdirectory(test)
