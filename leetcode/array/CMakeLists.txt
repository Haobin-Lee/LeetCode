cmake_minimum_required(VERSION 3.0.0)

set(TARGET leetcode)

project(${TARGET} CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

set(CMAKE_CURRENT_SOURCE_DIR ON)

include(CTest)
enable_testing()

add_executable(${TARGET}
    main.cpp
)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
