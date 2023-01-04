cmake_minimum_required(VERSION 3.23.2)

project(placeholder
    VERSION 0.0.1
    LANGUAGES C CXX
    DESCRIPTION ""
    )

include(CTEST)

add_subdirectory(src)

if (BUILD_TESTING)
    enable_testing()
    add_subdirectory(tests)
endif()