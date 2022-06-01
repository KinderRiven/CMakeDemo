set(SRC
    run_hello_cmake.cpp)

add_library(run_hello_cmake ${SRC})

# link to hello_cmake module
target_link_libraries(run_hello_cmake hello_cmake)