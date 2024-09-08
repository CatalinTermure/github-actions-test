cmake_minimum_required(VERSION 3.30.0)
project(actionstest VERSION 0.1.0 LANGUAGES C CXX)

include(${CMAKE_TOOLCHAIN_FILE})

include(CTest)

project(HelloWorld)

find_package(fmt CONFIG REQUIRED)

add_executable(actionstest main.cpp)
target_link_libraries(actionstest PRIVATE fmt::fmt)

