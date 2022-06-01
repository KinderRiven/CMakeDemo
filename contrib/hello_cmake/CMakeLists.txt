set(DEMO_SRC
    src/hello_cmake.cpp)

set(DEMO_INC include)

# add source file
add_library(hello_cmake ${DEMO_SRC})

# add header file
target_include_directories(hello_cmake PUBLIC "${DEMO_INC}")
