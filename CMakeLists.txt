cmake_minimum_required (VERSION 3.21)

set(PROJECT_NAME "Metal-cpp")
project(${PROJECT_NAME} LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_library(${PROJECT_NAME} OBJECT ${PROJECT_SOURCE_DIR}/src/Metal.impl.cpp)
target_include_directories(${PROJECT_NAME} PUBLIC ${PROJECT_SOURCE_DIR}/include)
