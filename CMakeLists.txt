cmake_minimum_required(VERSION 3.14)
project(hello_cmake)
add_subdirectory(contrib/hello_cmake)
add_subdirectory(src)

set(INC src)

add_executable(run_hello_cmake_client main.cpp)

target_link_libraries(run_hello_cmake_client run_hello_cmake)
target_include_directories(run_hello_cmake_client PUBLIC "${INC}")
